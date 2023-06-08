# Comparing `tmp/sparseml_nightly-1.6.0.20230604-py3-none-any.whl.zip` & `tmp/sparseml_nightly-1.6.0.20230608-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,370 +1,370 @@
-Zip file size: 946552 bytes, number of entries: 368
--rw-rw-r--  2.0 unx     1413 b- defN 23-Jun-04 01:31 sparseml/__init__.py
--rw-rw-r--  2.0 unx      898 b- defN 23-Jun-04 01:31 sparseml/analytics.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-Jun-04 01:31 sparseml/base.py
--rw-rw-r--  2.0 unx     2483 b- defN 23-Jun-04 01:31 sparseml/log.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-04 01:31 sparseml/version.py
--rw-rw-r--  2.0 unx      758 b- defN 23-Jun-04 01:31 sparseml/benchmark/__init__.py
--rw-rw-r--  2.0 unx    17631 b- defN 23-Jun-04 01:31 sparseml/benchmark/info.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-Jun-04 01:31 sparseml/benchmark/serialization.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jun-04 01:31 sparseml/deepsparse/__init__.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-Jun-04 01:31 sparseml/deepsparse/base.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jun-04 01:31 sparseml/deepsparse/framework/__init__.py
--rw-rw-r--  2.0 unx     6032 b- defN 23-Jun-04 01:31 sparseml/deepsparse/framework/info.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jun-04 01:31 sparseml/deepsparse/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1348 b- defN 23-Jun-04 01:31 sparseml/deepsparse/sparsification/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-04 01:31 sparseml/exporters/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-Jun-04 01:31 sparseml/exporters/base_exporter.py
--rw-rw-r--  2.0 unx     4783 b- defN 23-Jun-04 01:31 sparseml/exporters/onnx_to_deepsparse.py
--rw-rw-r--  2.0 unx     2252 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/__init__.py
--rw-rw-r--  2.0 unx     2333 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/base_transform.py
--rw-rw-r--  2.0 unx     1388 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/constants_to_initializers.py
--rw-rw-r--  2.0 unx     3866 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     5838 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/conv_to_qlinearconv.py
--rw-rw-r--  2.0 unx     2440 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/delete_repeated_qdq.py
--rw-rw-r--  2.0 unx     1842 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
--rw-rw-r--  2.0 unx     2181 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/flatten_qparams.py
--rw-rw-r--  2.0 unx     3553 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/fold_conv_div_bn.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/fold_identity_initializers.py
--rw-rw-r--  2.0 unx     2070 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/fold_relu_quants.py
--rw-rw-r--  2.0 unx     4418 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     7629 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     1645 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/initializers_to_uint8.py
--rw-rw-r--  2.0 unx     4470 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     4571 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
--rw-rw-r--  2.0 unx     4156 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     3724 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/onnx_transform.py
--rw-rw-r--  2.0 unx     3398 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/propagate_embedding_quantization.py
--rw-rw-r--  2.0 unx     4464 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/quantize_qat_embedding.py
--rw-rw-r--  2.0 unx     3869 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/quantize_residuals.py
--rw-rw-r--  2.0 unx     3331 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
--rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
--rw-rw-r--  2.0 unx     3210 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/skip_input_quantize.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/unwrap_batchnorms.py
--rw-rw-r--  2.0 unx      730 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/utils/__init__.py
--rw-rw-r--  2.0 unx     8704 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/utils/helpers.py
--rw-rw-r--  2.0 unx    14429 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/utils/matching.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jun-04 01:31 sparseml/framework/__init__.py
--rw-rw-r--  2.0 unx     9479 b- defN 23-Jun-04 01:31 sparseml/framework/info.py
--rw-rw-r--  2.0 unx      970 b- defN 23-Jun-04 01:31 sparseml/keras/__init__.py
--rw-rw-r--  2.0 unx     8054 b- defN 23-Jun-04 01:31 sparseml/keras/base.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/__init__.py
--rw-rw-r--  2.0 unx     3297 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/dataset.py
--rw-rw-r--  2.0 unx     2423 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/helpers.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/registry.py
--rw-rw-r--  2.0 unx      786 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     8369 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4301 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      793 b- defN 23-Jun-04 01:31 sparseml/keras/framework/__init__.py
--rw-rw-r--  2.0 unx     5906 b- defN 23-Jun-04 01:31 sparseml/keras/framework/info.py
--rw-rw-r--  2.0 unx      921 b- defN 23-Jun-04 01:31 sparseml/keras/models/__init__.py
--rw-rw-r--  2.0 unx    11814 b- defN 23-Jun-04 01:31 sparseml/keras/models/registry.py
--rw-rw-r--  2.0 unx      656 b- defN 23-Jun-04 01:31 sparseml/keras/models/classification/__init__.py
--rw-rw-r--  2.0 unx    17932 b- defN 23-Jun-04 01:31 sparseml/keras/models/classification/resnet.py
--rw-rw-r--  2.0 unx      768 b- defN 23-Jun-04 01:31 sparseml/keras/models/external/__init__.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-Jun-04 01:31 sparseml/keras/models/external/keras_applications.py
--rw-rw-r--  2.0 unx     1166 b- defN 23-Jun-04 01:31 sparseml/keras/optim/__init__.py
--rw-rw-r--  2.0 unx     5677 b- defN 23-Jun-04 01:31 sparseml/keras/optim/manager.py
--rw-rw-r--  2.0 unx    14777 b- defN 23-Jun-04 01:31 sparseml/keras/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    19740 b- defN 23-Jun-04 01:31 sparseml/keras/optim/mask_pruning_creator.py
--rw-rw-r--  2.0 unx     9183 b- defN 23-Jun-04 01:31 sparseml/keras/optim/modifier.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-Jun-04 01:31 sparseml/keras/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    14736 b- defN 23-Jun-04 01:31 sparseml/keras/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     5477 b- defN 23-Jun-04 01:31 sparseml/keras/optim/modifier_params.py
--rw-rw-r--  2.0 unx    24031 b- defN 23-Jun-04 01:31 sparseml/keras/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     1133 b- defN 23-Jun-04 01:31 sparseml/keras/optim/utils.py
--rw-rw-r--  2.0 unx      808 b- defN 23-Jun-04 01:31 sparseml/keras/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1356 b- defN 23-Jun-04 01:31 sparseml/keras/sparsification/info.py
--rw-rw-r--  2.0 unx      962 b- defN 23-Jun-04 01:31 sparseml/keras/utils/__init__.py
--rw-rw-r--  2.0 unx     8202 b- defN 23-Jun-04 01:31 sparseml/keras/utils/callbacks.py
--rw-rw-r--  2.0 unx     1022 b- defN 23-Jun-04 01:31 sparseml/keras/utils/compat.py
--rw-rw-r--  2.0 unx     5737 b- defN 23-Jun-04 01:31 sparseml/keras/utils/exporter.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-Jun-04 01:31 sparseml/keras/utils/logger.py
--rw-rw-r--  2.0 unx     1738 b- defN 23-Jun-04 01:31 sparseml/keras/utils/model.py
--rw-rw-r--  2.0 unx     1036 b- defN 23-Jun-04 01:31 sparseml/onnx/__init__.py
--rw-rw-r--  2.0 unx     6202 b- defN 23-Jun-04 01:31 sparseml/onnx/base.py
--rw-rw-r--  2.0 unx      743 b- defN 23-Jun-04 01:31 sparseml/onnx/benchmark/__init__.py
--rw-rw-r--  2.0 unx    15366 b- defN 23-Jun-04 01:31 sparseml/onnx/benchmark/info.py
--rw-rw-r--  2.0 unx      823 b- defN 23-Jun-04 01:31 sparseml/onnx/framework/__init__.py
--rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-04 01:31 sparseml/onnx/framework/info.py
--rw-rw-r--  2.0 unx      820 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/__init__.py
--rw-rw-r--  2.0 unx    13285 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/analyzer_model.py
--rw-rw-r--  2.0 unx    19639 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx     6470 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/structured_pruning.py
--rw-rw-r--  2.0 unx      815 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/quantization/__init__.py
--rw-rw-r--  2.0 unx    14532 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/quantization/calibration.py
--rw-rw-r--  2.0 unx    73551 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/quantization/quantize.py
--rw-rw-r--  2.0 unx     4552 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/quantization/quantize_model_post_training.py
--rw-rw-r--  2.0 unx      869 b- defN 23-Jun-04 01:31 sparseml/onnx/sparsification/__init__.py
--rw-rw-r--  2.0 unx    10209 b- defN 23-Jun-04 01:31 sparseml/onnx/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-Jun-04 01:31 sparseml/onnx/sparsification/info.py
--rw-rw-r--  2.0 unx     8009 b- defN 23-Jun-04 01:31 sparseml/onnx/sparsification/model_info.py
--rw-rw-r--  2.0 unx      867 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/__init__.py
--rw-rw-r--  2.0 unx    13013 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/data.py
--rw-rw-r--  2.0 unx    16407 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/graph_editor.py
--rw-rw-r--  2.0 unx     8133 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/graph_optimizer.py
--rw-rw-r--  2.0 unx    40230 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/helpers.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/loss.py
--rw-rw-r--  2.0 unx    31591 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/model.py
--rw-rw-r--  2.0 unx     5437 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/sparse_tensor.py
--rw-rw-r--  2.0 unx      931 b- defN 23-Jun-04 01:31 sparseml/openpifpaf/__init__.py
--rw-rw-r--  2.0 unx     3713 b- defN 23-Jun-04 01:31 sparseml/openpifpaf/export.py
--rw-rw-r--  2.0 unx    10950 b- defN 23-Jun-04 01:31 sparseml/openpifpaf/train.py
--rw-rw-r--  2.0 unx     4211 b- defN 23-Jun-04 01:31 sparseml/openpifpaf/trainer.py
--rw-rw-r--  2.0 unx      882 b- defN 23-Jun-04 01:31 sparseml/optim/__init__.py
--rw-rw-r--  2.0 unx     6302 b- defN 23-Jun-04 01:31 sparseml/optim/analyzer.py
--rw-rw-r--  2.0 unx    25563 b- defN 23-Jun-04 01:31 sparseml/optim/helpers.py
--rw-rw-r--  2.0 unx    25984 b- defN 23-Jun-04 01:31 sparseml/optim/manager.py
--rw-rw-r--  2.0 unx    30708 b- defN 23-Jun-04 01:31 sparseml/optim/modifier.py
--rw-rw-r--  2.0 unx    26315 b- defN 23-Jun-04 01:31 sparseml/optim/sensitivity.py
--rw-rw-r--  2.0 unx     1848 b- defN 23-Jun-04 01:31 sparseml/pytorch/__init__.py
--rw-rw-r--  2.0 unx     6173 b- defN 23-Jun-04 01:31 sparseml/pytorch/base.py
--rw-rw-r--  2.0 unx      933 b- defN 23-Jun-04 01:31 sparseml/pytorch/opset.py
--rw-rw-r--  2.0 unx    10864 b- defN 23-Jun-04 01:31 sparseml/pytorch/torch_to_onnx_exporter.py
--rw-rw-r--  2.0 unx      998 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/__init__.py
--rw-rw-r--  2.0 unx     4193 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/generic.py
--rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/registry.py
--rw-rw-r--  2.0 unx      828 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     3669 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4000 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/classification/mnist.py
--rw-rw-r--  2.0 unx      767 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/detection/__init__.py
--rw-rw-r--  2.0 unx    16159 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/detection/coco.py
--rw-rw-r--  2.0 unx     5705 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/detection/helpers.py
--rw-rw-r--  2.0 unx    10759 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/detection/voc.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/image_classification/__init__.py
--rw-rw-r--  2.0 unx     9512 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
--rw-rw-r--  2.0 unx      684 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/recommendation/__init__.py
--rw-rw-r--  2.0 unx      693 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/video/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-Jun-04 01:31 sparseml/pytorch/framework/__init__.py
--rw-rw-r--  2.0 unx     5580 b- defN 23-Jun-04 01:31 sparseml/pytorch/framework/info.py
--rw-rw-r--  2.0 unx      753 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/__init__.py
--rw-rw-r--  2.0 unx    18265 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/export.py
--rw-rw-r--  2.0 unx    15494 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/lr_analysis.py
--rw-rw-r--  2.0 unx    14444 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/pr_sensitivity.py
--rw-rw-r--  2.0 unx    29287 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/train.py
--rw-rw-r--  2.0 unx      682 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/utils/__init__.py
--rw-rw-r--  2.0 unx     4278 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/utils/cli_helpers.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/utils/constants.py
--rw-rw-r--  2.0 unx    20912 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/utils/helpers.py
--rw-rw-r--  2.0 unx    12056 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/utils/trainer.py
--rw-rw-r--  2.0 unx      976 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/registry.py
--rw-rw-r--  2.0 unx      901 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/__init__.py
--rw-rw-r--  2.0 unx    11658 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/darknet.py
--rw-rw-r--  2.0 unx    40293 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/efficientnet.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/inception_v3.py
--rw-rw-r--  2.0 unx     4164 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/mnist.py
--rw-rw-r--  2.0 unx     9546 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    13014 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    40800 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/resnet.py
--rw-rw-r--  2.0 unx    16649 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/vgg.py
--rw-rw-r--  2.0 unx      824 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/detection/__init__.py
--rw-rw-r--  2.0 unx     6820 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/detection/ssd.py
--rw-rw-r--  2.0 unx     8116 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/detection/ssd_lite.py
--rw-rw-r--  2.0 unx     4046 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/detection/ssd_mobilenet.py
--rw-rw-r--  2.0 unx     9069 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/detection/ssd_resnet.py
--rw-rw-r--  2.0 unx    10188 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/detection/yolo_v3.py
--rw-rw-r--  2.0 unx      763 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/external/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/external/torchvision.py
--rw-rw-r--  2.0 unx      676 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/recommendation/__init__.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-04 01:31 sparseml/pytorch/nn/__init__.py
--rw-rw-r--  2.0 unx     8673 b- defN 23-Jun-04 01:31 sparseml/pytorch/nn/activations.py
--rw-rw-r--  2.0 unx    11854 b- defN 23-Jun-04 01:31 sparseml/pytorch/nn/fatrelu.py
--rw-rw-r--  2.0 unx     1690 b- defN 23-Jun-04 01:31 sparseml/pytorch/nn/identity.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-Jun-04 01:31 sparseml/pytorch/nn/se.py
--rw-rw-r--  2.0 unx     1243 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/__init__.py
--rw-rw-r--  2.0 unx    13638 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/analyzer_as.py
--rw-rw-r--  2.0 unx    17069 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/analyzer_pruning.py
--rw-rw-r--  2.0 unx    26838 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/manager.py
--rw-rw-r--  2.0 unx    36844 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    23085 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    10449 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/mask_pruning_scorer.py
--rw-rw-r--  2.0 unx     6605 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/optimizer.py
--rw-rw-r--  2.0 unx    14879 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/sensitivity_as.py
--rw-rw-r--  2.0 unx     6101 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/sensitivity_lr.py
--rw-rw-r--  2.0 unx     9324 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      633 b- defN 23-Jun-04 01:31 sparseml/pytorch/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4534 b- defN 23-Jun-04 01:31 sparseml/pytorch/recipe_template/cli.py
--rw-rw-r--  2.0 unx     1559 b- defN 23-Jun-04 01:31 sparseml/pytorch/recipe_template/description.py
--rw-rw-r--  2.0 unx    15943 b- defN 23-Jun-04 01:31 sparseml/pytorch/recipe_template/main.py
--rw-rw-r--  2.0 unx      992 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1366 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/info.py
--rw-rw-r--  2.0 unx    32014 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/modifier.py
--rw-rw-r--  2.0 unx    18952 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/modifier_thinning.py
--rw-rw-r--  2.0 unx      705 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/distillation/__init__.py
--rw-rw-r--  2.0 unx     4741 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
--rw-rw-r--  2.0 unx    14742 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
--rw-rw-r--  2.0 unx    19177 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
--rw-rw-r--  2.0 unx     1158 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/__init__.py
--rw-rw-r--  2.0 unx    29250 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/mask_creator.py
--rw-rw-r--  2.0 unx    22391 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/mask_params.py
--rw-rw-r--  2.0 unx    13389 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_as.py
--rw-rw-r--  2.0 unx    10455 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
--rw-rw-r--  2.0 unx    33219 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
--rw-rw-r--  2.0 unx     5757 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
--rw-rw-r--  2.0 unx     8860 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
--rw-rw-r--  2.0 unx    15595 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
--rw-rw-r--  2.0 unx    63519 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
--rw-rw-r--  2.0 unx     8774 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
--rw-rw-r--  2.0 unx    24121 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
--rw-rw-r--  2.0 unx    18245 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
--rw-rw-r--  2.0 unx     4644 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/scorer.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/__init__.py
--rw-rw-r--  2.0 unx     2220 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/constants.py
--rw-rw-r--  2.0 unx    32271 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/helpers.py
--rw-rw-r--  2.0 unx    33626 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
--rw-rw-r--  2.0 unx    26778 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
--rw-rw-r--  2.0 unx    12558 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
--rw-rw-r--  2.0 unx    17591 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/quantize.py
--rw-rw-r--  2.0 unx    69997 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/training/__init__.py
--rw-rw-r--  2.0 unx     1778 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/training/modifier_epoch.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/training/modifier_logging.py
--rw-rw-r--  2.0 unx    24287 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/training/modifier_lr.py
--rw-rw-r--  2.0 unx    21497 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/training/modifier_params.py
--rw-rw-r--  2.0 unx     6690 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/training/modifier_regularizer.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jun-04 01:31 sparseml/pytorch/torchvision/__init__.py
--rw-rw-r--  2.0 unx     6490 b- defN 23-Jun-04 01:31 sparseml/pytorch/torchvision/export_onnx.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-Jun-04 01:31 sparseml/pytorch/torchvision/presets.py
--rw-rw-r--  2.0 unx     2530 b- defN 23-Jun-04 01:31 sparseml/pytorch/torchvision/sampler.py
--rw-rw-r--  2.0 unx    41409 b- defN 23-Jun-04 01:31 sparseml/pytorch/torchvision/train.py
--rw-rw-r--  2.0 unx     7128 b- defN 23-Jun-04 01:31 sparseml/pytorch/torchvision/transforms.py
--rw-rw-r--  2.0 unx    16675 b- defN 23-Jun-04 01:31 sparseml/pytorch/torchvision/utils.py
--rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/__init__.py
--rw-rw-r--  2.0 unx     9706 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/benchmarker.py
--rw-rw-r--  2.0 unx     2846 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/callbacks.py
--rw-rw-r--  2.0 unx     1061 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/distributed.py
--rw-rw-r--  2.0 unx    31098 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/exporter.py
--rw-rw-r--  2.0 unx    39284 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/helpers.py
--rw-rw-r--  2.0 unx     1663 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/log_sparsification_info.py
--rw-rw-r--  2.0 unx    31374 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/logger.py
--rw-rw-r--  2.0 unx    27048 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/loss.py
--rw-rw-r--  2.0 unx    11754 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/model.py
--rw-rw-r--  2.0 unx    39117 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/module.py
--rw-rw-r--  2.0 unx     8809 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/sparsification.py
--rw-rw-r--  2.0 unx    30059 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/ssd_helpers.py
--rw-rw-r--  2.0 unx    12337 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/yolo_helpers.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/sparsification_info/__init__.py
--rw-rw-r--  2.0 unx    10457 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/sparsification_info/configs.py
--rw-rw-r--  2.0 unx     4309 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/sparsification_info/helpers.py
--rw-rw-r--  2.0 unx     2946 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
--rw-rw-r--  2.0 unx      655 b- defN 23-Jun-04 01:31 sparseml/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4788 b- defN 23-Jun-04 01:31 sparseml/recipe_template/utils.py
--rw-rw-r--  2.0 unx     1058 b- defN 23-Jun-04 01:31 sparseml/sparsification/__init__.py
--rw-rw-r--  2.0 unx     9387 b- defN 23-Jun-04 01:31 sparseml/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     9065 b- defN 23-Jun-04 01:31 sparseml/sparsification/info.py
--rw-rw-r--  2.0 unx    15565 b- defN 23-Jun-04 01:31 sparseml/sparsification/model_info.py
--rw-rw-r--  2.0 unx     2002 b- defN 23-Jun-04 01:31 sparseml/sparsification/modifier_epoch.py
--rw-rw-r--  2.0 unx    10117 b- defN 23-Jun-04 01:31 sparseml/sparsification/modifier_lr.py
--rw-rw-r--  2.0 unx     5505 b- defN 23-Jun-04 01:31 sparseml/sparsification/modifier_params.py
--rw-rw-r--  2.0 unx    12845 b- defN 23-Jun-04 01:31 sparseml/sparsification/modifier_pruning.py
--rw-rw-r--  2.0 unx     3700 b- defN 23-Jun-04 01:31 sparseml/sparsification/oracle.py
--rw-rw-r--  2.0 unx    18570 b- defN 23-Jun-04 01:31 sparseml/sparsification/recipe_builder.py
--rw-rw-r--  2.0 unx    14413 b- defN 23-Jun-04 01:31 sparseml/sparsification/recipe_editor.py
--rw-rw-r--  2.0 unx     1250 b- defN 23-Jun-04 01:31 sparseml/sparsification/types.py
--rw-rw-r--  2.0 unx      987 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/__init__.py
--rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/base.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/__init__.py
--rw-rw-r--  2.0 unx     8121 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/dataset.py
--rw-rw-r--  2.0 unx     5600 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/helpers.py
--rw-rw-r--  2.0 unx     2768 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/registry.py
--rw-rw-r--  2.0 unx      807 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx    12686 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     8690 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     4695 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      805 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/framework/__init__.py
--rw-rw-r--  2.0 unx     5859 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/framework/info.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/__init__.py
--rw-rw-r--  2.0 unx    19752 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/estimator.py
--rw-rw-r--  2.0 unx    14774 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/registry.py
--rw-rw-r--  2.0 unx      822 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/classification/__init__.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/classification/mnist.py
--rw-rw-r--  2.0 unx    11161 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    18359 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    28103 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/classification/resnet.py
--rw-rw-r--  2.0 unx    26886 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/classification/vgg.py
--rw-rw-r--  2.0 unx      865 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/nn/__init__.py
--rw-rw-r--  2.0 unx    18670 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/nn/layers.py
--rw-rw-r--  2.0 unx     1238 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/__init__.py
--rw-rw-r--  2.0 unx     8607 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     9591 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/manager.py
--rw-rw-r--  2.0 unx    19683 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    33919 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    15955 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/modifier.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    10685 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     7092 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/modifier_params.py
--rw-rw-r--  2.0 unx    15702 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/schedule_lr.py
--rw-rw-r--  2.0 unx     9232 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1385 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/sparsification/info.py
--rw-rw-r--  2.0 unx      967 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/utils/__init__.py
--rw-rw-r--  2.0 unx    10913 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/utils/exporter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/utils/helpers.py
--rw-rw-r--  2.0 unx     1974 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/utils/loss.py
--rw-rw-r--  2.0 unx     8119 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/utils/nets_utils.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/utils/summary.py
--rw-rw-r--  2.0 unx    12536 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/utils/variable.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-04 01:31 sparseml/transformers/__init__.py
--rw-rw-r--  2.0 unx    21274 b- defN 23-Jun-04 01:31 sparseml/transformers/export.py
--rw-rw-r--  2.0 unx    30756 b- defN 23-Jun-04 01:31 sparseml/transformers/masked_language_modeling.py
--rw-rw-r--  2.0 unx    36557 b- defN 23-Jun-04 01:31 sparseml/transformers/question_answering.py
--rw-rw-r--  2.0 unx    40299 b- defN 23-Jun-04 01:31 sparseml/transformers/text_classification.py
--rw-rw-r--  2.0 unx    34350 b- defN 23-Jun-04 01:31 sparseml/transformers/token_classification.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jun-04 01:31 sparseml/transformers/sparsification/__init__.py
--rw-rw-r--  2.0 unx    19529 b- defN 23-Jun-04 01:31 sparseml/transformers/sparsification/question_answering.py
--rw-rw-r--  2.0 unx    43772 b- defN 23-Jun-04 01:31 sparseml/transformers/sparsification/trainer.py
--rw-rw-r--  2.0 unx     1890 b- defN 23-Jun-04 01:31 sparseml/transformers/sparsification/training_args.py
--rw-rw-r--  2.0 unx      794 b- defN 23-Jun-04 01:31 sparseml/transformers/utils/__init__.py
--rw-rw-r--  2.0 unx     3090 b- defN 23-Jun-04 01:31 sparseml/transformers/utils/helpers.py
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-04 01:31 sparseml/transformers/utils/metrics.py
--rw-rw-r--  2.0 unx    17072 b- defN 23-Jun-04 01:31 sparseml/transformers/utils/model.py
--rw-rw-r--  2.0 unx      844 b- defN 23-Jun-04 01:31 sparseml/utils/__init__.py
--rw-rw-r--  2.0 unx      886 b- defN 23-Jun-04 01:31 sparseml/utils/frameworks.py
--rw-rw-r--  2.0 unx    26321 b- defN 23-Jun-04 01:31 sparseml/utils/helpers.py
--rw-rw-r--  2.0 unx     3983 b- defN 23-Jun-04 01:31 sparseml/utils/restricted_eval.py
--rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-04 01:31 sparseml/utils/singleton.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-Jun-04 01:31 sparseml/utils/worker.py
--rw-rw-r--  2.0 unx     2952 b- defN 23-Jun-04 01:31 sparseml/utils/wrapper.py
--rw-rw-r--  2.0 unx      819 b- defN 23-Jun-04 01:31 sparseml/utils/datasets/__init__.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jun-04 01:31 sparseml/utils/datasets/cifar.py
--rw-rw-r--  2.0 unx     3750 b- defN 23-Jun-04 01:31 sparseml/utils/datasets/coco.py
--rw-rw-r--  2.0 unx     1217 b- defN 23-Jun-04 01:31 sparseml/utils/datasets/helpers.py
--rw-rw-r--  2.0 unx    23366 b- defN 23-Jun-04 01:31 sparseml/utils/datasets/imagenet.py
--rw-rw-r--  2.0 unx     8967 b- defN 23-Jun-04 01:31 sparseml/utils/datasets/imagenette.py
--rw-rw-r--  2.0 unx     1009 b- defN 23-Jun-04 01:31 sparseml/utils/datasets/voc.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-Jun-04 01:31 sparseml/yolact/COCO.sh
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-04 01:31 sparseml/yolact/COCO_test.sh
--rw-rw-r--  2.0 unx     4020 b- defN 23-Jun-04 01:31 sparseml/yolact/__init__.py
--rw-rw-r--  2.0 unx     1784 b- defN 23-Jun-04 01:31 sparseml/yolact/scripts.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-04 01:31 sparseml/yolov5/__init__.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-04 01:31 sparseml/yolov5/helpers.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-Jun-04 01:31 sparseml/yolov5/scripts.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-Jun-04 01:31 sparseml/yolov5/yolov5.status.yaml
--rw-rw-r--  2.0 unx     1115 b- defN 23-Jun-04 01:31 sparseml/yolov8/__init__.py
--rw-rw-r--  2.0 unx     5781 b- defN 23-Jun-04 01:31 sparseml/yolov8/default.yaml
--rw-rw-r--  2.0 unx     2502 b- defN 23-Jun-04 01:31 sparseml/yolov8/export.py
--rw-rw-r--  2.0 unx     2259 b- defN 23-Jun-04 01:31 sparseml/yolov8/modules.py
--rw-rw-r--  2.0 unx     7194 b- defN 23-Jun-04 01:31 sparseml/yolov8/train.py
--rw-rw-r--  2.0 unx    34788 b- defN 23-Jun-04 01:31 sparseml/yolov8/trainers.py
--rw-rw-r--  2.0 unx     2748 b- defN 23-Jun-04 01:31 sparseml/yolov8/val.py
--rw-rw-r--  2.0 unx     8196 b- defN 23-Jun-04 01:31 sparseml/yolov8/validators.py
--rw-rw-r--  2.0 unx      685 b- defN 23-Jun-04 01:31 sparseml/yolov8/utils/__init__.py
--rw-rw-r--  2.0 unx     6288 b- defN 23-Jun-04 01:31 sparseml/yolov8/utils/export_samples.py
--rw-rw-r--  2.0 unx     4041 b- defN 23-Jun-04 01:31 sparseml/yolov8/utils/helpers.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-04 01:33 sparseml_nightly-1.6.0.20230604.dist-info/LICENSE
--rw-rw-r--  2.0 unx    21640 b- defN 23-Jun-04 01:33 sparseml_nightly-1.6.0.20230604.dist-info/METADATA
--rw-rw-r--  2.0 unx     2158 b- defN 23-Jun-04 01:33 sparseml_nightly-1.6.0.20230604.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-04 01:33 sparseml_nightly-1.6.0.20230604.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2377 b- defN 23-Jun-04 01:33 sparseml_nightly-1.6.0.20230604.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-04 01:33 sparseml_nightly-1.6.0.20230604.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    36576 b- defN 23-Jun-04 01:33 sparseml_nightly-1.6.0.20230604.dist-info/RECORD
-368 files, 3426892 bytes uncompressed, 887344 bytes compressed:  74.1%
+Zip file size: 946842 bytes, number of entries: 368
+-rw-rw-r--  2.0 unx     1413 b- defN 23-Jun-08 01:31 sparseml/__init__.py
+-rw-rw-r--  2.0 unx      898 b- defN 23-Jun-08 01:31 sparseml/analytics.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-Jun-08 01:31 sparseml/base.py
+-rw-rw-r--  2.0 unx     2483 b- defN 23-Jun-08 01:31 sparseml/log.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-08 01:31 sparseml/version.py
+-rw-rw-r--  2.0 unx      758 b- defN 23-Jun-08 01:31 sparseml/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    17631 b- defN 23-Jun-08 01:31 sparseml/benchmark/info.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-Jun-08 01:31 sparseml/benchmark/serialization.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Jun-08 01:31 sparseml/deepsparse/__init__.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-Jun-08 01:31 sparseml/deepsparse/base.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jun-08 01:31 sparseml/deepsparse/framework/__init__.py
+-rw-rw-r--  2.0 unx     6032 b- defN 23-Jun-08 01:31 sparseml/deepsparse/framework/info.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jun-08 01:31 sparseml/deepsparse/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Jun-08 01:31 sparseml/deepsparse/sparsification/info.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-08 01:31 sparseml/exporters/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-Jun-08 01:31 sparseml/exporters/base_exporter.py
+-rw-rw-r--  2.0 unx     4783 b- defN 23-Jun-08 01:31 sparseml/exporters/onnx_to_deepsparse.py
+-rw-rw-r--  2.0 unx     2252 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/base_transform.py
+-rw-rw-r--  2.0 unx     1388 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/constants_to_initializers.py
+-rw-rw-r--  2.0 unx     3866 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     5838 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/conv_to_qlinearconv.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/delete_repeated_qdq.py
+-rw-rw-r--  2.0 unx     1842 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/flatten_qparams.py
+-rw-rw-r--  2.0 unx     3553 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/fold_conv_div_bn.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/fold_identity_initializers.py
+-rw-rw-r--  2.0 unx     2070 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/fold_relu_quants.py
+-rw-rw-r--  2.0 unx     4418 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     7629 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     1645 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/initializers_to_uint8.py
+-rw-rw-r--  2.0 unx     4470 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     4571 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
+-rw-rw-r--  2.0 unx     4156 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/onnx_transform.py
+-rw-rw-r--  2.0 unx     3398 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/propagate_embedding_quantization.py
+-rw-rw-r--  2.0 unx     4464 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/quantize_qat_embedding.py
+-rw-rw-r--  2.0 unx     3869 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/quantize_residuals.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
+-rw-rw-r--  2.0 unx     3210 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/skip_input_quantize.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/unwrap_batchnorms.py
+-rw-rw-r--  2.0 unx      730 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/utils/__init__.py
+-rw-rw-r--  2.0 unx     8704 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
+-rw-rw-r--  2.0 unx     6457 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/utils/helpers.py
+-rw-rw-r--  2.0 unx    14429 b- defN 23-Jun-08 01:31 sparseml/exporters/transforms/utils/matching.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jun-08 01:31 sparseml/framework/__init__.py
+-rw-rw-r--  2.0 unx     9479 b- defN 23-Jun-08 01:31 sparseml/framework/info.py
+-rw-rw-r--  2.0 unx     1144 b- defN 23-Jun-08 01:31 sparseml/keras/__init__.py
+-rw-rw-r--  2.0 unx     8054 b- defN 23-Jun-08 01:31 sparseml/keras/base.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2761 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/registry.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4301 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-08 01:31 sparseml/keras/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      793 b- defN 23-Jun-08 01:31 sparseml/keras/framework/__init__.py
+-rw-rw-r--  2.0 unx     5906 b- defN 23-Jun-08 01:31 sparseml/keras/framework/info.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-Jun-08 01:31 sparseml/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    11814 b- defN 23-Jun-08 01:31 sparseml/keras/models/registry.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jun-08 01:31 sparseml/keras/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    17932 b- defN 23-Jun-08 01:31 sparseml/keras/models/classification/resnet.py
+-rw-rw-r--  2.0 unx      768 b- defN 23-Jun-08 01:31 sparseml/keras/models/external/__init__.py
+-rw-rw-r--  2.0 unx     4402 b- defN 23-Jun-08 01:31 sparseml/keras/models/external/keras_applications.py
+-rw-rw-r--  2.0 unx     1166 b- defN 23-Jun-08 01:31 sparseml/keras/optim/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 23-Jun-08 01:31 sparseml/keras/optim/manager.py
+-rw-rw-r--  2.0 unx    14777 b- defN 23-Jun-08 01:31 sparseml/keras/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    19740 b- defN 23-Jun-08 01:31 sparseml/keras/optim/mask_pruning_creator.py
+-rw-rw-r--  2.0 unx     9183 b- defN 23-Jun-08 01:31 sparseml/keras/optim/modifier.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Jun-08 01:31 sparseml/keras/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    14736 b- defN 23-Jun-08 01:31 sparseml/keras/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     5477 b- defN 23-Jun-08 01:31 sparseml/keras/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    24031 b- defN 23-Jun-08 01:31 sparseml/keras/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     1133 b- defN 23-Jun-08 01:31 sparseml/keras/optim/utils.py
+-rw-rw-r--  2.0 unx      808 b- defN 23-Jun-08 01:31 sparseml/keras/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-Jun-08 01:31 sparseml/keras/sparsification/info.py
+-rw-rw-r--  2.0 unx      962 b- defN 23-Jun-08 01:31 sparseml/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx     8202 b- defN 23-Jun-08 01:31 sparseml/keras/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1022 b- defN 23-Jun-08 01:31 sparseml/keras/utils/compat.py
+-rw-rw-r--  2.0 unx     5737 b- defN 23-Jun-08 01:31 sparseml/keras/utils/exporter.py
+-rw-rw-r--  2.0 unx     6087 b- defN 23-Jun-08 01:31 sparseml/keras/utils/logger.py
+-rw-rw-r--  2.0 unx     1738 b- defN 23-Jun-08 01:31 sparseml/keras/utils/model.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-Jun-08 01:31 sparseml/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-Jun-08 01:31 sparseml/onnx/base.py
+-rw-rw-r--  2.0 unx      743 b- defN 23-Jun-08 01:31 sparseml/onnx/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    15366 b- defN 23-Jun-08 01:31 sparseml/onnx/benchmark/info.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-Jun-08 01:31 sparseml/onnx/framework/__init__.py
+-rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-08 01:31 sparseml/onnx/framework/info.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/__init__.py
+-rw-rw-r--  2.0 unx    13285 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/analyzer_model.py
+-rw-rw-r--  2.0 unx    19639 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/structured_pruning.py
+-rw-rw-r--  2.0 unx      815 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/quantization/__init__.py
+-rw-rw-r--  2.0 unx    14532 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/quantization/calibration.py
+-rw-rw-r--  2.0 unx    73551 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/quantization/quantize.py
+-rw-rw-r--  2.0 unx     4552 b- defN 23-Jun-08 01:31 sparseml/onnx/optim/quantization/quantize_model_post_training.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-Jun-08 01:31 sparseml/onnx/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 23-Jun-08 01:31 sparseml/onnx/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-Jun-08 01:31 sparseml/onnx/sparsification/info.py
+-rw-rw-r--  2.0 unx     8009 b- defN 23-Jun-08 01:31 sparseml/onnx/sparsification/model_info.py
+-rw-rw-r--  2.0 unx      867 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/__init__.py
+-rw-rw-r--  2.0 unx    13013 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/data.py
+-rw-rw-r--  2.0 unx    16407 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/graph_editor.py
+-rw-rw-r--  2.0 unx     8133 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/graph_optimizer.py
+-rw-rw-r--  2.0 unx    40230 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/helpers.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/loss.py
+-rw-rw-r--  2.0 unx    31591 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/model.py
+-rw-rw-r--  2.0 unx     5437 b- defN 23-Jun-08 01:31 sparseml/onnx/utils/sparse_tensor.py
+-rw-rw-r--  2.0 unx      931 b- defN 23-Jun-08 01:31 sparseml/openpifpaf/__init__.py
+-rw-rw-r--  2.0 unx     3713 b- defN 23-Jun-08 01:31 sparseml/openpifpaf/export.py
+-rw-rw-r--  2.0 unx    10950 b- defN 23-Jun-08 01:31 sparseml/openpifpaf/train.py
+-rw-rw-r--  2.0 unx     4211 b- defN 23-Jun-08 01:31 sparseml/openpifpaf/trainer.py
+-rw-rw-r--  2.0 unx      882 b- defN 23-Jun-08 01:31 sparseml/optim/__init__.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-Jun-08 01:31 sparseml/optim/analyzer.py
+-rw-rw-r--  2.0 unx    25563 b- defN 23-Jun-08 01:31 sparseml/optim/helpers.py
+-rw-rw-r--  2.0 unx    25984 b- defN 23-Jun-08 01:31 sparseml/optim/manager.py
+-rw-rw-r--  2.0 unx    30708 b- defN 23-Jun-08 01:31 sparseml/optim/modifier.py
+-rw-rw-r--  2.0 unx    26315 b- defN 23-Jun-08 01:31 sparseml/optim/sensitivity.py
+-rw-rw-r--  2.0 unx     1848 b- defN 23-Jun-08 01:31 sparseml/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     6173 b- defN 23-Jun-08 01:31 sparseml/pytorch/base.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-Jun-08 01:31 sparseml/pytorch/opset.py
+-rw-rw-r--  2.0 unx    10864 b- defN 23-Jun-08 01:31 sparseml/pytorch/torch_to_onnx_exporter.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4193 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/generic.py
+-rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/registry.py
+-rw-rw-r--  2.0 unx      828 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     3669 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4000 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/classification/mnist.py
+-rw-rw-r--  2.0 unx      767 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/detection/__init__.py
+-rw-rw-r--  2.0 unx    16159 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/detection/coco.py
+-rw-rw-r--  2.0 unx     5705 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/detection/helpers.py
+-rw-rw-r--  2.0 unx    10759 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/detection/voc.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/image_classification/__init__.py
+-rw-rw-r--  2.0 unx     9512 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      693 b- defN 23-Jun-08 01:31 sparseml/pytorch/datasets/video/__init__.py
+-rw-rw-r--  2.0 unx      814 b- defN 23-Jun-08 01:31 sparseml/pytorch/framework/__init__.py
+-rw-rw-r--  2.0 unx     5580 b- defN 23-Jun-08 01:31 sparseml/pytorch/framework/info.py
+-rw-rw-r--  2.0 unx      753 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/__init__.py
+-rw-rw-r--  2.0 unx    18265 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/export.py
+-rw-rw-r--  2.0 unx    15494 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/lr_analysis.py
+-rw-rw-r--  2.0 unx    14444 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/pr_sensitivity.py
+-rw-rw-r--  2.0 unx    29287 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/train.py
+-rw-rw-r--  2.0 unx      682 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/utils/__init__.py
+-rw-rw-r--  2.0 unx     4278 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/utils/cli_helpers.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/utils/constants.py
+-rw-rw-r--  2.0 unx    20912 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/utils/helpers.py
+-rw-rw-r--  2.0 unx    12056 b- defN 23-Jun-08 01:31 sparseml/pytorch/image_classification/utils/trainer.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/registry.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/darknet.py
+-rw-rw-r--  2.0 unx    40293 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/efficientnet.py
+-rw-rw-r--  2.0 unx    16512 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/inception_v3.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/mnist.py
+-rw-rw-r--  2.0 unx     9546 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    13014 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    40800 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    16649 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      824 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/detection/__init__.py
+-rw-rw-r--  2.0 unx     6820 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/detection/ssd.py
+-rw-rw-r--  2.0 unx     8116 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/detection/ssd_lite.py
+-rw-rw-r--  2.0 unx     4046 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/detection/ssd_mobilenet.py
+-rw-rw-r--  2.0 unx     9069 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/detection/ssd_resnet.py
+-rw-rw-r--  2.0 unx    10188 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/detection/yolo_v3.py
+-rw-rw-r--  2.0 unx      763 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/external/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/external/torchvision.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-Jun-08 01:31 sparseml/pytorch/models/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-08 01:31 sparseml/pytorch/nn/__init__.py
+-rw-rw-r--  2.0 unx     8673 b- defN 23-Jun-08 01:31 sparseml/pytorch/nn/activations.py
+-rw-rw-r--  2.0 unx    11854 b- defN 23-Jun-08 01:31 sparseml/pytorch/nn/fatrelu.py
+-rw-rw-r--  2.0 unx     1690 b- defN 23-Jun-08 01:31 sparseml/pytorch/nn/identity.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Jun-08 01:31 sparseml/pytorch/nn/se.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/__init__.py
+-rw-rw-r--  2.0 unx    13638 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/analyzer_as.py
+-rw-rw-r--  2.0 unx    17069 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/analyzer_pruning.py
+-rw-rw-r--  2.0 unx    26838 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/manager.py
+-rw-rw-r--  2.0 unx    36844 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    23085 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    10449 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/mask_pruning_scorer.py
+-rw-rw-r--  2.0 unx     6605 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/optimizer.py
+-rw-rw-r--  2.0 unx    14879 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/sensitivity_as.py
+-rw-rw-r--  2.0 unx     6101 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/sensitivity_lr.py
+-rw-rw-r--  2.0 unx     9324 b- defN 23-Jun-08 01:31 sparseml/pytorch/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-Jun-08 01:31 sparseml/pytorch/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4534 b- defN 23-Jun-08 01:31 sparseml/pytorch/recipe_template/cli.py
+-rw-rw-r--  2.0 unx     1559 b- defN 23-Jun-08 01:31 sparseml/pytorch/recipe_template/description.py
+-rw-rw-r--  2.0 unx    15943 b- defN 23-Jun-08 01:31 sparseml/pytorch/recipe_template/main.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1366 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/info.py
+-rw-rw-r--  2.0 unx    32014 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/modifier.py
+-rw-rw-r--  2.0 unx    18952 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/modifier_thinning.py
+-rw-rw-r--  2.0 unx      705 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/distillation/__init__.py
+-rw-rw-r--  2.0 unx     4741 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
+-rw-rw-r--  2.0 unx    14742 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
+-rw-rw-r--  2.0 unx    19177 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/__init__.py
+-rw-rw-r--  2.0 unx    29250 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/mask_creator.py
+-rw-rw-r--  2.0 unx    22391 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/mask_params.py
+-rw-rw-r--  2.0 unx    13389 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_as.py
+-rw-rw-r--  2.0 unx    10455 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
+-rw-rw-r--  2.0 unx    33219 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
+-rw-rw-r--  2.0 unx     8860 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
+-rw-rw-r--  2.0 unx    15595 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
+-rw-rw-r--  2.0 unx    63519 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
+-rw-rw-r--  2.0 unx     8774 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
+-rw-rw-r--  2.0 unx    24121 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
+-rw-rw-r--  2.0 unx    18245 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
+-rw-rw-r--  2.0 unx     4644 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/pruning/scorer.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/__init__.py
+-rw-rw-r--  2.0 unx     2220 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/constants.py
+-rw-rw-r--  2.0 unx    32271 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/helpers.py
+-rw-rw-r--  2.0 unx    33626 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
+-rw-rw-r--  2.0 unx    26778 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
+-rw-rw-r--  2.0 unx    12558 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
+-rw-rw-r--  2.0 unx    17905 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/quantize.py
+-rw-rw-r--  2.0 unx    70029 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/training/__init__.py
+-rw-rw-r--  2.0 unx     1778 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/training/modifier_epoch.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/training/modifier_logging.py
+-rw-rw-r--  2.0 unx    24287 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/training/modifier_lr.py
+-rw-rw-r--  2.0 unx    21497 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/training/modifier_params.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-Jun-08 01:31 sparseml/pytorch/sparsification/training/modifier_regularizer.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jun-08 01:31 sparseml/pytorch/torchvision/__init__.py
+-rw-rw-r--  2.0 unx     6490 b- defN 23-Jun-08 01:31 sparseml/pytorch/torchvision/export_onnx.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-Jun-08 01:31 sparseml/pytorch/torchvision/presets.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-Jun-08 01:31 sparseml/pytorch/torchvision/sampler.py
+-rw-rw-r--  2.0 unx    41409 b- defN 23-Jun-08 01:31 sparseml/pytorch/torchvision/train.py
+-rw-rw-r--  2.0 unx     7128 b- defN 23-Jun-08 01:31 sparseml/pytorch/torchvision/transforms.py
+-rw-rw-r--  2.0 unx    16675 b- defN 23-Jun-08 01:31 sparseml/pytorch/torchvision/utils.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/__init__.py
+-rw-rw-r--  2.0 unx     9706 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/benchmarker.py
+-rw-rw-r--  2.0 unx     2846 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/distributed.py
+-rw-rw-r--  2.0 unx    31098 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/exporter.py
+-rw-rw-r--  2.0 unx    39284 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/helpers.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/log_sparsification_info.py
+-rw-rw-r--  2.0 unx    31374 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/logger.py
+-rw-rw-r--  2.0 unx    27048 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/loss.py
+-rw-rw-r--  2.0 unx    11754 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/model.py
+-rw-rw-r--  2.0 unx    39117 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/module.py
+-rw-rw-r--  2.0 unx     8809 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/sparsification.py
+-rw-rw-r--  2.0 unx    30059 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/ssd_helpers.py
+-rw-rw-r--  2.0 unx    12337 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/yolo_helpers.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/sparsification_info/__init__.py
+-rw-rw-r--  2.0 unx    10457 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/sparsification_info/configs.py
+-rw-rw-r--  2.0 unx     4309 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/sparsification_info/helpers.py
+-rw-rw-r--  2.0 unx     2946 b- defN 23-Jun-08 01:31 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Jun-08 01:31 sparseml/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-Jun-08 01:31 sparseml/recipe_template/utils.py
+-rw-rw-r--  2.0 unx     1058 b- defN 23-Jun-08 01:31 sparseml/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     9387 b- defN 23-Jun-08 01:31 sparseml/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-Jun-08 01:31 sparseml/sparsification/info.py
+-rw-rw-r--  2.0 unx    15565 b- defN 23-Jun-08 01:31 sparseml/sparsification/model_info.py
+-rw-rw-r--  2.0 unx     2002 b- defN 23-Jun-08 01:31 sparseml/sparsification/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10117 b- defN 23-Jun-08 01:31 sparseml/sparsification/modifier_lr.py
+-rw-rw-r--  2.0 unx     5505 b- defN 23-Jun-08 01:31 sparseml/sparsification/modifier_params.py
+-rw-rw-r--  2.0 unx    12845 b- defN 23-Jun-08 01:31 sparseml/sparsification/modifier_pruning.py
+-rw-rw-r--  2.0 unx     3700 b- defN 23-Jun-08 01:31 sparseml/sparsification/oracle.py
+-rw-rw-r--  2.0 unx    18570 b- defN 23-Jun-08 01:31 sparseml/sparsification/recipe_builder.py
+-rw-rw-r--  2.0 unx    14413 b- defN 23-Jun-08 01:31 sparseml/sparsification/recipe_editor.py
+-rw-rw-r--  2.0 unx     1250 b- defN 23-Jun-08 01:31 sparseml/sparsification/types.py
+-rw-rw-r--  2.0 unx     1169 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/base.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/__init__.py
+-rw-rw-r--  2.0 unx     8121 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/dataset.py
+-rw-rw-r--  2.0 unx     5600 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2768 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/registry.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx    12686 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     8690 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     4695 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      805 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/framework/__init__.py
+-rw-rw-r--  2.0 unx     5859 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/framework/info.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/__init__.py
+-rw-rw-r--  2.0 unx    19752 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/estimator.py
+-rw-rw-r--  2.0 unx    14774 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/registry.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/classification/__init__.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/classification/mnist.py
+-rw-rw-r--  2.0 unx    11161 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    18359 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    28103 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    26886 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      865 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/nn/__init__.py
+-rw-rw-r--  2.0 unx    18670 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/nn/layers.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/__init__.py
+-rw-rw-r--  2.0 unx     8607 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     9591 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/manager.py
+-rw-rw-r--  2.0 unx    19683 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    33919 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    15955 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/modifier.py
+-rw-rw-r--  2.0 unx     1715 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10685 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     7092 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    15702 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     5682 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/schedule_lr.py
+-rw-rw-r--  2.0 unx     9232 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1385 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/sparsification/info.py
+-rw-rw-r--  2.0 unx      967 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/utils/__init__.py
+-rw-rw-r--  2.0 unx    10913 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/utils/exporter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/utils/helpers.py
+-rw-rw-r--  2.0 unx     1974 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/utils/loss.py
+-rw-rw-r--  2.0 unx     8119 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/utils/nets_utils.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/utils/summary.py
+-rw-rw-r--  2.0 unx    12536 b- defN 23-Jun-08 01:31 sparseml/tensorflow_v1/utils/variable.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-08 01:31 sparseml/transformers/__init__.py
+-rw-rw-r--  2.0 unx    21274 b- defN 23-Jun-08 01:31 sparseml/transformers/export.py
+-rw-rw-r--  2.0 unx    30756 b- defN 23-Jun-08 01:31 sparseml/transformers/masked_language_modeling.py
+-rw-rw-r--  2.0 unx    36557 b- defN 23-Jun-08 01:31 sparseml/transformers/question_answering.py
+-rw-rw-r--  2.0 unx    40299 b- defN 23-Jun-08 01:31 sparseml/transformers/text_classification.py
+-rw-rw-r--  2.0 unx    34350 b- defN 23-Jun-08 01:31 sparseml/transformers/token_classification.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jun-08 01:31 sparseml/transformers/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    19529 b- defN 23-Jun-08 01:31 sparseml/transformers/sparsification/question_answering.py
+-rw-rw-r--  2.0 unx    43772 b- defN 23-Jun-08 01:31 sparseml/transformers/sparsification/trainer.py
+-rw-rw-r--  2.0 unx     1890 b- defN 23-Jun-08 01:31 sparseml/transformers/sparsification/training_args.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-Jun-08 01:31 sparseml/transformers/utils/__init__.py
+-rw-rw-r--  2.0 unx     3090 b- defN 23-Jun-08 01:31 sparseml/transformers/utils/helpers.py
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-08 01:31 sparseml/transformers/utils/metrics.py
+-rw-rw-r--  2.0 unx    17072 b- defN 23-Jun-08 01:31 sparseml/transformers/utils/model.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Jun-08 01:31 sparseml/utils/__init__.py
+-rw-rw-r--  2.0 unx      886 b- defN 23-Jun-08 01:31 sparseml/utils/frameworks.py
+-rw-rw-r--  2.0 unx    26562 b- defN 23-Jun-08 01:31 sparseml/utils/helpers.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-Jun-08 01:31 sparseml/utils/restricted_eval.py
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-08 01:31 sparseml/utils/singleton.py
+-rw-rw-r--  2.0 unx     6312 b- defN 23-Jun-08 01:31 sparseml/utils/worker.py
+-rw-rw-r--  2.0 unx     2952 b- defN 23-Jun-08 01:31 sparseml/utils/wrapper.py
+-rw-rw-r--  2.0 unx      819 b- defN 23-Jun-08 01:31 sparseml/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jun-08 01:31 sparseml/utils/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-Jun-08 01:31 sparseml/utils/datasets/coco.py
+-rw-rw-r--  2.0 unx     1217 b- defN 23-Jun-08 01:31 sparseml/utils/datasets/helpers.py
+-rw-rw-r--  2.0 unx    23366 b- defN 23-Jun-08 01:31 sparseml/utils/datasets/imagenet.py
+-rw-rw-r--  2.0 unx     8967 b- defN 23-Jun-08 01:31 sparseml/utils/datasets/imagenette.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-Jun-08 01:31 sparseml/utils/datasets/voc.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Jun-08 01:31 sparseml/yolact/COCO.sh
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-08 01:31 sparseml/yolact/COCO_test.sh
+-rw-rw-r--  2.0 unx     4020 b- defN 23-Jun-08 01:31 sparseml/yolact/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Jun-08 01:31 sparseml/yolact/scripts.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-08 01:31 sparseml/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-08 01:31 sparseml/yolov5/helpers.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-Jun-08 01:31 sparseml/yolov5/scripts.py
+-rw-rw-r--  2.0 unx     1220 b- defN 23-Jun-08 01:31 sparseml/yolov5/yolov5.status.yaml
+-rw-rw-r--  2.0 unx     1115 b- defN 23-Jun-08 01:31 sparseml/yolov8/__init__.py
+-rw-rw-r--  2.0 unx     5781 b- defN 23-Jun-08 01:31 sparseml/yolov8/default.yaml
+-rw-rw-r--  2.0 unx     2502 b- defN 23-Jun-08 01:31 sparseml/yolov8/export.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-Jun-08 01:31 sparseml/yolov8/modules.py
+-rw-rw-r--  2.0 unx     7194 b- defN 23-Jun-08 01:31 sparseml/yolov8/train.py
+-rw-rw-r--  2.0 unx    34788 b- defN 23-Jun-08 01:31 sparseml/yolov8/trainers.py
+-rw-rw-r--  2.0 unx     2748 b- defN 23-Jun-08 01:31 sparseml/yolov8/val.py
+-rw-rw-r--  2.0 unx     8196 b- defN 23-Jun-08 01:31 sparseml/yolov8/validators.py
+-rw-rw-r--  2.0 unx      685 b- defN 23-Jun-08 01:31 sparseml/yolov8/utils/__init__.py
+-rw-rw-r--  2.0 unx     6288 b- defN 23-Jun-08 01:31 sparseml/yolov8/utils/export_samples.py
+-rw-rw-r--  2.0 unx     4041 b- defN 23-Jun-08 01:31 sparseml/yolov8/utils/helpers.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-08 01:33 sparseml_nightly-1.6.0.20230608.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    21640 b- defN 23-Jun-08 01:33 sparseml_nightly-1.6.0.20230608.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2158 b- defN 23-Jun-08 01:33 sparseml_nightly-1.6.0.20230608.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-08 01:33 sparseml_nightly-1.6.0.20230608.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2377 b- defN 23-Jun-08 01:33 sparseml_nightly-1.6.0.20230608.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-08 01:33 sparseml_nightly-1.6.0.20230608.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    36578 b- defN 23-Jun-08 01:33 sparseml_nightly-1.6.0.20230608.dist-info/RECORD
+368 files, 3427837 bytes uncompressed, 887634 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1077,29 +1077,29 @@
 
 Filename: sparseml/yolov8/utils/export_samples.py
 Comment: 
 
 Filename: sparseml/yolov8/utils/helpers.py
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230604.dist-info/LICENSE
+Filename: sparseml_nightly-1.6.0.20230608.dist-info/LICENSE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230604.dist-info/METADATA
+Filename: sparseml_nightly-1.6.0.20230608.dist-info/METADATA
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230604.dist-info/NOTICE
+Filename: sparseml_nightly-1.6.0.20230608.dist-info/NOTICE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230604.dist-info/WHEEL
+Filename: sparseml_nightly-1.6.0.20230608.dist-info/WHEEL
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230604.dist-info/entry_points.txt
+Filename: sparseml_nightly-1.6.0.20230608.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230604.dist-info/top_level.txt
+Filename: sparseml_nightly-1.6.0.20230608.dist-info/top_level.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230604.dist-info/RECORD
+Filename: sparseml_nightly-1.6.0.20230608.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparseml/keras/__init__.py

