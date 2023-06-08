# Comparing `tmp/flash_attn_wheels-1.0.8.tar.gz` & `tmp/flash_attn_wheels-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flash_attn_wheels-1.0.8.tar", last modified: Sun Jun  4 14:17:34 2023, max compression
+gzip compressed data, was "flash_attn_wheels-1.0.9.tar", last modified: Thu Jun  8 01:00:23 2023, max compression
```

## Comparing `flash_attn_wheels-1.0.8.tar` & `flash_attn_wheels-1.0.9.tar`

### file list

```diff
@@ -1,180 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.290331 flash_attn_wheels-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-06-04 14:17:34.286330 flash_attn_wheels-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.210325 flash_attn_wheels-1.0.8/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.214326 flash_attn_wheels-1.0.8/csrc/flash_attn/
--rw-r--r--   0 runner    (1001) docker     (123)    33267 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/fmha_api.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.226326 flash_attn_wheels-1.0.8/csrc/flash_attn/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.230327 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha/
--rw-r--r--   0 runner    (1001) docker     (123)    17999 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha/gemm.h
--rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha/gmem_tile.h
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha/kernel_traits.h
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha/mask.h
--rw-r--r--   0 runner    (1001) docker     (123)    74010 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha/smem_tile.h
--rw-r--r--   0 runner    (1001) docker     (123)    25514 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha/softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)    41059 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha.h
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_block_dgrad_fp16_kernel_loop.sm80.cu
--rw-r--r--   0 runner    (1001) docker     (123)    33506 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_block_dgrad_kernel_1xN_loop.h
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_block_fprop_fp16_kernel.sm80.cu
--rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_block_fprop_kernel_1xN.h
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_blockmask.h
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_bwd_hdim128.cu
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_bwd_hdim32.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_bwd_hdim64.cu
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_bwd_launch_template.h
--rw-r--r--   0 runner    (1001) docker     (123)    37168 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_dgrad_kernel_1xN_loop.h
--rw-r--r--   0 runner    (1001) docker     (123)    31042 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_fprop_kernel_1xN.h
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_fwd_hdim128.cu
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_fwd_hdim32.cu
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_fwd_hdim64.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_fwd_launch_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_kernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/philox.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/flash_attn/src/static_switch.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.234327 flash_attn_wheels-1.0.8/csrc/ft_attention/
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/ft_attention/cuda_bf16_fallbacks.cuh
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/ft_attention/cuda_bf16_wrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/ft_attention/decoder_masked_multihead_attention.cu
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/ft_attention/decoder_masked_multihead_attention.h
--rw-r--r--   0 runner    (1001) docker     (123)    53394 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/ft_attention/decoder_masked_multihead_attention_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/ft_attention/ft_attention.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.234327 flash_attn_wheels-1.0.8/csrc/fused_dense_lib/
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/fused_dense_lib/fused_dense.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24690 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/fused_dense_lib/fused_dense_cuda.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.234327 flash_attn_wheels-1.0.8/csrc/fused_softmax/
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/fused_softmax/fused_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23616 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/fused_softmax/scaled_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/fused_softmax/scaled_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    24659 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/fused_softmax/scaled_upper_triang_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/fused_softmax/scaled_upper_triang_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/fused_softmax/type_shim.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.266329 flash_attn_wheels-1.0.8/csrc/layer_norm/
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln.h
--rw-r--r--   0 runner    (1001) docker     (123)    36418 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_api.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_1024.cu
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_1280.cu
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_1536.cu
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_2048.cu
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_256.cu
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_2560.cu
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_3072.cu
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_4096.cu
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_512.cu
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_5120.cu
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_6144.cu
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_7168.cu
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_768.cu
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_8192.cu
--rw-r--r--   0 runner    (1001) docker     (123)    25647 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_kernels.cuh
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_1024.cu
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_1280.cu
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_1536.cu
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_2048.cu
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_256.cu
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_2560.cu
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_3072.cu
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_4096.cu
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_512.cu
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_5120.cu
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_6144.cu
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_7168.cu
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_768.cu
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_8192.cu
--rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_kernels.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_kernel_traits.h
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_1024.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_1280.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_1536.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_2048.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_256.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_2560.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_3072.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_4096.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_512.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_5120.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_6144.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_7168.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_768.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_8192.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_1024.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_1280.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_1536.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_2048.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_256.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_2560.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_3072.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_4096.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_512.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_5120.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_6144.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_7168.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_768.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_8192.cu
--rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_residual_bwd_kernels.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_residual_fwd_kernels.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    29989 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/ln_utils.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/layer_norm/static_switch.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.266329 flash_attn_wheels-1.0.8/csrc/rotary/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/rotary/rotary.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/rotary/rotary_cuda.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.266329 flash_attn_wheels-1.0.8/csrc/xentropy/
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/xentropy/interface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25783 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/csrc/xentropy/xentropy_kernel.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.274330 flash_attn_wheels-1.0.8/flash_attn/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/bert_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    20506 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/flash_attn_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    38148 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/flash_attn_triton.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/flash_attn_triton_og.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/flash_blocksparse_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/flash_blocksparse_attn_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/fused_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.274330 flash_attn_wheels-1.0.8/flash_attn/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/layers/patch_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/layers/rotary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.274330 flash_attn_wheels-1.0.8/flash_attn/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/losses/cross_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.282330 flash_attn_wheels-1.0.8/flash_attn/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26570 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/models/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)    38025 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/models/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/models/gpt_neox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/models/gptj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/models/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/models/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/models/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.282330 flash_attn_wheels-1.0.8/flash_attn/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/modules/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34607 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/modules/mha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/modules/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.286330 flash_attn_wheels-1.0.8/flash_attn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/ops/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/ops/fused_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    18366 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/ops/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/ops/rms_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.286330 flash_attn_wheels-1.0.8/flash_attn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/utils/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/utils/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/flash_attn/utils/pretrained.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:17:34.286330 flash_attn_wheels-1.0.8/flash_attn_wheels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-06-04 14:17:34.000000 flash_attn_wheels-1.0.8/flash_attn_wheels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-06-04 14:17:34.000000 flash_attn_wheels-1.0.8/flash_attn_wheels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 14:17:34.000000 flash_attn_wheels-1.0.8/flash_attn_wheels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-04 14:17:34.000000 flash_attn_wheels-1.0.8/flash_attn_wheels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 14:17:34.000000 flash_attn_wheels-1.0.8/flash_attn_wheels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 14:17:34.290331 flash_attn_wheels-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-06-04 14:15:25.000000 flash_attn_wheels-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.602519 flash_attn_wheels-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-06-08 01:00:23.602519 flash_attn_wheels-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.550517 flash_attn_wheels-1.0.9/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.554518 flash_attn_wheels-1.0.9/csrc/flash_attn/
+-rw-r--r--   0 runner    (1001) docker     (123)    33267 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/fmha_api.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.562518 flash_attn_wheels-1.0.9/csrc/flash_attn/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.562518 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha/
+-rw-r--r--   0 runner    (1001) docker     (123)    17999 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha/gemm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha/gmem_tile.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha/kernel_traits.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha/mask.h
+-rw-r--r--   0 runner    (1001) docker     (123)    74010 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha/smem_tile.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25514 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha/softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41059 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_block_dgrad_fp16_kernel_loop.sm80.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    33506 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_block_dgrad_kernel_1xN_loop.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_block_fprop_fp16_kernel.sm80.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_block_fprop_kernel_1xN.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_blockmask.h
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_bwd_hdim128.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_bwd_hdim32.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_bwd_hdim64.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_bwd_launch_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37168 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_dgrad_kernel_1xN_loop.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31042 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_fprop_kernel_1xN.h
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_fwd_hdim128.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_fwd_hdim32.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_fwd_hdim64.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_fwd_launch_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_kernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/philox.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/flash_attn/src/static_switch.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.566518 flash_attn_wheels-1.0.9/csrc/ft_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/ft_attention/cuda_bf16_fallbacks.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/ft_attention/cuda_bf16_wrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/ft_attention/decoder_masked_multihead_attention.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/ft_attention/decoder_masked_multihead_attention.h
+-rw-r--r--   0 runner    (1001) docker     (123)    53394 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/ft_attention/decoder_masked_multihead_attention_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/ft_attention/ft_attention.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.566518 flash_attn_wheels-1.0.9/csrc/fused_dense_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/fused_dense_lib/fused_dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24690 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/fused_dense_lib/fused_dense_cuda.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.570518 flash_attn_wheels-1.0.9/csrc/fused_softmax/
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/fused_softmax/fused_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23616 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/fused_softmax/scaled_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/fused_softmax/scaled_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    24659 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/fused_softmax/scaled_upper_triang_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/fused_softmax/scaled_upper_triang_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/fused_softmax/type_shim.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.590518 flash_attn_wheels-1.0.9/csrc/layer_norm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36418 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_api.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_1024.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_1280.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_1536.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_2048.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_256.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_2560.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_3072.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_4096.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_512.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_5120.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_6144.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_7168.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_768.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_8192.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    25647 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_kernels.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_1024.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_1280.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_1536.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_2048.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_256.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_2560.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_3072.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_4096.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_512.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_5120.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_6144.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_7168.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_768.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_8192.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_kernels.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_kernel_traits.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_1024.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_1280.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_1536.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_2048.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_256.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_2560.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_3072.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_4096.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_512.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_5120.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_6144.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_7168.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_768.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_8192.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_1024.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_1280.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_1536.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_2048.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_256.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_2560.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_3072.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_4096.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_512.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_5120.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_6144.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_7168.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_768.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_8192.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_residual_bwd_kernels.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_residual_fwd_kernels.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)    29989 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/ln_utils.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/layer_norm/static_switch.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.590518 flash_attn_wheels-1.0.9/csrc/rotary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/rotary/rotary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/rotary/rotary_cuda.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.590518 flash_attn_wheels-1.0.9/csrc/xentropy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/xentropy/interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25783 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/csrc/xentropy/xentropy_kernel.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.594519 flash_attn_wheels-1.0.9/flash_attn/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/bert_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20506 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/flash_attn_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38148 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/flash_attn_triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/flash_attn_triton_og.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/flash_blocksparse_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/flash_blocksparse_attn_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/fused_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.594519 flash_attn_wheels-1.0.9/flash_attn/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/layers/patch_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/layers/rotary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.594519 flash_attn_wheels-1.0.9/flash_attn/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/losses/cross_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.598518 flash_attn_wheels-1.0.9/flash_attn/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26570 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/models/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38025 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/models/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/models/gpt_neox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/models/gptj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/models/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/models/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/models/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.598518 flash_attn_wheels-1.0.9/flash_attn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/modules/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34607 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/modules/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/modules/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.602519 flash_attn_wheels-1.0.9/flash_attn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/ops/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/ops/fused_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18366 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/ops/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/ops/rms_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.602519 flash_attn_wheels-1.0.9/flash_attn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/utils/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/utils/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/flash_attn/utils/pretrained.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:00:23.602519 flash_attn_wheels-1.0.9/flash_attn_wheels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-06-08 01:00:23.000000 flash_attn_wheels-1.0.9/flash_attn_wheels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-08 01:00:23.000000 flash_attn_wheels-1.0.9/flash_attn_wheels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 01:00:23.000000 flash_attn_wheels-1.0.9/flash_attn_wheels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 01:00:23.000000 flash_attn_wheels-1.0.9/flash_attn_wheels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 01:00:23.000000 flash_attn_wheels-1.0.9/flash_attn_wheels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 01:00:23.606519 flash_attn_wheels-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-06-08 00:58:27.000000 flash_attn_wheels-1.0.9/setup.py
```

### Comparing `flash_attn_wheels-1.0.8/LICENSE` & `flash_attn_wheels-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/PKG-INFO` & `flash_attn_wheels-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flash_attn_wheels
-Version: 1.0.8
+Version: 1.0.9
 Summary: Flash Attention: Fast and Memory-Efficient Exact Attention
 Home-page: https://github.com/piercefreeman/flash-attention
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
@@ -68,14 +68,22 @@
 container from Nvidia, which has all the required tools to install FlashAttention.
 
 To install:
 ```sh
 pip install flash-attn
 ```
 