```diff
@@ -14,14 +14,21 @@
 
 """
 Functionality for working with and sparsifying Models in the Keras framework
 """
 
 # flake8: noqa
 
+from sparseml.utils import deprecation_warning as _deprecation_warning
+
+
+_deprecation_warning(
+    "sparseml.keras is deprecated and will be removed in a future version",
+)
+
 from sparseml.analytics import sparseml_analytics as _analytics
 
 from .base import *
 from .framework import detect_framework, framework_info, is_supported
 from .sparsification import sparsification_info
```

## sparseml/pytorch/sparsification/quantization/quantize.py

```diff
@@ -357,18 +357,21 @@
     submodule: Module, submodule_name: str, names_or_types: List[str]
 ) -> Optional[str]:
     # match preferences:
     #   1. match module type name
     #   2. match the submodule prefix (longest first)
     submodule_match = ""
     for name_or_type in names_or_types:
+        name_to_compare = submodule_name[:]
+        if name_to_compare.startswith("module."):
+            name_to_compare = name_to_compare[7:]
         if name_or_type == submodule.__class__.__name__:
             # type match, return type name
             return name_or_type
-        if submodule_name.startswith(name_or_type) and (
+        if name_to_compare.startswith(name_or_type) and (
             len(name_or_type) > len(submodule_match)
         ):
             # match to most specific submodule name
             submodule_match = name_or_type
     return submodule_match or None  # return None if no match
 
 
@@ -418,15 +421,18 @@
     ignore: Optional[List[str]] = None,
 ):
     def _get_unmatched_types_or_names(types_or_names):
         unmatched = []
         for type_or_name in types_or_names:
             matched = False
             for submodule_name, submodule in model.named_modules():
-                if submodule_name.startswith(type_or_name) or (
+                name_to_compare = submodule_name[:]
+                if name_to_compare.startswith("module."):
+                    name_to_compare = name_to_compare[7:]
+                if name_to_compare.startswith(type_or_name) or (
                     submodule.__class__.__name__ == type_or_name
                 ):
                     matched = True
                     break
             if not matched:
                 unmatched.append(type_or_name)
         return unmatched
```

## sparseml/pytorch/sparsification/quantization/quantize_qat_export.py

```diff
@@ -739,18 +739,18 @@
 def _add_quantized_conv_matmul_add_ops(
     model: ModelProto,
     node: NodeProto,
     input_quantize_node: NodeProto,
     weight_quantize_node: NodeProto,
     input_quantize_params: QuantizationParams,
     weight_quantize_params: QuantizationParams,
-    bias_initializer: onnx.TensorProto,
-    bias_add_name: str,
     target_output: str,
     transpose_weight: bool,
+    bias_add_name: str,
+    bias_initializer: Optional[onnx.TensorProto] = None,
     output_quantize_node: Optional[NodeProto] = None,
     output_dequantize_node: Optional[NodeProto] = None,
 ):
     # helper function for conversion of qat parameterized gemms, matmuls,
     # or convs to conv/matmul integer add blocks.
     # Adds new quantized ops to graph, does not
     # perform any checks or deletions (should be called by the operator main
@@ -802,85 +802,82 @@
             "MatMulInteger",
             integer_op_inputs,
             [integer_op_output],
             integer_op_name,
         )
     model.graph.node.append(integer_op_node)
 
-    # Add bias + zero point correction
-    # quantize bias
-    bias_initializer = numpy_helper.to_array(bias_initializer)
-    bias_scale = input_quantize_params.scale * weight_quantize_params.scale
-    bias_zero_point = 0
-    quantized_bias = _quantize_array(
-        bias_initializer, bias_scale, bias_zero_point, dtype=numpy.int32
-    )
-    if node.op_type == "Conv" and len(quantized_bias.shape) == 1:
-        # reshape for bias add broadcasting
-        quantized_bias = quantized_bias.reshape(1, quantized_bias.shape[0], 1, 1)
-
-    quantized_bias_name = "{}.bias_quantized".format(bias_add_name)
-    quantized_bias_initializer = numpy_helper.from_array(
-        quantized_bias, name=quantized_bias_name
-    )
-    model.graph.initializer.append(quantized_bias_initializer)
-    quantized_bias_scale_name = "{}.scale".format(quantized_bias_name)
+    output_scale = input_quantize_params.scale * weight_quantize_params.scale
+    output_scale_name = "{}_output.scale".format(node.name)
     model.graph.initializer.append(
-        numpy_helper.from_array(
-            numpy.asarray(bias_scale), name=quantized_bias_scale_name
-        )
-    )
-    quantized_bias_zero_point_name = "{}.zero_point".format(quantized_bias_name)
-    model.graph.initializer.append(
-        numpy_helper.from_array(
-            numpy.asarray(bias_zero_point, dtype=numpy.uint8),
-            name=quantized_bias_zero_point_name,
-        )
+        numpy_helper.from_array(numpy.asarray(output_scale), name=output_scale_name)
     )
 
-    # get INT32 Add inputs and outputs
-    quant_add_inputs = [
-        integer_op_output,  # MatMul/Conv integer outputs (INT32)
-        quantized_bias_name,  # Quantized bias (INT32)
-    ]
+    last_output = integer_op_output
 
-    quant_add_name = "{}_bias_add_quant".format(node.name)
-    quant_add_output = (
-        output_quantize_node.output[0]
-        if output_quantize_node
-        else f"{quant_add_name}_output"
-    )
+    # Add bias + zero point correction
+    # quantize bias
+    if bias_initializer is not None:
+        bias_initializer = numpy_helper.to_array(bias_initializer)
 
-    # create Add node and add it to graph
-    qadd_node = onnx.helper.make_node(
-        "Add",
-        quant_add_inputs,
-        [quant_add_output],
-        quant_add_name,
-    )
-    model.graph.node.append(qadd_node)
+        bias_zero_point = 0
+        quantized_bias = _quantize_array(
+            bias_initializer, output_scale, bias_zero_point, dtype=numpy.int32
+        )
+        if node.op_type == "Conv" and len(quantized_bias.shape) == 1:
+            # reshape for bias add broadcasting
+            quantized_bias = quantized_bias.reshape(1, quantized_bias.shape[0], 1, 1)
+
+        quantized_bias_name = "{}.bias_quantized".format(bias_add_name)
+        quantized_bias_initializer = numpy_helper.from_array(
+            quantized_bias, name=quantized_bias_name
+        )
+        model.graph.initializer.append(quantized_bias_initializer)
+
+        # get INT32 Add inputs and outputs
+        quant_add_inputs = [
+            last_output,  # MatMul/Conv integer outputs (INT32)
+            quantized_bias_name,  # Quantized bias (INT32)
+        ]
+
+        quant_add_name = "{}_bias_add_quant".format(node.name)
+        quant_add_output = (
+            output_quantize_node.output[0]
+            if output_quantize_node
+            else f"{quant_add_name}_output"
+        )
+
+        # create Add node and add it to graph
+        qadd_node = onnx.helper.make_node(
+            "Add",
+            quant_add_inputs,
+            [quant_add_output],
+            quant_add_name,
+        )
+        model.graph.node.append(qadd_node)
+        last_output = quant_add_output
 
     # create Cast node and add it to graph
-    cast_node_name = "{}_cast".format(quant_add_name)
-    cast_node_output = "{}_cast".format(quant_add_output)
+    cast_node_name = "{}_cast".format(node.name)
+    cast_node_output = "{}_output".format(cast_node_name)
     cast_node = onnx.helper.make_node(
         "Cast",
-        [quant_add_output],
+        [last_output],
         [cast_node_output],
         cast_node_name,
         to=getattr(onnx.TensorProto, "FLOAT"),  # get Float32 enum id
     )
     model.graph.node.append(cast_node)
 
     # create Mul node for rescale
     mul_node_inputs = [
         cast_node_output,  # a
-        quantized_bias_scale_name,  # b -> rescale factor
+        output_scale_name,  # b -> rescale factor
     ]
-    mul_node_name = "{}_rescale_mul".format(quant_add_name)
+    mul_node_name = "{}_rescale_mul".format(cast_node_name)
     mul_node = onnx.helper.make_node(
         "Mul",
         mul_node_inputs,
         [target_output],
         mul_node_name,
     )
     model.graph.node.append(mul_node)
@@ -975,18 +972,18 @@
         _add_quantized_conv_matmul_add_ops(
             model=model,
             node=gemm_node,
             input_quantize_node=input_quantize_node,
             weight_quantize_node=weight_quantize_node,
             input_quantize_params=input_quantize_params,
             weight_quantize_params=weight_quantize_params,
-            bias_initializer=bias_initializer,
-            bias_add_name="{}_bias_add".format(gemm_node.name),
             target_output=gemm_node.output[0],
             transpose_weight=transpose_weight,
+            bias_add_name="{}_bias_add".format(gemm_node.name),
+            bias_initializer=bias_initializer,
         )
 
         # Cleanup
         # delete folded quantization ops
         delete_quant_node(model, weight_dequantize_node)
         delete_quant_node(model, weight_quantize_node)
 
@@ -1104,22 +1101,22 @@
         _add_quantized_conv_matmul_add_ops(
             model=model,
             node=matmul_node,
             input_quantize_node=input_quantize_node,
             weight_quantize_node=weight_quantize_node,
             input_quantize_params=input_quantize_params,
             weight_quantize_params=weight_quantize_params,
-            bias_initializer=bias_initializer,
-            bias_add_name=bias_add_node.name,
             target_output=(
                 output_dequantize_node.output[0]
                 if output_dequantize_node
                 else bias_add_node.output[0]
             ),
             transpose_weight=True,
+            bias_add_name=bias_add_node.name,
+            bias_initializer=bias_initializer,
             output_quantize_node=output_quantize_node,
             output_dequantize_node=output_dequantize_node,
         )
 
         # Cleanup
         # delete folded quantization ops
         delete_quant_node(model, weight_dequantize_node)
@@ -1160,41 +1157,41 @@
     | Starting with:
     |          INPUT         QuantizeLinear (with constant kernel)
     |            |               |
     |     QuantizeLinear     DequantizeLinear
     |            |               |
     |     DequantizeLinear      |
     |                  |      |
-    |                   Conv (with bias)
+    |                   Conv (with optional bias)
     |                     |
     |                  OUTPUT
     | We end up converting to:
     |       INPUT
     |         |
     |     QuantizeLinear
     |         |
     |     ConvInteger (with constant uint8 kernel)
     |         |
-    |     Add (constant bias + zero point correction)
+    |     Add (optional, constant bias + zero point correction)
     |         |
     |     Cast (INT32 -> FP32)
     |         |
     |     Mul (Rescale from bias scale)
     |         |
     |       OUTPUT
     """
 
     conversion_count = 0
     conv_nodes = [n for n in model.graph.node if n.op_type in ["Conv"]]
     orig_conv_weight_name_to_node_ids = defaultdict(list)
     for conv_node in conv_nodes:
-        if len(conv_node.input) != 3:
-            # this function currently only converts Conv nodes with bias param
-            # (i.e. from folded batch norm value)
-            continue
+        # if len(conv_node.input) != 3:
+        #    # this function currently only converts Conv nodes with bias param
+        #    # (i.e. from folded batch norm value)
+        #    continue
 
         graph = ONNXGraph(model)
 
         #############
         # Matching
         #############
         weight_dequantize_node = graph.get_node_single_parent(conv_node, 1)
@@ -1222,33 +1219,36 @@
         )
         if weight_quantize_params.target is None:
             # weight initializer not included
             continue
         if input_quantize_node.op_type != "DequantizeLinear":
             continue
 
-        bias_initializer = graph.get_init_by_name(conv_node.input[2])
-        if bias_initializer is None:
-            _LOGGER.debug(f"Unable to find bias initializer: {conv_node.input[2]}")
-            continue
+        if len(conv_node.input) == 3:
+            bias_initializer = graph.get_init_by_name(conv_node.input[2])
+        else:
+            bias_initializer = None
 
-        _LOGGER.debug(f"Matched quantizable Conv weight and bias: {conv_node.name}")
+        if bias_initializer is None:
+            _LOGGER.debug(f"Matched quantizable Conv weight: {conv_node.name}")
+        else:
+            _LOGGER.debug(f"Matched quantizable Conv weight and bias: {conv_node.name}")
 
         # Conversion
         _add_quantized_conv_matmul_add_ops(
             model=model,
             node=conv_node,
             input_quantize_node=input_quantize_node,
             weight_quantize_node=weight_quantize_node,
             input_quantize_params=input_quantize_params,
             weight_quantize_params=weight_quantize_params,
-            bias_initializer=bias_initializer,
-            bias_add_name="{}_bias_add".format(conv_node.name),
             target_output=conv_node.output[0],
             transpose_weight=False,
+            bias_add_name="{}_bias_add".format(conv_node.name),
+            bias_initializer=bias_initializer,
         )
         orig_conv_weight_name_to_node_ids[input_quantize_node.input[0]].append(
             "{}_quant".format(conv_node.output[0])
         )
 
         # Cleanup
         # delete folded quantization ops
```