+If you see an error about `ModuleNotFoundError: No module named 'torch'`, it's likely because of pypi's installation isolation.
+
+To fix you can run:
+
+```sh
+pip install flash-attn --no-build-isolation
+```
+
 Alternatively you can compile from source:
 ```
 python setup.py install
 ```
 
 Interface: `src/flash_attention.py`
```

### Comparing `flash_attn_wheels-1.0.8/README.md` & `flash_attn_wheels-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,22 @@
 container from Nvidia, which has all the required tools to install FlashAttention.
 
 To install:
 ```sh
 pip install flash-attn
 ```
 
+If you see an error about `ModuleNotFoundError: No module named 'torch'`, it's likely because of pypi's installation isolation.
+
+To fix you can run:
+
+```sh
+pip install flash-attn --no-build-isolation
+```
+
 Alternatively you can compile from source:
 ```
 python setup.py install
 ```
 
 Interface: `src/flash_attention.py`
```

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/fmha_api.cpp` & `flash_attn_wheels-1.0.9/csrc/flash_attn/fmha_api.cpp`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha/gemm.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha/gemm.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha/gmem_tile.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha/gmem_tile.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha/kernel_traits.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha/kernel_traits.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha/mask.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha/mask.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha/smem_tile.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha/smem_tile.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha/softmax.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha/softmax.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha/utils.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha/utils.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_block_dgrad_fp16_kernel_loop.sm80.cu` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_block_dgrad_fp16_kernel_loop.sm80.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_block_dgrad_kernel_1xN_loop.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_block_dgrad_kernel_1xN_loop.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_block_fprop_fp16_kernel.sm80.cu` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_block_fprop_fp16_kernel.sm80.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_block_fprop_kernel_1xN.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_block_fprop_kernel_1xN.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_blockmask.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_blockmask.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_bwd_hdim32.cu` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_bwd_hdim32.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_bwd_hdim64.cu` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_bwd_hdim64.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_bwd_launch_template.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_bwd_launch_template.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_dgrad_kernel_1xN_loop.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_dgrad_kernel_1xN_loop.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_fprop_kernel_1xN.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_fprop_kernel_1xN.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_fwd_hdim32.cu` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_fwd_hdim32.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_fwd_hdim64.cu` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_fwd_hdim64.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_fwd_launch_template.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_fwd_launch_template.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_kernel.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_kernel.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/fmha_utils.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/fmha_utils.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/philox.cuh` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/philox.cuh`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/flash_attn/src/static_switch.h` & `flash_attn_wheels-1.0.9/csrc/flash_attn/src/static_switch.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/ft_attention/cuda_bf16_fallbacks.cuh` & `flash_attn_wheels-1.0.9/csrc/ft_attention/cuda_bf16_fallbacks.cuh`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/ft_attention/cuda_bf16_wrapper.h` & `flash_attn_wheels-1.0.9/csrc/ft_attention/cuda_bf16_wrapper.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/ft_attention/decoder_masked_multihead_attention.cu` & `flash_attn_wheels-1.0.9/csrc/ft_attention/decoder_masked_multihead_attention.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/ft_attention/decoder_masked_multihead_attention.h` & `flash_attn_wheels-1.0.9/csrc/ft_attention/decoder_masked_multihead_attention.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/ft_attention/decoder_masked_multihead_attention_utils.h` & `flash_attn_wheels-1.0.9/csrc/ft_attention/decoder_masked_multihead_attention_utils.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/ft_attention/ft_attention.cpp` & `flash_attn_wheels-1.0.9/csrc/ft_attention/ft_attention.cpp`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/fused_dense_lib/fused_dense.cpp` & `flash_attn_wheels-1.0.9/csrc/fused_dense_lib/fused_dense.cpp`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/fused_dense_lib/fused_dense_cuda.cu` & `flash_attn_wheels-1.0.9/csrc/fused_dense_lib/fused_dense_cuda.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/fused_softmax/fused_softmax.cpp` & `flash_attn_wheels-1.0.9/csrc/fused_softmax/fused_softmax.cpp`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/fused_softmax/scaled_masked_softmax.h` & `flash_attn_wheels-1.0.9/csrc/fused_softmax/scaled_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/fused_softmax/scaled_masked_softmax_cuda.cu` & `flash_attn_wheels-1.0.9/csrc/fused_softmax/scaled_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/fused_softmax/scaled_upper_triang_masked_softmax.h` & `flash_attn_wheels-1.0.9/csrc/fused_softmax/scaled_upper_triang_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/fused_softmax/scaled_upper_triang_masked_softmax_cuda.cu` & `flash_attn_wheels-1.0.9/csrc/fused_softmax/scaled_upper_triang_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/fused_softmax/type_shim.h` & `flash_attn_wheels-1.0.9/csrc/fused_softmax/type_shim.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln.h` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_api.cpp` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_api.cpp`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_1024.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_1024.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_1280.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_1280.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_1536.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_1536.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_2048.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_2048.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_256.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_256.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_2560.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_2560.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_3072.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_3072.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_4096.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_4096.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_512.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_512.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_5120.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_5120.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_6144.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_6144.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_7168.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_7168.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_768.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_768.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_8192.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_8192.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_bwd_kernels.cuh` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_bwd_kernels.cuh`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_1024.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_1024.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_1280.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_1280.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_1536.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_1536.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_2048.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_2048.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_256.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_256.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_2560.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_2560.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_3072.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_3072.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_4096.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_4096.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_512.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_512.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_5120.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_5120.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_6144.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_6144.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_7168.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_7168.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_768.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_768.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_8192.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_8192.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_fwd_kernels.cuh` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_fwd_kernels.cuh`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_kernel_traits.h` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_kernel_traits.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_1024.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_1024.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_1280.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_1280.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_1536.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_1536.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_2048.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_2048.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_256.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_256.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_2560.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_2560.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_3072.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_3072.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_4096.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_4096.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_512.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_512.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_5120.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_5120.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_6144.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_6144.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_7168.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_7168.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_768.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_768.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_bwd_8192.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_bwd_8192.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_1024.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_1024.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_1280.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_1280.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_1536.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_1536.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_2048.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_2048.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_256.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_256.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_2560.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_2560.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_3072.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_3072.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_4096.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_4096.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_512.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_512.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_5120.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_5120.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_6144.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_6144.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_7168.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_7168.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_768.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_768.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_fwd_8192.cu` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_fwd_8192.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_residual_bwd_kernels.cuh` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_residual_bwd_kernels.cuh`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_parallel_residual_fwd_kernels.cuh` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_parallel_residual_fwd_kernels.cuh`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/ln_utils.cuh` & `flash_attn_wheels-1.0.9/csrc/layer_norm/ln_utils.cuh`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/layer_norm/static_switch.h` & `flash_attn_wheels-1.0.9/csrc/layer_norm/static_switch.h`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/rotary/rotary.cpp` & `flash_attn_wheels-1.0.9/csrc/rotary/rotary.cpp`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/rotary/rotary_cuda.cu` & `flash_attn_wheels-1.0.9/csrc/rotary/rotary_cuda.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/xentropy/interface.cpp` & `flash_attn_wheels-1.0.9/csrc/xentropy/interface.cpp`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/csrc/xentropy/xentropy_kernel.cu` & `flash_attn_wheels-1.0.9/csrc/xentropy/xentropy_kernel.cu`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/bert_padding.py` & `flash_attn_wheels-1.0.9/flash_attn/bert_padding.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/flash_attention.py` & `flash_attn_wheels-1.0.9/flash_attn/flash_attention.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/flash_attn_interface.py` & `flash_attn_wheels-1.0.9/flash_attn/flash_attn_interface.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/flash_attn_triton.py` & `flash_attn_wheels-1.0.9/flash_attn/flash_attn_triton.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/flash_attn_triton_og.py` & `flash_attn_wheels-1.0.9/flash_attn/flash_attn_triton_og.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/flash_blocksparse_attention.py` & `flash_attn_wheels-1.0.9/flash_attn/flash_blocksparse_attention.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/flash_blocksparse_attn_interface.py` & `flash_attn_wheels-1.0.9/flash_attn/flash_blocksparse_attn_interface.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/fused_softmax.py` & `flash_attn_wheels-1.0.9/flash_attn/fused_softmax.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/layers/patch_embed.py` & `flash_attn_wheels-1.0.9/flash_attn/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/layers/rotary.py` & `flash_attn_wheels-1.0.9/flash_attn/layers/rotary.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/losses/cross_entropy.py` & `flash_attn_wheels-1.0.9/flash_attn/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/models/bert.py` & `flash_attn_wheels-1.0.9/flash_attn/models/bert.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/models/gpt.py` & `flash_attn_wheels-1.0.9/flash_attn/models/gpt.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/models/gpt_neox.py` & `flash_attn_wheels-1.0.9/flash_attn/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/models/gptj.py` & `flash_attn_wheels-1.0.9/flash_attn/models/gptj.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/models/llama.py` & `flash_attn_wheels-1.0.9/flash_attn/models/llama.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/models/opt.py` & `flash_attn_wheels-1.0.9/flash_attn/models/opt.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/models/vit.py` & `flash_attn_wheels-1.0.9/flash_attn/models/vit.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/modules/block.py` & `flash_attn_wheels-1.0.9/flash_attn/modules/block.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/modules/embedding.py` & `flash_attn_wheels-1.0.9/flash_attn/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/modules/mha.py` & `flash_attn_wheels-1.0.9/flash_attn/modules/mha.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/modules/mlp.py` & `flash_attn_wheels-1.0.9/flash_attn/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/ops/activations.py` & `flash_attn_wheels-1.0.9/flash_attn/ops/activations.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/ops/fused_dense.py` & `flash_attn_wheels-1.0.9/flash_attn/ops/fused_dense.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/ops/layer_norm.py` & `flash_attn_wheels-1.0.9/flash_attn/ops/layer_norm.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/ops/rms_norm.py` & `flash_attn_wheels-1.0.9/flash_attn/ops/rms_norm.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/utils/benchmark.py` & `flash_attn_wheels-1.0.9/flash_attn/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/utils/distributed.py` & `flash_attn_wheels-1.0.9/flash_attn/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/utils/generation.py` & `flash_attn_wheels-1.0.9/flash_attn/utils/generation.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn/utils/pretrained.py` & `flash_attn_wheels-1.0.9/flash_attn/utils/pretrained.py`

 * *Files identical despite different names*

### Comparing `flash_attn_wheels-1.0.8/flash_attn_wheels.egg-info/PKG-INFO` & `flash_attn_wheels-1.0.9/flash_attn_wheels.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flash-attn-wheels
-Version: 1.0.8
+Version: 1.0.9
 Summary: Flash Attention: Fast and Memory-Efficient Exact Attention
 Home-page: https://github.com/piercefreeman/flash-attention
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
@@ -68,14 +68,22 @@
 container from Nvidia, which has all the required tools to install FlashAttention.
 
 To install:
 ```sh
 pip install flash-attn
 ```
 