## sparseml/tensorflow_v1/__init__.py

```diff
@@ -14,14 +14,21 @@
 
 """
 Functionality for working with and sparsifying Models in the TensorFlow 1.x framework
 """
 
 # flake8: noqa
 
+from sparseml.utils import deprecation_warning as _deprecation_warning
+
+
+_deprecation_warning(
+    "sparseml.tensorflow_v1 is deprecated and will be removed in a future version",
+)
+
 from sparseml.analytics import sparseml_analytics as _analytics
 
 from .base import *
 from .framework import detect_framework, framework_info, is_supported
 from .sparsification import sparsification_info
```

## sparseml/utils/helpers.py

```diff
@@ -19,14 +19,15 @@
 
 import errno
 import fnmatch
 import json
 import logging
 import os
 import sys
+import warnings
 from collections import OrderedDict
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterable, List, Tuple, Union
 from urllib.parse import urlparse
 
 import numpy
 
@@ -60,14 +61,15 @@
     "save_numpy",
     "load_labeled_data",
     "NumpyArrayBatcher",
     "tensor_export",
     "tensors_export",
     "parse_optimization_str",
     "json_to_jsonl",
+    "deprecation_warning",
 ]
 
 
 ALL_TOKEN = "__ALL__"
 ALL_PRUNABLE_TOKEN = "__ALL_PRUNABLE__"
 FROM_PARAM_TOKEN = "__FROM_PARAM__"
 RECIPE_METADATA_KEY = "__metadata__"
@@ -816,7 +818,16 @@
         )
 
     jsonl_file_path = json_file_path + ("" if overwrite else "l")
     with open(jsonl_file_path, "w") as jsonl_file:
         for json_line in json_data:
             json.dump(json_line, jsonl_file)  # append json line
             jsonl_file.write("\n")  # newline
+
+
+def deprecation_warning(message: str):
+    warnings.simplefilter("always", DeprecationWarning)
+    warnings.warn(
+        message,
+        category=DeprecationWarning,
+        stacklevel=2,
+    )
```

## Comparing `sparseml_nightly-1.6.0.20230604.dist-info/LICENSE` & `sparseml_nightly-1.6.0.20230608.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230604.dist-info/METADATA` & `sparseml_nightly-1.6.0.20230608.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseml-nightly
-Version: 1.6.0.20230604
+Version: 1.6.0.20230608
 Summary: Libraries for applying sparsification recipes to neural networks with a few lines of code, enabling faster and smaller models
 Home-page: https://github.com/neuralmagic/sparseml
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,sparsity,pruning,deep learning libraries,onnx,quantization,automl
 Platform: UNKNOWN
```

## Comparing `sparseml_nightly-1.6.0.20230604.dist-info/NOTICE` & `sparseml_nightly-1.6.0.20230608.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230604.dist-info/entry_points.txt` & `sparseml_nightly-1.6.0.20230608.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230604.dist-info/RECORD` & `sparseml_nightly-1.6.0.20230608.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 sparseml/exporters/transforms/unwrap_batchnorms.py,sha256=ly7GHCXN_2r8Gnk8PABWCqcoS-NL3GMfquEK0hRlFCs,1373
 sparseml/exporters/transforms/utils/__init__.py,sha256=tXSSUnzdyIc_H73xQ5dYhHb1Gj4Nb7GLLDVwJds8c_s,730
 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py,sha256=lUutqioFTP3ZVa5IIA-Z5WbriNj_8m2mXut_QOyo_J0,8704
 sparseml/exporters/transforms/utils/helpers.py,sha256=vkEYL2Bdp_YNXlPg_TGd82Q2ef1EYEr11LVgmORQDiY,6457
 sparseml/exporters/transforms/utils/matching.py,sha256=CnVJLbJARBJwvFjoKh9vwYt6dLP4WXG3p7nCY5VUFaE,14429
 sparseml/framework/__init__.py,sha256=EcIX435yx552d7BkbxmAbQ_X3KAISInHVbD9X-AT1Uk,790
 sparseml/framework/info.py,sha256=TaZAMYdhBHcjl9Xyk3PWjJkDB6g3_f4vD3B6KmhgOl8,9479