+If you see an error about `ModuleNotFoundError: No module named 'torch'`, it's likely because of pypi's installation isolation.
+
+To fix you can run:
+
+```sh
+pip install flash-attn --no-build-isolation
+```
+
 Alternatively you can compile from source:
 ```
 python setup.py install
 ```
 
 Interface: `src/flash_attention.py`
```

### Comparing `flash_attn_wheels-1.0.8/flash_attn_wheels.egg-info/SOURCES.txt` & `flash_attn_wheels-1.0.9/flash_attn_wheels.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
 setup.py
 csrc/flash_attn/fmha_api.cpp
 csrc/flash_attn/src/fmha.h
 csrc/flash_attn/src/fmha_block_dgrad_fp16_kernel_loop.sm80.cu
 csrc/flash_attn/src/fmha_block_dgrad_kernel_1xN_loop.h
 csrc/flash_attn/src/fmha_block_fprop_fp16_kernel.sm80.cu
 csrc/flash_attn/src/fmha_block_fprop_kernel_1xN.h
```

### Comparing `flash_attn_wheels-1.0.8/setup.py` & `flash_attn_wheels-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 import re
 import ast
 from pathlib import Path
 from packaging.version import parse, Version
 import platform
 
 from setuptools import setup, find_packages
-from setuptools.command.install import install
 import subprocess
 
 import urllib.request
 import urllib.error
 import torch
 from torch.utils.cpp_extension import BuildExtension, CppExtension, CUDAExtension, CUDA_HOME
+from wheel.bdist_wheel import bdist_wheel as _bdist_wheel
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 # ninja build does not work unless include_dirs are abs path
 this_dir = os.path.dirname(os.path.abspath(__file__))
 
+PACKAGE_NAME = "flash_attn_wheels"
 
 # @pierce - TODO: Update for proper release
 BASE_WHEEL_URL = "https://github.com/piercefreeman/flash-attention/releases/download/{tag_name}/{wheel_name}"
 
 # FORCE_BUILD: Force a fresh build locally, instead of attempting to find prebuilt wheels
 # SKIP_CUDA_BUILD: Intended to allow CI to use a simple `python setup.py sdist` run to copy over raw files, without any cuda compilation
 FORCE_BUILD = os.getenv("FLASH_ATTENTION_FORCE_BUILD", "FALSE") == "TRUE"
@@ -197,56 +198,69 @@
     local_version = os.environ.get("FLASH_ATTN_LOCAL_VERSION")
     if local_version:
         return f"{public_version}+{local_version}"
     else:
         return str(public_version)
 
 
-class CachedWheelsCommand(install):
-    """
-    Installer hook to scan for existing wheels that match the current platform environment.
-    Falls back to building from source if no wheel is found.
+class CachedWheelsCommand(_bdist_wheel):
+     """
+     The CachedWheelsCommand plugs into the default bdist wheel, which is ran by pip when it cannot
+     find an existing wheel (which is currently the case for all flash attention installs). We use
+     the environment parameters to detect whether there is already a pre-built version of a compatible
+     wheel available and short-circuits the standard full build pipeline.
 