-sparseml/keras/__init__.py,sha256=G-uSbckWq3vn9YUFr5pD0xbaO694SFgIlc5AVQMDafU,970
+sparseml/keras/__init__.py,sha256=9D-eU-wi0UGuq55i2BTYDgS0mD6UJB10Gi8LQwh9KSk,1144
 sparseml/keras/base.py,sha256=yt1EO6KIeCkdg8rF37U5Y3FNGeAqOQLVGyxRANsyBy0,8054
 sparseml/keras/datasets/__init__.py,sha256=USLH-kFbXiubqgMW8IMkZfycVByQAOdAtzuPHzTok9I,943
 sparseml/keras/datasets/dataset.py,sha256=W6wdx4WXtyy4r1JVbc8fO0Xt5SM03zm8Vq306uNFkaw,3297
 sparseml/keras/datasets/helpers.py,sha256=PfDBKDMr3A8XG9wP0QRABu4h63eHZT15gDuO8naIXxY,2423
 sparseml/keras/datasets/registry.py,sha256=41aieOOADwl0V1n127OA6zyxhCwLwHy4jo7SkyzSUwo,2761
 sparseml/keras/datasets/classification/__init__.py,sha256=YGWvyTK6h32vDtAD3Vcr3bsNqGvfFXOiQy9wydvzEDc,786
 sparseml/keras/datasets/classification/imagefolder.py,sha256=Ay5xsUH4zR2xgTg6HM7qXiOMs02PMMg3-_pD0tgzzgE,8369