-    """
-    def run(self):
+     """
+     def run(self):
         if FORCE_BUILD:
-            return install.run(self)
+            return super().run()
 
         raise_if_cuda_home_none("flash_attn")
 
         # Determine the version numbers that will be used to determine the correct wheel
         _, cuda_version_raw = get_cuda_bare_metal_version(CUDA_HOME)
         torch_version_raw = parse(torch.__version__)
         python_version = f"cp{sys.version_info.major}{sys.version_info.minor}"
         platform_name = get_platform()
         flash_version = get_package_version()
         cuda_version = f"{cuda_version_raw.major}{cuda_version_raw.minor}"
         torch_version = f"{torch_version_raw.major}.{torch_version_raw.minor}.{torch_version_raw.micro}"
 
         # Determine wheel URL based on CUDA version, torch version, python version and OS
-        wheel_filename = f'flash_attn-{flash_version}+cu{cuda_version}torch{torch_version}-{python_version}-{python_version}-{platform_name}.whl'
+        wheel_filename = f'{PACKAGE_NAME}-{flash_version}+cu{cuda_version}torch{torch_version}-{python_version}-{python_version}-{platform_name}.whl'
         wheel_url = BASE_WHEEL_URL.format(
             tag_name=f"v{flash_version}",
             wheel_name=wheel_filename
         )
         print("Guessing wheel URL: ", wheel_url)
         
         try:
             urllib.request.urlretrieve(wheel_url, wheel_filename)