@@ -216,16 +216,16 @@
 sparseml/pytorch/sparsification/pruning/scorer.py,sha256=8gyYSv611GOJwmpQeD7FsWVrLxF8jeM_f59zhQlC6f8,4644
 sparseml/pytorch/sparsification/quantization/__init__.py,sha256=OjbeCzzhoeFJEJQvLmXZc89pghO83sLRhmvNF7_q_oQ,813
 sparseml/pytorch/sparsification/quantization/constants.py,sha256=sla-j0QwLFq92AbDZkHkNLxugpGrNEQJIuLWoWqV3Ks,2220
 sparseml/pytorch/sparsification/quantization/helpers.py,sha256=MmY5iOMlBUBEMrotPyj3H5drzpXhf13v4FJjb1N2aaw,32271
 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py,sha256=TToI4dGYZZEzB1q61m1YVg0THlvH7Ew1CZ2y-ajpTts,33626
 sparseml/pytorch/sparsification/quantization/modifier_quantization.py,sha256=LkHNB1IsiFlZugUecB4-LZMjWuoboFYf_PXPx6uPl1g,26778
 sparseml/pytorch/sparsification/quantization/quantization_scheme.py,sha256=10KNttNCHqUTNq706kPB6k7u6mvvfV0WTvx5D5Uqd-Y,12558