-            os.system(f'pip install {wheel_filename}')
-            os.remove(wheel_filename)
+
+            # Make the archive
+            # Lifted from the root wheel processing command
+            # https://github.com/pypa/wheel/blob/cf71108ff9f6ffc36978069acb28824b44ae028e/src/wheel/bdist_wheel.py#LL381C9-L381C85
+            if not os.path.exists(self.dist_dir):
+                os.makedirs(self.dist_dir)
+
+            impl_tag, abi_tag, plat_tag = self.get_tag()
+            archive_basename = f"{self.wheel_dist_name}-{impl_tag}-{abi_tag}-{plat_tag}"
+        
+            wheel_path = os.path.join(self.dist_dir, archive_basename + ".whl")
+            print("Raw wheel path", wheel_path)
+            os.rename(wheel_filename, wheel_path)
         except urllib.error.HTTPError:
             print("Precompiled wheel not found. Building from source...")
             # If the wheel could not be downloaded, build from source
-            install.run(self)
+            super().run()
 
 
 setup(
     # @pierce - TODO: Revert for official release
-    name="flash_attn_wheels",
+    name=PACKAGE_NAME,
     version=get_package_version(),
     packages=find_packages(
         exclude=("build", "csrc", "include", "tests", "dist", "docs", "benchmarks", "flash_attn.egg-info",)
     ),
     #author="Tri Dao",
     #author_email="trid@stanford.edu",
     # @pierce - TODO: Revert for official release
@@ -260,18 +274,18 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: Unix",
     ],
     ext_modules=ext_modules,
     cmdclass={
-        'install': CachedWheelsCommand,
+        'bdist_wheel': CachedWheelsCommand,
         "build_ext": BuildExtension
     } if ext_modules else {
-        'install': CachedWheelsCommand,
+        'bdist_wheel': CachedWheelsCommand,
     },
     python_requires=">=3.7",
     install_requires=[
         "torch",
         "einops",
         "packaging",
         "ninja",
```