-sparseml/pytorch/sparsification/quantization/quantize.py,sha256=4vWbjp2WfeZ0BUf1_3BtDqLlbJfAdcrRsnzwhB5OAz8,17591
-sparseml/pytorch/sparsification/quantization/quantize_qat_export.py,sha256=bGDDqIeX-x6S_gjhsGr-yQOJwq8qp8D02qB5q4ZCapE,69997
+sparseml/pytorch/sparsification/quantization/quantize.py,sha256=bqqH2qBEWYHfea5jzAHmz52uPddfRdmP3TFaCKgQqjM,17905
+sparseml/pytorch/sparsification/quantization/quantize_qat_export.py,sha256=9szHTgbPqgiZFw_dL3h_BXThUR2sklsSqiVQ4sQf-U0,70029
 sparseml/pytorch/sparsification/training/__init__.py,sha256=4GGhQf6KVSOYwtr_WL9Xcvx4mR-k8yKMVI_zuTBHGO4,790
 sparseml/pytorch/sparsification/training/modifier_epoch.py,sha256=_5p1EZk2qbwTnWsMXbVan3vRj1IRyIM4wYYZdLGA5GE,1778
 sparseml/pytorch/sparsification/training/modifier_logging.py,sha256=K1NMqhea5EBPko6yim8CThShbiSJKN5P_ca_TCyZXto,2883
 sparseml/pytorch/sparsification/training/modifier_lr.py,sha256=m_tCydo_BHiXCHMUKZu6iqKLAP24acAT8-NLjH9RIlE,24287
 sparseml/pytorch/sparsification/training/modifier_params.py,sha256=G_0eVqu0Cup8WNLFhkfPmYnKtJlNrxcJt0FcOOdq9tA,21497
 sparseml/pytorch/sparsification/training/modifier_regularizer.py,sha256=ezHbcwI8ITgq4vwkzsWXgnq_ls6NONW_D8jEN-YR7u8,6690
 sparseml/pytorch/torchvision/__init__.py,sha256=fD0HjvgSO8WgfyPPSn7r_Fej6xWAelVJVbgWfI9ypY4,943
@@ -263,15 +263,15 @@
 sparseml/sparsification/modifier_lr.py,sha256=-3t0ozub6vfyh9NAgvgRgbyXIP1yu9_URuArr5TdTXg,10117
 sparseml/sparsification/modifier_params.py,sha256=n6O1tD4nsOTeeGJ5ym4hB7PQwSEWNduymW8_ObjAO7g,5505
 sparseml/sparsification/modifier_pruning.py,sha256=7_i4dzdkfOFcD7A_d8cublgX5KB-hyOGOJZtU41JUwU,12845
 sparseml/sparsification/oracle.py,sha256=9J8iIdr_aztwc06tRgw-2ZdGN_1RgJBYWZDY1ZfHhAY,3700
 sparseml/sparsification/recipe_builder.py,sha256=i8cFAkDemk8UXiPff5s9necHXECk6WO2AySnqiqr8MU,18570
 sparseml/sparsification/recipe_editor.py,sha256=6PqExzex1nmMj2a0jkE7JUeeuMTGA27GCH32C9B8V40,14413
 sparseml/sparsification/types.py,sha256=wi05A10SkgSBFmBUtzdHIIMTsY4lPTXP0ycZrBgbub0,1250
-sparseml/tensorflow_v1/__init__.py,sha256=JfUGMyYgBnal1xMpGR_i0oA4juUVt2QvkbcBZxFZG6w,987
+sparseml/tensorflow_v1/__init__.py,sha256=0ZHOevyiQP_YkWyOhV2Jgx48YmQrxD0kltIQYW9Qzxk,1169
 sparseml/tensorflow_v1/base.py,sha256=PHZOsjEtcG3gEGRdU7tu2jNRAYYo8KrCmPenZyo5IQo,7272
 sparseml/tensorflow_v1/datasets/__init__.py,sha256=X0o7cmzhXhLwjrawfN3pIqrFTKALH_xftMIerzWaLjQ,925
 sparseml/tensorflow_v1/datasets/dataset.py,sha256=t4OfviMyfbn63kNrNiH19blDvoxcxhyBiLgUh03Ryhc,8121
 sparseml/tensorflow_v1/datasets/helpers.py,sha256=mGy1YuQqERWRG-dknPmOspyWtzUinY9GUSEdSPycGF8,5600
 sparseml/tensorflow_v1/datasets/registry.py,sha256=2H2fG0iUQ0h41XVpZp-GHXM3Ti6axePI1O2LQKqSqhI,2768
 sparseml/tensorflow_v1/datasets/classification/__init__.py,sha256=xNLlq5y7_cssxlZZP95CuYioqEiU6TanVbzMCqoCVTo,807
 sparseml/tensorflow_v1/datasets/classification/cifar.py,sha256=_ETXHcC9cPtQbQIoBLgQQd2GC0Ue6kEO3XXpaZY54xg,12686
@@ -324,15 +324,15 @@
 sparseml/transformers/sparsification/training_args.py,sha256=gGivIDchLi__PZMNQRmzDOaQcQLkUVFystq3LaVko3Y,1890
 sparseml/transformers/utils/__init__.py,sha256=dxyg6b2XznhBzOsduHdOalgTmoX1JC32Rb4AHns6rVk,794
 sparseml/transformers/utils/helpers.py,sha256=pgxtf0ygP7qJEVPse_dGxm7UpWSJ9JVebA_ex1c8Muw,3090
 sparseml/transformers/utils/metrics.py,sha256=ciZsxgdrzlSMnyzbgKOFE3spWsKql0z82BiYFRXiVOU,2536
 sparseml/transformers/utils/model.py,sha256=JRq-p0CqKlWLdbhD9e8V2YkFtSZ6xLE9B512TTR8d2M,17072
 sparseml/utils/__init__.py,sha256=-WKBN4DERhw7rTJkarilkyAM9pw4rW8qkXGRPSEJ8SM,844
 sparseml/utils/frameworks.py,sha256=S-cGkbVc6DoWfI6Hu5AkIqF0Vi1PyxKX5GfhwRfpv_E,886
-sparseml/utils/helpers.py,sha256=smNZXr2VnhVfvM6s_1XTq1UIJtjRg0-cDn5to_DBIWs,26321
+sparseml/utils/helpers.py,sha256=qaooDtSTHgwLTjyfavDR7xPyS2mi26fGzla9VcHWJZg,26562
 sparseml/utils/restricted_eval.py,sha256=bBScMel61Cl3OcXs1TvxQgao1P2cJgmeDHeLSHF5Cqg,3983
 sparseml/utils/singleton.py,sha256=SbOoiw_CW7d9TEYIcvfb_ueaAD4iKbURZiTlBfM173g,1083
 sparseml/utils/worker.py,sha256=swoPegdTmV8nYbyie2WUytLLdwaK9skjx4RejHD3cww,6312
 sparseml/utils/wrapper.py,sha256=xrhPKRrXajQtDGIS--ZZxLsvnVTnnP0vlcnt_Tyd--g,2952
 sparseml/utils/datasets/__init__.py,sha256=HFbqzS5n0692VGBO5eqlTxc14WlRM2S_Qt2xhFxsGE4,819
 sparseml/utils/datasets/cifar.py,sha256=tvkMGu8afg9-EVlHXAEfEYXkje8nFzgnlG4mREsbxzE,833
 sparseml/utils/datasets/coco.py,sha256=5w9Fm0O2kUtrC1upa6DCC4WZ13df-ZlORPUHEwGFDLc,3750
@@ -355,14 +355,14 @@
 sparseml/yolov8/train.py,sha256=DeZMrZ_moAc3fIojJloq3IvQqiPC_cgPgTjYFSOoG7E,7194
 sparseml/yolov8/trainers.py,sha256=mzOuog5BmQg3tER3m35zqTcKRlxiw9IqCpgBy-Ep1sA,34788
 sparseml/yolov8/val.py,sha256=hlFImvknSpV1nONOxA3ivYgvzm64EmK0_Lh-JHLbOsw,2748
 sparseml/yolov8/validators.py,sha256=ytG7g_LOXvKFmxLPmQloT-wNf78convSoRRXVTYCR0Y,8196
 sparseml/yolov8/utils/__init__.py,sha256=6JekgnibQP-8p8Dm1dGiIEGCGdBOAkSOnEds0BMSYhQ,685
 sparseml/yolov8/utils/export_samples.py,sha256=gn7et_J-OfnCTEYP0iLXx2W-HARgxqUnHqJWHBG72KM,6288
 sparseml/yolov8/utils/helpers.py,sha256=8JZNaTT1zPKiZaOccmMtQu5mXCSMGkq8BDEgUqaPVIs,4041
-sparseml_nightly-1.6.0.20230604.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sparseml_nightly-1.6.0.20230604.dist-info/METADATA,sha256=2W7rnW2LXAXgS9oa8LHJikGqJzXhlwL_gUH3RQv2cT4,21640
-sparseml_nightly-1.6.0.20230604.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
-sparseml_nightly-1.6.0.20230604.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sparseml_nightly-1.6.0.20230604.dist-info/entry_points.txt,sha256=KbSvJr3uXYQgZRF0Mzi5B89ijSwsiZalXMxinJRaass,2377
-sparseml_nightly-1.6.0.20230604.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
-sparseml_nightly-1.6.0.20230604.dist-info/RECORD,,
+sparseml_nightly-1.6.0.20230608.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sparseml_nightly-1.6.0.20230608.dist-info/METADATA,sha256=EkTusfaRUQwBO-vLiYYRkox3Z5OIG2_ZofHVJl-Lw-8,21640
+sparseml_nightly-1.6.0.20230608.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
+sparseml_nightly-1.6.0.20230608.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sparseml_nightly-1.6.0.20230608.dist-info/entry_points.txt,sha256=KbSvJr3uXYQgZRF0Mzi5B89ijSwsiZalXMxinJRaass,2377
+sparseml_nightly-1.6.0.20230608.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
+sparseml_nightly-1.6.0.20230608.dist-info/RECORD,,
```

