# Comparing `tmp/dace-0.9.0.tar.gz` & `tmp/dace-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dace-0.9.0.tar", last modified: Tue Oct 22 22:29:54 2019, max compression
+gzip compressed data, was "dist/dace-0.9.5.tar", last modified: Mon Jan  6 18:53:51 2020, max compression
```

## Comparing `dace-0.9.0.tar` & `dace-0.9.5.tar`

### file list

```diff
@@ -1,156 +1,149 @@
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:54.000000 dace-0.9.0/
--rw-rw-rw-   0 xl        (1000) xl        (1000)     6196 2019-10-22 22:29:54.000000 dace-0.9.0/PKG-INFO
--rw-rw-rw-   0 xl        (1000) xl        (1000)     4979 2019-10-22 22:28:46.000000 dace-0.9.0/README.md
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:53.000000 dace-0.9.0/dace/
--rw-rw-rw-   0 xl        (1000) xl        (1000)      487 2019-10-22 19:03:14.000000 dace-0.9.0/dace/__init__.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:53.000000 dace-0.9.0/dace/codegen/
--rw-rw-rw-   0 xl        (1000) xl        (1000)        0 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/__init__.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     3125 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/codegen.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     1287 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/codeobject.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    19177 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/compiler.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    35947 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/cppunparse.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:53.000000 dace-0.9.0/dace/codegen/instrumentation/
--rw-rw-rw-   0 xl        (1000) xl        (1000)      448 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/instrumentation/__init__.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     5605 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/instrumentation/cuda_events.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)   118201 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/instrumentation/papi.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     3179 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/instrumentation/perfdb.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     6907 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/instrumentation/provider.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     3039 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/instrumentation/timer.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     2719 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/prettycode.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:53.000000 dace-0.9.0/dace/codegen/targets/
--rw-rw-rw-   0 xl        (1000) xl        (1000)        1 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/targets/__init__.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)   106956 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/targets/cpu.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    85294 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/targets/cuda.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    40172 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/targets/framecode.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    10743 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/targets/immaterial.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     4269 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/targets/mpi.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    28830 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/targets/target.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    75018 2019-10-22 19:03:14.000000 dace-0.9.0/dace/codegen/targets/xilinx.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    10091 2019-10-22 19:03:14.000000 dace-0.9.0/dace/config.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    21374 2019-10-22 19:03:14.000000 dace-0.9.0/dace/data.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    22418 2019-10-22 19:03:14.000000 dace-0.9.0/dace/dtypes.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:53.000000 dace-0.9.0/dace/frontend/
--rw-rw-rw-   0 xl        (1000) xl        (1000)        0 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/__init__.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:53.000000 dace-0.9.0/dace/frontend/common/
--rw-rw-rw-   0 xl        (1000) xl        (1000)      298 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/common/__init__.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    73265 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/common/op_impl.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     2847 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/common/op_repository.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:53.000000 dace-0.9.0/dace/frontend/octave/
--rw-rw-rw-   0 xl        (1000) xl        (1000)       46 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/octave/__init__.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     9531 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/octave/ast_arrayaccess.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     7554 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/octave/ast_assign.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    12920 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/octave/ast_expression.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    13987 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/octave/ast_function.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     9051 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/octave/ast_loop.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     7394 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/octave/ast_matrix.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    11128 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/octave/ast_node.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     1193 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/octave/ast_nullstmt.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     2191 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/octave/ast_range.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     3542 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/octave/ast_values.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    10716 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/octave/lexer.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    15644 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/octave/parse.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     6248 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/operations.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:53.000000 dace-0.9.0/dace/frontend/python/
--rw-rw-rw-   0 xl        (1000) xl        (1000)        1 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/python/__init__.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     5252 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/python/astnodes.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    15137 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/python/astutils.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     2177 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/python/decorators.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     6093 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/python/ndarray.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     2208 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/python/ndloop.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)   115982 2019-10-22 22:13:33.000000 dace-0.9.0/dace/frontend/python/newast.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     9432 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/python/parser.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    29097 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/python/simulator.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:53.000000 dace-0.9.0/dace/frontend/tensorflow/
--rw-rw-rw-   0 xl        (1000) xl        (1000)       50 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/tensorflow/__init__.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)   154993 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/tensorflow/tensorflow.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    27423 2019-10-22 19:03:15.000000 dace-0.9.0/dace/frontend/tensorflow/winograd.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:53.000000 dace-0.9.0/dace/graph/
--rw-rw-rw-   0 xl        (1000) xl        (1000)        0 2019-10-22 19:03:15.000000 dace-0.9.0/dace/graph/__init__.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     7967 2019-10-22 19:03:15.000000 dace-0.9.0/dace/graph/dot.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     8405 2019-10-22 19:03:15.000000 dace-0.9.0/dace/graph/edges.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    21858 2019-10-22 19:03:15.000000 dace-0.9.0/dace/graph/graph.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    29633 2019-10-22 19:03:15.000000 dace-0.9.0/dace/graph/labeling.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    28856 2019-10-22 19:03:15.000000 dace-0.9.0/dace/graph/nodes.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    23993 2019-10-22 19:03:15.000000 dace-0.9.0/dace/graph/nxutil.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     1349 2019-10-22 19:03:15.000000 dace-0.9.0/dace/jupyter.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    12315 2019-10-22 19:03:15.000000 dace-0.9.0/dace/memlet.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    45450 2019-10-22 19:03:15.000000 dace-0.9.0/dace/properties.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)   163468 2019-10-22 19:03:15.000000 dace-0.9.0/dace/sdfg.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    26897 2019-10-22 19:03:15.000000 dace-0.9.0/dace/subsets.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    24489 2019-10-22 19:03:15.000000 dace-0.9.0/dace/symbolic.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:53.000000 dace-0.9.0/dace/transformation/
--rw-rw-rw-   0 xl        (1000) xl        (1000)        0 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/__init__.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:53.000000 dace-0.9.0/dace/transformation/dataflow/
--rw-rw-rw-   0 xl        (1000) xl        (1000)     1125 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/__init__.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     5772 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/copy_to_device.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     7208 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/fpga_transform.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    11116 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/gpu_transform.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    23614 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/gpu_transform_local_storage.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     3663 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/map_collapse.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     2230 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/map_dim_interchange.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     4869 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/map_expansion.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     7425 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/map_for_loop.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    21278 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/map_fusion.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     5592 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/map_interchange.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    19498 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/mapreduce.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     6694 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/mpi.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     6721 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/reduce_expansion.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     3617 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/redundant_array.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     9584 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/redundant_array_copying.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    16424 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/stream_transient.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    14066 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/strip_mining.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     3835 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/tensorflow_redundant_array.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    15534 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/tiling.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     5061 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/dataflow/vectorization.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:53.000000 dace-0.9.0/dace/transformation/interstate/
--rw-rw-rw-   0 xl        (1000) xl        (1000)      356 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/interstate/__init__.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     7304 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/interstate/double_buffering.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     1468 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/interstate/fpga_transform_sdfg.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     7785 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/interstate/fpga_transform_state.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    13974 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/interstate/gpu_transform_sdfg.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    14172 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/interstate/sdfg_nesting.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     8828 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/interstate/state_fusion.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     9652 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/optimizer.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    16788 2019-10-22 19:03:15.000000 dace-0.9.0/dace/transformation/pattern_matching.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:53.000000 dace-0.9.0/dace.egg-info/
--rw-rw-rw-   0 xl        (1000) xl        (1000)     6196 2019-10-22 22:29:53.000000 dace-0.9.0/dace.egg-info/PKG-INFO
--rw-rw-rw-   0 xl        (1000) xl        (1000)     4283 2019-10-22 22:29:53.000000 dace-0.9.0/dace.egg-info/SOURCES.txt
--rw-rw-rw-   0 xl        (1000) xl        (1000)        1 2019-10-22 22:29:53.000000 dace-0.9.0/dace.egg-info/dependency_links.txt
--rw-rw-rw-   0 xl        (1000) xl        (1000)       97 2019-10-22 22:29:53.000000 dace-0.9.0/dace.egg-info/requires.txt
--rw-rw-rw-   0 xl        (1000) xl        (1000)       11 2019-10-22 22:29:53.000000 dace-0.9.0/dace.egg-info/top_level.txt
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:53.000000 dace-0.9.0/diode/
--rw-rw-rw-   0 xl        (1000) xl        (1000)        0 2019-10-22 19:03:15.000000 dace-0.9.0/diode/__init__.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     3366 2019-10-22 19:03:15.000000 dace-0.9.0/diode/abstract_sdfg.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)       98 2019-10-22 19:03:15.000000 dace-0.9.0/diode/adjust_settings.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     4852 2019-10-22 19:03:17.000000 dace-0.9.0/diode/config_ui.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:54.000000 dace-0.9.0/diode/db_scripts/
--rw-rw-rw-   0 xl        (1000) xl        (1000)        0 2019-10-22 19:03:17.000000 dace-0.9.0/diode/db_scripts/__init__.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     1870 2019-10-22 19:03:17.000000 dace-0.9.0/diode/db_scripts/db_insert.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     2057 2019-10-22 19:03:17.000000 dace-0.9.0/diode/db_scripts/db_query.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     2967 2019-10-22 19:03:17.000000 dace-0.9.0/diode/db_scripts/db_setup.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    75994 2019-10-22 19:03:17.000000 dace-0.9.0/diode/db_scripts/sql_to_json.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)      953 2019-10-22 19:03:17.000000 dace-0.9.0/diode/db_scripts/sql_to_json_test.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    55667 2019-10-22 19:03:17.000000 dace-0.9.0/diode/diode1.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    11268 2019-10-22 19:03:17.000000 dace-0.9.0/diode/diode_client.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     3494 2019-10-22 19:03:17.000000 dace-0.9.0/diode/diode_optscript_translator.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    51280 2019-10-22 19:03:17.000000 dace-0.9.0/diode/diode_rest.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    31032 2019-10-22 19:03:17.000000 dace-0.9.0/diode/images.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:54.000000 dace-0.9.0/diode/optgraph/
--rw-rw-rw-   0 xl        (1000) xl        (1000)     8331 2019-10-22 19:03:17.000000 dace-0.9.0/diode/optgraph/DaceState.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)        1 2019-10-22 19:03:17.000000 dace-0.9.0/diode/optgraph/__init__.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    14061 2019-10-22 19:03:17.000000 dace-0.9.0/diode/optgraph/optgraph.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    14492 2019-10-22 19:03:17.000000 dace-0.9.0/diode/pattern_editor.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     1392 2019-10-22 19:03:17.000000 dace-0.9.0/diode/performance_plot.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    23385 2019-10-22 19:03:17.000000 dace-0.9.0/diode/property_renderer.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    19690 2019-10-22 19:03:17.000000 dace-0.9.0/diode/remote_execution.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     8875 2019-10-22 19:03:17.000000 dace-0.9.0/diode/rendered_graph.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    25949 2019-10-22 19:03:17.000000 dace-0.9.0/diode/rendered_graph_html5.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     5881 2019-10-22 19:03:17.000000 dace-0.9.0/diode/rendered_graphs.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)    29105 2019-10-22 19:03:17.000000 dace-0.9.0/diode/sdfg_editor.py
--rw-rw-rw-   0 xl        (1000) xl        (1000)     1119 2019-10-22 19:03:17.000000 dace-0.9.0/diode/sdfv.py
-drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2019-10-22 22:29:54.000000 dace-0.9.0/scripts/
--rwxrwxrwx   0 xl        (1000) xl        (1000)     1648 2019-10-22 19:03:18.000000 dace-0.9.0/scripts/dacelab
--rwxrwxrwx   0 xl        (1000) xl        (1000)       47 2019-10-22 19:03:18.000000 dace-0.9.0/scripts/diode
--rwxrwxrwx   0 xl        (1000) xl        (1000)       41 2019-10-22 19:03:18.000000 dace-0.9.0/scripts/sdfv
--rw-rw-rw-   0 xl        (1000) xl        (1000)       38 2019-10-22 22:29:54.000000 dace-0.9.0/setup.cfg
--rw-rw-rw-   0 xl        (1000) xl        (1000)     2597 2019-10-22 22:19:06.000000 dace-0.9.0/setup.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     6579 2020-01-06 18:53:51.000000 dace-0.9.5/PKG-INFO
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     5346 2019-12-25 16:20:41.000000 dace-0.9.5/README.md
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/dace/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)      488 2019-11-06 16:08:10.000000 dace-0.9.5/dace/__init__.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/dace/codegen/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)        0 2019-10-22 19:03:14.000000 dace-0.9.5/dace/codegen/__init__.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     5824 2019-12-25 16:20:41.000000 dace-0.9.5/dace/codegen/codegen.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     1521 2019-12-25 16:20:41.000000 dace-0.9.5/dace/codegen/codeobject.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    21333 2019-12-25 16:20:41.000000 dace-0.9.5/dace/codegen/compiler.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    44126 2020-01-06 18:40:49.000000 dace-0.9.5/dace/codegen/cppunparse.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/dace/codegen/instrumentation/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)      448 2019-10-22 19:03:14.000000 dace-0.9.5/dace/codegen/instrumentation/__init__.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     5605 2019-10-22 19:03:14.000000 dace-0.9.5/dace/codegen/instrumentation/cuda_events.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)   116018 2020-01-06 18:40:49.000000 dace-0.9.5/dace/codegen/instrumentation/papi.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     3179 2019-10-22 19:03:14.000000 dace-0.9.5/dace/codegen/instrumentation/perfdb.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     6907 2019-12-25 16:20:41.000000 dace-0.9.5/dace/codegen/instrumentation/provider.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     3039 2019-10-22 19:03:14.000000 dace-0.9.5/dace/codegen/instrumentation/timer.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     2916 2019-12-25 16:20:41.000000 dace-0.9.5/dace/codegen/prettycode.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/dace/codegen/targets/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)        1 2019-10-22 19:03:14.000000 dace-0.9.5/dace/codegen/targets/__init__.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)      977 2020-01-06 18:40:49.000000 dace-0.9.5/dace/codegen/targets/common.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)   112850 2020-01-06 18:40:49.000000 dace-0.9.5/dace/codegen/targets/cpu.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    86677 2020-01-06 18:40:49.000000 dace-0.9.5/dace/codegen/targets/cuda.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    62131 2020-01-06 18:40:49.000000 dace-0.9.5/dace/codegen/targets/fpga.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    42192 2019-12-25 16:20:41.000000 dace-0.9.5/dace/codegen/targets/framecode.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    10605 2020-01-06 18:40:49.000000 dace-0.9.5/dace/codegen/targets/immaterial.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    52422 2020-01-06 18:40:49.000000 dace-0.9.5/dace/codegen/targets/intel_fpga.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     4427 2019-12-25 16:20:41.000000 dace-0.9.5/dace/codegen/targets/mpi.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    28792 2019-12-25 16:20:41.000000 dace-0.9.5/dace/codegen/targets/target.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    31410 2020-01-06 18:40:49.000000 dace-0.9.5/dace/codegen/targets/xilinx.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    10158 2019-12-25 16:20:41.000000 dace-0.9.5/dace/config.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    20586 2020-01-06 18:40:49.000000 dace-0.9.5/dace/data.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    31317 2019-12-25 16:20:41.000000 dace-0.9.5/dace/dtypes.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/dace/frontend/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)        0 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/__init__.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/dace/frontend/common/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)      298 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/common/__init__.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    72983 2020-01-06 18:40:49.000000 dace-0.9.5/dace/frontend/common/op_impl.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     2847 2019-12-25 16:20:41.000000 dace-0.9.5/dace/frontend/common/op_repository.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/dace/frontend/octave/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)       47 2019-12-25 16:20:41.000000 dace-0.9.5/dace/frontend/octave/__init__.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     9423 2019-12-25 16:20:41.000000 dace-0.9.5/dace/frontend/octave/ast_arrayaccess.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     7554 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/octave/ast_assign.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    12920 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/octave/ast_expression.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    13987 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/octave/ast_function.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     9051 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/octave/ast_loop.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     7394 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/octave/ast_matrix.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    11128 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/octave/ast_node.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     1193 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/octave/ast_nullstmt.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     2191 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/octave/ast_range.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     3542 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/octave/ast_values.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    10716 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/octave/lexer.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    15644 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/octave/parse.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     6246 2019-12-25 16:20:41.000000 dace-0.9.5/dace/frontend/operations.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/dace/frontend/python/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)        1 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/python/__init__.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     5252 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/python/astnodes.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    15137 2019-12-25 16:20:41.000000 dace-0.9.5/dace/frontend/python/astutils.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     2177 2019-12-25 16:20:41.000000 dace-0.9.5/dace/frontend/python/decorators.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     2181 2019-12-25 16:20:41.000000 dace-0.9.5/dace/frontend/python/ndloop.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)   141423 2020-01-06 18:40:49.000000 dace-0.9.5/dace/frontend/python/newast.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    10038 2019-12-25 16:20:41.000000 dace-0.9.5/dace/frontend/python/parser.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    29094 2019-12-25 16:20:41.000000 dace-0.9.5/dace/frontend/python/simulator.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     2110 2019-11-06 16:08:10.000000 dace-0.9.5/dace/frontend/python/wrappers.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/dace/frontend/tensorflow/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)       50 2019-10-22 19:03:15.000000 dace-0.9.5/dace/frontend/tensorflow/__init__.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)   154975 2019-12-25 16:20:41.000000 dace-0.9.5/dace/frontend/tensorflow/tensorflow.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    27405 2019-12-25 16:20:41.000000 dace-0.9.5/dace/frontend/tensorflow/winograd.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/dace/graph/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)        0 2019-10-22 19:03:15.000000 dace-0.9.5/dace/graph/__init__.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     7966 2019-12-25 16:20:41.000000 dace-0.9.5/dace/graph/dot.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     8706 2019-12-25 16:20:41.000000 dace-0.9.5/dace/graph/edges.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    21995 2020-01-06 18:40:49.000000 dace-0.9.5/dace/graph/graph.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    29943 2020-01-06 18:40:49.000000 dace-0.9.5/dace/graph/labeling.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    30650 2020-01-06 18:40:49.000000 dace-0.9.5/dace/graph/nodes.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    23930 2020-01-06 18:40:49.000000 dace-0.9.5/dace/graph/nxutil.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     1389 2020-01-06 18:40:49.000000 dace-0.9.5/dace/jupyter.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    13436 2020-01-06 18:40:49.000000 dace-0.9.5/dace/memlet.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    39372 2019-12-25 16:20:41.000000 dace-0.9.5/dace/properties.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)   172731 2020-01-06 18:40:49.000000 dace-0.9.5/dace/sdfg.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     7035 2019-12-25 16:20:41.000000 dace-0.9.5/dace/serialize.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    26260 2020-01-06 18:40:49.000000 dace-0.9.5/dace/subsets.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    25542 2020-01-06 18:40:49.000000 dace-0.9.5/dace/symbolic.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/dace/transformation/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)        0 2019-10-22 19:03:15.000000 dace-0.9.5/dace/transformation/__init__.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/dace/transformation/dataflow/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     1183 2020-01-06 18:40:49.000000 dace-0.9.5/dace/transformation/dataflow/__init__.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     7103 2020-01-06 18:40:49.000000 dace-0.9.5/dace/transformation/dataflow/copy_to_device.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     9979 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/dataflow/double_buffering.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     7202 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/dataflow/fpga_transform.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     4933 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/dataflow/gpu_transform.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    24873 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/dataflow/gpu_transform_local_storage.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     5566 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/dataflow/local_storage.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     4263 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/dataflow/map_collapse.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     2264 2019-12-25 16:20:41.000000 dace-0.9.5/dace/transformation/dataflow/map_dim_interchange.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     4579 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/dataflow/map_expansion.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     4743 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/dataflow/map_for_loop.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    18215 2019-12-25 16:20:41.000000 dace-0.9.5/dace/transformation/dataflow/map_fusion.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     6248 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/dataflow/map_interchange.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    20404 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/dataflow/mapreduce.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     4321 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/dataflow/merge_arrays.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     6524 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/dataflow/mpi.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     6721 2019-10-22 19:03:15.000000 dace-0.9.5/dace/transformation/dataflow/reduce_expansion.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     3617 2019-12-25 16:20:41.000000 dace-0.9.5/dace/transformation/dataflow/redundant_array.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     9584 2019-12-25 16:20:41.000000 dace-0.9.5/dace/transformation/dataflow/redundant_array_copying.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     7807 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/dataflow/stream_transient.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    13023 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/dataflow/strip_mining.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     3835 2019-12-25 16:20:41.000000 dace-0.9.5/dace/transformation/dataflow/tensorflow_redundant_array.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     3631 2019-12-25 16:20:41.000000 dace-0.9.5/dace/transformation/dataflow/tiling.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     6379 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/dataflow/vectorization.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     9198 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/helpers.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/dace/transformation/interstate/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)      311 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/interstate/__init__.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     1938 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/interstate/fpga_transform_sdfg.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    11895 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/interstate/fpga_transform_state.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    14639 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/interstate/gpu_transform_sdfg.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    21466 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/interstate/sdfg_nesting.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     9478 2019-12-25 16:20:41.000000 dace-0.9.5/dace/transformation/interstate/state_fusion.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    12175 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/optimizer.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    14915 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/pattern_matching.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     4633 2020-01-06 18:40:50.000000 dace-0.9.5/dace/transformation/testing.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/dace.egg-info/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     6579 2020-01-06 18:53:50.000000 dace-0.9.5/dace.egg-info/PKG-INFO
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     4183 2020-01-06 18:53:50.000000 dace-0.9.5/dace.egg-info/SOURCES.txt
+-rw-rw-rw-   0 xl        (1000) xl        (1000)        1 2020-01-06 18:53:50.000000 dace-0.9.5/dace.egg-info/dependency_links.txt
+-rw-rw-rw-   0 xl        (1000) xl        (1000)      116 2020-01-06 18:53:50.000000 dace-0.9.5/dace.egg-info/requires.txt
+-rw-rw-rw-   0 xl        (1000) xl        (1000)       11 2020-01-06 18:53:50.000000 dace-0.9.5/dace.egg-info/top_level.txt
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/diode/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     7694 2020-01-06 18:40:50.000000 dace-0.9.5/diode/DaceState.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)        0 2019-10-22 19:03:15.000000 dace-0.9.5/diode/__init__.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     3366 2019-10-22 19:03:15.000000 dace-0.9.5/diode/abstract_sdfg.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)       99 2019-12-25 16:20:41.000000 dace-0.9.5/diode/adjust_settings.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     4852 2019-10-22 19:03:17.000000 dace-0.9.5/diode/config_ui.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/diode/db_scripts/
+-rw-rw-rw-   0 xl        (1000) xl        (1000)        0 2019-10-22 19:03:17.000000 dace-0.9.5/diode/db_scripts/__init__.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     2998 2019-12-25 16:20:41.000000 dace-0.9.5/diode/db_scripts/db_setup.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    76085 2019-12-25 16:20:41.000000 dace-0.9.5/diode/db_scripts/sql_to_json.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     1117 2019-12-25 16:20:41.000000 dace-0.9.5/diode/db_scripts/sql_to_json_test.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    12765 2019-12-25 16:20:41.000000 dace-0.9.5/diode/diode_client.py
+-rwxrwxrwx   0 xl        (1000) xl        (1000)    48230 2020-01-06 18:40:50.000000 dace-0.9.5/diode/diode_server.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)    18541 2020-01-06 18:40:50.000000 dace-0.9.5/diode/remote_execution.py
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     1594 2019-12-25 16:20:41.000000 dace-0.9.5/diode/sdfv.py
+drwxrwxrwx   0 xl        (1000) xl        (1000)        0 2020-01-06 18:53:51.000000 dace-0.9.5/scripts/
+-rwxrwxrwx   0 xl        (1000) xl        (1000)     1648 2019-10-22 19:03:18.000000 dace-0.9.5/scripts/dacelab
+-rwxrwxrwx   0 xl        (1000) xl        (1000)       49 2019-12-25 16:20:43.000000 dace-0.9.5/scripts/diode
+-rwxrwxrwx   0 xl        (1000) xl        (1000)       41 2019-10-22 19:03:18.000000 dace-0.9.5/scripts/sdfv
+-rw-rw-rw-   0 xl        (1000) xl        (1000)       38 2020-01-06 18:53:51.000000 dace-0.9.5/setup.cfg
+-rw-rw-rw-   0 xl        (1000) xl        (1000)     2344 2020-01-06 18:46:08.000000 dace-0.9.5/setup.py
```

### Comparing `dace-0.9.0/PKG-INFO` & `dace-0.9.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: dace
-Version: 0.9.0
+Version: 0.9.5
 Summary: Data-Centric Parallel Programming Framework
 Home-page: https://github.com/spcl/dace
 Author: SPCL @ ETH Zurich
 Author-email: talbn@inf.ethz.ch
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/spcl/dace.svg?branch=master)](https://travis-ci.org/spcl/dace)
+        [![Documentation Status](https://readthedocs.org/projects/spcldace/badge/?version=latest)](https://spcldace.readthedocs.io/en/latest/?badge=latest)
+        [![PyPI version](https://badge.fury.io/py/dace.svg)](https://badge.fury.io/py/dace)
         
         
         ![D](dace.svg)aCe - Data-Centric Parallel Programming
         =====================================================
         
         _Decoupling domain science from performance optimization._
         
@@ -20,15 +22,15 @@
         DaCe can be written inline in Python and transformed in the command-line/Jupyter Notebooks, or SDFGs can be interactively modified using the Data-centric Interactive Optimization Development Environment (DIODE, currently experimental).
         
         For more information, see our [paper](http://www.arxiv.org/abs/1902.10345).
         
         Tutorials
         ---------
         
-        * _Data-Centric Python Programs with NumPy (coming soon)_
+        * [Data-Centric Python Programs with NumPy](https://nbviewer.jupyter.org/github/spcl/dace/blob/master/tutorials/numpy_frontend.ipynb)
         * [Explicit Dataflow in Python](https://nbviewer.jupyter.org/github/spcl/dace/blob/master/tutorials/explicit.ipynb)
         * [SDFG API](https://nbviewer.jupyter.org/github/spcl/dace/blob/master/tutorials/sdfg_api.ipynb)
         * [Transformations](https://nbviewer.jupyter.org/github/spcl/dace/blob/master/tutorials/transformations.ipynb)
         
         Installation and Dependencies
         -----------------------------
         
@@ -40,21 +42,21 @@
          * CMake 2.8.12 or newer (for Windows, CMake 3.15 is recommended)
         
         Running
         -------
         
         **Python scripts:** Run DaCe programs (in implicit, explicit, or TensorFlow syntax) using Python directly.
         
-        **DIODE interactive development (experimental):**: Either run the installed script `diode`, or call `python3 -m diode.diode_rest` from the shell. Then, follow the printed instructions to enter the web interface.
+        **DIODE interactive development (experimental):**: Either run the installed script `diode`, or call `python3 -m diode.diode_server` from the shell. Then, follow the printed instructions to enter the web interface.
         
         **Octave scripts (experimental):** `.m` files can be run using the installed script `dacelab`, which will create the appropriate SDFG file.
         
         **Jupyter Notebooks:** DaCe is Jupyter-compatible. If a result is an SDFG or a state, it will show up directly in the notebook. See the [tutorials](tutorials) for examples.
         
-        **SDFV (standalone SDFG viewer):** To view SDFGs separately, run the `sdfv` installed script with the `.sdfg` file as an argument. Alternatively, you can open `diode/sdfv.html` directly and choose a file in the browser.
+        **[SDFV (standalone SDFG viewer)](https://spcl.github.io/dace/sdfv.html):** To view SDFGs separately, run the `sdfv` installed script with the `.sdfg` file as an argument. Alternatively, you can use the link or open `diode/sdfv.html` directly and choose a file in the browser.
         
         **Note for Windows/Visual C++ users:** If compilation fails in the linkage phase, try setting the following environment variable to force Visual C++ to use Multi-Threaded linkage:
         ```
         X:\path\to\dace> set _CL_=/MT
         ```
```

### Comparing `dace-0.9.0/README.md` & `dace-0.9.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 [![Build Status](https://travis-ci.org/spcl/dace.svg?branch=master)](https://travis-ci.org/spcl/dace)
+[![Documentation Status](https://readthedocs.org/projects/spcldace/badge/?version=latest)](https://spcldace.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/dace.svg)](https://badge.fury.io/py/dace)
 
 
 ![D](dace.svg)aCe - Data-Centric Parallel Programming
 =====================================================
 
 _Decoupling domain science from performance optimization._
 
@@ -12,15 +14,15 @@
 DaCe can be written inline in Python and transformed in the command-line/Jupyter Notebooks, or SDFGs can be interactively modified using the Data-centric Interactive Optimization Development Environment (DIODE, currently experimental).
 
 For more information, see our [paper](http://www.arxiv.org/abs/1902.10345).
 
 Tutorials
 ---------
 
-* _Data-Centric Python Programs with NumPy (coming soon)_
+* [Data-Centric Python Programs with NumPy](https://nbviewer.jupyter.org/github/spcl/dace/blob/master/tutorials/numpy_frontend.ipynb)
 * [Explicit Dataflow in Python](https://nbviewer.jupyter.org/github/spcl/dace/blob/master/tutorials/explicit.ipynb)
 * [SDFG API](https://nbviewer.jupyter.org/github/spcl/dace/blob/master/tutorials/sdfg_api.ipynb)
 * [Transformations](https://nbviewer.jupyter.org/github/spcl/dace/blob/master/tutorials/transformations.ipynb)
 
 Installation and Dependencies
 -----------------------------
 
@@ -32,21 +34,21 @@
  * CMake 2.8.12 or newer (for Windows, CMake 3.15 is recommended)
 
 Running
 -------
 
 **Python scripts:** Run DaCe programs (in implicit, explicit, or TensorFlow syntax) using Python directly.
 
-**DIODE interactive development (experimental):**: Either run the installed script `diode`, or call `python3 -m diode.diode_rest` from the shell. Then, follow the printed instructions to enter the web interface.
+**DIODE interactive development (experimental):**: Either run the installed script `diode`, or call `python3 -m diode.diode_server` from the shell. Then, follow the printed instructions to enter the web interface.
 
 **Octave scripts (experimental):** `.m` files can be run using the installed script `dacelab`, which will create the appropriate SDFG file.
 
 **Jupyter Notebooks:** DaCe is Jupyter-compatible. If a result is an SDFG or a state, it will show up directly in the notebook. See the [tutorials](tutorials) for examples.
 
-**SDFV (standalone SDFG viewer):** To view SDFGs separately, run the `sdfv` installed script with the `.sdfg` file as an argument. Alternatively, you can open `diode/sdfv.html` directly and choose a file in the browser.
+**[SDFV (standalone SDFG viewer)](https://spcl.github.io/dace/sdfv.html):** To view SDFGs separately, run the `sdfv` installed script with the `.sdfg` file as an argument. Alternatively, you can use the link or open `diode/sdfv.html` directly and choose a file in the browser.
 
 **Note for Windows/Visual C++ users:** If compilation fails in the linkage phase, try setting the following environment variable to force Visual C++ to use Multi-Threaded linkage:
 ```
 X:\path\to\dace> set _CL_=/MT
 ```
```

### Comparing `dace-0.9.0/dace/codegen/codeobject.py` & `dace-0.9.5/dace/codegen/codeobject.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 class CodeObject(object):
     name = Property(dtype=str, desc="Filename to use")
     code = Property(dtype=str, desc="The code attached to this object")
     language = Property(
         dtype=str,
         desc="Language used for this code (same " +
         "as its file extension)")  # dtype=dtypes.Language?
-    target = Property(dtype=type, desc="Target to use for compilation")
+    target = Property(
+        dtype=type, desc="Target to use for compilation", allow_none=True)
+    target_type = Property(
+        dtype=str,
+        desc="Sub-target within target (e.g., host or device code)",
+        default="")
     title = Property(dtype=str, desc="Title of code for GUI")
     extra_compiler_kwargs = Property(
         dtype=dict,
         desc="Additional compiler argument "
         "variables to add to template")
     linkable = Property(
         dtype=bool, desc='Should this file participate in '
@@ -21,18 +26,20 @@
 
     def __init__(self,
                  name,
                  code,
                  language,
                  target,
                  title,
+                 target_type="",
                  additional_compiler_kwargs=None,
                  linkable=True):
         super(CodeObject, self).__init__()
 
         self.name = name
         self.code = code
         self.language = language
         self.target = target
+        self.target_type = target_type
         self.title = title
         self.extra_compiler_kwargs = additional_compiler_kwargs or {}
         self.linkable = linkable
```

### Comparing `dace-0.9.0/dace/codegen/compiler.py` & `dace-0.9.5/dace/codegen/compiler.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,28 +3,25 @@
     compiles each target separately, links all targets to one binary, and
     returns the corresponding CompiledSDFG object. """
 
 from __future__ import print_function
 
 import ctypes
 import os
-import re
 import six
 import shutil
+import hashlib
 import subprocess
-import string
-import subprocess as sp
 import re
 from typing import List
 import numpy as np
 
 import dace
 from dace.frontend import operations
-from dace.frontend.python import ndarray
-from dace import symbolic, dtypes, data as dt
+from dace import symbolic, data as dt
 from dace.config import Config
 from dace.codegen import codegen
 from dace.codegen.codeobject import CodeObject
 from dace.codegen.targets.target import make_absolute
 
 
 # Specialized exception classes
@@ -45,24 +42,24 @@
 
 
 class ReloadableDLL(object):
     """ A reloadable shared object (or dynamically linked library), which
         bypasses Python's dynamic library reloading issues. """
 
     def __init__(self, library_filename, program_name):
-        """ Creates a new reloadable shared object. 
-            @param library_filename: Path to library file.
-            @param program_name: Name of the DaCe program (for use in finding
+        """ Creates a new reloadable shared object.
+            :param library_filename: Path to library file.
+            :param program_name: Name of the DaCe program (for use in finding
                                  the stub library loader).
         """
         self._stub_filename = os.path.join(
             os.path.dirname(os.path.realpath(library_filename)),
             'libdacestub_%s.%s' %
             (program_name, Config.get('compiler', 'library_extension')))
-        self._library_filename = library_filename
+        self._library_filename = os.path.realpath(library_filename)
         self._stub = None
         self._lib = None
 
     def get_symbol(self, name, restype=ctypes.c_int):
         """ Returns a symbol (e.g., function name) in the loaded library. """
 
         if self._lib is None or self._lib.value is None:
@@ -143,27 +140,31 @@
         self._lastargs = ()
         lib.load()  # Explicitly load the library
         self._init = lib.get_symbol('__dace_init')
         self._exit = lib.get_symbol('__dace_exit')
         self._cfunc = lib.get_symbol('__program_{}'.format(sdfg.name))
 
     @property
+    def filename(self):
+        return self._lib._library_filename
+
+    @property
     def sdfg(self):
         return self._sdfg
 
     def __del__(self):
-        if self._initialized == True:
+        if self._initialized is True:
             self.finalize(*self._lastargs)
             self._initialized = False
         self._lib.unload()
 
     def _construct_args(self, **kwargs):
         """ Main function that controls argument construction for calling
-            the C prototype of the SDFG. 
-            
+            the C prototype of the SDFG.
+
             Organizes arguments first by `sdfg.arglist`, then data descriptors
             by alphabetical order, then symbols by alphabetical order.
         """
 
         # Argument construction
         sig = self._sdfg.signature_arglist(with_types=False)
         typedict = self._sdfg.arglist()
@@ -242,19 +243,18 @@
         # Replace symbols with their values
         callparams = tuple(
             (atype(symbolic.eval(arg)),
              atype) if symbolic.issymbolic(arg, constants) else (arg, atype)
             for arg, atype in callparams)
 
         # Replace arrays with their pointers
-        newargs = tuple(
-            (ctypes.c_void_p(arg.__array_interface__['data'][0]),
-             atype) if (isinstance(arg, ndarray.ndarray)
-                        or isinstance(arg, np.ndarray)) else (arg, atype)
-            for arg, atype in callparams)
+        newargs = tuple((ctypes.c_void_p(arg.__array_interface__['data'][0]),
+                         atype) if isinstance(arg, np.ndarray) else (arg,
+                                                                     atype)
+                        for arg, atype in callparams)
 
         newargs = tuple(
             atype(arg) if (not isinstance(arg, ctypes._SimpleCData)) else arg
             for arg, atype in newargs)
 
         self._lastargs = newargs
         return self._lastargs
@@ -268,46 +268,74 @@
         self._initialized = True
 
     def finalize(self, *argtuple):
         if self._exit is not None:
             self._exit(*argtuple)
 
     def __call__(self, **kwargs):
-        argtuple = self._construct_args(**kwargs)
+        try:
+            argtuple = self._construct_args(**kwargs)
 
-        # Call initializer function if necessary, then SDFG
-        if self._initialized == False:
-            self.initialize(*argtuple)
-
-        # PROFILING
-        if Config.get_bool('profiling'):
-            operations.timethis(self._sdfg.name, 'DaCe', 0, self._cfunc,
-                                *argtuple)
-        else:
-            return self._cfunc(*argtuple)
+            # Call initializer function if necessary, then SDFG
+            if self._initialized is False:
+                self.initialize(*argtuple)
+
+            # PROFILING
+            if Config.get_bool('profiling'):
+                operations.timethis(self._sdfg.name, 'DaCe', 0, self._cfunc,
+                                    *argtuple)
+            else:
+                return self._cfunc(*argtuple)
+        except (RuntimeError, TypeError, UnboundLocalError, KeyError,
+                DuplicateDLLError, ReferenceError):
+            self._lib.unload()
+            raise
 
 
 def unique_flags(flags):
     pattern = '[^ ]+[`\'"][^"\'`]+["\'`]|[^ ]+'
     if not isinstance(flags, str):
         flags = " ".join(flags)
     return set(re.findall(pattern, flags))
 
 
+def identical_file_exists(filename: str, file_contents: str):
+    # If file did not exist before, return False
+    if not os.path.isfile(filename):
+        return False
+
+    # Read file in blocks and compare strings
+    block_size = 65536
+    with open(filename, 'r') as fp:
+        file_buffer = fp.read(block_size)
+        while len(file_buffer) > 0:
+            block = file_contents[:block_size]
+            if file_buffer != block:
+                return False
+            file_contents = file_contents[block_size:]
+            file_buffer = fp.read(block_size)
+
+    # More contents appended to the new file
+    if len(file_contents) > 0:
+        return False
+
+    return True
+
+
 def generate_program_folder(sdfg,
                             code_objects: List[CodeObject],
                             out_path: str,
                             config=None):
     """ Writes all files required to configure and compile the DaCe program
         into the specified folder.
 
-        @param sdfg: The SDFG to generate the program folder for.
-        @param code_objects: List of generated code objects.
-        @param out_path: The folder in which the build files should be written.
-        @return: Path to the program folder.
+        :param sdfg: The SDFG to generate the program folder for.
+        :param code_objects: List of generated code objects.
+        :param out_path: The folder in which the build files should be written.
+        :return: Path to the program folder.
     """
 
     src_path = os.path.join(out_path, "src")
 
     try:
         os.makedirs(src_path)
     except FileExistsError:
@@ -316,31 +344,39 @@
     filelist = []
     # Write each code object to a file
     for code_object in code_objects:
 
         name = code_object.name
         extension = code_object.language
         target_name = code_object.target.target_name
+        target_type = code_object.target_type
 
         # Create target folder
         target_folder = os.path.join(src_path, target_name)
+        if target_type:
+            target_folder = os.path.join(target_folder, target_type)
         try:
             os.makedirs(target_folder)
         except FileExistsError:
             pass
 
         # Write code to file
         basename = "{}.{}".format(name, extension)
         code_path = os.path.join(target_folder, basename)
-        with open(code_path, "w") as code_file:
-            clean_code = re.sub(r'[ \t]*////__DACE:[^\n]*', '',
-                                code_object.code)
-            code_file.write(clean_code)
+        clean_code = re.sub(r'[ \t]*////__DACE:[^\n]*', '', code_object.code)
 
-        filelist.append("{},{}".format(target_name, basename))
+        # Save the file only if it changed (keeps old timestamps and saves
+        # build time)
+        if not identical_file_exists(code_path, clean_code):
+            with open(code_path, "w") as code_file:
+                code_file.write(clean_code)
+
+        if code_object.linkable == True:
+            filelist.append("{},{},{}".format(target_name, target_type,
+                                              basename))
 
     # Write list of files
     with open(os.path.join(out_path, "dace_files.csv"), "w") as filelist_file:
         filelist_file.write("\n".join(filelist))
 
     # Copy snapshot of configuration script
     if config is not None:
@@ -350,22 +386,26 @@
 
     # Save the SDFG itself
     sdfg.save(os.path.join(out_path, "program.sdfg"))
 
     return out_path
 
 
-def configure_and_compile(program_folder, program_name=None):
+def configure_and_compile(program_folder,
+                          program_name=None,
+                          output_stream=None):
     """ Configures and compiles a DaCe program in the specified folder into a
         shared library file.
 
-        @param program_folder: Folder containing all files necessary to build,
+        :param program_folder: Folder containing all files necessary to build,
                                equivalent to what was passed to
                                `generate_program_folder`.
-        @return: Path to the compiled shared library file.
+        :param output_stream: Additional output stream to write to (used for
+                              DIODE client).
+        :return: Path to the compiled shared library file.
     """
 
     if program_name is None:
         program_name = os.path.basename(program_folder)
     program_folder = os.path.abspath(program_folder)
     src_folder = os.path.join(program_folder, "src")
 
@@ -384,25 +424,29 @@
         line.strip().split(",")
         for line in open(os.path.join(program_folder, "dace_files.csv"), "r")
     ]
 
     # Get absolute paths and targets for all source files
     files = []
     targets = {}  # {target name: target class}
-    for target_name, file_name in file_list:
-        path = os.path.join(src_folder, target_name, file_name)
+    for target_name, target_type, file_name in file_list:
+        if target_type:
+            path = os.path.join(target_name, target_type, file_name)
+        else:
+            path = os.path.join(target_name, file_name)
         files.append(path)
         targets[target_name] = codegen.STRING_TO_TARGET[target_name]
 
     # Start forming CMake command
     dace_path = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
     cmake_command = [
         "cmake",
         "-A x64" if os.name == 'nt' else "",  # Windows-specific flag
         '"' + os.path.join(dace_path, "codegen") + '"',
+        "-DDACE_SRC_DIR=\"{}\"".format(src_folder),
         "-DDACE_FILES=\"{}\"".format(";".join(files)),
         "-DDACE_PROGRAM_NAME={}".format(program_name),
     ]
 
     # Replace backslashes with forward slashes
     cmake_command = [cmd.replace('\\', '/') for cmd in cmake_command]
 
@@ -422,43 +466,56 @@
         "-DDACE_LIBS=\"{}\"".format(" ".join(libraries)),
         "-DCMAKE_LINKER=\"{}\"".format(
             make_absolute(Config.get('compiler', 'linker', 'executable'))),
         "-DCMAKE_SHARED_LINKER_FLAGS=\"{}\"".format(
             Config.get('compiler', 'linker', 'args') +
             Config.get('compiler', 'linker', 'additional_args')),
     ]
+    cmake_command = ' '.join(cmake_command)
 
+    cmake_filename = os.path.join(build_folder, 'cmake_configure.sh')
     ##############################################
     # Configure
     try:
-        _run_liveoutput(" ".join(cmake_command), shell=True, cwd=build_folder)
+        _run_liveoutput(
+            cmake_command,
+            shell=True,
+            cwd=build_folder,
+            output_stream=output_stream)
     except subprocess.CalledProcessError as ex:
         # Clean CMake directory and try once more
         if Config.get_bool('debugprint'):
             print('Cleaning CMake build folder and retrying...')
         shutil.rmtree(build_folder)
         os.makedirs(build_folder)
         try:
             _run_liveoutput(
-                " ".join(cmake_command), shell=True, cwd=build_folder)
+                cmake_command,
+                shell=True,
+                cwd=build_folder,
+                output_stream=output_stream)
         except subprocess.CalledProcessError as ex:
             # If still unsuccessful, print results
             if Config.get_bool('debugprint'):
                 raise CompilerConfigurationError('Configuration failure')
             else:
                 raise CompilerConfigurationError('Configuration failure:\n' +
                                                  ex.output)
 
+        with open(cmake_filename, "w") as fp:
+            fp.write(cmake_command)
+
     # Compile and link
     try:
         _run_liveoutput(
             "cmake --build . --config %s" % (Config.get(
                 'compiler', 'build_type')),
             shell=True,
-            cwd=build_folder)
+            cwd=build_folder,
+            output_stream=output_stream)
     except subprocess.CalledProcessError as ex:
         # If unsuccessful, print results
         if Config.get_bool('debugprint'):
             raise CompilationError('Compiler failure')
         else:
             raise CompilationError('Compiler failure:\n' + ex.output)
 
@@ -496,15 +553,15 @@
     else:
         name = os.path.join(
             '.dacecache', object_name, "build",
             'lib%s_%s.%s' % (object_name, object_hash, lib_extension))
     return name
 
 
-def _run_liveoutput(command, **kwargs):
+def _run_liveoutput(command, output_stream=None, **kwargs):
     process = subprocess.Popen(
         command, stderr=subprocess.STDOUT, stdout=subprocess.PIPE, **kwargs)
     output = six.StringIO()
     while True:
         line = process.stdout.readline().rstrip()
         if not line:
             break
@@ -512,14 +569,16 @@
         if Config.get_bool('debugprint'):
             print(line.decode('utf-8'), flush=True)
     stdout, stderr = process.communicate()
     if Config.get_bool('debugprint'):
         print(stdout.decode('utf-8'), flush=True)
         if stderr is not None:
             print(stderr.decode('utf-8'), flush=True)
+    if output_stream is not None:
+        output_stream.write(stdout.decode('utf-8'), flush=True)
     output.write(stdout.decode('utf-8'))
     if stderr is not None:
         output.write(stderr.decode('utf-8'))
 
     # An error occurred, raise exception
     if process.returncode != 0:
         raise subprocess.CalledProcessError(process.returncode, command,
```

### Comparing `dace-0.9.0/dace/codegen/instrumentation/cuda_events.py` & `dace-0.9.5/dace/codegen/instrumentation/cuda_events.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/codegen/instrumentation/papi.py` & `dace-0.9.5/dace/codegen/instrumentation/papi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dace.codegen.instrumentation.provider import InstrumentationProvider
+from dace.codegen.targets.common import sym2cpp
 from dace.graph.nodes import EntryNode, ExitNode, MapEntry, MapExit, Tasklet
 from dace.graph.graph import SubgraphView
 from dace.memlet import Memlet
 from dace.data import Array
 
 from dace import symbolic, subsets
 from dace.codegen import cppunparse
@@ -23,76 +24,14 @@
 from dace.graph import nodes
 
 # Helper function to get the module path
 if __name__ == "__main__":
     print("path: " + os.path.dirname(__file__))
 
 
-############# COPIED FROM cpu.py TO AVOID IMPORT LOOPS. TODO: Move elsewhere #############
-def sym2cpp(s):
-    """ Converts an array of symbolic variables (or one) to C++ strings. """
-    if not isinstance(s, list):
-        return cppunparse.pyexpr2cpp(symbolic.symstr(s))
-    return [cppunparse.pyexpr2cpp(symbolic.symstr(d)) for d in s]
-
-
-def cpp_offset_expr(d, subset_in, offset=None, packed_veclen=1):
-    """ Creates a C++ expression that can be added to a pointer in order
-        to offset it to the beginning of the given subset and offset.
-        @param d: The data structure to use for sizes/strides.
-        @param subset: The subset to offset by.
-        @param offset: An additional list of offsets or a Subset object
-        @param packed_veclen: If packed types are targeted, specifies the
-                              vector length that the final offset should be
-                              divided by.
-        @return: A string in C++ syntax with the correct offset
-    """
-    subset = copy.deepcopy(subset_in)
-
-    # Offset according to parameters
-    if offset is not None:
-        if isinstance(offset, subsets.Subset):
-            subset.offset(offset, False)
-        else:
-            subset.offset(subsets.Indices(offset), False)
-
-    # Then, offset according to array
-    subset.offset(subsets.Indices(d.offset), False)
-
-    # Obtain start range from offsetted subset
-    slice = [0] * len(d.strides)  # subset.min_element()
-
-    index = subset.at(slice, d.strides)
-    if packed_veclen > 1:
-        index /= packed_veclen
-
-    return sym2cpp(index)
-
-
-def cpp_array_expr(sdfg,
-                   memlet,
-                   with_brackets=True,
-                   offset=None,
-                   relative_offset=True,
-                   packed_veclen=1):
-    """ Converts an Indices/Range object to a C++ array access string. """
-    s = memlet.subset if relative_offset else subsets.Indices(offset)
-    o = offset if relative_offset else None
-    offset_cppstr = cpp_offset_expr(sdfg.arrays[memlet.data], s, o,
-                                    packed_veclen)
-
-    if with_brackets:
-        return "%s[%s]" % (memlet.data, offset_cppstr)
-    else:
-        return offset_cppstr
-
-
-############# END OF COPY FROM cpu.py #############
-
-
 class PAPISettings(object):
     @staticmethod
     def get_config(*key_hierarchy, config=None):
         if config is None:
             return Config.get(*key_hierarchy)
         else:
             return config.get(*key_hierarchy)
@@ -756,16 +695,16 @@
         # Inner part
         result = inner_stream
 
         # Instrumenting this is a bit flaky: Since the consume interally creates threads, it must be instrumented like a normal map. However, it seems to spawn normal std::threads (instead of going for openMP)
         # This implementation only allows to measure on a per-task basis (instead of per-thread). This is much more overhead.
         if PAPIInstrumentation.instrument_entry(node, state):
             result.write(
-                ("auto __perf_tlp_{id}_releaser = __perf_tlp_{id}.enqueue();\n".
-                 format(id=unified_id)) +
+                ("auto __perf_tlp_{id}_releaser = __perf_tlp_{id}.enqueue();\n"
+                 .format(id=unified_id)) +
                 PAPIInstrumentation.perf_counter_start_measurement_string(
                     node,
                     unified_id,
                     "__perf_tlp_{id}.getAndIncreaseCounter()".format(
                         id=unified_id),
                     core_str="dace_perf::getThreadID()",
                 ),
@@ -1033,15 +972,15 @@
 
         def get(self, name: str):
             try:
                 return self.values[name]
             except:
                 return None
 
-        def toJSON(self):
+        def to_json(self):
             return '{{ "node": "{node}",\n"thread": "{thread}",\n"iteration": "{iteration}",\n"flags": {flags},\n"values": [{values}]\n}}\n'.format(
                 node=str(self.nodeid),
                 thread=str(self.coreid),
                 iteration=str(self.iteration),
                 flags=str(self.flags),
                 values=", ".join([
                     '{{ "{code}": {value} }}'.format(
@@ -1187,21 +1126,21 @@
             for x in self.entries:
                 ret += delim.join([
                     prepend, "node" + str(self.nodeid), self.threadid,
                     x.toCSVsubstring(delim)
                 ]) + linedelim
             return ret
 
-        def toJSON(self):
+        def to_json(self):
             return '{{ "entry_node": {entry_node}, "static_movement": {datasize}, "input_size": {input_size}, "entry_core": {core}, "entries": ['.format(
                 entry_node=self.nodeid,
                 datasize=self.datasize,
                 input_size=self.input_datasize,
                 core=self.threadid) + ", ".join(
-                    [x.toJSON() for x in self.entries]) + "]}"
+                    [x.to_json() for x in self.entries]) + "]}"
 
         def toSQL(self, conn: sqlite3.Connection, c: sqlite3.Cursor,
                   supersection_id, order):
             # section_id must be set by the calling section and represent its
             # DB key, order is an integer that must be monotonically increasing
             c.execute(
                 '''INSERT INTO `Sections`
@@ -1305,18 +1244,18 @@
             for x in self.sections.values():
                 for y in x:
                     ret += y.toCSVsubstring("supernode" + str(self.supernode),
                                             delim, linedelim)
             ret += "ENDSUPERSECTION" + linedelim
             return ret
 
-        def toJSON(self):
+        def to_json(self):
             return '{{ "hint": "supersection", "supernode": {supernode},\n "sections": [{sections}] }}'.format(
                 supernode=self.supernode,
-                sections=",\n".join([x.toJSON() for x in self.getSections()]))
+                sections=",\n".join([x.to_json() for x in self.getSections()]))
 
         def toSQL(self, conn: sqlite3.Connection, c: sqlite3.Cursor, run_id,
                   order):
             """ Create a supersection entry for a given run_id """
             c.execute(
                 '''
             INSERT INTO `SuperSections`
@@ -1474,15 +1413,15 @@
 
             target.was_collapsed = True  # If selection is []
 
             assert target.was_collapsed
 
         # Debug
         removed_nodes = [x for x in sections if not (x in collapsed)]
-        print("Removed nodes: " + str([x.toJSON() for x in removed_nodes]))
+        print("Removed nodes: " + str([x.to_json() for x in removed_nodes]))
         print(
             "Reduced from %d sections to %d" % (len(sections), len(collapsed)))
         return collapsed
 
 
 class PAPIUtils(object):
     _unique_counter = 0
@@ -2845,15 +2784,16 @@
             conn.close()
         # endif PAPISettings.perf_use_sql()
 
         try:
             totstr = '{ "type": "PerfInfo", "payload": [' + ", ".join(
                 [
                     '{"runopts": "%s", "data": [%s]}' % (o, ", ".join(
-                        [x.toJSON() for x in r_supersections if x.is_valid()]))
+                        [x.to_json() for x in r_supersections
+                         if x.is_valid()]))
                     for o, r_supersections in multirun_supersections
                 ]
             ) + '], "overhead_percentage": %s, "mode": "%s", "default_depth": %d %s}' % (
                 str(percent_diff), modestr,
                 PAPISettings.perf_max_scope_depth(), overhead_number_string)
 
             if False:  # Disable debug json and csv by default
@@ -2871,15 +2811,15 @@
             import traceback
             print("[Error] Failed to jsonify")
             print(traceback.format_exc())
 
         # Check if this runs
         try:
             for s in sections:
-                json.loads(s.toJSON())
+                json.loads(s.to_json())
         except:
             print("[Error] JSON contains syntax errors!")
 
         PAPISettings.transcriptor_print(
             "\t===>Print instrumentation output end")
 
         if print_values:
```

### Comparing `dace-0.9.0/dace/codegen/instrumentation/perfdb.py` & `dace-0.9.5/dace/codegen/instrumentation/perfdb.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/codegen/instrumentation/provider.py` & `dace-0.9.5/dace/codegen/instrumentation/provider.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,132 +8,132 @@
             raise ValueError("Nodeid is too large to fit in 16 bits!")
         if state_id > 0x0FFFF:
             raise ValueError("Stateid is too large to fit in 16 bits!")
         return (int(state_id) << 16) | int(node_id)
 
     def report(self, local_stream, global_stream):
         """ Emits an instrumentation report code.
-            @param local_stream: Code generator for the in-function code.
-            @param global_stream: Code generator for global (external) code.
+            :param local_stream: Code generator for the in-function code.
+            :param global_stream: Code generator for global (external) code.
         """
         pass
 
     def on_sdfg_begin(self, sdfg, local_stream, global_stream):
         """ Event called at the beginning of SDFG code generation.
-            @param sdfg: The generated SDFG object.
-            @param local_stream: Code generator for the in-function code.
-            @param global_stream: Code generator for global (external) code.
+            :param sdfg: The generated SDFG object.
+            :param local_stream: Code generator for the in-function code.
+            :param global_stream: Code generator for global (external) code.
         """
         pass
 
     def on_sdfg_end(self, sdfg, local_stream, global_stream):
         """ Event called at the end of SDFG code generation.
-            @param sdfg: The generated SDFG object.
-            @param local_stream: Code generator for the in-function code.
-            @param global_stream: Code generator for global (external) code.
+            :param sdfg: The generated SDFG object.
+            :param local_stream: Code generator for the in-function code.
+            :param global_stream: Code generator for global (external) code.
         """
         pass
 
     def on_state_begin(self, sdfg, state, local_stream, global_stream):
         """ Event called at the beginning of SDFG state code generation.
-            @param sdfg: The generated SDFG object.
-            @param state: The generated SDFGState object.
-            @param local_stream: Code generator for the in-function code.
-            @param global_stream: Code generator for global (external) code.
+            :param sdfg: The generated SDFG object.
+            :param state: The generated SDFGState object.
+            :param local_stream: Code generator for the in-function code.
+            :param global_stream: Code generator for global (external) code.
         """
         pass
 
     def on_state_end(self, sdfg, state, local_stream, global_stream):
         """ Event called at the end of SDFG state code generation.
-            @param sdfg: The generated SDFG object.
-            @param state: The generated SDFGState object.
-            @param local_stream: Code generator for the in-function code.
-            @param global_stream: Code generator for global (external) code.
+            :param sdfg: The generated SDFG object.
+            :param state: The generated SDFGState object.
+            :param local_stream: Code generator for the in-function code.
+            :param global_stream: Code generator for global (external) code.
         """
         pass
 
     def on_scope_entry(self, sdfg, state, node, outer_stream, inner_stream,
                        global_stream):
         """ Event called at the beginning of a scope (on generating an
             EntryNode).
-            @param sdfg: The generated SDFG object.
-            @param state: The generated SDFGState object.
-            @param node: The EntryNode object from which code is generated.
-            @param outer_stream: Code generator for the internal code before
+            :param sdfg: The generated SDFG object.
+            :param state: The generated SDFGState object.
+            :param node: The EntryNode object from which code is generated.
+            :param outer_stream: Code generator for the internal code before
                                  the scope is opened.
-            @param inner_stream: Code generator for the internal code within
+            :param inner_stream: Code generator for the internal code within
                                  the scope (at the beginning).
-            @param global_stream: Code generator for global (external) code.
+            :param global_stream: Code generator for global (external) code.
         """
         pass
 
     def on_scope_exit(self, sdfg, state, node, outer_stream, inner_stream,
                       global_stream):
         """ Event called at the end of a scope (on generating an ExitNode).
-            @param sdfg: The generated SDFG object.
-            @param state: The generated SDFGState object.
-            @param node: The ExitNode object from which code is generated.
-            @param outer_stream: Code generator for the internal code after
+            :param sdfg: The generated SDFG object.
+            :param state: The generated SDFGState object.
+            :param node: The ExitNode object from which code is generated.
+            :param outer_stream: Code generator for the internal code after
                                  the scope is closed.
-            @param inner_stream: Code generator for the internal code within
+            :param inner_stream: Code generator for the internal code within
                                  the scope (at the end).
-            @param global_stream: Code generator for global (external) code.
+            :param global_stream: Code generator for global (external) code.
         """
         pass
 
     def on_copy_begin(self, sdfg, state, src_node, dst_node, edge,
                       local_stream, global_stream, copy_shape, src_strides,
                       dst_strides):
         """ Event called at the beginning of generating a copy operation.
-            @param sdfg: The generated SDFG object.
-            @param state: The generated SDFGState object.
-            @param src_node: The source node of the copy.
-            @param dst_node: The destination node of the copy.
-            @param edge: An edge in the memlet path of the copy.
-            @param local_stream: Code generator for the internal code.
-            @param global_stream: Code generator for global (external) code.
-            @param copy_shape: Tuple representing the shape of the copy.
-            @param src_strides: Element-skipping strides for each dimension of the copied source.
-            @param dst_strides: Element-skipping strides for each dimension of the copied destination.
+            :param sdfg: The generated SDFG object.
+            :param state: The generated SDFGState object.
+            :param src_node: The source node of the copy.
+            :param dst_node: The destination node of the copy.
+            :param edge: An edge in the memlet path of the copy.
+            :param local_stream: Code generator for the internal code.
+            :param global_stream: Code generator for global (external) code.
+            :param copy_shape: Tuple representing the shape of the copy.
+            :param src_strides: Element-skipping strides for each dimension of the copied source.
+            :param dst_strides: Element-skipping strides for each dimension of the copied destination.
         """
         pass
 
     def on_copy_end(self, sdfg, state, src_node, dst_node, edge, local_stream,
                     global_stream):
         """ Event called at the end of generating a copy operation.
-            @param sdfg: The generated SDFG object.
-            @param state: The generated SDFGState object.
-            @param src_node: The source node of the copy.
-            @param dst_node: The destination node of the copy.
-            @param edge: An edge in the memlet path of the copy.
-            @param local_stream: Code generator for the internal code.
-            @param global_stream: Code generator for global (external) code.
+            :param sdfg: The generated SDFG object.
+            :param state: The generated SDFGState object.
+            :param src_node: The source node of the copy.
+            :param dst_node: The destination node of the copy.
+            :param edge: An edge in the memlet path of the copy.
+            :param local_stream: Code generator for the internal code.
+            :param global_stream: Code generator for global (external) code.
         """
         pass
 
     def on_node_begin(self, sdfg, state, node, outer_stream, inner_stream,
                       global_stream):
         """ Event called at the beginning of generating a node.
-            @param sdfg: The generated SDFG object.
-            @param state: The generated SDFGState object.
-            @param node: The generated node.
-            @param outer_stream: Code generator for the internal code before
+            :param sdfg: The generated SDFG object.
+            :param state: The generated SDFGState object.
+            :param node: The generated node.
+            :param outer_stream: Code generator for the internal code before
                                  the scope is opened.
-            @param inner_stream: Code generator for the internal code within
+            :param inner_stream: Code generator for the internal code within
                                  the scope (at the beginning).
-            @param global_stream: Code generator for global (external) code.
+            :param global_stream: Code generator for global (external) code.
         """
         pass
 
     def on_node_end(self, sdfg, state, node, outer_stream, inner_stream,
                     global_stream):
         """ Event called at the end of generating a node.
-            @param sdfg: The generated SDFG object.
-            @param state: The generated SDFGState object.
-            @param node: The generated node.
-            @param outer_stream: Code generator for the internal code after
+            :param sdfg: The generated SDFG object.
+            :param state: The generated SDFGState object.
+            :param node: The generated node.
+            :param outer_stream: Code generator for the internal code after
                                  the scope is closed.
-            @param inner_stream: Code generator for the internal code within
+            :param inner_stream: Code generator for the internal code within
                                  the scope (at the end).
-            @param global_stream: Code generator for global (external) code.
+            :param global_stream: Code generator for global (external) code.
         """
         pass
```

### Comparing `dace-0.9.0/dace/codegen/instrumentation/timer.py` & `dace-0.9.5/dace/codegen/instrumentation/timer.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/codegen/prettycode.py` & `dace-0.9.5/dace/codegen/prettycode.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,16 +53,19 @@
 
             codeline = self._indent * self._spaces * ' ' + line.strip()
 
             # Location identifier is written at character 81 and on, find out
             # how many spaces we need to add for that
             loc_spaces = max(80 - len(codeline), 2)
 
-            super(CodeIOStream, self).write(codeline + loc_spaces * ' ' +
-                                            location_identifier + '\n')
+            if location_identifier != '':
+                super(CodeIOStream, self).write(codeline + loc_spaces * ' ' +
+                                                location_identifier + '\n')
+            else:  # avoid ending spaces (useful for OpenCL and multiline macros)
+                super(CodeIOStream, self).write(codeline + '\n')
             if brace_balance > 0:
                 self._indent += brace_balance
 
             # If indentation failed, warn user
             if self._indent < -1:
                 super(CodeIOStream, self).write(
                     '///WARNING: Indentation failure! This probably ' +
```

### Comparing `dace-0.9.0/dace/codegen/targets/cpu.py` & `dace-0.9.5/dace/codegen/targets/cpu.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 from dace.codegen import cppunparse
 
 import dace
 from dace.config import Config
 from dace.frontend import operations
 from dace import data, subsets, symbolic, dtypes, memlet as mmlt
+from dace.codegen.targets.common import (sym2cpp, find_incoming_edges,
+                                         find_outgoing_edges)
 from dace.codegen.prettycode import CodeIOStream
 from dace.codegen.targets.target import TargetCodeGenerator, make_absolute, DefinedType
 from dace.graph import nodes, nxutil
 from dace.sdfg import (ScopeSubgraphView, SDFG, scope_contains_scope,
                        find_input_arraynode, find_output_arraynode,
                        is_devicelevel, is_array_stream_view)
 
@@ -47,14 +49,17 @@
         dispatcher = self._dispatcher
 
         self._locals = cppunparse.CPPLocals()
         # Scope depth (for use of the 'auto' keyword when
         # defining locals)
         self._ldepth = 0
 
+        # Keep nested SDFG schedule when descending into it
+        self._toplevel_schedule = None
+
         # FIXME: this allows other code generators to change the CPU
         # behavior to assume that arrays point to packed types, thus dividing
         # all addresess by the vector length.
         self._packed_types = False
 
         # Keep track of traversed nodes
         self._generated_nodes = set()
@@ -165,15 +170,15 @@
         try:
             self._dispatcher.defined_vars.get(name)
             return  # Array was already allocated in this or upper scopes
         except KeyError:  # Array not allocated yet
             pass
 
         # Compute array size
-        arrsize = " * ".join([sym2cpp(s) for s in nodedesc.strides])
+        arrsize = nodedesc.total_size
 
         if isinstance(nodedesc, data.Scalar):
             callsite_stream.write("%s %s;\n" % (nodedesc.dtype.ctype, name),
                                   sdfg, state_id, node)
             self._dispatcher.defined_vars.add(name, DefinedType.Scalar)
         elif isinstance(nodedesc, data.Stream):
             ###################################################################
@@ -237,39 +242,41 @@
             self._dispatcher.defined_vars.add(name, DefinedType.Stream)
 
         elif (nodedesc.storage == dtypes.StorageType.CPU_Heap
               or nodedesc.storage == dtypes.StorageType.Immaterial
               ):  # TODO: immaterial arrays should not allocate memory
             callsite_stream.write(
                 "%s *%s = new %s DACE_ALIGN(64)[%s];\n" %
-                (nodedesc.dtype.ctype, name, nodedesc.dtype.ctype, arrsize),
+                (nodedesc.dtype.ctype, name, nodedesc.dtype.ctype,
+                 sym2cpp(arrsize)),
                 sdfg,
                 state_id,
                 node,
             )
             self._dispatcher.defined_vars.add(name, DefinedType.Pointer)
             if node.setzero:
-                callsite_stream.write("memset(%s, 0, sizeof(%s)*%s);" %
-                                      (name, nodedesc.dtype.ctype, arrsize))
+                callsite_stream.write(
+                    "memset(%s, 0, sizeof(%s)*%s);" %
+                    (name, nodedesc.dtype.ctype, sym2cpp(arrsize)))
             return
         elif (nodedesc.storage == dtypes.StorageType.CPU_Stack
               or nodedesc.storage == dtypes.StorageType.Register):
             if node.setzero:
                 callsite_stream.write(
                     "%s %s[%s]  DACE_ALIGN(64) = {0};\n" %
-                    (nodedesc.dtype.ctype, name, arrsize),
+                    (nodedesc.dtype.ctype, name, sym2cpp(arrsize)),
                     sdfg,
                     state_id,
                     node,
                 )
                 self._dispatcher.defined_vars.add(name, DefinedType.Pointer)
                 return
             callsite_stream.write(
                 "%s %s[%s]  DACE_ALIGN(64);\n" % (nodedesc.dtype.ctype, name,
-                                                  arrsize),
+                                                  sym2cpp(arrsize)),
                 sdfg,
                 state_id,
                 node,
             )
             self._dispatcher.defined_vars.add(name, DefinedType.Pointer)
             return
         else:
@@ -479,14 +486,17 @@
                     # Stream -> Array - pop bulk
                     if is_array_stream_view(sdfg, dfg, src_node):
                         return  # Do nothing (handled by ArrayStreamView)
 
                     array_subset = (memlet.subset
                                     if memlet.data == dst_node.data else
                                     memlet.other_subset)
+                    if array_subset is None:  # Need to use entire array
+                        array_subset = subsets.Range.from_array(dst_nodedesc)
+
                     # stream_subset = (memlet.subset
                     #                  if memlet.data == src_node.data else
                     #                  memlet.other_subset)
                     stream_subset = memlet.subset
                     if memlet.data != src_node.data and memlet.other_subset:
                         stream_subset = memlet.other_subset
 
@@ -605,15 +615,16 @@
                 if instr is not None:
                     instr.on_copy_begin(sdfg, state_dfg, src_node, dst_node,
                                         edge, stream, None, copy_shape,
                                         src_strides, dst_strides)
 
             nc = True
             if memlet.wcr is not None:
-                nc = not is_write_conflicted(dfg, edge)
+                nc = not is_write_conflicted(
+                    dfg, edge, sdfg_schedule=self._toplevel_schedule)
             if nc:
                 stream.write(
                     """
                     dace::CopyND{copy_tmpl}::{shape_tmpl}::{copy_func}(
                         {copy_args});""".format(
                         copy_tmpl=copy_tmpl,
                         shape_tmpl=shape_tmpl,
@@ -649,30 +660,31 @@
                 instr.on_copy_end(sdfg, state_dfg, src_node, dst_node, edge,
                                   stream, None)
         #############################################################
 
     ###########################################################################
     # Memlet handling
 
-    def process_out_memlets(
-            self,
-            sdfg,
-            state_id,
-            node,
-            dfg,
-            dispatcher,
-            result,
-            locals_defined,
-            function_stream,
-    ):
+    def process_out_memlets(self,
+                            sdfg,
+                            state_id,
+                            node,
+                            dfg,
+                            dispatcher,
+                            result,
+                            locals_defined,
+                            function_stream,
+                            skip_wcr=False):
 
         scope_dict = sdfg.nodes()[state_id].scope_dict()
 
         for edge in dfg.out_edges(node):
             _, uconn, v, _, memlet = edge
+            if skip_wcr and memlet.wcr is not None:
+                continue
             dst_node = dfg.memlet_path(edge)[-1].dst
 
             # Target is neither a data nor a tasklet node
             if isinstance(node, nodes.AccessNode) and (
                     not isinstance(dst_node, nodes.AccessNode)
                     and not isinstance(dst_node, nodes.CodeNode)):
                 continue
@@ -707,16 +719,16 @@
             if node == dst_node:
                 continue
 
             # Tasklet -> array
             if isinstance(node, nodes.CodeNode):
                 if not uconn:
                     raise SyntaxError(
-                        "Cannot copy memlet without a local connector: {} to {}".
-                        format(str(edge.src), str(edge.dst)))
+                        "Cannot copy memlet without a local connector: {} to {}"
+                        .format(str(edge.src), str(edge.dst)))
 
                 try:
                     positive_accesses = bool(memlet.num_accesses >= 0)
                 except TypeError:
                     positive_accesses = False
 
                 if memlet.subset.data_dims() == 0 and positive_accesses:
@@ -730,15 +742,16 @@
                         assert len(in_memlets) == 1
                         in_local_name = self.memlet_ctor(
                             sdfg, in_memlets[0], False)
 
                     state_dfg = sdfg.nodes()[state_id]
 
                     if memlet.wcr is not None:
-                        nc = not is_write_conflicted(dfg, edge)
+                        nc = not is_write_conflicted(
+                            dfg, edge, sdfg_schedule=self._toplevel_schedule)
                         result.write(
                             write_and_resolve_expr(
                                 sdfg, memlet, nc, out_local_name,
                                 in_local_name), sdfg, state_id, node)
                     else:
                         result.write(
                             "%s.write(%s);\n" % (out_local_name,
@@ -766,15 +779,15 @@
         memlet_params = []
 
         memlet_name = memlet.data
         def_type = self._dispatcher.defined_vars.get(memlet_name)
 
         if def_type == DefinedType.Pointer:
             memlet_expr = memlet_name  # Common case
-        elif def_type == DefinedType.Scalar or def_type == DefinedType.ScalarView:
+        elif def_type == DefinedType.Scalar:
             memlet_expr = "&" + memlet_name
         elif def_type == DefinedType.ArrayView:
             memlet_expr = memlet_name + ".ptr()"
         else:
             raise TypeError("Unsupported connector type {}".format(def_type))
 
         if isinstance(memlet.subset, subsets.Indices):
@@ -904,35 +917,31 @@
                     # The value will be written during the tasklet, and will be
                     # automatically written out after
                     result += "{} {};".format(memlet_type, local_name)
                 self._dispatcher.defined_vars.add(
                     local_name,
                     DefinedType.Scalar,
                     allow_shadowing=allow_shadowing)
-            elif memlet.num_accesses == -1:
+            else:
                 if output:
                     # Variable number of writes: get reference to the target of
                     # the view to reflect writes at the data
                     result += "auto &{} = __{}.ref<{}>();".format(
                         local_name, local_name, memlet.veclen)
                 else:
                     # Variable number of reads: get a const reference that can
                     # be read if necessary
                     result += "auto const &{} = __{}.ref<{}>();".format(
                         local_name, local_name, memlet.veclen)
                 self._dispatcher.defined_vars.add(
                     local_name,
                     DefinedType.Scalar,
                     allow_shadowing=allow_shadowing)
-            else:
-                raise dace.codegen.codegen.CodegenError(
-                    "Unsupported number of accesses {} for scalar {}".format(
-                        memlet.num_accesses, local_name))
         elif var_type == DefinedType.Pointer:
-            if memlet.num_accesses == 1:
+            if memlet.num_accesses == 1 and memlet.subset.num_elements() == 1:
                 if output:
                     result += "{} {};".format(memlet_type, local_name)
                 else:
                     result += "{} {} = __{}.val<{}>();".format(
                         memlet_type, local_name, local_name, memlet.veclen)
                 self._dispatcher.defined_vars.add(
                     local_name,
@@ -950,15 +959,18 @@
                 else:
                     result += "auto *{} = __{}.ptr<{}>();".format(
                         local_name, local_name, memlet.veclen)
                     self._dispatcher.defined_vars.add(
                         local_name,
                         DefinedType.Pointer,
                         allow_shadowing=allow_shadowing)
-        elif var_type == DefinedType.Stream or var_type == DefinedType.StreamArray:
+        elif var_type in [
+                DefinedType.Stream, DefinedType.StreamArray,
+                DefinedType.StreamView
+        ]:
             if memlet.num_accesses == 1:
                 if output:
                     result += "{} {};".format(memlet_type, local_name)
                 else:
                     result += "auto {} = __{}.pop();".format(
                         local_name, local_name)
                 self._dispatcher.defined_vars.add(
@@ -966,40 +978,48 @@
                     DefinedType.Scalar,
                     allow_shadowing=allow_shadowing)
             else:
                 # Just forward actions to the underlying object
                 result += "auto &{} = __{};".format(local_name, local_name)
                 self._dispatcher.defined_vars.add(
                     local_name,
-                    DefinedType.Stream,
+                    DefinedType.StreamView,
                     allow_shadowing=allow_shadowing)
         else:
             raise TypeError("Unknown variable type: {}".format(var_type))
 
         return result
 
     def memlet_stream_ctor(self, sdfg, memlet):
+        def_type = self._dispatcher.defined_vars.get(memlet.data)
+
         stream = sdfg.arrays[memlet.data]
-        dtype = "dace::vec<{}, {}>".format(stream.dtype.ctype,
-                                           symbolic.symstr(memlet.veclen))
-        return "dace::make_streamview({})".format(memlet.data + (
-            "[{}]".format(cpp_offset_expr(stream, memlet.subset))
-            if isinstance(stream, dace.data.Stream)
-            and stream.is_stream_array() else ""))
+        expr = memlet.data + ("[{}]".format(
+            cpp_offset_expr(stream, memlet.subset))
+                              if isinstance(stream, dace.data.Stream)
+                              and stream.is_stream_array() else "")
+
+        if def_type == DefinedType.StreamView:
+            return expr
+
+        return "dace::make_streamview({})".format(expr)
 
     def memlet_ctor(self, sdfg, memlet, is_output):
 
         def_type = self._dispatcher.defined_vars.get(memlet.data)
 
-        if def_type == DefinedType.Stream or def_type == DefinedType.StreamArray:
+        if def_type in [
+                DefinedType.Stream, DefinedType.StreamArray,
+                DefinedType.StreamView
+        ]:
             return self.memlet_stream_ctor(sdfg, memlet)
 
-        elif (def_type == DefinedType.Pointer or def_type == DefinedType.Scalar
-              or def_type == DefinedType.ScalarView
-              or def_type == DefinedType.ArrayView):
+        elif def_type in [
+                DefinedType.Pointer, DefinedType.Scalar, DefinedType.ArrayView
+        ]:
             return self.memlet_view_ctor(sdfg, memlet, is_output)
 
         else:
             raise NotImplementedError(
                 "Connector type {} not yet implemented".format(def_type))
 
     def copy_expr(
@@ -1051,24 +1071,24 @@
         elif def_type == DefinedType.ArrayView:
             return "{}{}.ptr(){}".format(
                 dt, expr, " + {}".format(offset_cppstr) if add_offset else "")
 
         elif def_type == DefinedType.StreamArray:
             return "{}[{}]".format(expr, offset_cppstr)
 
-        elif (def_type == DefinedType.Scalar
-              or def_type == DefinedType.ScalarView
-              or def_type == DefinedType.Stream):
+        elif def_type in [
+                DefinedType.Scalar, DefinedType.Stream, DefinedType.StreamView
+        ]:
 
             if add_offset:
                 raise TypeError(
                     "Tried to offset address of scalar {}: {}".format(
                         dataname, offset_cppstr))
 
-            if def_type == DefinedType.Scalar or def_type == DefinedType.ScalarView:
+            if def_type == DefinedType.Scalar:
                 return "{}&{}".format(dt, expr)
             else:
                 return dataname
 
         else:
             raise NotImplementedError(
                 "copy_expr not implemented "
@@ -1138,17 +1158,17 @@
 
         src_strides = src_subset.absolute_strides(src_nodedesc.strides)
         dst_strides = dst_subset.absolute_strides(dst_nodedesc.strides)
 
         # Try to turn into degenerate/strided ND copies
         result = ndcopy_to_strided_copy(
             copy_shape,
-            src_nodedesc.strides,
+            src_nodedesc.shape,
             src_strides,
-            dst_nodedesc.strides,
+            dst_nodedesc.shape,
             dst_strides,
             memlet.subset,
             src_subset,
             dst_subset,
         )
         if result is not None:
             copy_shape, src_strides, dst_strides = result
@@ -1350,24 +1370,17 @@
         instr = self._dispatcher.instrumentation[node.instrument]
         if instr is not None:
             instr.on_node_begin(sdfg, state_dfg, node, outer_stream_begin,
                                 inner_stream, function_stream)
 
         inner_stream.write("\n    ///////////////////\n", sdfg, state_id, node)
 
-        unparse_tasklet(
-            sdfg,
-            state_id,
-            dfg,
-            node,
-            function_stream,
-            inner_stream,
-            self._locals,
-            self._ldepth,
-        )
+        unparse_tasklet(sdfg, state_id, dfg, node, function_stream,
+                        inner_stream, self._locals, self._ldepth,
+                        self._toplevel_schedule)
 
         inner_stream.write("    ///////////////////\n\n", sdfg, state_id, node)
 
         # Process outgoing memlets
         self.process_out_memlets(
             sdfg,
             state_id,
@@ -1395,78 +1408,118 @@
         self._dispatcher.defined_vars.exit_scope(node)
 
     def _generate_EmptyTasklet(self, sdfg, dfg, state_id, node,
                                function_stream, callsite_stream):
         self._generate_Tasklet(sdfg, dfg, state_id, node, function_stream,
                                callsite_stream)
 
+    def _emit_memlet_reference(self, sdfg: SDFG, memlet: mmlt.Memlet,
+                               pointer_name: str):
+        """ Returns a string with a definition of a reference to an existing
+            memlet. Used in nested SDFG arguments. """
+        desc = sdfg.arrays[memlet.data]
+        typedef = 'auto'  # TODO(later): Use non-auto types (vec, Stream<>...)
+        datadef = memlet.data
+        offset_expr = '[' + cpp_offset_expr(desc, memlet.subset) + ']'
+
+        # Get defined type (pointer, stream etc.) and change the type definition
+        # accordingly.
+        defined_type = self._dispatcher.defined_vars.get(memlet.data)
+        if defined_type == DefinedType.Pointer:
+            typedef += '*'
+            datadef = '&' + datadef
+        elif defined_type == DefinedType.Scalar:
+            typedef += '&'
+            offset_expr = ''
+        elif defined_type == DefinedType.Stream:
+            typedef += '&'
+            offset_expr = ''
+        else:
+            typedef += '&'
+            defined_type = DefinedType.Pointer
+
+        # Register defined variable
+        self._dispatcher.defined_vars.add(
+            pointer_name, defined_type, allow_shadowing=True)
+
+        return '%s %s = %s%s;' % (typedef, pointer_name, datadef, offset_expr)
+
     def _generate_NestedSDFG(
             self,
             sdfg,
             dfg: ScopeSubgraphView,
             state_id,
             node,
             function_stream: CodeIOStream,
             callsite_stream: CodeIOStream,
     ):
-
         self._dispatcher.defined_vars.enter_scope(sdfg)
 
         # If SDFG parent is not set, set it
         state_dfg = sdfg.nodes()[state_id]
         node.sdfg.parent = state_dfg
         node.sdfg._parent_sdfg = sdfg
 
         # Connectors that are both input and output share the same name
         inout = set(node.in_connectors & node.out_connectors)
 
+        # TODO: Emit nested SDFG as a separate function
+
+        # Emit accessors as pointers/references (rather than new objects)
         # Take care of nested SDFG I/O
         for _, _, _, vconn, in_memlet in state_dfg.in_edges(node):
             if vconn in inout or in_memlet.data is None:
                 continue
-            # TODO: Instead of allowing shadowing, emit nested SDFG as a
-            #       separate function
             callsite_stream.write(
                 self.memlet_definition(
                     sdfg, in_memlet, False, vconn, allow_shadowing=True), sdfg,
                 state_id, node)
         for _, uconn, _, _, out_memlet in state_dfg.out_edges(node):
             if out_memlet.data is not None:
-                callsite_stream.write(
-                    self.memlet_definition(
-                        sdfg, out_memlet, True, uconn, allow_shadowing=True),
-                    sdfg, state_id, node)
+                if out_memlet.wcr is not None:
+                    out_code = self._emit_memlet_reference(
+                        sdfg, out_memlet, uconn)
+                else:
+                    out_code = self.memlet_definition(
+                        sdfg, out_memlet, True, uconn, allow_shadowing=True)
+
+                callsite_stream.write(out_code, sdfg, state_id, node)
 
         callsite_stream.write("\n    ///////////////////\n", sdfg, state_id,
                               node)
 
+        old_schedule = self._toplevel_schedule
+        self._toplevel_schedule = node.schedule
+
         sdfg_label = "_%d_%d" % (state_id, dfg.node_id(node))
         # Generate code for internal SDFG
         global_code, local_code, used_targets = self._frame.generate_code(
             node.sdfg, node.schedule, sdfg_label)
 
         # Write generated code in the proper places (nested SDFG writes
         # location info)
         function_stream.write(global_code)
         callsite_stream.write(local_code)
 
+        self._toplevel_schedule = old_schedule
+
         callsite_stream.write("    ///////////////////\n\n", sdfg, state_id,
                               node)
 
         # Process outgoing memlets with the internal SDFG
         self.process_out_memlets(
             sdfg,
             state_id,
             node,
             state_dfg,
             self._dispatcher,
             callsite_stream,
             True,
             function_stream,
-        )
+            skip_wcr=True)
 
         self._dispatcher.defined_vars.exit_scope(sdfg)
 
     def _generate_MapEntry(
             self,
             sdfg,
             dfg,
@@ -1478,14 +1531,24 @@
         state_dfg = sdfg.node(state_id)
         map_params = node.map.params
         map_name = "__DACEMAP_" + str(state_id) + "_" + str(dfg.node_id(node))
 
         result = callsite_stream
         map_header = ""
 
+        # Encapsulate map with a C scope
+        # TODO: Refactor out of MapEntry generation (generate_scope_header?)
+        callsite_stream.write('{', sdfg, state_id, node)
+
+        # Define all input connectors of this map entry
+        for e in dace.sdfg.dynamic_map_inputs(state_dfg, node):
+            callsite_stream.write(
+                self.memlet_definition(sdfg, e.data, False, e.dst_conn), sdfg,
+                state_id, node)
+
         # Instrumentation: Pre-scope
         instr = self._dispatcher.instrumentation[node.map.instrument]
         if instr is not None:
             inner_stream = CodeIOStream()
             instr.on_scope_entry(sdfg, state_dfg, node, callsite_stream,
                                  inner_stream, function_stream)
 
@@ -1662,14 +1725,16 @@
         else:
             for i, r in enumerate(map_node.map.range):
                 result.write("}", sdfg, state_id, node)
 
         if outer_stream is not None:
             result.write(outer_stream.getvalue())
 
+        callsite_stream.write('}', sdfg, state_id, node)
+
     def _generate_ConsumeEntry(
             self,
             sdfg,
             dfg,
             state_id,
             node: nodes.MapEntry,
             function_stream,
@@ -1740,29 +1805,29 @@
             node,
         )
 
         # Since consume is an alias node, we create an actual array for the
         # consumed element and modify the outgoing memlet path ("OUT_stream")
         # TODO: do this before getting to the codegen
         if node.consume.chunksize == 1:
-            consumed_element = sdfg.add_scalar(
+            newname, _ = sdfg.add_scalar(
                 node.consume.label + "_element",
                 input_streamdesc.dtype,
                 transient=True,
-                storage=dtypes.StorageType.Register)
-            ce_node = nodes.AccessNode(node.consume.label + '_element',
-                                       dtypes.AccessType.ReadOnly)
+                storage=dtypes.StorageType.Register,
+                find_new_name=True)
+            ce_node = nodes.AccessNode(newname, dtypes.AccessType.ReadOnly)
         else:
-            consumed_element = sdfg.add_array(
+            newname, _ = sdfg.add_array(
                 node.consume.label + '_elements', [node.consume.chunksize],
                 input_streamdesc.dtype,
                 transient=True,
-                storage=dtypes.StorageType.Register)
-            ce_node = nodes.AccessNode(node.consume.label + '_elements',
-                                       dtypes.AccessType.ReadOnly)
+                storage=dtypes.StorageType.Register,
+                find_new_name=True)
+            ce_node = nodes.AccessNode(newname, dtypes.AccessType.ReadOnly)
         state_dfg.add_node(ce_node)
         out_memlet_path = state_dfg.memlet_path(output_sedge)
         state_dfg.remove_edge(out_memlet_path[0])
         state_dfg.add_edge(
             out_memlet_path[0].src,
             out_memlet_path[0].src_conn,
             ce_node,
@@ -1871,61 +1936,108 @@
         output_memlet = output_edge.data
 
         output_type = "dace::vec<%s, %s>" % (
             sdfg.arrays[output_memlet.data].dtype.ctype,
             output_memlet.veclen,
         )
 
+        # Example:
+        #
+        # inp = array(K, M, N)
+        # out = array(L, M, N)
+        # out[i] = reduce(lambda a, b: a + b, inp, axes=0)
+        #
+        # Pseudocode:
+        # for m in range(M):
+        #     for n in range(N):
+        #         for k in range(K):
+        #             out[i, m, n] += inp[k, m, n]
+
+        # The number of output dimensions is equal to the number of input
+        # dimensions, minus the number of dimensions being reduced (axes)
+        # Example:
+        # 3D array inp reduced to a 2D array
+        # NOTE: The number of output dimensions is less or equal to the number
+        # of dimensions of the output array, where the result is stored.
+        input_num_dims = input_memlet.subset.dims()
         # If axes were not defined, use all input dimensions
-        input_dims = input_memlet.subset.dims()
-        output_dims = output_memlet.subset.data_dims()
         if axes is None:
-            axes = tuple(range(input_dims))
+            axes = tuple(range(input_num_dims))
+        output_num_dims = input_num_dims - len(axes)
 
         # Obtain variable names per output and reduction axis
-        axis_vars = []
-        octr = 0
-        for d in range(input_dims):
+        axis_vars = []  # Iteration variables for the input dimensions
+        output_axis_vars = dict()  # Dict matching the dimensions of the input
+        # that are NOT being reduced with the
+        # equivalent dimensions of the output array.
+        output_dims = []  # The equivalent output array dimensions
+        # of the input dimensions NOT being reduced.
+        octr = 0  # First index for the dimensions NOT being reduced.
+        input_size = input_memlet.subset.size()
+        output_size = output_memlet.subset.size()
+        for d in range(input_num_dims):
             if d in axes:
+                # Dimension is being reduced.
                 axis_vars.append("__i%d" % d)
             else:
+                # Dimension is NOT being reduced.
                 axis_vars.append("__o%d" % octr)
+                ri = input_size[d]
+                # Iterate over the dimensions of the output memlet and find
+                # the one that is matching with the input memlet dimension.
+                for i, ro in enumerate(output_size):
+                    # This is needed in case where there are multiple NOT
+                    # reduced dimensions with the same size.
+                    if i in output_axis_vars.keys():
+                        continue
+                    if ri == ro:
+                        output_dims.append(i)
+                        output_axis_vars[i] = octr
+                        break
                 octr += 1
+        # Example:
+        # __i0 -> first dimension of inp (size K)
+        # __o0 -> second dimension of inp and out (size M)
+        # __o1 -> third dimensions of inp and out (size N)
 
         # Instrumentation: Post-scope
         instr = self._dispatcher.instrumentation[node.instrument]
         if instr is not None:
             inner_stream = CodeIOStream()
             instr.on_node_begin(sdfg, state_dfg, node, callsite_stream,
                                 inner_stream, function_stream)
 
         # Write OpenMP loop pragma if there are output dimensions
-        if output_dims > 0:
+        if output_num_dims > 0:
             callsite_stream.write(loop_header, sdfg, state_id, node)
 
         # Generate outer loops
         output_subset = output_memlet.subset
-        for axis in range(output_dims):
+        for axis in output_dims:
+            octr = output_axis_vars[axis]
             callsite_stream.write(
                 "for (int {var} = {begin}; {var} < {end}; {var} += {skip}) {{".
                 format(
-                    var="__o%d" % axis,
+                    var="__o%d" % octr,
                     begin=output_subset[axis][0],
                     end=output_subset[axis][1] + 1,
                     skip=output_subset[axis][2],
                 ),
                 sdfg,
                 state_id,
                 node,
             )
 
             end_braces += 1
+        # Example:
+        # for (int __o0 = 0; __o0 < M; __o0 += 1) {
+        #     for (int __o1 = 0; __o1 < N; __o1 += 1) {
 
         use_tmpout = False
-        if len(axes) == input_dims:
+        if len(axes) == input_num_dims:
             # Add OpenMP reduction clause if reducing all axes
             if (redtype != dtypes.ReductionType.Custom
                     and node.schedule == dtypes.ScheduleType.CPU_Multicore):
                 loop_header += " reduction(%s: __tmpout)" % (
                     _REDUCTION_TYPE_TO_OPENMP[redtype])
 
             # Output initialization
@@ -1939,19 +2051,23 @@
             end_braces += 1
             use_tmpout = True
 
         # Compute output expression
         outvar = ("__tmpout" if use_tmpout else cpp_array_expr(
             sdfg,
             output_memlet,
-            offset=["__o%d" % i for i in range(output_dims)],
+            offset=[("__o%d" % output_axis_vars[i])
+                    if i in output_axis_vars.keys() else r[0]
+                    for i, r in enumerate(output_subset)],
             relative_offset=False,
         ))
+        # Example (pseudocode):
+        # out[i, __o0, __o1]
 
-        if len(axes) != input_dims and node.identity is not None:
+        if len(axes) != input_num_dims and node.identity is not None:
             # Write code for identity value in multiple axes
             callsite_stream.write(
                 "%s = %s;" % (outvar, sym2cpp(node.identity)), sdfg, state_id,
                 node)
 
         # Instrumentation: internal part
         if instr is not None:
@@ -1969,14 +2085,16 @@
                     skip=input_subset[axis][2],
                 ),
                 sdfg,
                 state_id,
                 node,
             )
             end_braces += 1
+        # Example:
+        # for (int __i0 = 0; __i0 < K; __i0 += 1) {
 
         # Generate reduction code
         credtype = "dace::ReductionType::" + str(
             redtype)[str(redtype).find(".") + 1:]
 
         invar = cpp_array_expr(
             sdfg, input_memlet, offset=axis_vars, relative_offset=False)
@@ -2003,16 +2121,31 @@
                 if instr is not None:
                     outer_stream = CodeIOStream()
                     instr.on_node_end(sdfg, state_dfg, node, outer_stream,
                                       callsite_stream, function_stream)
 
             # Store back tmpout into the true output
             if i == end_braces - 1 and use_tmpout:
+                # TODO: This is a targeted fix that has to be generalized when
+                # refactoring code generation. The issue is related to an
+                # inconsistency on whether an output connector generates a tmp
+                # scalar variable to be used with __write or a pointer to the
+                # output array.
+                scalar_output = True
+                for r in output_subset:
+                    if r != 0 and r != (0, 0, 1):
+                        scalar_output = False
+                        break
+                arr = sdfg.arrays[output_memlet.data]
+                if scalar_output and sdfg.parent_sdfg and not arr.transient:
+                    out_var = output_memlet.data
+                else:
+                    out_var = cpp_array_expr(sdfg, output_memlet)
                 callsite_stream.write(
-                    "%s = __tmpout;" % cpp_array_expr(sdfg, output_memlet),
+                    "%s = __tmpout;" % out_var,
                     sdfg,
                     state_id,
                     node,
                 )
 
             callsite_stream.write("}", sdfg, state_id, node)
 
@@ -2115,36 +2248,48 @@
         src_subset,
         dst_subset,
 ):
     """ Detects situations where an N-dimensional copy can be degenerated into
         a (faster) 1D copy or 2D strided copy. Returns new copy
         dimensions and offsets to emulate the requested copy.
 
-        @return: a 3-tuple: copy_shape, src_strides, dst_strides
+        :return: a 3-tuple: copy_shape, src_strides, dst_strides
     """
     dims = len(copy_shape)
 
     # Cannot degenerate tiled copies
     if any(ts != 1 for ts in subset.tile_sizes):
         return None
 
     # If the copy is contiguous, the difference between the first and last
     # pointers should be the shape of the copy
-    first_src_index = src_subset.at([0] * src_subset.dims(), src_shape)
-    first_dst_index = dst_subset.at([0] * dst_subset.dims(), dst_shape)
+    first_src_index = src_subset.at([0] * src_subset.dims(), src_strides)
+    first_dst_index = dst_subset.at([0] * dst_subset.dims(), dst_strides)
     last_src_index = src_subset.at([d - 1 for d in src_subset.size()],
-                                   src_shape)
+                                   src_strides)
     last_dst_index = dst_subset.at([d - 1 for d in dst_subset.size()],
-                                   dst_shape)
+                                   dst_strides)
     copy_length = functools.reduce(lambda x, y: x * y, copy_shape)
     src_copylen = last_src_index - first_src_index + 1
     dst_copylen = last_dst_index - first_dst_index + 1
-    if (tuple(copy_shape) == tuple(src_shape)
-            and tuple(copy_shape) == tuple(dst_shape)) or (
-                src_copylen == copy_length and dst_copylen == copy_length):
+
+    # Make expressions symbolic and simplify
+    copy_length = symbolic.pystr_to_symbolic(copy_length).simplify()
+    src_copylen = symbolic.pystr_to_symbolic(src_copylen).simplify()
+    dst_copylen = symbolic.pystr_to_symbolic(dst_copylen).simplify()
+
+    # Detect 1D copies. The first condition is the general one, whereas the
+    # second one applies when the arrays are completely equivalent in strides
+    # and shapes to the copy. The second condition is there because sometimes
+    # the symbolic math engine fails to produce the same expressions for both
+    # arrays.
+    if ((src_copylen == copy_length and dst_copylen == copy_length)
+            or (tuple(src_shape) == tuple(copy_shape)
+                and tuple(dst_shape) == tuple(copy_shape)
+                and tuple(src_strides) == tuple(dst_strides))):
         # Emit 1D copy of the whole array
         copy_shape = [functools.reduce(lambda x, y: x * y, copy_shape)]
         return copy_shape, [1], [1]
     # 1D strided copy
     elif sum([0 if c == 1 else 1 for c in copy_shape]) == 1:
         # Find the copied dimension:
         # In copy shape
@@ -2177,40 +2322,40 @@
         return "0"
 
     for i, d in enumerate(slice):
         if isinstance(d, tuple):
             raise SyntaxError(
                 "CPU backend does not yet support ranges as inputs/outputs")
 
-        # TODO(later): Use access order
-
         result.write(sym2cpp(d))
 
         # If not last
         if i < len(slice) - 1:
+            # We use the shape as-is since this function is intended for
+            # constant arrays only
             strdims = [str(dim) for dim in dims[i + 1:]]
             result.write(
                 "*%s + " % "*".join(strdims))  # Multiply by leading dimensions
 
     return result.getvalue()
 
 
 def cpp_offset_expr(d: data.Data,
                     subset_in: subsets.Subset,
                     offset=None,
                     packed_veclen=1):
     """ Creates a C++ expression that can be added to a pointer in order
         to offset it to the beginning of the given subset and offset.
-        @param d: The data structure to use for sizes/strides.
-        @param subset: The subset to offset by.
-        @param offset: An additional list of offsets or a Subset object
-        @param packed_veclen: If packed types are targeted, specifies the
-                              vector length that the final offset should be 
+        :param d: The data structure to use for sizes/strides.
+        :param subset: The subset to offset by.
+        :param offset: An additional list of offsets or a Subset object
+        :param packed_veclen: If packed types are targeted, specifies the
+                              vector length that the final offset should be
                               divided by.
-        @return: A string in C++ syntax with the correct offset
+        :return: A string in C++ syntax with the correct offset
     """
     subset = copy.deepcopy(subset_in)
 
     # Offset according to parameters
     if offset is not None:
         if isinstance(offset, subsets.Subset):
             subset.offset(offset, False)
@@ -2275,15 +2420,15 @@
         tmpl=reduction_tmpl,
         iname=inname,
         wcr=custom_reduction,
         ind=indstr,
     )
 
 
-def is_write_conflicted(dfg, edge, datanode=None):
+def is_write_conflicted(dfg, edge, datanode=None, sdfg_schedule=None):
     """ Detects whether a write-conflict-resolving edge can be emitted without
         using atomics or critical sections. """
 
     if edge.data.wcr_conflict is not None and not edge.data.wcr_conflict:
         return False
 
     if edge is None:
@@ -2315,14 +2460,19 @@
                 and e.dst.map.schedule != dtypes.ScheduleType.Sequential):
             return True
         # Should never happen (no such thing as write-conflicting reads)
         if (isinstance(e.src, nodes.EntryNode)
                 and e.src.map.schedule != dtypes.ScheduleType.Sequential):
             return True
 
+    # If SDFG schedule is not None (top-level) or not sequential
+    if (sdfg_schedule is not None
+            and sdfg_schedule != dtypes.ScheduleType.Sequential):
+        return True
+
     return False
 
 
 class LambdaToFunction(ast.NodeTransformer):
     def visit_Lambda(self, node: ast.Lambda):
         newbody = [ast.Return(value=node.body)]
         newnode = ast.FunctionDef(
@@ -2361,15 +2511,15 @@
 
     # Construct a C++ lambda function out of a function
     return '[] (%s) { %s }' % (', '.join('const auto& %s' % a
                                          for a in args), body_cpp)
 
 
 def unparse_tasklet(sdfg, state_id, dfg, node, function_stream,
-                    callsite_stream, locals, ldepth):
+                    callsite_stream, locals, ldepth, toplevel_schedule):
 
     if node.label is None or node.label == "":
         return ""
 
     state_dfg = sdfg.nodes()[state_id]
 
     # Not [], "" or None
@@ -2424,15 +2574,16 @@
     body = node.code
 
     # Map local names to memlets (for WCR detection)
     memlets = {}
     for edge in state_dfg.all_edges(node):
         u, uconn, v, vconn, memlet = edge
         if u == node:
-            memlet_nc = not is_write_conflicted(dfg, edge)
+            memlet_nc = not is_write_conflicted(
+                dfg, edge, sdfg_schedule=toplevel_schedule)
             memlet_wcr = memlet.wcr
 
             memlets[uconn] = (memlet, memlet_nc, memlet_wcr)
         elif v == node:
             memlets[vconn] = (memlet, False, None)
 
     callsite_stream.write("// Tasklet code (%s)\n" % node.label, sdfg,
@@ -2448,50 +2599,21 @@
         if rk is not None:
             # Unparse to C++ and add 'auto' declarations if locals not declared
             result = StringIO()
             cppunparse.CPPUnparser(rk, ldepth + 1, locals, result)
             callsite_stream.write(result.getvalue(), sdfg, state_id, node)
 
 
-def find_incoming_edges(node, dfg):
-    # If it's an entire SDFG, look in each state
-    if isinstance(dfg, SDFG):
-        result = []
-        for state in dfg.nodes():
-            result.extend(list(state.in_edges(node)))
-        return result
-    else:  # If it's one state
-        return list(dfg.in_edges(node))
-
-
-def find_outgoing_edges(node, dfg):
-    # If it's an entire SDFG, look in each state
-    if isinstance(dfg, SDFG):
-        result = []
-        for state in dfg.nodes():
-            result.extend(list(state.out_edges(node)))
-        return result
-    else:  # If it's one state
-        return list(dfg.out_edges(node))
-
-
-def sym2cpp(s):
-    """ Converts an array of symbolic variables (or one) to C++ strings. """
-    if not isinstance(s, list):
-        return cppunparse.pyexpr2cpp(symbolic.symstr(s))
-    return [cppunparse.pyexpr2cpp(symbolic.symstr(d)) for d in s]
-
-
 class DaCeKeywordRemover(ExtNodeTransformer):
-    """ Removes memlets and other DaCe keywords from a Python AST, and 
+    """ Removes memlets and other DaCe keywords from a Python AST, and
         converts array accesses to C++ methods that can be generated.
-        
-        Used for unparsing Python tasklets into C++ that uses the DaCe 
+
+        Used for unparsing Python tasklets into C++ that uses the DaCe
         runtime.
-        
+
         @note: Assumes that the DaCe syntax is correct (as verified by the
                Python frontend).
     """
 
     def __init__(self, sdfg, memlets, constants):
         self.sdfg = sdfg
         self.memlets = memlets
@@ -2659,19 +2781,14 @@
             return ast.copy_location(
                 ast.Name(id="(%s) { %s }" % (tname, fields), ctx=ast.Load),
                 node)
 
         return self.generic_visit(node)
 
 
-def unique(seq):
-    seen = set()
-    return [x for x in seq if not (x in seen or seen.add(x))]
-
-
 # TODO: This should be in the CUDA code generator. Add appropriate conditions to node dispatch predicate
 def presynchronize_streams(sdfg, dfg, state_id, node, callsite_stream):
     state_dfg = sdfg.nodes()[state_id]
     if hasattr(node, "_cuda_stream") or is_devicelevel(sdfg, state_dfg, node):
         return
     for e in state_dfg.in_edges(node):
         if hasattr(e.src, "_cuda_stream"):
```

### Comparing `dace-0.9.0/dace/codegen/targets/cuda.py` & `dace-0.9.5/dace/codegen/targets/cuda.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from six import StringIO
 import ast
 import ctypes
 import functools
 import os
 import sympy
+import warnings
 
 import dace
 from dace.frontend import operations
 from dace import subsets, symbolic, dtypes, data as dt
 from dace.config import Config
 from dace.graph import nodes
-from dace.sdfg import ScopeSubgraphView, SDFG, SDFGState, scope_contains_scope, is_devicelevel, is_array_stream_view
+from dace.sdfg import ScopeSubgraphView, SDFG, SDFGState, scope_contains_scope, is_devicelevel, is_array_stream_view, has_dynamic_map_inputs, dynamic_map_inputs
 from dace.codegen.codeobject import CodeObject
 from dace.codegen.prettycode import CodeIOStream
 from dace.codegen.targets.target import (TargetCodeGenerator, IllegalCopy,
                                          make_absolute, DefinedType)
 from dace.codegen.targets.cpu import (sym2cpp, unparse_cr, unparse_cr_split,
                                       cpp_array_expr, synchronize_streams)
 from dace.codegen.targets.framecode import _set_default_schedule_and_storage_types
@@ -33,14 +34,23 @@
 
 def _expr(val):
     if isinstance(val, symbolic.SymExpr):
         return val.expr
     return val
 
 
+def cpu_to_gpu_cpred(sdfg, state, src_node, dst_node):
+    """ Copy predicate from CPU to GPU that determines when a copy is illegal.
+        Returns True if copy is illegal, False otherwise.
+    """
+    if isinstance(sdfg.arrays[src_node.data], dt.Scalar):
+        return False
+    return True
+
+
 class CUDACodeGen(TargetCodeGenerator):
     """ GPU (CUDA) code generator. """
     target_name = 'cuda'
     title = 'CUDA'
     language = 'cu'
 
     def __init__(self, frame_codegen, sdfg):
@@ -110,16 +120,21 @@
                 dispatcher.register_copy_dispatcher(gst, st, None,
                                                     illegal_copy)
         for st in cpu_unpinned_storage:
             for sched_type in [
                     dtypes.ScheduleType.GPU_Device,
                     dtypes.ScheduleType.GPU_ThreadBlock
             ]:
+                # NOTE: Only reading to GPU has an exception (for Scalar inputs)
                 dispatcher.register_copy_dispatcher(
-                    st, dtypes.StorageType.Register, sched_type, illegal_copy)
+                    st,
+                    dtypes.StorageType.Register,
+                    sched_type,
+                    illegal_copy,
+                    predicate=cpu_to_gpu_cpred)
                 dispatcher.register_copy_dispatcher(
                     dtypes.StorageType.Register, st, sched_type, illegal_copy)
         # End of illegal copies
         # End of dispatcher registration
         ######################################
 
     def _emit_sync(self, codestream: CodeIOStream):
@@ -270,20 +285,18 @@
 
         nodedesc = node.desc(sdfg)
         if isinstance(nodedesc, dace.data.Stream):
             return self.allocate_stream(sdfg, dfg, state_id, node,
                                         function_stream, callsite_stream)
 
         result = StringIO()
-        arrsize = ' * '.join([
-            cppunparse.pyexpr2cpp(symbolic.symstr(s)) for s in nodedesc.strides
-        ])
-        is_dynamically_sized = any(
-            symbolic.issymbolic(s, sdfg.constants) for s in nodedesc.strides)
-        arrsize_malloc = arrsize + ' * sizeof(%s)' % nodedesc.dtype.ctype
+        arrsize = nodedesc.total_size
+        is_dynamically_sized = symbolic.issymbolic(arrsize, sdfg.constants)
+        arrsize_malloc = '%s * sizeof(%s)' % (sym2cpp(arrsize),
+                                              nodedesc.dtype.ctype)
         dataname = node.data
 
         # Different types of GPU arrays
         if nodedesc.storage == dtypes.StorageType.GPU_Global:
             result.write(
                 '%s *%s = nullptr;\n' % (nodedesc.dtype.ctype, dataname))
             self._dispatcher.defined_vars.add(dataname, DefinedType.Pointer)
@@ -304,31 +317,31 @@
                 'cudaMallocHost(&%s, %s);\n' % (dataname, arrsize_malloc))
             if node.setzero:
                 result.write(
                     'memset(%s, 0, %s);\n' % (dataname, arrsize_malloc))
         elif nodedesc.storage == dtypes.StorageType.GPU_Shared:
             if is_dynamically_sized:
                 raise NotImplementedError('Dynamic shared memory unsupported')
-            result.write("__shared__ %s %s[%s];\n" % (nodedesc.dtype.ctype,
-                                                      dataname, arrsize))
+            result.write("__shared__ %s %s[%s];\n" %
+                         (nodedesc.dtype.ctype, dataname, sym2cpp(arrsize)))
             self._dispatcher.defined_vars.add(dataname, DefinedType.Pointer)
             if node.setzero:
                 result.write(
                     'dace::ResetShared<{type}, {block_size}, {elements}, '
                     '1, false>::Reset({ptr});\n'.format(
                         type=nodedesc.dtype.ctype,
                         block_size=', '.join(_topy(self._block_dims)),
                         ptr=dataname,
-                        elements=arrsize))
+                        elements=sym2cpp(arrsize)))
         elif nodedesc.storage == dtypes.StorageType.GPU_Stack:
             if is_dynamically_sized:
                 raise ValueError('Dynamic allocation of registers not allowed')
             szstr = ' = {0}' if node.setzero else ''
             result.write("%s %s[%s]%s;\n" % (nodedesc.dtype.ctype, dataname,
-                                             arrsize, szstr))
+                                             sym2cpp(arrsize), szstr))
             self._dispatcher.defined_vars.add(dataname, DefinedType.Pointer)
         else:
             raise NotImplementedError("CUDA: Unimplemented storage type " +
                                       str(nodedesc.storage))
 
         callsite_stream.write(result.getvalue(), sdfg, state_id, node)
 
@@ -436,20 +449,20 @@
     def _compute_cudastreams(self,
                              sdfg: SDFG,
                              default_stream=0,
                              default_event=0):
         """ Annotates an SDFG (and all nested ones) to include a `_cuda_stream`
             field. This field is applied to all GPU maps, tasklets, and copies
             that can be executed in parallel.
-            @param sdfg: The sdfg to modify.
-            @param default_stream: The stream ID to start counting from (used
+            :param sdfg: The sdfg to modify.
+            :param default_stream: The stream ID to start counting from (used
                                    in recursion to nested SDFGs).
-            @param default_event: The event ID to start counting from (used
+            :param default_event: The event ID to start counting from (used
                                   in recursion to nested SDFGs).
-            @return: 2-tuple of the number of streams, events to create.
+            :return: 2-tuple of the number of streams, events to create.
         """
         concurrent_streams = int(
             Config.get('compiler', 'cuda', 'max_concurrent_streams'))
         if concurrent_streams < 0:
             return 0, 0
 
         def increment(streams):
@@ -942,28 +955,42 @@
             return
 
         # If not device-level code, ensure the schedule is correct
         if scope_entry.map.schedule != dtypes.ScheduleType.GPU_Device:
             raise TypeError('Cannot schedule %s directly from non-GPU code' %
                             str(scope_entry.map.schedule))
 
+        # Modify thread-blocks if dynamic ranges are detected
+        for node, graph in dfg_scope.all_nodes_recursive():
+            if isinstance(node, nodes.MapEntry):
+                smap = node.map
+                if (smap.schedule == dtypes.ScheduleType.GPU_ThreadBlock
+                        and has_dynamic_map_inputs(graph, node)):
+                    warnings.warn('Thread-block map cannot be used with '
+                                  'dynamic ranges, switching map "%s" to '
+                                  'sequential schedule' % smap.label)
+                    smap.schedule = dtypes.ScheduleType.Sequential
+
         # Determine whether to create a global (grid) barrier object
         create_grid_barrier = False
         for node in dfg_scope.nodes():
             if scope_entry == node: continue
             if (isinstance(node, nodes.EntryNode)
                     and node.map.schedule == dtypes.ScheduleType.GPU_Device):
                 create_grid_barrier = True
 
         kernel_name = '%s_%d_%d' % (
             scope_entry.map.label, dfg.node_id(scope_entry), sdfg.node_id(dfg))
 
         # Get parameters from input/output memlets to this map
         params = set(d.data for node in dfg_scope.source_nodes() for _,_,_,_,d in dfg.in_edges(node)) | \
                  set(d.data for node in dfg_scope.sink_nodes() for _,_,_,_,d in dfg.out_edges(node))
+        params -= set(
+            e.data.data
+            for e in dace.sdfg.dynamic_map_inputs(dfg, scope_entry))
 
         # Get symbolic parameters (free symbols) for kernel
         syms = sdfg.symbols_defined_at(scope_entry)
 
         # Pointers to callback functions cannot be used within CUDA kernels
         syms_copy = {}
         for _n, _s in syms.items():
@@ -973,16 +1000,16 @@
                 else:
                     syms_copy[_n] = _s
             except AttributeError:
                 syms_copy[_n] = _s
         syms = syms_copy
         freesyms = {
             k: v
-            for k, v in syms.items()
-            if k not in sdfg.constants and k not in scope_entry.map.params
+            for k, v in syms.items() if k not in sdfg.constants
+            and k not in scope_entry.map.params and k not in params
         }
         symbol_sigs = [
             v.dtype.ctype + ' ' + k for k, v in sorted(freesyms.items())
         ]
         symbol_names = [k for k in sorted(freesyms.keys())]
 
         # Hijack symbol_sigs to create a grid barrier object
@@ -1062,22 +1089,24 @@
         # Compute dynamic shared memory
         dynsmem_size = 0
         # For all access nodes, if array storage == GPU_Shared and size is
         # symbolic, add it. If nested SDFG, check all internal arrays
         for node in dfg_scope.nodes():
             if isinstance(node, nodes.AccessNode):
                 arr = sdfg.arrays[node.data]
-                if arr.storage == dtypes.StorageType.GPU_Shared:
+                if (arr.storage == dtypes.StorageType.GPU_Shared
+                        and arr.transient):
                     numel = functools.reduce(lambda a, b: a * b, arr.shape)
                     if symbolic.issymbolic(numel, sdfg.constants):
                         dynsmem_size += numel
             elif isinstance(node, nodes.NestedSDFG):
                 for sdfg_internal, _, arr in node.sdfg.arrays_recursive():
                     if (arr is not None
-                            and arr.storage == dtypes.StorageType.GPU_Shared):
+                            and arr.storage == dtypes.StorageType.GPU_Shared
+                            and arr.transient):
                         numel = functools.reduce(lambda a, b: a * b, arr.shape)
                         if symbolic.issymbolic(numel, sdfg_internal.constants):
                             dynsmem_size += numel
 
         max_streams = int(
             Config.get('compiler', 'cuda', 'max_concurrent_streams'))
         if max_streams >= 0:
@@ -1104,22 +1133,25 @@
         # Add invocation to calling code (in another file)
         function_stream.write(
             'DACE_EXPORTED void __dace_runkernel_%s(%s);\n' %
             (kernel_name, ', '.join(kernel_args_typed)), sdfg, state_id,
             scope_entry)
 
         # Synchronize all events leading to dynamic map range connectors
-        for e in dfg.in_edges(scope_entry):
-            if not e.dst_conn.startswith('IN_') and hasattr(e, '_cuda_event'):
+        for e in dace.sdfg.dynamic_map_inputs(dfg, scope_entry):
+            if hasattr(e, '_cuda_event'):
                 ev = e._cuda_event
                 callsite_stream.write(
-                    'DACE_CUDA_CHECK(cudaEventSynchronize(dace::cuda::__events[{ev}]));'.
-                    format(ev=ev),
+                    'DACE_CUDA_CHECK(cudaEventSynchronize(dace::cuda::__events[{ev}]));'
+                    .format(ev=ev),
                     sdfg,
                     state_id, [e.src, e.dst])
+            callsite_stream.write(
+                self._cpu_codegen.memlet_definition(
+                    sdfg, e.data, False, e.dst_conn), sdfg, state_id, node)
 
         # Invoke kernel call
         callsite_stream.write(
             '__dace_runkernel_%s(%s);\n' %
             (kernel_name, ', '.join(kernel_args)), sdfg, state_id, scope_entry)
 
         synchronize_streams(sdfg, dfg, state_id, scope_entry, scope_exit,
@@ -1180,17 +1212,17 @@
                     for n in state.nodes() if isinstance(n, nodes.MapEntry)
                     and n.schedule == dtypes.ScheduleType.GPU_ThreadBlock
                 ])
 
         # Case (1): no thread-block maps
         if len(tb_maps) == 0:
 
-            print('WARNING: Thread-block maps not found in kernel, assuming ' +
-                  'block size of (%s)' %
-                  Config.get('compiler', 'cuda', 'default_block_size'))
+            warnings.warn('Thread-block maps not found in kernel, assuming ' +
+                          'block size of (%s)' %
+                          Config.get('compiler', 'cuda', 'default_block_size'))
             block_size = [
                 int(b) for b in Config.get('compiler', 'cuda',
                                            'default_block_size').split(',')
             ]
             assert (len(block_size) >= 1 and len(block_size) <= 3)
 
             int_ceil = sympy.Function('int_ceil')
@@ -1236,14 +1268,18 @@
     def generate_kernel_scope(
             self, sdfg: SDFG, dfg_scope: ScopeSubgraphView, state_id: int,
             kernel_map: nodes.Map, kernel_name: str, grid_dims: list,
             block_dims: list, has_tbmap: bool, kernel_params: list,
             function_stream: CodeIOStream, kernel_stream: CodeIOStream):
         node = dfg_scope.source_nodes()[0]
 
+        # Add extra opening brace (dynamic map ranges, closed in MapExit
+        # generator)
+        kernel_stream.write('{', sdfg, state_id, node)
+
         if not node.map.flatten:
             # Add more opening braces for scope exit to close
             for dim in range(len(node.map.range) - 1):
                 kernel_stream.write('{\n', sdfg, state_id, node)
 
         # Generate all index arguments for kernel grid
         krange = subsets.Range(kernel_map.range[::-1])
@@ -1308,32 +1344,14 @@
             self._dispatcher.dispatch_allocate(sdfg, dfg_scope, state_id,
                                                child, function_stream,
                                                kernel_stream)
             self._dispatcher.dispatch_initialize(sdfg, dfg_scope, state_id,
                                                  child, function_stream,
                                                  kernel_stream)
 
-        # Generate register definitions for inter-tasklet memlets
-        dfg = sdfg.nodes()[state_id]
-        scope_dict = dfg.scope_dict()
-        for edge in dfg.edges():
-            # Only interested in edges within current scope
-            if scope_dict[edge.src] != node or scope_dict[edge.dst] != node:
-                continue
-            if (isinstance(edge.src, nodes.CodeNode)
-                    and isinstance(edge.dst, nodes.CodeNode)):
-                local_name = edge.data.data
-                # Allocate variable type
-                code = 'dace::vec<%s, %s> %s;' % (
-                    sdfg.arrays[edge.data.data].dtype.ctype,
-                    sym2cpp(edge.data.veclen), local_name)
-                kernel_stream.write(code, sdfg, state_id, [edge.src, edge.dst])
-                self._dispatcher.defined_vars.add(local_name,
-                                                  DefinedType.Scalar)
-
         # Generate conditions for this block's execution using min and max
         # element, e.g., skipping out-of-bounds threads in trailing block
         if has_tbmap == False:
             dsym_end = [d + bs - 1 for d, bs in zip(dsym, self._block_dims)]
             minels = krange.min_element()
             maxels = krange.max_element()
             for i, (v, minel, maxel) in enumerate(
@@ -1397,14 +1415,18 @@
 
         dfg = sdfg.nodes()[state_id]
         sdict = dfg.scope_dict()
         scope_entry = dfg_scope.source_nodes()[0]
         scope_map = scope_entry.map
         next_scopes = self.get_next_scope_entries(dfg, scope_entry)
 
+        # Add extra opening brace (dynamic map ranges, closed in MapExit
+        # generator)
+        callsite_stream.write('{', sdfg, state_id, scope_entry)
+
         if scope_map.schedule == dtypes.ScheduleType.GPU_ThreadBlock_Dynamic:
             if len(scope_map.params) > 1:
                 raise ValueError('Only one-dimensional maps are supported for '
                                  'dynamic block map schedule (got %d)' % len(
                                      scope_map.params))
             total_block_size = 1
             for bdim in self._block_dims:
@@ -1424,17 +1446,28 @@
                 raise NotImplementedError(
                     'Dynamic block map schedule only '
                     'implemented for 1D blocks currently')
             pscope = sdict[scope_entry]
             while pscope is not None and pscope.map.schedule != dtypes.ScheduleType.GPU_ThreadBlock:
                 pscope = sdict[pscope]
             if pscope is None:
-                raise NotImplementedError('Dynamic block map schedule '
-                                          'currently requires block map')
-            bname = pscope.map.params[0]
+                callsite_stream.write('int __dace_tid = threadIdx.x;', sdfg,
+                                      state_id, scope_entry)
+                bname = '__dace_tid'
+            else:
+                bname = pscope.map.params[0]
+
+            # Define all input connectors of this map entry
+            # Note: no need for a C scope around these, as there will not be
+            #       more than one dynamic thread-block map in a GPU device map
+            for e in dace.sdfg.dynamic_map_inputs(dfg, scope_entry):
+                callsite_stream.write(
+                    self._cpu_codegen.memlet_definition(
+                        sdfg, e.data, False, e.dst_conn), sdfg, state_id,
+                    scope_entry)
 
             callsite_stream.write(
                 'dace::DynamicMap<{bsize}>::template '
                 'schedule({begin}, {end}, {tid}, [&](auto {param}, '
                 'auto {tid}) {{'.format(
                     bsize=total_block_size,
                     begin=scope_map.range[0][0],
@@ -1572,27 +1605,33 @@
             return  # skip
 
         self._cpu_codegen.generate_node(sdfg, dfg, state_id, node,
                                         function_stream, callsite_stream)
 
     def _generate_NestedSDFG(self, sdfg, dfg, state_id, node, function_stream,
                              callsite_stream):
+        old_schedule = self._toplevel_schedule
         self._toplevel_schedule = node.schedule
+
         self._cpu_codegen._generate_NestedSDFG(
             sdfg, dfg, state_id, node, function_stream, callsite_stream)
 
+        self._toplevel_schedule = old_schedule
+
     def _generate_MapExit(self, sdfg, dfg, state_id, node, function_stream,
                           callsite_stream):
         if node.map.schedule == dtypes.ScheduleType.GPU_ThreadBlock:
             # Close block invocation conditions
             for i in range(len(node.map.params)):
                 callsite_stream.write('}', sdfg, state_id, node)
         elif node.map.schedule == dtypes.ScheduleType.GPU_ThreadBlock_Dynamic:
             # Close lambda function
             callsite_stream.write('});', sdfg, state_id, node)
+            # Close block invocation
+            callsite_stream.write('}', sdfg, state_id, node)
             return
 
         self._cpu_codegen._generate_MapExit(sdfg, dfg, state_id, node,
                                             function_stream, callsite_stream)
 
     def _generate_Reduce(self, sdfg, dfg, state_id, node, function_stream,
                          callsite_stream):
@@ -1644,14 +1683,32 @@
             sdfg, input_memlet, with_brackets=False))
         output = (output_memlet.data + ' + ' + cpp_array_expr(
             sdfg, output_memlet, with_brackets=False))
 
         # Options: Device-wide reduction (even from device code),
         #          block-wide reduction, sequential reduction (for loop)
         if node.schedule == dtypes.ScheduleType.GPU_Device:
+
+            input_dims = input_memlet.subset.dims()
+            output_dims = output_memlet.subset.data_dims()
+
+            reduce_all_axes = (node.axes is None
+                               or len(node.axes) == input_dims)
+            if reduce_all_axes:
+                reduce_last_axes = False
+            else:
+                reduce_last_axes = sorted(node.axes) == list(
+                    range(input_dims - len(node.axes), input_dims))
+
+            if (not reduce_all_axes) and (not reduce_last_axes):
+                raise NotImplementedError(
+                    'Multiple axis reductions not supported on GPUs. Please '
+                    'apply ReduceExpansion or make reduce axes to be last in the array'
+                )
+
             # Verify that data is on the GPU
             if input_data.desc(sdfg).storage not in [
                     dtypes.StorageType.GPU_Global,
                     dtypes.StorageType.CPU_Pinned
             ]:
                 raise ValueError('Input of GPU reduction must either reside '
                                  ' in global GPU memory or pinned CPU memory')
@@ -1678,24 +1735,50 @@
             self._globalcode.write(
                 """
                 void *__cub_storage_{sdfg}_{state}_{node} = NULL;
                 size_t __cub_ssize_{sdfg}_{state}_{node} = 0;
             """.format(sdfg=sdfg.name, state=state_id, node=node_id), sdfg,
                 state_id, node)
 
+            if reduce_all_axes:
+                reduce_type = 'DeviceReduce'
+                reduce_range = num_items
+                reduce_range_def = 'size_t num_items'
+                reduce_range_use = 'num_items'
+                reduce_range_call = num_items
+            elif reduce_last_axes:
+                num_reduce_axes = len(node.axes)
+                not_reduce_axes = reduce_shape[:-num_reduce_axes]
+                reduce_axes = reduce_shape[-num_reduce_axes:]
+
+                num_segments = ' * '.join([_topy(s) for s in not_reduce_axes])
+                segment_size = ' * '.join([_topy(s) for s in reduce_axes])
+
+                reduce_type = 'DeviceSegmentedReduce'
+                iterator = 'dace::stridedIterator({size})'.format(
+                    size=segment_size)
+                reduce_range = '{num}, {it}, {it} + 1'.format(
+                    num=num_segments, it=iterator)
+                reduce_range_def = 'size_t num_segments, size_t segment_size'
+                iterator_use = 'dace::stridedIterator(segment_size)'
+                reduce_range_use = 'num_segments, {it}, {it} + 1'.format(
+                    it=iterator_use)
+                reduce_range_call = '%s, %s' % (num_segments, segment_size)
+
             # Call CUB to get the storage size, allocate and free it
             self.scope_entry_stream.write(
                 """
-                cub::DeviceReduce::{kname}(nullptr, __cub_ssize_{sdfg}_{state}_{node},
-                                          ({intype}*)nullptr, ({outtype}*)nullptr, {num_items}{redop});
+                cub::{reduce_type}::{kname}(nullptr, __cub_ssize_{sdfg}_{state}_{node},
+                                          ({intype}*)nullptr, ({outtype}*)nullptr, {reduce_range}{redop});
                 cudaMalloc(&__cub_storage_{sdfg}_{state}_{node}, __cub_ssize_{sdfg}_{state}_{node});
 """.format(sdfg=sdfg.name,
             state=state_id,
             node=node_id,
-            num_items=num_items,
+            reduce_type=reduce_type,
+            reduce_range=reduce_range,
             redop=reduce_op,
             intype=input_data.desc(sdfg).dtype.ctype,
             outtype=output_data.desc(sdfg).dtype.ctype,
             kname=kname), sdfg, state_id, node)
 
             self.scope_exit_stream.write(
                 'cudaFree(__cub_storage_{sdfg}_{state}_{node});'.format(
@@ -1708,97 +1791,53 @@
                 cudastream = 'dace::cuda::__streams[%d]' % node._cuda_stream
             else:
                 cudastream = 'nullptr'
 
             # Write reduction function definition
             self._localcode.write(
                 """
-DACE_EXPORTED void __dace_reduce_{id}({intype} *input, {outtype} *output,
-                                      size_t num_items);
-void __dace_reduce_{id}({intype} *input, {outtype} *output, size_t num_items)
+DACE_EXPORTED void __dace_reduce_{id}({intype} *input, {outtype} *output, {reduce_range_def});
+void __dace_reduce_{id}({intype} *input, {outtype} *output, {reduce_range_def})
 {{
-    cub::DeviceReduce::{kname}(__cub_storage_{id}, __cub_ssize_{id},
-                                input, output, num_items{redop}, {stream});
+    cub::{reduce_type}::{kname}(__cub_storage_{id}, __cub_ssize_{id},
+                                input, output, {reduce_range_use}{redop}, {stream});
 }}
             """.format(
                     id=idstr,
                     intype=input_data.desc(sdfg).dtype.ctype,
                     outtype=output_data.desc(sdfg).dtype.ctype,
+                    reduce_type=reduce_type,
+                    reduce_range_def=reduce_range_def,
+                    reduce_range_use=reduce_range_use,
                     kname=kname,
                     redop=reduce_op,
                     stream=cudastream), sdfg, state_id, node)
 
             # Write reduction function definition in caller file
             function_stream.write(
                 """
-DACE_EXPORTED void __dace_reduce_{id}({intype} *input, {outtype} *output,
-                                      size_t num_items);
+DACE_EXPORTED void __dace_reduce_{id}({intype} *input, {outtype} *output, {reduce_range_def});
             """.format(
                     id=idstr,
+                    reduce_range_def=reduce_range_def,
                     intype=input_data.desc(sdfg).dtype.ctype,
                     outtype=output_data.desc(sdfg).dtype.ctype), sdfg,
                 state_id, node)
 
             # Call reduction function where necessary
-            input_dims = input_memlet.subset.dims()
-            output_dims = output_memlet.subset.data_dims()
-            if (node.axes is None or len(node.axes) == input_dims):
-                callsite_stream.write(
-                    '__dace_reduce_{id}({input}, {output}, {num_items});'.
-                    format(
-                        id=idstr,
-                        input=input,
-                        output=output,
-                        num_items=num_items), sdfg, state_id, node)
-            else:
-                raise NotImplementedError(
-                    'Multiple axis reductions not supported on GPUs. Please '
-                    'apply ReduceExpansion')
-                # Generate for loops around CUB calls and properly offset input
-                # and output arrays
-                #for axis in range(output_dims):
-                #    if axis not in node.axes:
-                #        callsite_stream.write(
-                #            'for (int {var} = {begin}; {var} < {end}; {var} += {skip}) {{'.
-                #            format(
-                #                var='__o%d' % axis,
-                #                begin=output_subset[axis][0],
-                #                end=output_subset[axis][1] + 1,
-                #                skip=output_subset[axis][2]), sdfg, state_id, node)
-                #
-                ### Obtain variable names per output and reduction axis
-                #axis_vars = []
-                #octr = 0
-                #for d in range(input_dims):
-                #    if d not in axes:
-                #        axis_vars.append('__o%d' % octr)
-                #        octr += 1
-                #
-                #input = (input_memlet.data.name + ' + ' + cpp_array_expr(
-                #            sdfg, input_memlet, with_brackets=False))
-                #output = (output_memlet.data.name + ' + ' + cpp_array_expr(
-                #            sdfg, output_memlet, with_brackets=False))
-                #num_items =
-                #
-                #callsite_stream.write(
-                #    '__dace_reduce_{id}({input}, {output}, {num_items});'
-                #    .format(
-                #        id=idstr,
-                #        input=input,
-                #        output=output,
-                #        num_items=num_items), sdfg, state_id, node)
-                #
-                ##cpp_array_expr(sdfg,
-                ##            output_memlet,
-                ##            offset=['__o%d' % i for i in range(output_dims)],
-                ##            relative_offset=False))
-                ##        invar = cpp_array_expr(sdfg,
-                ##            input_memlet, offset=axis_vars, relative_offset=False)
-                #for axis in range(output_dims):
-                #    callsite_stream.write('}\n', sdfg, state_id, node)
+            callsite_stream.write(
+                '__dace_reduce_{id}({input}, {output}, {reduce_range_call});'.
+                format(
+                    id=idstr,
+                    input=input,
+                    output=output,
+                    reduce_range_call=reduce_range_call), sdfg, state_id, node)
+
+            synchronize_streams(sdfg, dfg, state_id, node, node,
+                                callsite_stream)
             return
 
         # Block-wide reduction
         elif node.schedule == dtypes.ScheduleType.GPU_ThreadBlock:
             # Checks
             if not self._in_device_code:
                 raise ValueError('Block-wide GPU reduction must occur within'
```

### Comparing `dace-0.9.0/dace/codegen/targets/framecode.py` & `dace-0.9.5/dace/codegen/targets/framecode.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import collections
 import dace
 import functools
 from dace.codegen.prettycode import CodeIOStream
 from dace.codegen.targets.target import TargetCodeGenerator, TargetDispatcher
 from dace.sdfg import SDFG, SDFGState, ScopeSubgraphView
 from dace.graph import nodes
-from dace import dtypes, config
+from dace import dtypes, data, config
 
-from dace.frontend.python import ndarray
+from dace.frontend.python import wrappers
 from dace.codegen import cppunparse
 
 import networkx as nx
 import numpy as np
 
 
 class DaCeCodeGenerator(object):
@@ -35,37 +35,34 @@
         return self._dispatcher
 
     ##################################################################
     # Code generation
 
     def generate_constants(self, sdfg: SDFG, callsite_stream: CodeIOStream):
         # Write constants
-        for cstname, cstval in sdfg.constants.items():
-            if isinstance(cstval, np.ndarray):
-                if isinstance(cstval, ndarray.ndarray):
-                    dtype = cstval.descriptor.dtype
-                else:
-                    dtype = dtypes.typeclass(cstval.dtype.type)
-                const_str = "constexpr " + dtype.ctype + \
+        for cstname, (csttype, cstval) in sdfg.constants_prop.items():
+            if isinstance(csttype, data.Array):
+                const_str = "constexpr " + csttype.dtype.ctype + \
                     " " + cstname + "[" + str(cstval.size) + "] = {"
                 it = np.nditer(cstval, order='C')
                 for i in range(cstval.size - 1):
                     const_str += str(it[0]) + ", "
                     it.iternext()
                 const_str += str(it[0]) + "};\n"
                 callsite_stream.write(const_str, sdfg)
             else:
                 callsite_stream.write(
-                    "constexpr auto %s = %s;\n" % (cstname, str(cstval)), sdfg)
+                    "constexpr %s %s = %s;\n" % (csttype.dtype.ctype, cstname,
+                                                 str(cstval)), sdfg)
 
     def generate_fileheader(self, sdfg: SDFG, global_stream: CodeIOStream):
         """ Generate a header in every output file that includes custom types
             and constants.
-            @param sdfg: The input SDFG.
-            @param global_stream: Stream to write to (global).
+            :param sdfg: The input SDFG.
+            :param global_stream: Stream to write to (global).
         """
         #########################################################
         # Custom types
         datatypes = set()
         # Types of this SDFG
         for _, arrname, arr in sdfg.arrays_recursive():
             if arr is not None:
@@ -84,17 +81,17 @@
 
         global_stream.write(sdfg.global_code, sdfg)
 
     def generate_header(self, sdfg: SDFG, global_stream: CodeIOStream,
                         callsite_stream: CodeIOStream):
         """ Generate the header of the frame-code. Code exists in a separate
             function for overriding purposes.
-            @param sdfg: The input SDFG.
-            @param global_stream: Stream to write to (global).
-            @param callsite_stream: Stream to write to (at call site).
+            :param sdfg: The input SDFG.
+            :param global_stream: Stream to write to (global).
+            :param callsite_stream: Stream to write to (at call site).
         """
         fname = sdfg.name
         params = sdfg.signature()
 
         # Write frame code - header
         global_stream.write(
             '/* DaCe AUTO-GENERATED FILE. DO NOT MODIFY */\n' +
@@ -110,17 +107,17 @@
             if instr is not None:
                 instr.on_sdfg_begin(sdfg, callsite_stream, global_stream)
 
     def generate_footer(self, sdfg: SDFG, global_stream: CodeIOStream,
                         callsite_stream: CodeIOStream):
         """ Generate the footer of the frame-code. Code exists in a separate
             function for overriding purposes.
-            @param sdfg: The input SDFG.
-            @param global_stream: Stream to write to (global).
-            @param callsite_stream: Stream to write to (at call site).
+            :param sdfg: The input SDFG.
+            :param global_stream: Stream to write to (global).
+            :param callsite_stream: Stream to write to (at call site).
         """
         fname = sdfg.name
         params = sdfg.signature()
         paramnames = sdfg.signature(False, for_call=True)
 
         # Invoke all instrumentation providers
         for instr in self._dispatcher.instrumentation.values():
@@ -300,15 +297,16 @@
         callsite_stream.write(
             "goto __state_{}_{};".format(sdfg.name, edge.dst.label), sdfg, sid)
 
         if not always_true:
             callsite_stream.write("}")
 
     def generate_states(self, sdfg, scope_label, control_flow, global_stream,
-                        callsite_stream, scope, states_generated):
+                        callsite_stream, scope, states_generated,
+                        generated_edges):
 
         states_topological = list(sdfg.topological_sort(sdfg.start_state))
         states_to_generate = collections.deque([
             s for s in states_topological
             if s in scope and s not in states_generated
         ])
         if len(states_to_generate) == 0:
@@ -360,48 +358,50 @@
 
                     for control in control_flow[edge]:
 
                         if isinstance(control,
                                       dace.graph.edges.LoopAssignment):
                             # Generate the transition, but leave the
                             # assignments to the loop
-                            generate_transition = True
-                            generate_assignments = False
+                            generate_transition &= True
+                            generate_assignments &= False
 
                         elif isinstance(control, dace.graph.edges.LoopBack):
-                            generate_transition = False
-                            generate_assignments = False
+                            generate_transition &= False
+                            generate_assignments &= False
 
                         elif isinstance(control, dace.graph.edges.LoopExit):
                             # Need to strip the condition, so generate it from
                             # the loop entry
-                            generate_transition = False
-                            generate_assignments = True
-                            pass
+                            generate_transition &= False
+                            generate_assignments &= True
 
                         elif isinstance(control, dace.graph.edges.LoopEntry):
-                            generate_transition = False
-                            generate_assignments = False
+                            generate_transition &= False
+                            generate_assignments &= False
 
                             if control.scope.assignment is not None:
                                 assignment_edge = control.scope.assignment.edge
                                 init_assignments = ", ".join(
                                     DaCeCodeGenerator._generate_assignments(
                                         assignment_edge.data.assignments))
+                                generated_edges.add(assignment_edge)
                             else:
                                 init_assignments = ""
 
                             back_edge = control.scope.back.edge
                             continue_assignments = ", ".join(
                                 DaCeCodeGenerator._generate_assignments(
                                     back_edge.data.assignments))
+                            generated_edges.add(back_edge)
 
                             entry_edge = control.scope.entry.edge
                             condition = cppunparse.cppunparse(
                                 entry_edge.data.condition, False)
+                            generated_edges.add(entry_edge)
 
                             if (len(init_assignments) > 0
                                     or len(continue_assignments) > 0):
                                 callsite_stream.write(
                                     "for ({}; {}; {}) {{".format(
                                         init_assignments, condition,
                                         continue_assignments), sdfg, sid)
@@ -410,15 +410,16 @@
                                     "while ({}) {{".format(condition), sdfg,
                                     sid)
 
                             # Generate loop body
                             self.generate_states(
                                 sdfg, entry_edge.src.label + "_loop",
                                 control_flow, global_stream, callsite_stream,
-                                control.scope, states_generated)
+                                control.scope, states_generated,
+                                generated_edges)
 
                             callsite_stream.write("}", sdfg, sid)
 
                             exit_edge = control.scope.exit.edge
 
                             # Update states to generate after nested call
                             states_to_generate = collections.deque([
@@ -427,57 +428,64 @@
                             ])
                             # If the next state to be generated is the exit
                             # state, we can omit the goto
                             if (len(states_to_generate) > 0
                                     and states_to_generate[0] == exit_edge.dst
                                     and exit_edge.dst not in states_generated):
                                 pass
+                            elif edge in generated_edges:
+                                # This edge has more roles, goto doesn't apply
+                                pass
                             else:
                                 callsite_stream.write(
                                     "goto __state_{}_{};".format(
                                         sdfg.name,
                                         control.scope.exit.edge.dst))
+                                generated_edges.add(control.scope.exit.edge)
 
                         elif isinstance(control, dace.graph.edges.IfExit):
-                            generate_transition = True
-                            generate_assignments = True
+                            generate_transition &= True
+                            generate_assignments &= True
 
                         elif isinstance(control, dace.graph.edges.IfEntry):
-                            generate_transition = False
-                            generate_assignments = True
+                            generate_transition &= False
+                            generate_assignments &= True
 
                             if len(set(control.scope) - states_generated) == 0:
                                 continue
 
                             then_scope = control.scope.if_then_else.then_scope
                             else_scope = control.scope.if_then_else.else_scope
 
                             then_entry = then_scope.entry.edge
 
                             condition = cppunparse.cppunparse(
                                 then_entry.data.condition, False)
 
                             callsite_stream.write(
                                 "if ({}) {{".format(condition), sdfg, sid)
+                            generated_edges.add(then_entry)
 
                             # Generate the then-scope
-                            self.generate_states(sdfg, state.label + "_then",
-                                                 control_flow, global_stream,
-                                                 callsite_stream, then_scope,
-                                                 states_generated)
+                            self.generate_states(
+                                sdfg, state.label + "_then", control_flow,
+                                global_stream, callsite_stream, then_scope,
+                                states_generated, generated_edges)
 
                             callsite_stream.write("} else {", sdfg, sid)
+                            generated_edges.add(else_scope.entry.edge)
 
                             # Generate the else-scope
-                            self.generate_states(sdfg, state.label + "_else",
-                                                 control_flow, global_stream,
-                                                 callsite_stream, else_scope,
-                                                 states_generated)
+                            self.generate_states(
+                                sdfg, state.label + "_else", control_flow,
+                                global_stream, callsite_stream, else_scope,
+                                states_generated, generated_edges)
 
                             callsite_stream.write("}", sdfg, sid)
+                            generated_edges.add(else_scope.exit.edge)
 
                             # Update states to generate after nested call
                             states_to_generate = collections.deque([
                                 s for s in states_to_generate
                                 if s not in states_generated
                             ])
 
@@ -527,14 +535,16 @@
 
                 if generate_assignments:
 
                     callsite_stream.write(
                         ";\n".join(
                             DaCeCodeGenerator._generate_assignments(
                                 assignments_to_generate) + [""]), sdfg, sid)
+                generated_edges.add(edge)
+                # End of out_edges loop
 
             if (((len(out_edges) == 0) or
                  (not isinstance(scope, dace.graph.edges.ControlFlowScope) and
                   (len(states_to_generate) == 0)))
                     and (len(states_generated) != sdfg.number_of_nodes())):
                 callsite_stream.write(
                     "goto __state_exit_{}_{};".format(sdfg.name, scope_label),
@@ -571,33 +581,33 @@
     def generate_code(self,
                       sdfg: SDFG,
                       schedule: dtypes.ScheduleType,
                       sdfg_id: str = ""
                       ) -> (str, str, Set[TargetCodeGenerator]):
         """ Generate frame code for a given SDFG, calling registered targets'
             code generation callbacks for them to generate their own code.
-            @param sdfg: The SDFG to generate code for.
-            @param schedule: The schedule the SDFG is currently located, or
+            :param sdfg: The SDFG to generate code for.
+            :param schedule: The schedule the SDFG is currently located, or
                              None if the SDFG is top-level.
-            @param sdfg_id: An optional string id given to the SDFG label
-            @return: A tuple of the generated global frame code, local frame
+            :param sdfg_id: An optional string id given to the SDFG label
+            :return: A tuple of the generated global frame code, local frame
                      code, and a set of targets that have been used in the
                      generation of this SDFG.
         """
 
         sdfg_label = sdfg.name + sdfg_id
 
         global_stream = CodeIOStream()
         callsite_stream = CodeIOStream()
 
         # Set default storage/schedule types in SDFG
         _set_default_schedule_and_storage_types(sdfg, schedule)
 
         # Generate preamble (if top-level)
-        if schedule is None:
+        if sdfg.parent is None:
             self.generate_header(sdfg, global_stream, callsite_stream)
 
         # Generate code
         ###########################
 
         if sdfg.parent is not None:
             # Nested SDFG
@@ -654,14 +664,17 @@
             # Order according to topological sort
             all_cycles = [
                 sorted(c, key=lambda x: states_topological.index(x))
                 for c in all_cycles
             ]
             # Group in terms of starting node
             starting_nodes = [c[0] for c in all_cycles]
+            # Order cycles according to starting node in topological sort
+            starting_nodes = sorted(
+                starting_nodes, key=lambda x: states_topological.index(x))
             cycles_by_node = [[c for c in all_cycles if c[0] == n]
                               for n in starting_nodes]
             for cycles in cycles_by_node:
 
                 # Use arbitrary cycle to find the first and last nodes
                 first_node = cycles[0][0]
                 last_node = cycles[0][-1]
@@ -685,17 +698,17 @@
                 back_edge = sdfg.edges_between(last_node, first_node)
                 if len(back_edge) != 1:
                     raise RuntimeError("Expected exactly one edge in cycle")
                 back_edge = back_edge[0]
 
                 # Build a set of all nodes in all cycles associated with this
                 # set of start and end node
-                internal_nodes = functools.reduce(lambda a, b: a | b,
-                                                  [set(c) for c in cycles
-                                                   ]) - {first_node}
+                internal_nodes = functools.reduce(
+                    lambda a, b: a | b, [set(c)
+                                         for c in cycles]) - {first_node}
 
                 exit_edge = [
                     e for e in sdfg.out_edges(first_node)
                     if e.dst not in internal_nodes | {first_node}
                 ]
                 if len(exit_edge) != 1:
                     # No single stopping condition: not a for or while
@@ -709,16 +722,37 @@
                 if len(entry_edge) != 1:
                     # No single starting condition: not a for or while
                     continue
                 entry_edge = entry_edge[0]
 
                 # Make sure this is not already annotated to be another construct
                 if (len(control_flow[entry_edge]) != 0
-                        or len(control_flow[back_edge]) != 0
-                        or len(control_flow[exit_edge]) != 0):
+                        or len(control_flow[back_edge]) != 0):
+                    continue
+
+                # Nested loops case I - previous edge of internal loop is a
+                # loop-entry of an external loop (first state in a loop is
+                # another loop)
+                if (len(control_flow[previous_edge]) == 1
+                        and isinstance(control_flow[previous_edge][0],
+                                       dace.graph.edges.LoopEntry)):
+                    # Nested loop, mark parent scope
+                    loop_parent = control_flow[previous_edge][0].scope
+                # Nested loops case II - exit edge of internal loop is a
+                # back-edge of an external loop (last state in a loop is another
+                # loop)
+                elif (len(control_flow[exit_edge]) == 1
+                      and isinstance(control_flow[exit_edge][0],
+                                     dace.graph.edges.LoopBack)):
+                    # Nested loop, mark parent scope
+                    loop_parent = control_flow[exit_edge][0].scope
+                elif (len(control_flow[exit_edge]) == 0
+                      or len(control_flow[previous_edge]) == 0):
+                    loop_parent = None
+                else:
                     continue
 
                 if entry_edge == back_edge:
                     # No entry check (we don't support do-loops)
                     # TODO: do we want to add some support for self-loops?
                     continue
 
@@ -728,16 +762,18 @@
                 if any([len(set(c) - internal_nodes) > 1 for c in cycles]):
                     continue
 
                 # This is a loop! Generate the necessary annotation objects.
                 loop_scope = dace.graph.edges.LoopScope(internal_nodes)
 
                 if ((len(previous_edge.data.assignments) > 0
-                     or len(back_edge.data.assignments) > 0)
-                        and len(control_flow[previous_edge]) == 0):
+                     or len(back_edge.data.assignments) > 0) and
+                    (len(control_flow[previous_edge]) == 0 or
+                     (len(control_flow[previous_edge]) == 1 and
+                      control_flow[previous_edge][0].scope == loop_parent))):
                     # Generate assignment edge, if available
                     control_flow[previous_edge].append(
                         dace.graph.edges.LoopAssignment(
                             loop_scope, previous_edge))
                 # Assign remaining control flow constructs
                 control_flow[entry_edge].append(
                     dace.graph.edges.LoopEntry(loop_scope, entry_edge))
@@ -845,17 +881,18 @@
                     control_flow[left_exit].append(
                         dace.graph.edges.IfExit(else_scope, left_exit))
 
         #######################################################################
         # State transition generation
 
         states_generated = set()  # For sanity check
-        self.generate_states(sdfg, "sdfg", control_flow,
-                             global_stream, callsite_stream,
-                             set(states_topological), states_generated)
+        generated_edges = set()
+        self.generate_states(
+            sdfg, "sdfg", control_flow, global_stream, callsite_stream,
+            set(states_topological), states_generated, generated_edges)
 
         #############################
         # End of code generation
 
         if len(states_generated) != len(sdfg.nodes()):
             raise RuntimeError(
                 "Not all states were generated in SDFG {}!"
@@ -874,15 +911,15 @@
                         sdfg, state, None, node, global_stream,
                         callsite_stream)
                     deallocated.add(node.data)
 
         ###########################
 
         # Generate footer (if top-level)
-        if schedule is None:
+        if sdfg.parent is None:
             self.generate_footer(sdfg, global_stream, callsite_stream)
 
         # Clear out all the annotated control flow
 
         # Return the generated global and local code strings
         return (global_stream.getvalue(), callsite_stream.getvalue(),
                 self._dispatcher.used_targets)
@@ -915,16 +952,15 @@
                     if node.consume.schedule == dtypes.ScheduleType.Default:
                         node.consume._schedule = \
                             dtypes.SCOPEDEFAULT_SCHEDULE[parent_schedule]
                     # Also traverse children (recursively)
                     set_default_in_scope(node)
                 elif getattr(node, 'schedule', False):
                     if node.schedule == dtypes.ScheduleType.Default:
-                        node._schedule = \
-                            dtypes.SCOPEDEFAULT_SCHEDULE[parent_schedule]
+                        node._schedule = parent_schedule
 
         ## End of recursive function
 
         # Start with top-level nodes
         set_default_in_scope(None)
 
         # Set default storage type
```

### Comparing `dace-0.9.0/dace/codegen/targets/immaterial.py` & `dace-0.9.5/dace/codegen/targets/immaterial.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,18 +183,15 @@
                                            memlet.subset.ranges[-1][0])))
                 else:  # Non-contiguous dimension
                     useskip = True
                     memlet_params[-1] += ' + %s' % cpp_array_expr(
                         sdfg, memlet, False)
                     memlet_range = memlet.subset.ranges[indexdim]
 
-                    # TODO(later): Access order
-                    memlet_stride = functools.reduce(
-                        lambda x, y: x * y,
-                        sdfg.arrays[memlet.data].shape[indexdim + 1:])
+                    memlet_stride = sdfg.arrays[memlet.data].strides[indexdim]
                     memlet_stride = sym2cpp(memlet_stride)
 
                     memlet_params.append(
                         '0, %s, %s' %
                         (sym2cpp(memlet_range[1] - memlet_range[0]),
                          sym2cpp(memlet_stride)))
```

### Comparing `dace-0.9.0/dace/codegen/targets/mpi.py` & `dace-0.9.5/dace/codegen/targets/mpi.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,18 @@
         # Take care of map header
         assert len(dfg_scope.source_nodes()) == 1
         map_header = dfg_scope.source_nodes()[0]
 
         function_stream.write('extern int __dace_comm_size, __dace_comm_rank;',
                               sdfg, state_id, map_header)
 
+        # Add extra opening brace (dynamic map ranges, closed in MapExit
+        # generator)
+        callsite_stream.write('{', sdfg, state_id, map_header)
+
         if len(map_header.map.params) > 1:
             raise NotImplementedError(
                 'Multi-dimensional MPI maps are not supported')
 
         for var, r in zip(map_header.map.params, map_header.map.range):
             begin, end, skip = r
```

### Comparing `dace-0.9.0/dace/codegen/targets/target.py` & `dace-0.9.5/dace/codegen/targets/target.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,140 +19,140 @@
             to files with generated code.
             @see: CodeObject
         """
         raise NotImplementedError('Abstract class')
 
     @property
     def has_initializer(self):
-        """ Returns True if the target generates a `__dace_init_<TARGET>` 
+        """ Returns True if the target generates a `__dace_init_<TARGET>`
             function that should be called on initialization. """
         raise NotImplementedError('Abstract class')
 
     @property
     def has_finalizer(self):
-        """ Returns True if the target generates a `__dace_exit_<TARGET>` 
+        """ Returns True if the target generates a `__dace_exit_<TARGET>`
             function that should be called on finalization. """
         raise NotImplementedError('Abstract class')
 
     def generate_state(self, sdfg, state, function_stream, callsite_stream):
-        """ Generates code for an SDFG state, outputting it to the given 
+        """ Generates code for an SDFG state, outputting it to the given
             code streams.
-            @param sdfg: The SDFG to generate code from.
-            @param state: The SDFGState to generate code from.
-            @param function_stream: A `CodeIOStream` object that will be
+            :param sdfg: The SDFG to generate code from.
+            :param state: The SDFGState to generate code from.
+            :param function_stream: A `CodeIOStream` object that will be
                                     generated outside the calling code, for
                                     use when generating global functions.
-            @param callsite_stream: A `CodeIOStream` object that points
+            :param callsite_stream: A `CodeIOStream` object that points
                                     to the current location (call-site)
                                     in the code.
         """
         raise NotImplementedError('Abstract class')
 
     def generate_scope(self, sdfg, dfg_scope, state_id, function_stream,
                        callsite_stream):
         """ Generates code for an SDFG state scope (from a scope-entry node
-            to its corresponding scope-exit node), outputting it to the given 
+            to its corresponding scope-exit node), outputting it to the given
             code streams.
-            @param sdfg: The SDFG to generate code from.
-            @param dfg_scope: The `ScopeSubgraphView` to generate code from.
-            @param state_id: The node ID of the state in the given SDFG.
-            @param function_stream: A `CodeIOStream` object that will be
+            :param sdfg: The SDFG to generate code from.
+            :param dfg_scope: The `ScopeSubgraphView` to generate code from.
+            :param state_id: The node ID of the state in the given SDFG.
+            :param function_stream: A `CodeIOStream` object that will be
                                     generated outside the calling code, for
                                     use when generating global functions.
-            @param callsite_stream: A `CodeIOStream` object that points
+            :param callsite_stream: A `CodeIOStream` object that points
                                     to the current location (call-site)
                                     in the code.
         """
         raise NotImplementedError('Abstract class')
 
     def generate_node(self, sdfg, dfg, state_id, node, function_stream,
                       callsite_stream):
-        """ Generates code for a single node, outputting it to the given 
+        """ Generates code for a single node, outputting it to the given
             code streams.
-            @param sdfg: The SDFG to generate code from.
-            @param dfg: The SDFG state to generate code from.
-            @param state_id: The node ID of the state in the given SDFG.
-            @param node: The node to generate code from.
-            @param function_stream: A `CodeIOStream` object that will be
+            :param sdfg: The SDFG to generate code from.
+            :param dfg: The SDFG state to generate code from.
+            :param state_id: The node ID of the state in the given SDFG.
+            :param node: The node to generate code from.
+            :param function_stream: A `CodeIOStream` object that will be
                                     generated outside the calling code, for
                                     use when generating global functions.
-            @param callsite_stream: A `CodeIOStream` object that points
+            :param callsite_stream: A `CodeIOStream` object that points
                                     to the current location (call-site)
                                     in the code.
         """
         raise NotImplementedError('Abstract class')
 
     def allocate_array(self, sdfg, dfg, state_id, node, function_stream,
                        callsite_stream):
-        """ Generates code for allocating an array, outputting to the given 
+        """ Generates code for allocating an array, outputting to the given
             code streams.
-            @param sdfg: The SDFG to generate code from.
-            @param dfg: The SDFG state to generate code from.
-            @param state_id: The node ID of the state in the given SDFG.
-            @param node: The data node to generate allocation for.
-            @param function_stream: A `CodeIOStream` object that will be
+            :param sdfg: The SDFG to generate code from.
+            :param dfg: The SDFG state to generate code from.
+            :param state_id: The node ID of the state in the given SDFG.
+            :param node: The data node to generate allocation for.
+            :param function_stream: A `CodeIOStream` object that will be
                                     generated outside the calling code, for
                                     use when generating global functions.
-            @param callsite_stream: A `CodeIOStream` object that points
+            :param callsite_stream: A `CodeIOStream` object that points
                                     to the current location (call-site)
                                     in the code.
         """
         raise NotImplementedError('Abstract class')
 
     def initialize_array(self, sdfg, dfg, state_id, node, function_stream,
                          callsite_stream):
-        """ Generates code for initializing an array, outputting to the given 
+        """ Generates code for initializing an array, outputting to the given
             code streams.
-            @param sdfg: The SDFG to generate code from.
-            @param dfg: The SDFG state to generate code from.
-            @param state_id: The node ID of the state in the given SDFG.
-            @param node: The data node to generate initialization for.
-            @param function_stream: A `CodeIOStream` object that will be
+            :param sdfg: The SDFG to generate code from.
+            :param dfg: The SDFG state to generate code from.
+            :param state_id: The node ID of the state in the given SDFG.
+            :param node: The data node to generate initialization for.
+            :param function_stream: A `CodeIOStream` object that will be
                                     generated outside the calling code, for
                                     use when generating global functions.
-            @param callsite_stream: A `CodeIOStream` object that points
+            :param callsite_stream: A `CodeIOStream` object that points
                                     to the current location (call-site)
                                     in the code.
         """
         raise NotImplementedError('Abstract class')
 
     def deallocate_array(self, sdfg, dfg, state_id, node, function_stream,
                          callsite_stream):
-        """ Generates code for deallocating an array, outputting to the given 
+        """ Generates code for deallocating an array, outputting to the given
             code streams.
-            @param sdfg: The SDFG to generate code from.
-            @param dfg: The SDFG state to generate code from.
-            @param state_id: The node ID of the state in the given SDFG.
-            @param node: The data node to generate deallocation for.
-            @param function_stream: A `CodeIOStream` object that will be
+            :param sdfg: The SDFG to generate code from.
+            :param dfg: The SDFG state to generate code from.
+            :param state_id: The node ID of the state in the given SDFG.
+            :param node: The data node to generate deallocation for.
+            :param function_stream: A `CodeIOStream` object that will be
                                     generated outside the calling code, for
                                     use when generating global functions.
-            @param callsite_stream: A `CodeIOStream` object that points
+            :param callsite_stream: A `CodeIOStream` object that points
                                     to the current location (call-site)
                                     in the code.
         """
         raise NotImplementedError('Abstract class')
 
     def copy_memory(self, sdfg, dfg, state_id, src_node, dst_node, edge,
                     function_stream, callsite_stream):
-        """ Generates code for copying memory, either from a data access 
-            node (array/stream) to another, a code node (tasklet/nested 
+        """ Generates code for copying memory, either from a data access
+            node (array/stream) to another, a code node (tasklet/nested
             SDFG) to another, or a combination of the two.
-            @param sdfg: The SDFG to generate code from.
-            @param dfg: The SDFG state to generate code from.
-            @param state_id: The node ID of the state in the given SDFG.
-            @param src_node: The source node to generate copy code for.
-            @param dst_node: The destination node to generate copy code for.
-            @param edge: The edge representing the copy (in the innermost
+            :param sdfg: The SDFG to generate code from.
+            :param dfg: The SDFG state to generate code from.
+            :param state_id: The node ID of the state in the given SDFG.
+            :param src_node: The source node to generate copy code for.
+            :param dst_node: The destination node to generate copy code for.
+            :param edge: The edge representing the copy (in the innermost
                          scope, adjacent to either the source or destination
                          node).
-            @param function_stream: A `CodeIOStream` object that will be
+            :param function_stream: A `CodeIOStream` object that will be
                                     generated outside the calling code, for
                                     use when generating global functions.
-            @param callsite_stream: A `CodeIOStream` object that points
+            :param callsite_stream: A `CodeIOStream` object that points
                                     to the current location (call-site)
                                     in the code.
         """
         raise NotImplementedError('Abstract class')
 
 
 class IllegalCopy(TargetCodeGenerator):
@@ -166,19 +166,19 @@
 
 
 class DefinedType(dace.dtypes.AutoNumber):
     """ Data types for `DefinedMemlets`.
         @see: DefinedMemlets
     """
     Pointer = ()
-    ArrayView = ()
     Scalar = ()
-    ScalarView = ()
+    ArrayView = ()
     Stream = ()
     StreamArray = ()
+    StreamView = ()
 
 
 class DefinedMemlets:
     """ Keeps track of the type of defined memlets to ensure that they are
         referenced correctly in nested scopes and SDFGs. """
 
     def __init__(self):
@@ -266,16 +266,16 @@
         """ Returns a list of targets (code generators) that were triggered
             during generation. """
         return self._used_targets
 
     def register_state_dispatcher(self, dispatcher, predicate=None):
         """ Registers a code generator that processes a single state, calling
             `generate_state`.
-            @param dispatcher: The code generator to use.
-            @param predicate: A lambda function that accepts the SDFG and 
+            :param dispatcher: The code generator to use.
+            :param predicate: A lambda function that accepts the SDFG and
                               state, and triggers the code generator when True
                               is returned. If None, registers `dispatcher`
                               as the default state dispatcher.
             @see: TargetCodeGenerator
         """
 
         if not hasattr(dispatcher, "generate_state"):
@@ -293,17 +293,17 @@
     def get_predicated_state_dispatchers(self):
         """ Returns a list of state dispatchers with predicates. """
         return list(self._state_dispatchers)
 
     def register_node_dispatcher(self, dispatcher, predicate=None):
         """ Registers a code generator that processes a single node, calling
             `generate_node`.
-            @param dispatcher: The code generator to use.
-            @param predicate: A lambda function that accepts the SDFG, state,
-                              and node, and triggers the code generator when 
+            :param dispatcher: The code generator to use.
+            :param predicate: A lambda function that accepts the SDFG, state,
+                              and node, and triggers the code generator when
                               True is returned. If None, registers `dispatcher`
                               as the default node dispatcher.
             @see: TargetCodeGenerator
         """
         if not hasattr(dispatcher, "generate_node"):
             raise TypeError("Node dispatcher must "
                             "implement \"generate_node\"")
@@ -319,16 +319,16 @@
     def get_predicated_node_dispatchers(self):
         """ Returns a list of node dispatchers with predicates. """
         return list(self._node_dispatchers)
 
     def register_map_dispatcher(self, schedule_type, func):
         """ Registers a function that processes a scope, used when calling
             `dispatch_subgraph` and `dispatch_scope`.
-            @param schedule_type: The scope schedule that triggers `func`.
-            @param func: A TargetCodeGenerator object that contains an 
+            :param schedule_type: The scope schedule that triggers `func`.
+            :param func: A TargetCodeGenerator object that contains an
                          implementation of `generate_scope`.
             @see: TargetCodeGenerator
         """
         if isinstance(schedule_type, list):
             for stype in schedule_type:
                 self.register_map_dispatcher(stype, func)
             return
@@ -337,19 +337,19 @@
         if not isinstance(func, TargetCodeGenerator): raise TypeError
         if schedule_type in self._map_dispatchers:
             raise ValueError('Schedule already mapped to ' +
                              str(self._map_dispatchers[schedule_type]))
         self._map_dispatchers[schedule_type] = func
 
     def register_array_dispatcher(self, storage_type, func):
-        """ Registers a function that processes data allocation,   
+        """ Registers a function that processes data allocation,
             initialization, and deinitialization. Used when calling
             `dispatch_allocate/deallocate/initialize`.
-            @param storage_type: The data storage type that triggers `func`.
-            @param func: A TargetCodeGenerator object that contains an 
+            :param storage_type: The data storage type that triggers `func`.
+            :param func: A TargetCodeGenerator object that contains an
                          implementation of data memory management functions.
             @see: TargetCodeGenerator
         """
         if isinstance(storage_type, list):
             for stype in storage_type:
                 self.register_array_dispatcher(stype, func)
             return
@@ -360,31 +360,31 @@
 
     def register_copy_dispatcher(self,
                                  src_storage,
                                  dst_storage,
                                  dst_schedule,
                                  func,
                                  predicate=None):
-        """ Registers code generation of data-to-data (or data from/to 
-            tasklet, if src/dst storage is StorageType.Register) copy 
-            functions. Can also be target-schedule specific, or 
+        """ Registers code generation of data-to-data (or data from/to
+            tasklet, if src/dst storage is StorageType.Register) copy
+            functions. Can also be target-schedule specific, or
             dst_schedule=None if the function will be invoked on any schedule.
-            @param src_storage: The source data storage type that triggers 
+            :param src_storage: The source data storage type that triggers
                                 `func`.
-            @param dst_storage: The destination data storage type that 
+            :param dst_storage: The destination data storage type that
                                 triggers `func`.
-            @param dst_schedule: An optional destination scope schedule type 
+            :param dst_schedule: An optional destination scope schedule type
                                  that triggers `func`.
-            @param func: A TargetCodeGenerator object that contains an 
+            :param func: A TargetCodeGenerator object that contains an
                          implementation of `copy_memory`.
-            @param predicate: A lambda function that accepts the SDFG, state,
-                              and source and destination nodes, and triggers 
+            :param predicate: A lambda function that accepts the SDFG, state,
+                              and source and destination nodes, and triggers
                               the code generator when True is returned. If
                               None, always dispatches with this dispatcher.
-            @see: TargetCodeGenerator            
+            @see: TargetCodeGenerator
         """
 
         if not isinstance(src_storage, dtypes.StorageType): raise TypeError
         if not isinstance(dst_storage, dtypes.StorageType): raise TypeError
         if (dst_schedule is not None
                 and not isinstance(dst_schedule, dtypes.ScheduleType)):
             raise TypeError
@@ -428,15 +428,15 @@
     def dispatch_subgraph(self,
                           sdfg,
                           dfg,
                           state_id,
                           function_stream,
                           callsite_stream,
                           skip_entry_node=False):
-        """ Dispatches a code generator for a scope subgraph of an 
+        """ Dispatches a code generator for a scope subgraph of an
             `SDFGState`. """
 
         start_nodes = list(
             v for v in dfg.nodes() if len(list(dfg.predecessors(v))) == 0)
 
         # Mark nodes to skip in order to be able to skip
         nodes_to_skip = set()
@@ -491,15 +491,15 @@
             # Otherwise use the generic code generator (CPU)
             self._used_targets.add(self._generic_node_dispatcher)
             self._generic_node_dispatcher.generate_node(
                 sdfg, dfg, state_id, node, function_stream, callsite_stream)
 
     def dispatch_scope(self, map_schedule, sdfg, sub_dfg, state_id,
                        function_stream, callsite_stream):
-        """ Dispatches a code generator function for a scope in an SDFG 
+        """ Dispatches a code generator function for a scope in an SDFG
             state. """
         entry_node = sub_dfg.source_nodes()[0]
         self.defined_vars.enter_scope(entry_node)
         self._used_targets.add(self._map_dispatchers[map_schedule])
         self._map_dispatchers[map_schedule].generate_scope(
             sdfg, sub_dfg, state_id, function_stream, callsite_stream)
         self.defined_vars.exit_scope(entry_node)
@@ -612,15 +612,15 @@
         target.copy_memory(sdfg, dfg, state_id, src_node, dst_node, edge,
                            function_stream, output_stream)
 
 
 def make_absolute(path):
     if os.path.isfile(path):
         if os.path.isabs(path):
-            # Path is abolute, we're happy
+            # Path is absolute, we're happy
             return path
         else:
             # Path is relative: make it absolute
             return os.path.abspath(path)
     else:
         # This is not a path, probably just an executable name, such
         # as "g++". Try to find it on the PATH
```

### Comparing `dace-0.9.0/dace/codegen/targets/xilinx.py` & `dace-0.9.5/dace/codegen/targets/fpga.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 from six import StringIO
 import collections
 import functools
-import os
 import itertools
 import re
 import sympy as sp
+import numpy as np
 
 import dace
 from dace import subsets
 from dace.config import Config
 from dace.frontend import operations
 from dace.graph import nodes
 from dace.sdfg import ScopeSubgraphView, find_input_arraynode, find_output_arraynode
 from dace.codegen.codeobject import CodeObject
 from dace.codegen.prettycode import CodeIOStream
+from dace.codegen.targets.target import TargetCodeGenerator, DefinedType
 from dace.codegen.targets.target import (TargetCodeGenerator, IllegalCopy,
                                          make_absolute, DefinedType)
 from dace.codegen.targets.cpu import cpp_offset_expr, cpp_array_expr
-from dace.codegen.targets import cpu, cuda
-
+from dace.codegen.targets import cpu
 from dace.codegen import cppunparse
-
-REDUCTION_TYPE_TO_HLSLIB = {
-    dace.dtypes.ReductionType.Min: "hlslib::op::Min",
-    dace.dtypes.ReductionType.Max: "hlslib::op::Max",
-    dace.dtypes.ReductionType.Sum: "hlslib::op::Sum",
-    dace.dtypes.ReductionType.Product: "hlslib::op::Product",
-    dace.dtypes.ReductionType.Logical_And: "hlslib::op::And",
-}
+from dace.properties import Property, make_properties, indirect_properties
 
 
-class XilinxCodeGen(TargetCodeGenerator):
-    """ Xilinx FPGA code generator. """
-    target_name = 'xilinx'
-    title = 'Xilinx'
-    language = 'hls'
+class FPGACodeGen(TargetCodeGenerator):
+    # Set by deriving class
+    target_name = None
+    title = None
+    language = None
 
     def __init__(self, frame_codegen, sdfg):
+
+        # The inheriting class must set target_name, title and language.
+
         self._in_device_code = False
         self._cpu_codegen = None
         self._frame = frame_codegen
         self._dispatcher = frame_codegen.dispatcher
 
         self._global_sdfg = sdfg
         self._program_name = sdfg.name
@@ -52,42 +48,43 @@
 
         # Register dispatchers
         self._cpu_codegen = self._dispatcher.get_generic_node_dispatcher()
 
         self._host_codes = []
         self._kernel_codes = []
 
-        # Register additional Xilinx dispatchers
+        # Register additional FPGA dispatchers
         self._dispatcher.register_map_dispatcher(
             [dace.dtypes.ScheduleType.FPGA_Device], self)
 
         self._dispatcher.register_state_dispatcher(
             self,
             predicate=lambda sdfg, state: len(state.data_nodes()) > 0 and all([
                 n.desc(sdfg).storage in [
-                    dace.dtypes.StorageType.FPGA_Global,
-                    dace.dtypes.StorageType.FPGA_Local,
-                    dace.dtypes.StorageType.FPGA_Registers]
-                for n in state.data_nodes()]))
+                    dace.dtypes.StorageType.FPGA_Global, dace.dtypes.
+                    StorageType.FPGA_Local, dace.dtypes.StorageType.
+                    FPGA_Registers
+                ] for n in state.data_nodes()
+            ]))
 
         self._dispatcher.register_node_dispatcher(
             self, predicate=lambda *_: self._in_device_code)
 
-        xilinx_storage = [
+        fpga_storage = [
             dace.dtypes.StorageType.FPGA_Global,
             dace.dtypes.StorageType.FPGA_Local,
             dace.dtypes.StorageType.FPGA_Registers,
         ]
-        self._dispatcher.register_array_dispatcher(xilinx_storage, self)
+        self._dispatcher.register_array_dispatcher(fpga_storage, self)
 
         # Register permitted copies
         for storage_from in itertools.chain(
-                xilinx_storage, [dace.dtypes.StorageType.Register]):
+                fpga_storage, [dace.dtypes.StorageType.Register]):
             for storage_to in itertools.chain(
-                    xilinx_storage, [dace.dtypes.StorageType.Register]):
+                    fpga_storage, [dace.dtypes.StorageType.Register]):
                 if (storage_from == dace.dtypes.StorageType.Register
                         and storage_to == dace.dtypes.StorageType.Register):
                     continue
                 self._dispatcher.register_copy_dispatcher(
                     storage_from, storage_to, None, self)
         self._dispatcher.register_copy_dispatcher(
             dace.dtypes.StorageType.FPGA_Global,
@@ -106,41 +103,17 @@
     def has_initializer(self):
         return True
 
     @property
     def has_finalizer(self):
         return False
 
-    @staticmethod
-    def cmake_options():
-        compiler = make_absolute(
-            Config.get("compiler", "xilinx", "executable"))
-        host_flags = Config.get("compiler", "xilinx", "host_flags")
-        synthesis_flags = Config.get("compiler", "xilinx", "synthesis_flags")
-        build_flags = Config.get("compiler", "xilinx", "build_flags")
-        mode = Config.get("compiler", "xilinx", "mode")
-        target_platform = Config.get("compiler", "xilinx", "platform")
-        enable_debugging = ("ON"
-                            if Config.get_bool("compiler", "xilinx",
-                                               "enable_debugging") else "OFF")
-        options = [
-            "-DSDACCEL_ROOT_DIR={}".format(
-                os.path.dirname(os.path.dirname(compiler))),
-            "-DDACE_XILINX_HOST_FLAGS=\"{}\"".format(host_flags),
-            "-DDACE_XILINX_SYNTHESIS_FLAGS=\"{}\"".format(synthesis_flags),
-            "-DDACE_XILINX_BUILD_FLAGS=\"{}\"".format(build_flags),
-            "-DDACE_XILINX_MODE={}".format(mode),
-            "-DDACE_XILINX_TARGET_PLATFORM=\"{}\"".format(target_platform),
-            "-DDACE_XILINX_ENABLE_DEBUGGING={}".format(enable_debugging),
-        ]
-        return options
-
     def generate_state(self, sdfg, state, function_stream, callsite_stream):
-        """ Generate a kernel that runs all connected components within a state
-            as concurrent dataflow modules. """
+        """Generate a kernel that runs all connected components within a state
+           as concurrent dataflow modules."""
 
         state_id = sdfg.node_id(state)
 
         # Determine independent components
         subgraphs = dace.sdfg.concurrent_subgraphs(state)
 
         # Generate kernel code
@@ -187,16 +160,16 @@
                                                      node, function_stream,
                                                      callsite_stream)
             self.generate_nested_state(sdfg, state, state.label, subgraphs,
                                        function_stream, callsite_stream)
 
     @staticmethod
     def shared_data(subgraphs):
-        """ Returns a set of data objects that are shared between two or more 
-            of the specified subgraphs. """
+        """Returns a set of data objects that are shared between two or more of
+           the specified subgraphs."""
         shared = set()
         if len(subgraphs) >= 2:
             seen = {}
             for sg in subgraphs:
                 for node in sg:
                     if isinstance(node, dace.graph.nodes.AccessNode):
                         if node.data in seen:
@@ -204,46 +177,47 @@
                                 shared.add(node.data)
                         else:
                             seen[node.data] = sg
         return shared
 
     @staticmethod
     def global_transient_nodes(subgraphs):
-        """ Generator that returns all transient global arrays nested in the
-            passed subgraphs on the form (is_output, AccessNode). """
+        """Generator that returns all transient global arrays nested in the
+           passed subgraphs on the form (is_output, AccessNode)"""
         seen = set()
         for subgraph in subgraphs:
             for n, scope in subgraph.all_nodes_recursive():
                 if (isinstance(n, dace.graph.nodes.AccessNode)
                         and n.desc(sdfg).transient and n.desc(sdfg).storage ==
                         dace.dtypes.StorageType.FPGA_Global):
                     if n.data in seen:
                         continue
                     seen.add(n.data)
                     if scope.out_degree(n) > 0:
                         yield (False, n)
                     if scope.in_degree(n) > 0:
                         yield (True, n)
 
-    @staticmethod
-    def make_parameters(sdfg, state, subgraphs):
-        """ Determines the parameters that must be passed to the passed list of
-            subgraphs, as well as to the global kernel. """
+    @classmethod
+    def make_parameters(cls, sdfg, state, subgraphs):
+        """Determines the parameters that must be passed to the passed list of
+           subgraphs, as well as to the global kernel."""
 
         # Get a set of data nodes that are shared across subgraphs
-        shared_data = XilinxCodeGen.shared_data(subgraphs)
+        shared_data = cls.shared_data(subgraphs)
 
         # For some reason the array allocation dispatcher takes nodes, not
         # arrays. Build a dictionary of arrays to arbitrary data nodes
         # referring to them.
         data_to_node = {}
 
-        global_data_params = []
+        global_data_parameters = []
+        global_data_names = set()
         top_level_local_data = []
-        subgraph_params = collections.OrderedDict()  # {subgraph: [params]}
+        subgraph_parameters = collections.OrderedDict()  # {subgraph: [params]}
         nested_global_transients = []
         nested_global_transients_seen = set()
         for subgraph in subgraphs:
             data_to_node.update({
                 node.data: node
                 for node in subgraph.nodes()
                 if isinstance(node, dace.graph.nodes.AccessNode)
@@ -274,79 +248,82 @@
                             if (isinstance(n.desc(scope), dace.data.Array)
                                     and n.desc(scope).storage ==
                                     dace.dtypes.StorageType.FPGA_Global and
                                     n.data not in nested_global_transients_seen
                                 ):
                                 nested_global_transients.append(n)
                             nested_global_transients_seen.add(n.data)
-            subgraph_params[subgraph] = []
+            subgraph_parameters[subgraph] = []
             # Differentiate global and local arrays. The former are allocated
             # from the host and passed to the device code, while the latter are
             # (statically) allocated on the device side.
             for is_output, dataname, data in candidates:
                 if (isinstance(data, dace.data.Array)
                         or isinstance(data, dace.data.Scalar)
                         or isinstance(data, dace.data.Stream)):
                     if data.storage == dace.dtypes.StorageType.FPGA_Global:
-                        subgraph_params[subgraph].append((is_output, dataname,
-                                                          data))
+                        subgraph_parameters[subgraph].append((is_output,
+                                                              dataname, data))
                         if is_output:
-                            global_data_params.append((is_output, dataname,
-                                                       data))
+                            global_data_parameters.append((is_output, dataname,
+                                                           data))
                         else:
-                            global_data_params.append((is_output, dataname,
-                                                       data))
+                            global_data_parameters.append((is_output, dataname,
+                                                           data))
+                        global_data_names.add(dataname)
                     elif (data.storage == dace.dtypes.StorageType.FPGA_Local
                           or data.storage ==
                           dace.dtypes.StorageType.FPGA_Registers):
                         if dataname in shared_data:
                             # Only transients shared across multiple components
                             # need to be allocated outside and passed as
                             # parameters
-                            subgraph_params[subgraph].append((is_output,
-                                                              dataname, data))
+                            subgraph_parameters[subgraph].append(
+                                (is_output, dataname, data))
                             # Resolve the data to some corresponding node to be
                             # passed to the allocator
                             top_level_local_data.append(dataname)
                     else:
                         raise ValueError("Unsupported storage type: {}".format(
                             data.storage))
                 else:
                     raise TypeError("Unsupported data type: {}".format(
                         type(data).__name__))
-            subgraph_params[subgraph] = dace.dtypes.deduplicate(
-                subgraph_params[subgraph])
+            subgraph_parameters[subgraph] = dace.dtypes.deduplicate(
+                subgraph_parameters[subgraph])
 
         # Deduplicate
-        global_data_params = dace.dtypes.deduplicate(global_data_params)
+        global_data_parameters = dace.dtypes.deduplicate(
+            global_data_parameters)
         top_level_local_data = dace.dtypes.deduplicate(top_level_local_data)
         top_level_local_data = [data_to_node[n] for n in top_level_local_data]
 
-        # Get scalar parameters
         scalar_parameters = sdfg.scalar_parameters(False)
         symbol_parameters = sdfg.undefined_symbols(False)
 
-        return (global_data_params, top_level_local_data, subgraph_params,
-                scalar_parameters, symbol_parameters, nested_global_transients)
+        return (global_data_parameters, top_level_local_data,
+                subgraph_parameters, scalar_parameters, symbol_parameters,
+                nested_global_transients)
 
     def generate_nested_state(self, sdfg, state, nest_name, subgraphs,
                               function_stream, callsite_stream):
 
         for sg in subgraphs:
-
             self._dispatcher.dispatch_subgraph(
                 sdfg,
                 sg,
                 sdfg.node_id(state),
                 function_stream,
                 callsite_stream,
                 skip_entry_node=False)
 
     @staticmethod
     def detect_memory_widths(subgraphs):
+        # For each memory, checks that all the memlets are consistent (they have the same width).
+        # This allow us to instantiate to generate data paths with a single data size throughout the subgraph.
         stack = []
         for sg in subgraphs:
             stack += [(n, sg) for n in sg.nodes()]
         memory_widths = {}
         seen = set()
         while len(stack) > 0:
             node, graph = stack.pop()
@@ -376,170 +353,14 @@
                             raise dace.codegen.codegen.CodegenError(
                                 "Inconsistent vector length "
                                 "on FPGA for \"{}\": got {}, had {}".format(
                                     node.data, edge.data.veclen,
                                     memory_widths[node.data]))
         return memory_widths
 
-    def generate_kernel(self, sdfg, state, kernel_name, subgraphs,
-                        function_stream, callsite_stream):
-
-        state_id = sdfg.node_id(state)
-
-        (global_data_params, top_level_local_data, subgraph_params,
-         scalar_parameters, symbol_parameters,
-         nested_global_transients) = type(self).make_parameters(
-             sdfg, state, subgraphs)
-
-        # Scalar parameters are never output
-        sc_parameters = [(False, pname, param)
-                         for pname, param in scalar_parameters]
-
-        symbol_params = [
-            v.signature(with_types=True, name=k)
-            for k, v in symbol_parameters.items()
-        ]
-
-        # Inspect the vector length of all memlets leading to each memory, to
-        # make sure that they're consistent, and to allow us to instantiate the
-        # memories as vector types to enable HLS to generate wider data paths.
-        # Since we cannot pass this auxiliary data structure to the allocator,
-        # which is called by the dispatcher, we temporarily store it in the
-        # codegen object.
-        self._memory_widths = XilinxCodeGen.detect_memory_widths(subgraphs)
-
-        # Write host code
-        self.generate_host_code(sdfg, state, kernel_name,
-                                global_data_params + sc_parameters,
-                                symbol_parameters, nested_global_transients,
-                                function_stream, callsite_stream)
-        if self._in_device_code:
-            raise CodegenError("Tried to generate kernel from device code")
-        self._in_device_code = True
-        self._cpu_codegen._packed_types = True
-
-        # Now we write the device code
-        module_stream = CodeIOStream()
-        kernel_stream = CodeIOStream()
-
-        # Write header
-        module_stream.write("#include <dace/xilinx/device.h>\n\n", sdfg)
-        self._frame.generate_fileheader(sdfg, module_stream)
-        module_stream.write("\n", sdfg)
-
-        # Build kernel signature
-        kernel_args = []
-        for is_output, dataname, data in global_data_params:
-            if isinstance(data, dace.data.Array):
-                kernel_args.append("dace::vec<{}, {}> *{}_{}".format(
-                    data.dtype.ctype, self._memory_widths[dataname], dataname,
-                    "out" if is_output else "in"))
-            else:
-                kernel_args.append(
-                    data.signature(with_types=True, name=dataname))
-        kernel_args += ([
-            arg.signature(with_types=True, name=argname)
-            for argname, arg in scalar_parameters
-        ] + symbol_params)
-
-        # Write kernel signature
-        kernel_stream.write(
-            "DACE_EXPORTED void {}({}) {{\n".format(
-                kernel_name, ', '.join(kernel_args)), sdfg, state_id)
-
-        # Insert interface pragmas
-        mapped_args = 0
-        for arg in kernel_args:
-            var_name = re.findall("\w+", arg)[-1]
-            if "*" in arg:
-                kernel_stream.write(
-                    "#pragma HLS INTERFACE m_axi port={} "
-                    "offset=slave bundle=gmem{}".format(var_name, mapped_args),
-                    sdfg, state_id)
-                mapped_args += 1
-
-        for arg in kernel_args + ["return"]:
-            var_name = re.findall("\w+", arg)[-1]
-            kernel_stream.write(
-                "#pragma HLS INTERFACE s_axilite port={} bundle=control".
-                format(var_name))
-
-        # TODO: add special case if there's only one module for niceness
-        kernel_stream.write("\n#pragma HLS DATAFLOW")
-        kernel_stream.write("\nHLSLIB_DATAFLOW_INIT();")
-
-        # Actual kernel code generation
-        self.generate_modules(sdfg, state, kernel_name, subgraphs,
-                              subgraph_params, sc_parameters,
-                              symbol_parameters, top_level_local_data,
-                              function_stream, module_stream, kernel_stream)
-
-        kernel_stream.write("HLSLIB_DATAFLOW_FINALIZE();\n}\n")
-        self._in_device_code = False
-        self._cpu_codegen._packed_types = False
-
-        concatenated_code = (
-            module_stream.getvalue() + kernel_stream.getvalue())
-
-        # Store code strings to be passed to compilation phase
-        self._kernel_codes.append((kernel_name, concatenated_code))
-
-        # Delete the field we've used to pass this dictionary to the memory
-        # allocator
-        del self._memory_widths
-        self._allocated_global_arrays = set()
-
-    def generate_modules(self, sdfg, state, kernel_name, subgraphs, params,
-                         scalar_parameters, symbol_parameters,
-                         top_level_local_data, function_stream, module_stream,
-                         kernel_stream):
-
-        # Emit allocations
-        state_id = sdfg.node_id(state)
-        for node in top_level_local_data:
-            self._dispatcher.dispatch_allocate(sdfg, state, state_id, node,
-                                               module_stream, kernel_stream)
-            self._dispatcher.dispatch_initialize(sdfg, state, state_id, node,
-                                                 module_stream, kernel_stream)
-
-        # Module generation
-        for subgraph in subgraphs:
-            # Traverse to find first tasklets reachable in topological order
-            to_traverse = subgraph.source_nodes()
-            seen = set()
-            while len(to_traverse) > 0:
-                n = to_traverse.pop()
-                if n in seen:
-                    continue
-                seen.add(n)
-                if (not isinstance(n, dace.graph.nodes.Tasklet)
-                        and not isinstance(n, dace.graph.nodes.NestedSDFG)):
-                    for e in subgraph.out_edges(n):
-                        if e.dst not in seen:
-                            to_traverse.append(e.dst)
-            # Name module according to all reached tasklets (can be just one)
-            labels = [
-                n.label.replace(" ", "_") for n in seen
-                if isinstance(n, dace.graph.nodes.Tasklet)
-                or isinstance(n, dace.graph.nodes.NestedSDFG)
-            ]
-            if len(labels) == 0:
-                labels = [
-                    n.label.replace(" ", "_") for n in seen
-                    if isinstance(n, dace.graph.nodes.AccessNode)
-                ]
-            if len(labels) == 0:
-                raise RuntimeError(
-                    "Expected at least one tasklet or data node")
-            module_name = "_".join(labels)
-            self.generate_module(sdfg, state, module_name, subgraph,
-                                 params[subgraph] + scalar_parameters,
-                                 symbol_parameters, function_stream,
-                                 module_stream, kernel_stream)
-
     def generate_scope(self, sdfg, dfg_scope, state_id, function_stream,
                        callsite_stream):
 
         if not self._in_device_code:
             # If we're not already generating kernel code we need to set up the
             # kernel launch
             subgraphs = [dfg_scope]
@@ -556,390 +377,21 @@
             sdfg,
             dfg_scope,
             state_id,
             function_stream,
             callsite_stream,
             skip_entry_node=True)
 
-    def generate_host_code(self, sdfg, state, kernel_name, params,
-                           symbol_parameters, nested_global_transients,
-                           function_stream, callsite_stream):
-
-        state_id = sdfg.node_id(state)
-
-        # We exclude nested transients from the CPU code function call, as they
-        # have not yet been allocated at this point
-        nested_transient_set = {n.data for n in nested_global_transients}
-
-        symbol_sigs = [
-            v.signature(with_types=True, name=k)
-            for k, v in symbol_parameters.items()
-        ]
-        symbol_names = list(symbol_parameters.keys())
-        seen = set(nested_transient_set)
-        kernel_args_call_wrapper = []
-        kernel_args_call_host = []
-        for is_output, pname, p in params:
-            kernel_args_call_wrapper.append(p.signature(False, name=pname))
-            # Only pass each array once from the host code
-            if p in seen:
-                continue
-            seen.add(p)
-            kernel_args_call_host.append(p.signature(False, name=pname))
-        kernel_args_call_wrapper += symbol_names
-        kernel_args_call_host += symbol_names
-        kernel_args_opencl = (XilinxCodeGen.sdaccel_params(
-            sdfg, [p for p in params
-                   if p[1] not in nested_transient_set]) + symbol_sigs)
-        kernel_args_hls = []
-        kernel_args_hls_without_vectorization = []
-        for is_output, argname, arg in params:
-            if isinstance(arg, dace.data.Array):
-                kernel_args_hls.append("dace::vec<{}, {}> *{}_{}".format(
-                    arg.dtype.ctype, self._memory_widths[argname], argname,
-                    "out" if is_output else "in"))
-                kernel_args_hls_without_vectorization.append(
-                    "{} *{}_{}".format(arg.dtype.ctype, argname, "out"
-                                       if is_output else "in"))
-            else:
-                kernel_args_hls.append(
-                    arg.signature(with_types=True, name=argname))
-                kernel_args_hls_without_vectorization.append(
-                    arg.signature(with_types=True, name=argname))
-        kernel_args_hls += symbol_sigs
-        kernel_args_hls_without_vectorization += symbol_sigs
-
-        kernel_function_name = kernel_name
-
-        #----------------------------------------------------------------------
-        # Generate OpenCL host-code
-        #----------------------------------------------------------------------
-
-        kernel_file_name = "{}.xclbin".format(kernel_name)
-        host_function_name = "__dace_runkernel_{}".format(kernel_name)
-
-        # Write OpenCL host function
-        code = CodeIOStream()
-        code.write("""\
-// Signature of kernel function (with raw pointers) for argument matching
-DACE_EXPORTED void {kernel_function_name}({kernel_args_hls_novec});
-
-DACE_EXPORTED void {host_function_name}({kernel_args_opencl}) {{""".format(
-            kernel_function_name=kernel_function_name,
-            kernel_args_hls_novec=", ".join(
-                kernel_args_hls_without_vectorization),
-            host_function_name=host_function_name,
-            kernel_args_opencl=", ".join(kernel_args_opencl)))
-
-        # Any extra transients stored in global memory on the FPGA must now be
-        # allocated and passed to the kernel
-        for arr_node in nested_global_transients:
-            self._dispatcher.dispatch_allocate(sdfg, state, None, arr_node,
-                                               None, code)
-            self._dispatcher.dispatch_initialize(sdfg, state, None, arr_node,
-                                                 None, code)
-
-        code.write("""\
-  hlslib::ocl::Program program =
-      hlslib::ocl::GlobalContext().CurrentlyLoadedProgram();
-  auto kernel = program.MakeKernel({kernel_function_name}, "{kernel_function_name}", {kernel_args});
-  const std::pair<double, double> elapsed = kernel.ExecuteTask();
-  std::cout << "Kernel executed in " << elapsed.second << " seconds.\\n" << std::flush;
-}}""".format(
-            kernel_function_name=kernel_function_name,
-            kernel_args=", ".join(kernel_args_call_wrapper)))
-
-        # Store code to be passed to compilation phase
-        self._host_codes.append((kernel_name, code.getvalue()))
-
-        #----------------------------------------------------------------------
-        # Inject header for OpenCL host code in the calling code file
-        #----------------------------------------------------------------------
-
-        host_declaration = "\n\nDACE_EXPORTED void {}({});\n\n".format(
-            host_function_name, ", ".join(kernel_args_opencl))
-        function_stream.write(host_declaration, sdfg, state_id, None)
-
-        #----------------------------------------------------------------------
-        # Call the OpenCL host function from the callsite
-        #----------------------------------------------------------------------
-
-        callsite_stream.write(
-            "{}({});".format(host_function_name,
-                             ", ".join(kernel_args_call_host)), sdfg, state_id,
-            None)
-
-
-# Unused?
-#    def generate_caller_code(self, sdfg, state, kernel_name, params,
-#                             symbol_parameters, function_stream,
-#                             callsite_stream):
-#
-#        state_id = sdfg.node_id(state)
-#
-#        symbol_sigs = [v.ctype + ' ' + k for k, v in symbol_parameters.items()]
-#        symbol_names = symbol_parameters.keys()
-#        kernel_args_call = [p.signature(False) for p in params] + symbol_names
-#        kernel_args_plain = [i.signature() for i in params] + symbol_sigs
-#
-#        kernel_function_name = kernel_name
-#
-#        callsite_stream.write(
-#            "{}({});".format(kernel_function_name,
-#                             ", ".join(kernel_args_call)), sdfg, state_id,
-#            None)
-
-    def generate_module(self, sdfg, state, name, subgraph, params,
-                        symbol_parameters, function_stream, module_stream,
-                        kernel_stream):
-        """Generates a module that will run as a dataflow function in the FPGA
-           kernel."""
-
-        state_id = sdfg.node_id(state)
-        dfg = sdfg.nodes()[state_id]
-
-        symbol_sigs = [
-            v.signature(with_types=True, name=k)
-            for k, v in symbol_parameters.items()
-        ]
-        symbol_names = list(symbol_parameters.keys())
-        kernel_args_call = []
-        kernel_args_module = []
-        added = set()
-        for is_output, pname, p in params:
-            if isinstance(p, dace.data.Array):
-                arr_name = "{}_{}".format(pname, "out" if is_output else "in")
-                kernel_args_call.append(arr_name)
-                kernel_args_module.append("dace::vec<{}, {}> {}*{}".format(
-                    p.dtype.ctype, self._memory_widths[pname], "const "
-                    if not is_output else "", arr_name))
-            else:
-                # Don't make duplicate arguments for other types than arrays
-                if pname in added:
-                    continue
-                added.add(pname)
-                if isinstance(p, dace.data.Stream):
-                    kernel_args_call.append(
-                        p.signature(with_types=False, name=pname))
-                    if p.is_stream_array():
-                        kernel_args_module.append(
-                            "dace::FIFO<{}, {}, {}> {}[{}]".format(
-                                p.dtype.ctype, p.veclen, p.buffer_size, pname,
-                                p.size_string()))
-                    else:
-                        kernel_args_module.append(
-                            "dace::FIFO<{}, {}, {}> &{}".format(
-                                p.dtype.ctype, p.veclen, p.buffer_size, pname))
-                else:
-                    kernel_args_call.append(
-                        p.signature(with_types=False, name=pname))
-                    kernel_args_module.append(
-                        p.signature(with_types=True, name=pname))
-        kernel_args_call += symbol_names
-        kernel_args_module += symbol_sigs
-
-        module_function_name = "module_" + name
-
-        # Unrolling processing elements: if the first scope of the subgraph
-        # is an unrolled map, generate a processing element for each iteration
-        scope_dict = subgraph.scope_dict(node_to_children=True)
-        top_scopes = [
-            n for n in scope_dict[None]
-            if isinstance(n, dace.graph.nodes.EntryNode)
-        ]
-        unrolled_loops = 0
-        if len(top_scopes) == 1:
-            scope = top_scopes[0]
-            if scope.unroll:
-                self._unrolled_pes.add(scope.map)
-                kernel_args_call += ", ".join(scope.map.params)
-                kernel_args_module += ["int " + p for p in scope.params]
-                for p, r in zip(scope.map.params, scope.map.range):
-                    if len(r) > 3:
-                        raise dace.codegen.codegen.CodegenError(
-                            "Strided unroll not supported")
-                    kernel_stream.write(
-                        "for (int {param} = {begin}; {param} < {end}; "
-                        "{param} += {increment}) {{\n#pragma HLS UNROLL".
-                        format(
-                            param=p, begin=r[0], end=r[1] + 1, increment=r[2]))
-                    unrolled_loops += 1
-
-        # Generate caller code in top-level function
-        kernel_stream.write(
-            "HLSLIB_DATAFLOW_FUNCTION({}, {});".format(
-                module_function_name, ", ".join(kernel_args_call)), sdfg,
-            state_id)
-
-        for _ in range(unrolled_loops):
-            kernel_stream.write("}")
-
-        #----------------------------------------------------------------------
-        # Generate kernel code
-        #----------------------------------------------------------------------
-
-        self._dispatcher.defined_vars.enter_scope(subgraph)
-
-        module_body_stream = CodeIOStream()
-
-        module_body_stream.write(
-            "void {}({}) {{".format(module_function_name,
-                                    ", ".join(kernel_args_module)), sdfg,
-            state_id)
-
-        # Construct ArrayInterface wrappers to pack input and output pointers
-        # to the same global array
-        in_args = {
-            argname
-            for out, argname, arg in params
-            if isinstance(arg, dace.data.Array)
-            and arg.storage == dace.dtypes.StorageType.FPGA_Global and not out
-        }
-        out_args = {
-            argname
-            for out, argname, arg in params
-            if isinstance(arg, dace.data.Array)
-            and arg.storage == dace.dtypes.StorageType.FPGA_Global and out
-        }
-        if len(in_args) > 0 or len(out_args) > 0:
-            # Add ArrayInterface objects to wrap input and output pointers to
-            # the same array
-            module_body_stream.write("\n")
-            interfaces_added = set()
-            for _, argname, arg in params:
-                if argname in interfaces_added:
-                    continue
-                interfaces_added.add(argname)
-                has_in_ptr = argname in in_args
-                has_out_ptr = argname in out_args
-                if not has_in_ptr and not has_out_ptr:
-                    continue
-                in_ptr = ("{}_in".format(argname) if has_in_ptr else "nullptr")
-                out_ptr = ("{}_out".format(argname)
-                           if has_out_ptr else "nullptr")
-                module_body_stream.write(
-                    "dace::ArrayInterface<{}, {}> {}({}, {});".format(
-                        arg.dtype.ctype, self._memory_widths[argname], argname,
-                        in_ptr, out_ptr))
-            module_body_stream.write("\n")
-
-        # Allocate local transients
-        data_to_allocate = (set(subgraph.top_level_transients()) - set(
-            sdfg.shared_transients()) - set([p[1] for p in params]))
-        allocated = set()
-        for node in subgraph.nodes():
-            if not isinstance(node, nodes.AccessNode):
-                continue
-            if node.data not in data_to_allocate or node.data in allocated:
-                continue
-            allocated.add(node.data)
-            self._dispatcher.dispatch_allocate(sdfg, state, state_id, node,
-                                               function_stream,
-                                               module_body_stream)
-            self._dispatcher.dispatch_initialize(sdfg, state, state_id, node,
-                                                 function_stream,
-                                                 module_body_stream)
-
-        self._dispatcher.dispatch_subgraph(
-            sdfg,
-            subgraph,
-            state_id,
-            module_stream,
-            module_body_stream,
-            skip_entry_node=False)
-
-        module_stream.write(module_body_stream.getvalue(), sdfg, state_id)
-        module_stream.write("}\n\n")
-
-        self._dispatcher.defined_vars.exit_scope(subgraph)
-
-    def get_generated_codeobjects(self):
-
-        execution_mode = Config.get("compiler", "xilinx", "mode")
-        sdaccel_dir = os.path.dirname(
-            os.path.dirname(
-                make_absolute(Config.get("compiler", "xilinx", "executable"))))
-        sdaccel_platform = Config.get("compiler", "xilinx", "platform")
-
-        kernel_file_name = "DACE_BINARY_DIR \"{}".format(self._program_name)
-        if execution_mode == "software_emulation":
-            kernel_file_name += "_sw_emu.xclbin\""
-            xcl_emulation_mode = "sw_emu"
-            xilinx_sdx = sdaccel_dir
-        elif execution_mode == "hardware_emulation":
-            kernel_file_name += "_hw_emu.xclbin\""
-            xcl_emulation_mode = "sw_emu"
-            xilinx_sdx = sdaccel_dir
-        elif execution_mode == "hardware" or execution_mode == "simulation":
-            kernel_file_name += "_hw.xclbin\""
-            xcl_emulation_mode = None
-            xilinx_sdx = None
-        else:
-            raise dace.codegen.codegen.CodegenError(
-                "Unknown Xilinx execution mode: {}".format(execution_mode))
-
-        set_env_vars = ""
-        set_str = "dace::set_environment_variable(\"{}\", \"{}\");\n"
-        unset_str = "dace::unset_environment_variable(\"{}\");\n"
-        set_env_vars += (set_str.format("XCL_EMULATION_MODE",
-                                        xcl_emulation_mode)
-                         if xcl_emulation_mode is not None else
-                         unset_str.format("XCL_EMULATION_MODE"))
-        set_env_vars += (set_str.format("XILINX_SDX", xilinx_sdx)
-                         if xilinx_sdx is not None else
-                         unset_str.format("XILINX_SDX"))
-
-        host_code = CodeIOStream()
-        host_code.write("""\
-#include "dace/xilinx/host.h"
-#include "dace/dace.h"
-#include <iostream>\n\n""")
-
-        self._frame.generate_fileheader(self._global_sdfg, host_code)
-
-        host_code.write("""
-DACE_EXPORTED int __dace_init_xilinx({signature}) {{
-    {environment_variables}
-    hlslib::ocl::GlobalContext().MakeProgram({kernel_file_name});
-    return 0;
-}}
-
-{host_code}""".format(
-            signature=self._global_sdfg.signature(),
-            environment_variables=set_env_vars,
-            kernel_file_name=kernel_file_name,
-            host_code="".join([
-                "{separator}\n// Kernel: {kernel_name}"
-                "\n{separator}\n\n{code}\n\n".format(
-                    separator="/" * 79, kernel_name=name, code=code)
-                for (name, code) in self._host_codes
-            ])))
-
-        host_code_obj = CodeObject(self._program_name + "_host",
-                                   host_code.getvalue(), "cpp", XilinxCodeGen,
-                                   "Xilinx")
-
-        kernel_code_objs = [
-            CodeObject("kernel_" + kernel_name, code, "cpp", XilinxCodeGen,
-                       "Xilinx") for (kernel_name, code) in self._kernel_codes
-        ]
-
-        return [host_code_obj] + kernel_code_objs
-
     def allocate_array(self, sdfg, dfg, state_id, node, function_stream,
                        callsite_stream):
         result = StringIO()
         nodedesc = node.desc(sdfg)
-        arrsize = " * ".join([
-            cppunparse.pyexpr2cpp(dace.symbolic.symstr(s))
-            for s in nodedesc.strides
-        ])
-        is_dynamically_sized = any(
-            dace.symbolic.issymbolic(s, sdfg.constants)
-            for s in nodedesc.strides)
+        arrsize = nodedesc.total_size
+        is_dynamically_sized = dace.symbolic.issymbolic(
+            arrsize, sdfg.constants)
 
         dataname = node.data
 
         if isinstance(nodedesc, dace.data.Stream):
 
             if not self._in_device_code:
                 raise dace.codegen.codegen.CodegenError(
@@ -949,41 +401,34 @@
                 raise dace.codegen.codegen.CodegenError(
                     "Arrays of streams cannot have dynamic size on FPGA")
 
             if nodedesc.buffer_size < 1:
                 raise dace.codegen.codegen.CodegenError(
                     "Streams cannot be unbounded on FPGA")
 
-            buffer_length_dynamically_sized = (
-                isinstance(nodedesc.buffer_size, sp.Expr)
-                and len(nodedesc.free_symbols) > 0)
+            buffer_length_dynamically_sized = (dace.symbolic.issymbolic(
+                nodedesc.buffer_size, sdfg.constants))
 
             if buffer_length_dynamically_sized:
                 raise dace.codegen.codegen.CodegenError(
                     "Buffer length of stream cannot have dynamic size on FPGA")
 
-            if arrsize != "1":
-                is_stream_array = True
-            else:
-                is_stream_array = False
-
-            if is_stream_array:
-                result.write("dace::FIFO<{}, {}, {}> {}[{}];\n".format(
-                    nodedesc.dtype.ctype, nodedesc.veclen,
-                    nodedesc.buffer_size, dataname, arrsize))
-                result.write("dace::SetNames({}, \"{}\", {});".format(
-                    dataname, dataname, arrsize))
+            if cpu.sym2cpp(arrsize) != "1":
+                # Is a stream array
                 self._dispatcher.defined_vars.add(dataname,
                                                   DefinedType.StreamArray)
             else:
-                result.write("dace::FIFO<{}, {}, {}> {}(\"{}\");".format(
-                    nodedesc.dtype.ctype, nodedesc.veclen,
-                    nodedesc.buffer_size, dataname, dataname))
+                # Single stream
                 self._dispatcher.defined_vars.add(dataname, DefinedType.Stream)
 
+            # Language-specific implementation
+            self.define_stream(nodedesc.dtype, nodedesc.veclen,
+                               nodedesc.buffer_size, dataname, arrsize,
+                               function_stream, result)
+
         elif isinstance(nodedesc, dace.data.Array):
 
             if nodedesc.storage == dace.dtypes.StorageType.FPGA_Global:
 
                 if self._in_device_code:
 
                     if nodedesc not in self._allocated_global_arrays:
@@ -991,23 +436,22 @@
                                            "from device code: {} in {}".format(
                                                node.label, sdfg.name))
 
                 else:
 
                     devptr_name = dataname
                     if isinstance(nodedesc, dace.data.Array):
-                        # TODO: Distinguish between read, write, and
-                        #       read+write
-                        # TODO: Handle memory banks (location?)
+                        # TODO: Distinguish between read, write, and read+write
+                        # TODO: Handle memory banks
                         self._allocated_global_arrays.add(node.data)
                         result.write(
                             "auto {} = hlslib::ocl::GlobalContext()."
                             "MakeBuffer<{}, hlslib::ocl::Access::readWrite>"
                             "({});".format(dataname, nodedesc.dtype.ctype,
-                                           arrsize))
+                                           cpu.sym2cpp(arrsize)))
                         self._dispatcher.defined_vars.add(
                             dataname, DefinedType.Pointer)
 
             elif (nodedesc.storage == dace.dtypes.StorageType.FPGA_Local or
                   nodedesc.storage == dace.dtypes.StorageType.FPGA_Registers):
 
                 if not self._in_device_code:
@@ -1019,51 +463,46 @@
                         "Dynamic allocation of FPGA fast memory not allowed")
 
                 # Absorb vector size into type and adjust array size
                 # accordingly
                 veclen = self._memory_widths[node.data]
                 generate_scalar = False
                 if veclen > 1:
-                    arrsize_symbolic = functools.reduce(
-                        sp.mul.Mul, nodedesc.strides)
+                    arrsize_symbolic = nodedesc.total_size
                     arrsize_eval = dace.symbolic.eval(
                         arrsize_symbolic / veclen)
                     if cpu.sym2cpp(arrsize_eval) == "1":
                         generate_scalar = True
                     arrsize_vec = "({}) / {}".format(arrsize, veclen)
                 else:
                     arrsize_vec = arrsize
 
                 # If the array degenerates to a single element because of
                 # vectorization, generate the variable as a scalar instead of
                 # an array of size 1
                 if generate_scalar:
-                    result.write("dace::vec<{}, {}> {};\n".format(
-                        nodedesc.dtype.ctype, veclen, dataname))
+                    # Language-specific
+                    define_str = "{} {};".format(
+                        self.make_vector_type(nodedesc.dtype, veclen, False),
+                        dataname)
+                    callsite_stream.write(define_str, sdfg, state_id, node)
                     self._dispatcher.defined_vars.add(dataname,
                                                       DefinedType.Scalar)
                 else:
-                    result.write("dace::vec<{}, {}> {}[{}];\n".format(
-                        nodedesc.dtype.ctype, veclen, dataname, arrsize_vec))
+                    # Language-specific
+                    self.define_local_array(nodedesc.dtype, veclen, dataname,
+                                            arrsize_vec, nodedesc.storage,
+                                            nodedesc.shape, function_stream,
+                                            result, sdfg, state_id, node)
                     self._dispatcher.defined_vars.add(dataname,
                                                       DefinedType.Pointer)
-                    if nodedesc.storage == dace.dtypes.StorageType.FPGA_Registers:
-                        result.write("#pragma HLS ARRAY_PARTITION variable={} "
-                                     "complete\n".format(dataname))
-                    elif len(nodedesc.shape) > 1:
-                        result.write("#pragma HLS ARRAY_PARTITION variable={} "
-                                     "block factor={}\n".format(
-                                         dataname, nodedesc.shape[-2]))
-                    # result.write(
-                    #     "#pragma HLS DEPENDENCE variable={} false".format(
-                    #         dataname))
 
             else:
-                raise NotImplementedError("Xilinx: Unimplemented storage type "
-                                          + str(nodedesc.storage))
+                raise NotImplementedError("Unimplemented storage type " +
+                                          str(nodedesc.storage))
 
         elif isinstance(nodedesc, dace.data.Scalar):
 
             result.write("{} {};\n".format(nodedesc.dtype.ctype, dataname))
             self._dispatcher.defined_vars.add(dataname, DefinedType.Scalar)
 
         else:
@@ -1089,25 +528,27 @@
         fpga_storage_types = [
             dace.dtypes.StorageType.FPGA_Global,
             dace.dtypes.StorageType.FPGA_Local,
             dace.dtypes.StorageType.FPGA_Registers,
         ]
 
         # Determine directionality
-        if isinstance(src_node,
-                      nodes.AccessNode) and memlet.data == src_node.data:
+        if isinstance(
+                src_node,
+                dace.graph.nodes.AccessNode) and memlet.data == src_node.data:
             outgoing_memlet = True
-        elif isinstance(dst_node,
-                        nodes.AccessNode) and memlet.data == dst_node.data:
+        elif isinstance(
+                dst_node,
+                dace.graph.nodes.AccessNode) and memlet.data == dst_node.data:
             outgoing_memlet = False
         else:
             raise LookupError("Memlet does not point to any of the nodes")
 
-        data_to_data = (isinstance(src_node, nodes.AccessNode)
-                        and isinstance(dst_node, nodes.AccessNode))
+        data_to_data = (isinstance(src_node, dace.graph.nodes.AccessNode)
+                        and isinstance(dst_node, dace.graph.nodes.AccessNode))
 
         host_to_device = (data_to_data and src_storage in cpu_storage_types and
                           dst_storage == dace.dtypes.StorageType.FPGA_Global)
         device_to_host = (data_to_data and
                           src_storage == dace.dtypes.StorageType.FPGA_Global
                           and dst_storage in cpu_storage_types)
         device_to_device = (
@@ -1129,15 +570,15 @@
             ])
             offset = cpp_array_expr(sdfg, memlet, with_brackets=False)
 
             if (not sum(copy_shape) == 1
                     and (not isinstance(memlet.subset, subsets.Range)
                          or any([step != 1 for _, _, step in memlet.subset]))):
                 raise NotImplementedError("Only contiguous copies currently "
-                                          "supported for Xilinx FPGA.")
+                                          "supported for FPGA codegen.")
 
             if host_to_device:
 
                 callsite_stream.write(
                     "{}.CopyFromHost({}, {}, {});".format(
                         dst_node.data, (offset if not outgoing_memlet else 0),
                         copysize,
@@ -1191,110 +632,154 @@
 
             # TODO: detect in which cases we shouldn't unroll
             register_to_register = (src_node.desc(
                 sdfg).storage == dace.dtypes.StorageType.FPGA_Registers
                                     or dst_node.desc(sdfg).storage ==
                                     dace.dtypes.StorageType.FPGA_Registers)
 
+            num_loops = len([dim for dim in copy_shape if dim != 1])
+            if num_loops > 0:
+                if not register_to_register:
+                    # Language-specific
+                    self.generate_pipeline_loop_pre(callsite_stream, sdfg,
+                                                    state_id, dst_node)
+                if len(copy_shape) > 1:
+                    # Language-specific
+                    self.generate_flatten_loop_pre(callsite_stream, sdfg,
+                                                   state_id, dst_node)
+                for node in [src_node, dst_node]:
+                    if (isinstance(node.desc(sdfg), dace.data.Array)
+                            and node.desc(sdfg).storage in [
+                                dace.dtypes.StorageType.FPGA_Local,
+                                dace.StorageType.FPGA_Registers
+                            ]):
+                        # Language-specific
+                        self.generate_no_dependence_pre(
+                            node.data, callsite_stream, sdfg, state_id,
+                            dst_node)
+
             # Loop intro
-            num_loops = 0
             for i, copy_dim in enumerate(copy_shape):
                 if copy_dim != 1:
+                    if register_to_register:
+                        # Language-specific
+                        self.generate_unroll_loop_pre(callsite_stream, None,
+                                                      sdfg, state_id, dst_node)
                     callsite_stream.write(
-                        "for (auto __dace_copy{} = 0; __dace_copy{} < {}; "
-                        "++__dace_copy{}) {{".format(i, i, copy_dim, i))
+                        "for (int __dace_copy{} = 0; __dace_copy{} < {}; "
+                        "++__dace_copy{}) {{".format(i, i, copy_dim, i), sdfg,
+                        state_id, dst_node)
                     if register_to_register:
-                        callsite_stream.write("#pragma HLS UNROLL")
-                    num_loops += 1
+                        # Language-specific
+                        self.generate_unroll_loop_post(
+                            callsite_stream, None, sdfg, state_id, dst_node)
 
             # Pragmas
             if num_loops > 0:
                 if not register_to_register:
-                    callsite_stream.write("#pragma HLS PIPELINE II=1")
+                    # Language-specific
+                    self.generate_pipeline_loop_post(callsite_stream, sdfg,
+                                                     state_id, dst_node)
                 if len(copy_shape) > 1:
-                    callsite_stream.write("#pragma HLS LOOP_FLATTEN")
+                    # Language-specific
+                    self.generate_flatten_loop_post(callsite_stream, sdfg,
+                                                    state_id, dst_node)
 
             # Construct indices (if the length of the stride array is zero,
             # resolves to an empty string)
-            src_index = " + ".join(([""] if len(dst_strides) > 0 else []) + [
+            src_index = " + ".join([
                 "__dace_copy{} * {}".format(i, cpu.sym2cpp(stride))
                 for i, stride in enumerate(src_strides) if copy_shape[i] != 1
             ])
-            dst_index = " + ".join(([""] if len(dst_strides) > 0 else []) + [
+            dst_index = " + ".join([
                 "__dace_copy{} * {}".format(i, cpu.sym2cpp(stride))
                 for i, stride in enumerate(dst_strides) if copy_shape[i] != 1
             ])
 
             src_def_type = self._dispatcher.defined_vars.get(src_node.data)
             dst_def_type = self._dispatcher.defined_vars.get(dst_node.data)
 
-            if src_def_type == DefinedType.Stream:
-                read_expr = src_expr
-            elif src_def_type == DefinedType.Scalar:
-                read_expr = src_node.label
-            else:
-                read_expr = "dace::Read<{}, {}>({}{})".format(
-                    ctype, memlet.veclen, src_expr, src_index)
+            pattern = re.compile("([^\s]+)(\s*\+\s*)?(.*)")
 
-            if dst_def_type == DefinedType.Stream:
-                callsite_stream.write("{}.push({});".format(
-                    dst_expr, read_expr))
-            else:
-                if dst_def_type == DefinedType.Scalar:
-                    write_expr = dst_node.label
-                callsite_stream.write("dace::Write<{}, {}>({}{}, {});".format(
-                    ctype, memlet.veclen, dst_expr, dst_index, read_expr))
+            def sanitize_index(expr, index):
+                var_name, _, expr_index = re.match(pattern, expr).groups()
+                index = index.strip()
+                expr_index = expr_index.strip()
+                if index:
+                    if expr_index:
+                        return var_name, index + " + " + expr_index
+                    return var_name, index
+                else:
+                    if expr_index:
+                        return var_name, expr_index
+                    return var_name, "0"
+
+            # Pull out indices from expressions
+            src_expr, src_index = sanitize_index(src_expr, src_index)
+            dst_expr, dst_index = sanitize_index(dst_expr, dst_index)
+
+            # Language specific
+            read_expr = self.make_read(src_def_type, ctype, src_node.label,
+                                       memlet.veclen, src_expr, src_index)
+
+            # Language specific
+            write_expr = self.make_write(dst_def_type, ctype, dst_node.label,
+                                         memlet.veclen, dst_expr, dst_index,
+                                         read_expr, memlet.wcr)
 
-            # Inject dependence pragmas (DaCe semantics implies no conflict)
+            callsite_stream.write(write_expr)
+
+            # Inject dependence pragmas (DACE semantics implies no conflict)
             for node in [src_node, dst_node]:
                 if (isinstance(node.desc(sdfg), dace.data.Array)
                         and node.desc(sdfg).storage in [
                             dace.dtypes.StorageType.FPGA_Local,
                             dace.StorageType.FPGA_Registers
                         ]):
-                    callsite_stream.write(
-                        "#pragma HLS DEPENDENCE variable={} false".format(
-                            node.data))
+                    # Language-specific
+                    self.generate_no_dependence_post(
+                        node.data, callsite_stream, sdfg, state_id, dst_node)
 
             # Loop outtro
             for _ in range(num_loops):
                 callsite_stream.write("}")
 
         else:
 
-            self._cpu_codegen.copy_memory(sdfg, dfg, state_id, src_node,
-                                          dst_node, edge, None,
-                                          callsite_stream)
+            self.generate_memlet_definition(sdfg, dfg, state_id, src_node,
+                                            dst_node, edge, callsite_stream)
 
     @staticmethod
-    def sdaccel_params(sdfg, kernel_params):
+    def opencl_parameters(sdfg, kernel_parameters):
         seen = set()
-        out_params = []
-        for is_output, pname, param in kernel_params:
+        out_parameters = []
+        for is_output, pname, param in kernel_parameters:
             # Since we can have both input and output versions of the same
             # array, make sure we only pass it once from the host code
             if param in seen:
                 continue
             seen.add(param)
             if isinstance(param, dace.data.Array):
-                out_params.append("hlslib::ocl::Buffer<{}, "
-                                  "hlslib::ocl::Access::readWrite> &{}".format(
-                                      param.dtype.ctype, pname))
+                out_parameters.append(
+                    "hlslib::ocl::Buffer<{}, "
+                    "hlslib::ocl::Access::readWrite> &{}".format(
+                        param.dtype.ctype, pname))
             else:
-                out_params.append(param.signature(with_types=True, name=pname))
-        return out_params
+                out_parameters.append(
+                    param.signature(with_types=True, name=pname))
+        return out_parameters
 
     def get_next_scope_entries(self, sdfg, dfg, scope_entry):
         parent_scope_entry = dfg.scope_dict()[scope_entry]
         parent_scope = dfg.scope_subgraph(parent_scope_entry)
 
         # Get all scopes from the same level
         all_scopes = [
             node for node in parent_scope.topological_sort()
-            if isinstance(node, nodes.EntryNode)
+            if isinstance(node, dace.graph.nodes.EntryNode)
         ]
 
         return all_scopes[all_scopes.index(scope_entry) + 1:]
 
     def generate_node(self, sdfg, dfg, state_id, node, function_stream,
                       callsite_stream):
         method_name = "_generate_" + type(node).__name__
@@ -1321,26 +806,26 @@
 
     def initialize_array(self, *args, **kwargs):
         pass
 
     def copy_memory(self, sdfg, dfg, state_id, src_node, dst_node, edge,
                     function_stream, callsite_stream):
 
-        if isinstance(src_node, nodes.Tasklet):
+        if isinstance(src_node, dace.graph.nodes.CodeNode):
             src_storage = dace.dtypes.StorageType.Register
             try:
                 src_parent = dfg.scope_dict()[src_node]
             except KeyError:
                 src_parent = None
             dst_schedule = (None
                             if src_parent is None else src_parent.map.schedule)
         else:
             src_storage = src_node.desc(sdfg).storage
 
-        if isinstance(dst_node, nodes.Tasklet):
+        if isinstance(dst_node, dace.graph.nodes.CodeNode):
             dst_storage = dace.dtypes.StorageType.Register
         else:
             dst_storage = dst_node.desc(sdfg).storage
 
         try:
             dst_parent = dfg.scope_dict()[dst_node]
         except KeyError:
@@ -1350,78 +835,164 @@
         state_dfg = sdfg.nodes()[state_id]
 
         # Emit actual copy
         self._emit_copy(sdfg, state_id, src_node, src_storage, dst_node,
                         dst_storage, dst_schedule, edge, state_dfg,
                         callsite_stream)
 
+    def _generate_PipelineEntry(self, *args, **kwargs):
+        self._generate_MapEntry(*args, **kwargs)
+
     def _generate_MapEntry(self, sdfg, dfg, state_id, node, function_stream,
                            callsite_stream):
 
         result = callsite_stream
 
         scope_dict = dfg.scope_dict()
-
         if node.map in self._unrolled_pes:
 
             # This is a top-level unrolled map, meaning it has been used to
             # replicate processing elements. Don't generate anything here.
             pass
 
         else:
-
-            # Generate nested loops
-            for i, r in enumerate(node.map.range):
-                var = node.map.params[i]
-                begin, end, skip = r
-                result.write(
-                    "for (auto {} = {}; {} < {}; {} += {}) {{\n".format(
-                        var, cpu.sym2cpp(begin), var, cpu.sym2cpp(end + 1),
-                        var, cpu.sym2cpp(skip)), sdfg, state_id, node)
+            # Add extra opening brace (dynamic map ranges, closed in MapExit
+            # generator)
+            callsite_stream.write('{', sdfg, state_id, node)
 
             # Pipeline innermost loops
             scope = dfg.scope_dict(True)[node]
 
+            # Generate custom iterators if this is a pipelined (and thus
+            # flattened) loop
+            if isinstance(node, PipelineEntry):
+                for i in range(len(node.map.range)):
+                    result.write("long {} = {};\n".format(
+                        node.map.params[i], node.map.range[i][0]))
+
             if node.map.unroll:
-                result.write("#pragma HLS UNROLL\n", sdfg, state_id, node)
+                self.generate_unroll_loop_pre(result, None, sdfg, state_id,
+                                              node)
             else:
                 is_innermost = not any(
-                    [isinstance(x, nodes.EntryNode) for x in scope])
+                    [isinstance(x, dace.graph.nodes.EntryNode) for x in scope])
                 if is_innermost:
+                    self.generate_pipeline_loop_pre(result, sdfg, state_id,
+                                                    node)
+                    self.generate_flatten_loop_pre(result, sdfg, state_id,
+                                                   node)
+
+            # Generate nested loops
+            if not isinstance(node, PipelineEntry):
+                for i, r in enumerate(node.map.range):
+                    var = node.map.params[i]
+                    begin, end, skip = r
+                    # decide type of loop variable
+                    loop_var_type = "int"
+                    # try to decide type of loop variable
+                    try:
+                        if dace.symbolic.eval(
+                                begin) >= 0 and dace.symbolic.eval(skip) > 0:
+                            # it could be an unsigned (uint32) variable: we need to check to the type of 'end',
+                            # if we are able to determine it
+                            end_type = dace.symbolic.symbol.s_types.get(
+                                cpu.sym2cpp(end + 1))
+                            if end_type is not None:
+                                if np.dtype(end_type.dtype.type) > np.dtype(
+                                        'uint32'):
+                                    loop_var_type = end.ctype
+                                elif np.issubdtype(
+                                        np.dtype(end_type.dtype.type),
+                                        np.unsignedinteger):
+                                    loop_var_type = "size_t"
+                    except UnboundLocalError:
+                        pass
+
                     result.write(
-                        "#pragma HLS PIPELINE II=1\n#pragma HLS LOOP_FLATTEN",
+                        "for ({} {} = {}; {} < {}; {} += {}) {{\n".format(
+                            loop_var_type, var, cpu.sym2cpp(begin), var,
+                            cpu.sym2cpp(end + 1), var, cpu.sym2cpp(skip)),
                         sdfg, state_id, node)
+            else:
+                pipeline = node.pipeline
+                flat_it = pipeline.iterator_str()
+                bound = pipeline.loop_bound_str()
+                result.write(
+                    "for (long {it} = 0; {it} < {bound}; ++{it}) {{\n".format(
+                        it=flat_it, bound=node.pipeline.loop_bound_str()))
+                if pipeline.init_size > 0:
+                    result.write("const bool {} = {} < {};\n".format(
+                        node.pipeline.init_condition(), flat_it,
+                        cpu.sym2cpp(pipeline.init_size)))
+                if pipeline.drain_size > 0:
+                    result.write("const bool {} = {} >= {};\n".format(
+                        node.pipeline.drain_condition(), flat_it,
+                        bound + (" - " + cpu.sym2cpp(pipeline.drain_size)
+                                 if pipeline.drain_size != 0 else "")))
 
-            if node.map.flatten:
-                result.write("#pragma HLS LOOP_FLATTEN\n", sdfg, state_id,
-                             node)
+            if node.map.unroll:
+                self.generate_unroll_loop_post(result, None, sdfg, state_id,
+                                               node)
+            else:
+                is_innermost = not any(
+                    [isinstance(x, dace.graph.nodes.EntryNode) for x in scope])
+                if is_innermost:
+                    self.generate_pipeline_loop_post(result, sdfg, state_id,
+                                                     node)
+                    self.generate_flatten_loop_post(result, sdfg, state_id,
+                                                    node)
 
         # Emit internal transient array allocation
         to_allocate = dace.sdfg.local_transients(
             sdfg, sdfg.find_state(state_id), node)
         allocated = set()
         for child in dfg.scope_dict(node_to_children=True)[node]:
-            if not isinstance(child, nodes.AccessNode):
+            if not isinstance(child, dace.graph.nodes.AccessNode):
                 continue
             if child.data not in to_allocate or child.data in allocated:
                 continue
             allocated.add(child.data)
             self._dispatcher.dispatch_allocate(sdfg, dfg, state_id, child,
                                                None, result)
             self._dispatcher.dispatch_initialize(sdfg, dfg, state_id, child,
                                                  None, result)
 
+    def _generate_PipelineExit(self, *args, **kwargs):
+        self._generate_MapExit(*args, **kwargs)
+
     def _generate_MapExit(self, sdfg, dfg, state_id, node, function_stream,
                           callsite_stream):
         scope_dict = dfg.scope_dict()
         entry_node = scope_dict[node]
         if entry_node.map in self._unrolled_pes:
             # This was generated as unrolled processing elements, no need to
             # generate anything here
             return
+        if isinstance(node, PipelineExit):
+            flat_it = node.pipeline.iterator_str()
+            bound = node.pipeline.loop_bound_str()
+            pipeline = node.pipeline
+            cond = []
+            if pipeline.init_size > 0 and pipeline.init_overlap == False:
+                cond.append("!" + pipeline.init_condition())
+            if pipeline.drain_size > 0 and pipeline.drain_overlap == False:
+                cond.append("!" + pipeline.drain_condition())
+            if len(cond) > 0:
+                callsite_stream.write("if ({}) {{".format(" && ".join(cond)))
+            for it, r in reversed(list(zip(pipeline.params, pipeline.range))):
+                callsite_stream.write(
+                    "if ({it} >= {end}) {{\n{it} = {begin};\n".format(
+                        it=it, begin=r[0], end=r[1]))
+            for it, r in zip(pipeline.params, pipeline.range):
+                callsite_stream.write(
+                    "}} else {{\n{it} += {step};\n}}\n".format(
+                        it=it, step=r[2]))
+            if len(cond) > 0:
+                callsite_stream.write("}\n")
+
         self._cpu_codegen._generate_MapExit(sdfg, dfg, state_id, node,
                                             function_stream, callsite_stream)
 
     def _generate_Reduce(self, sdfg, dfg, state_id, node, function_stream,
                          callsite_stream):
 
         end_braces = 0
@@ -1429,16 +1000,16 @@
         axes = node.axes
         input_memlet = dfg.in_edges(node)[0].data
         src_data = sdfg.arrays[input_memlet.data]
         output_edge = dfg.out_edges(node)[0]
         output_memlet = output_edge.data
         dst_data = sdfg.arrays[output_memlet.data]
 
-        output_type = 'dace::vec<%s, %s>' % (dst_data.dtype.ctype,
-                                             output_memlet.veclen)
+        output_type = self.make_vector_type(dst_data.dtype,
+                                            output_memlet.veclen, False)
 
         # If axes were not defined, use all input dimensions
         input_dims = input_memlet.subset.dims()
         output_dims = output_memlet.subset.data_dims()
         if axes is None:
             axes = tuple(range(input_dims))
         output_axes = [a for a in range(input_dims) if a not in axes]
@@ -1469,216 +1040,340 @@
                 pipeline_dim = i
 
         if node.identity is not None:
             identity = cpu.sym2cpp(node.identity)
         else:
             identity = None
 
+        # Determine reduction type
+        reduction_type = operations.detect_reduction_type(node.wcr)
+        if reduction_type == dace.dtypes.ReductionType.Custom:
+            raise NotImplementedError("Custom reduction for FPGA is NYI")
+
         # Initialize accumulator variable if we're collapsing to a single value
         all_axes_collapsed = (len(axes) == input_dims)
         if all_axes_collapsed:
             accumulator = "_{}_accumulator".format(output_memlet.data)
-            callsite_stream.write("{} {};".format(output_type, accumulator),
-                                  sdfg, state_id, node)
+            init_value = ""
+            if identity is not None:
+                init_value = " = " + identity
+            elif reduction_type == dace.dtypes.ReductionType.Sum:
+                # Set initial value to zero. Helpful for single cycle clock accumulator in Intel.
+                init_value = " = 0"
+            callsite_stream.write(
+                "{} {}{};".format(output_type, accumulator, init_value), sdfg,
+                state_id, node)
 
         # Generate inner loops (for each collapsed dimension)
         input_subset = input_memlet.subset
         iterators_inner = ["__i{}".format(axis) for axis in axes]
         for i, axis in enumerate(axes):
+            if axis == pipeline_dim:
+                self.generate_pipeline_loop_pre(callsite_stream, sdfg,
+                                                state_id, node)
+                self.generate_flatten_loop_pre(callsite_stream, sdfg, state_id,
+                                               node)
+            if unroll_dim[axis]:
+                self.generate_unroll_loop_pre(callsite_stream, None, sdfg,
+                                              state_id, node)
             callsite_stream.write(
-                'for (int {var} = {begin}; {var} < {end}; {var} += {skip}) {{'.
-                format(
+                'for (size_t {var} = {begin}; {var} < {end}; {var} += {skip}) {{'
+                .format(
                     var=iterators_inner[i],
                     begin=input_subset[axis][0],
                     end=input_subset[axis][1] + 1,
                     skip=input_subset[axis][2]), sdfg, state_id, node)
-            if unroll_dim[axis]:
-                callsite_stream.write("#pragma HLS UNROLL\n")
             if axis == pipeline_dim:
-                callsite_stream.write(
-                    "#pragma HLS PIPELINE II=1\n#pragma HLS LOOP_FLATTEN")
+                self.generate_pipeline_loop_post(callsite_stream, sdfg,
+                                                 state_id, node)
+                self.generate_flatten_loop_post(callsite_stream, sdfg,
+                                                state_id, node)
+            if unroll_dim[axis]:
+                self.generate_unroll_loop_post(callsite_stream, None, sdfg,
+                                               state_id, node)
             end_braces += 1
 
         # Generate outer loops (over different output locations)
         output_subset = output_memlet.subset
         iterators_outer = ["__o{}".format(axis) for axis in range(output_dims)]
         for i, axis in enumerate(output_axes):
+            if axis == pipeline_dim:
+                self.generate_pipeline_loop_pre(callsite_stream, sdfg,
+                                                state_id, node)
+                self.generate_flatten_loop_pre(callsite_stream, sdfg, state_id,
+                                               node)
+            if unroll_dim[axis]:
+                self.generate_unroll_loop_pre(callsite_stream, None, sdfg,
+                                              state_id, node)
             callsite_stream.write(
-                'for (int {var} = {begin}; {var} < {end}; {var} += {skip}) {{'.
-                format(
+                'for (size_t {var} = {begin}; {var} < {end}; {var} += {skip}) {{'
+                .format(
                     var=iterators_outer[i],
                     begin=output_subset[i][0],
                     end=output_subset[i][1] + 1,
                     skip=output_subset[i][2]), sdfg, state_id, node)
-            if unroll_dim[axis]:
-                callsite_stream.write("#pragma HLS UNROLL\n")
             if axis == pipeline_dim:
-                callsite_stream.write(
-                    "#pragma HLS PIPELINE II=1\n#pragma HLS LOOP_FLATTEN")
+                self.generate_pipeline_loop_post(callsite_stream, sdfg,
+                                                 state_id, node)
+                self.generate_flatten_loop_post(callsite_stream, sdfg,
+                                                state_id, node)
+            if unroll_dim[axis]:
+                self.generate_unroll_loop_post(callsite_stream, None, sdfg,
+                                               state_id, node)
             end_braces += 1
 
-        # Determine reduction type
-        reduction_type = operations.detect_reduction_type(node.wcr)
-        if reduction_type == dace.dtypes.ReductionType.Custom:
-            raise NotImplementedError("Custom reduction for FPGA is NYI")
-
         # Input and output variables
         out_var = (accumulator
                    if all_axes_collapsed else cpp_array_expr(
                        sdfg,
                        output_memlet,
                        offset=iterators_outer,
                        relative_offset=False))
         in_var = cpp_array_expr(
             sdfg, input_memlet, offset=axis_vars, relative_offset=False)
 
-        # Call library function to perform reduction
-        reduction_cpp = "dace::Reduce<{}, {}, {}, {}<{}>>".format(
-            dst_data.dtype.ctype, input_memlet.veclen, output_memlet.veclen,
-            REDUCTION_TYPE_TO_HLSLIB[reduction_type], dst_data.dtype.ctype)
-
-        # Check if this is the first iteration of accumulating into this
-        # location
-        is_first_iteration = " && ".join([
-            "{} == {}".format(iterators_inner[i], input_subset[axis][0])
-            for i, axis in enumerate(axes)
-        ])
-        if identity is not None:
-            # If this is the first iteration, set the previous value to be
-            # identity, otherwise read the value from the output location
-            prev_var = "{}_prev".format(output_memlet.data)
-            callsite_stream.write(
-                "{} {} = ({}) ? ({}) : ({});".format(
-                    output_type, prev_var, is_first_iteration, identity,
-                    out_var), sdfg, state_id, node)
-            callsite_stream.write(
-                "{} = {}({}, {});".format(out_var, reduction_cpp, prev_var,
-                                          in_var), sdfg, state_id, node)
-        else:
-            # If this is the first iteration, assign the value read from the
-            # input directly to the output
-            callsite_stream.write(
-                "{} = ({}) ? ({}) : {}({}, {});".format(
-                    out_var, is_first_iteration, in_var, reduction_cpp,
-                    out_var, in_var), sdfg, state_id, node)
+        # generate reduction code
+
+        self.make_reduction(sdfg, state_id, node, output_memlet,
+                            dst_data.dtype, input_memlet.veclen,
+                            output_memlet.veclen, output_type, reduction_type,
+                            callsite_stream, iterators_inner, input_subset,
+                            identity, out_var, in_var)
 
         # Generate closing braces
         for i in range(end_braces):
             callsite_stream.write('}', sdfg, state_id, node)
-            if i == end_braces - 1 and all_axes_collapsed:
-                dst_expr = output_memlet.data
-                offset = cpp_offset_expr(
-                    dst_data,
-                    output_memlet.subset,
-                    packed_veclen=output_memlet.veclen)
-                if offset:
-                    dst_expr += " + " + offset
-                callsite_stream.write(
-                    "dace::Write({}, {});".format(dst_expr, out_var), sdfg,
-                    state_id, node)
 
-    def _generate_Tasklet(self, sdfg, dfg, state_id, node, function_stream,
-                          callsite_stream):
+        if all_axes_collapsed:
+            dst_expr = output_memlet.data
+            offset = cpp_offset_expr(
+                dst_data,
+                output_memlet.subset,
+                packed_veclen=output_memlet.veclen)
+            if offset:
+                dst_expr += " + " + offset
+            def_type = self._dispatcher.defined_vars.get(output_memlet.data)
+            callsite_stream.write(
+                self.make_write(def_type, dst_data.dtype.ctype,
+                                output_memlet.data, output_memlet.veclen,
+                                dst_expr, "", out_var, output_memlet.wcr),
+                sdfg, state_id, node)
 
-        # TODO: this is copied from the CPU-codegen, necessary to inject
-        # pragmas at the output memlets! Should consolidate.
+    def generate_kernel(self, sdfg, state, kernel_name, subgraphs,
+                        function_stream, callsite_stream):
 
-        callsite_stream.write('{\n', sdfg, state_id, node)
+        # Inspect the vector length of all memlets leading to each memory, to
+        # make sure that they're consistent, and to allow us to instantiate the
+        # memories as vector types to enable HLS to generate wider data paths.
+        # Since we cannot pass this auxiliary data structure to the allocator,
+        # which is called by the dispatcher, we temporarily store it in the
+        # codegen object (naughty).
+        self._memory_widths = type(self).detect_memory_widths(subgraphs)
 
-        state_dfg = sdfg.nodes()[state_id]
+        if self._in_device_code:
+            raise CodegenError("Tried to generate kernel from device code")
+        self._in_device_code = True
+        self._cpu_codegen._packed_types = True
 
-        self._dispatcher.defined_vars.enter_scope(node)
+        kernel_stream = CodeIOStream()
 
-        arrays = set()
-        for edge in dfg.in_edges(node):
-            u = edge.src
-            memlet = edge.data
-
-            if edge.dst_conn:  # Not (None or "")
-                if edge.dst_conn in arrays:  # Disallow duplicates
-                    raise SyntaxError('Duplicates found in memlets')
-                # Special case: code->code
-                if isinstance(edge.src, nodes.CodeNode):
-                    shared_data_name = 's%d_n%d%s_n%d%s' % (
-                        state_id, dfg.node_id(edge.src), edge.src_conn,
-                        dfg.node_id(edge.dst), edge.dst_conn)
+        # Actual kernel code generation
+        self.generate_kernel_internal(sdfg, state, kernel_name, subgraphs,
+                                      kernel_stream, function_stream,
+                                      callsite_stream)
 
-                    # Read variable from shared storage
-                    callsite_stream.write(
-                        'const dace::vec<%s, %s>& %s = __%s;' %
-                        (edge.data.data.dtype.ctype, sym2cpp(edge.data.veclen),
-                         edge.dst_conn, shared_data_name), sdfg, state_id,
-                        [edge.src, edge.dst])
-                    self._dispatcher.defined_vars.add(edge.dst_conn,
-                                                      DefinedType.Scalar)
+        self._in_device_code = False
+        self._cpu_codegen._packed_types = False
 
-                else:
-                    src_node = find_input_arraynode(state_dfg, edge)
+        # Store code strings to be passed to compilation phase
+        self._kernel_codes.append((kernel_name, kernel_stream.getvalue()))
 
-                    self._dispatcher.dispatch_copy(
-                        src_node, node, edge, sdfg, state_dfg, state_id,
-                        function_stream, callsite_stream)
-
-                # Also define variables in the C++ unparser scope
-                self._cpu_codegen._locals.define(edge.dst_conn, -1,
-                                                 self._cpu_codegen._ldepth + 1)
-                arrays.add(edge.dst_conn)
-
-        callsite_stream.write('\n', sdfg, state_id, node)
-
-        # Use outgoing edges to preallocate output local vars
-        for edge in dfg.out_edges(node):
-            v = edge.dst
-            memlet = edge.data
+        # Delete the field we've abused to pass this dictionary to the memory
+        # allocator
+        del self._memory_widths
+        self._allocated_global_arrays = set()
+
+    def generate_modules(self, sdfg, state, kernel_name, subgraphs,
+                         subgraph_parameters, scalar_parameters,
+                         symbol_parameters, module_stream, entry_stream,
+                         host_stream):
+        """Main entry function for generating a Xilinx kernel."""
 
-            if edge.src_conn:
-                if edge.src_conn in arrays:  # Disallow duplicates
+        # Module generation
+        for subgraph in subgraphs:
+            # Traverse to find first tasklets reachable in topological order
+            to_traverse = subgraph.source_nodes()
+            seen = set()
+            tasklet_list = []
+            access_nodes = []
+            while len(to_traverse) > 0:
+                n = to_traverse.pop()
+                if n in seen:
                     continue
-                # Special case: code->code
-                if isinstance(edge.dst, nodes.CodeNode):
-                    callsite_stream.write(
-                        'dace::vec<%s, %s> %s;' %
-                        (sdfg.arrays[memlet.data].dtype.ctype,
-                         sym2cpp(memlet.veclen), edge.src_conn), sdfg,
-                        state_id, [edge.src, edge.dst])
-                    self._dispatcher.defined_vars.add(edge.src_conn,
-                                                      DefinedType.Scalar)
+                seen.add(n)
+                if (isinstance(n, dace.graph.nodes.Tasklet)
+                        or isinstance(n, dace.graph.nodes.NestedSDFG)):
+                    tasklet_list.append(n)
                 else:
-                    dst_node = find_output_arraynode(state_dfg, edge)
+                    if isinstance(n, dace.graph.nodes.AccessNode):
+                        access_nodes.append(n)
+                    for e in subgraph.out_edges(n):
+                        if e.dst not in seen:
+                            to_traverse.append(e.dst)
+            # Name module according to all reached tasklets (can be just one)
+            labels = [n.label.replace(" ", "_") for n in tasklet_list]
+            # If there are no tasklets, name it after access nodes in the
+            # subgraph
+            if len(labels) == 0:
+                labels = [n.label.replace(" ", "_") for n in access_nodes]
+            if len(labels) == 0:
+                raise RuntimeError(
+                    "Expected at least one tasklet or data node")
+            module_name = "_".join(labels)
+            self.generate_module(
+                sdfg, state, module_name, subgraph,
+                subgraph_parameters[subgraph] + scalar_parameters,
+                symbol_parameters, module_stream, entry_stream, host_stream)
+
+    def generate_host_function_boilerplate(
+            self, sdfg, state, kernel_name, parameters, symbol_parameters,
+            nested_global_transients, host_code_stream, header_stream,
+            callsite_stream):
+
+        # Generates:
+        # - Definition of wrapper function in caller code
+        # - Definition of kernel function in host code file
+        # - Signature and opening brace of host code function in host code file
 
-                    self._dispatcher.dispatch_copy(
-                        node, dst_node, edge, sdfg, state_dfg, state_id,
-                        function_stream, callsite_stream)
-
-                # Also define variables in the C++ unparser scope
-                self._cpu_codegen._locals.define(edge.src_conn, -1,
-                                                 self._cpu_codegen._ldepth + 1)
-                arrays.add(edge.src_conn)
-
-        callsite_stream.write('\n    ///////////////////\n', sdfg, state_id,
-                              node)
-
-        cpu.unparse_tasklet(sdfg, state_id, dfg, node, function_stream,
-                            callsite_stream, self._cpu_codegen._locals,
-                            self._cpu_codegen._ldepth)
-
-        callsite_stream.write('    ///////////////////\n\n', sdfg, state_id,
-                              node)
-
-        # Process outgoing memlets
-        self._cpu_codegen.process_out_memlets(
-            sdfg, state_id, node, state_dfg, self._dispatcher, callsite_stream,
-            True, function_stream)
-
-        for edge in state_dfg.out_edges(node):
-            datadesc = sdfg.arrays[edge.data.data]
-            if (isinstance(datadesc, dace.data.Array) and
-                (datadesc.storage == dace.dtypes.StorageType.FPGA_Local
-                 or datadesc.storage == dace.dtypes.StorageType.FPGA_Registers)
-                    and edge.data.wcr is None):
-                callsite_stream.write(
-                    "#pragma HLS DEPENDENCE variable=__{} false".format(
-                        edge.src_conn))
+        # We exclude nested transients from the CPU code function call, as they
+        # have not yet been allocated at this point
+        nested_transient_set = {n.data for n in nested_global_transients}
+
+        seen = set(nested_transient_set)
+        kernel_args_call_host = []
+        for is_output, argname, arg in parameters:
+            # Only pass each array once from the host code
+            if arg in seen:
+                continue
+            seen.add(arg)
+            if not isinstance(arg, dace.data.Stream):
+                kernel_args_call_host.append(
+                    arg.signature(False, name=argname))
+
+        # Treat scalars as symbols, assuming they can be input only
+        symbol_sigs = [
+            p.signature(name=name) for name, p in symbol_parameters.items()
+        ]
+        symbol_names = symbol_parameters.keys()
+
+        kernel_args_call_host += symbol_names
+        kernel_args_opencl = (self.opencl_parameters(
+            sdfg, [p for p in parameters
+                   if p[1] not in nested_transient_set]) + symbol_sigs)
+
+        host_function_name = "__dace_runkernel_{}".format(kernel_name)
+
+        # Write OpenCL host function
+        host_code_stream.write(
+            """\
+DACE_EXPORTED void {host_function_name}({kernel_args_opencl}) {{
+  hlslib::ocl::Program program = hlslib::ocl::GlobalContext().CurrentlyLoadedProgram();"""
+            .format(
+                host_function_name=host_function_name,
+                kernel_args_opencl=", ".join(kernel_args_opencl)))
 
-        callsite_stream.write('}\n', sdfg, state_id, node)
+        header_stream.write("\n\nDACE_EXPORTED void {}({});\n\n".format(
+            host_function_name, ", ".join(kernel_args_opencl)))
+
+        callsite_stream.write("{}({});".format(
+            host_function_name, ", ".join(kernel_args_call_host)))
+
+        # Any extra transients stored in global memory on the FPGA must now be
+        # allocated and passed to the kernel
+        for arr_node in nested_global_transients:
+            self._dispatcher.dispatch_allocate(sdfg, state, None, arr_node,
+                                               None, host_code_stream)
+            self._dispatcher.dispatch_initialize(sdfg, state, None, arr_node,
+                                                 None, host_code_stream)
+
+
+# ------------------------------------------------------------------------------
+
+
+class PipelineEntry(dace.graph.nodes.MapEntry):
+    @property
+    def pipeline(self):
+        return self._map
+
+    @pipeline.setter
+    def pipeline(self, val):
+        self._map = val
+
+
+class PipelineExit(dace.graph.nodes.MapExit):
+    @property
+    def pipeline(self):
+        return self._map
 
-        self._dispatcher.defined_vars.exit_scope(node)
+    @pipeline.setter
+    def pipeline(self, val):
+        self._map = val
+
+
+@make_properties
+class Pipeline(dace.graph.nodes.Map):
+    """ This a convenience-subclass of Map that allows easier implementation of
+        loop nests (using regular Map indices) that need a constant-sized
+        initialization and drain phase (e.g., N*M + c iterations), which would
+        otherwise need a flattened one-dimensional map.
+    """
+    init_size = Property(
+        dtype=int, desc="Number of initialization iterations.")
+    init_overlap = Property(
+        dtype=int,
+        desc="Whether to increment regular map indices during initialization.")
+    drain_size = Property(dtype=int, desc="Number of drain iterations.")
+    drain_overlap = Property(
+        dtype=int,
+        desc="Whether to increment regular map indices during pipeline drain.")
+
+    def __init__(self,
+                 *args,
+                 init_size=0,
+                 init_overlap=False,
+                 drain_size=0,
+                 drain_overlap=False,
+                 **kwargs):
+        super(Pipeline, self).__init__(*args, **kwargs)
+        self.init_size = init_size
+        self.init_overlap = init_overlap
+        self.drain_size = drain_size
+        self.drain_overlap = drain_overlap
+        self.flatten = True
+
+    def iterator_str(self):
+        return "__" + "".join(self.params)
+
+    def loop_bound_str(self):
+        bound = 1
+        for begin, end, step in self.range:
+            bound *= (step + end - begin) // step
+        # Add init and drain phases when relevant
+        add_str = (" + " + cpu.sym2cpp(self.init_size)
+                   if self.init_size != 0 and not self.init_overlap else "")
+        add_str += (" + " + cpu.sym2cpp(self.drain_size)
+                    if self.drain_size != 0 and not self.drain_overlap else "")
+        return cpu.sym2cpp(bound) + add_str
+
+    def init_condition(self):
+        """Variable that can be checked to see if pipeline is currently in
+           initialization phase."""
+        if self.init_size <= 0:
+            raise ValueError("No init condition exists for " + self.label)
+        return self.iterator_str() + "_init"
+
+    def drain_condition(self):
+        """Variable that can be checked to see if pipeline is currently in
+           draining phase."""
+        if self.drain_size <= 0:
+            raise ValueError("No drain condition exists for " + self.label)
+        return self.iterator_str() + "_drain"
```

### Comparing `dace-0.9.0/dace/config.py` & `dace-0.9.5/dace/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 import platform
 import yaml
 
 
 def _env2bool(envval):
     """ Converts an arbitrary value to boolean.
-        @param envval: Arbitrary value.
-        @return: True if the input value matches a valid TRUE
+        :param envval: Arbitrary value.
+        :return: True if the input value matches a valid TRUE
                   value, or False otherwise.
     """
     return str(envval).lower() in ['true', '1', 'y', 'yes', 'on']
 
 
 def _add_defaults(config, metadata):
     """ Add defaults to configuration from metadata.
-        @return: True if configuration was modified, False otherwise.
+        :return: True if configuration was modified, False otherwise.
     """
     osname = platform.system()
     modified = False
     for k, v in metadata.items():
         # Recursive call for fields inside the dictionary
         if v['type'] == 'dict':
             if k not in config:
@@ -92,99 +92,102 @@
             Config._config = {}
             _add_defaults(Config._config, Config._config_metadata['required'])
             Config.save()
 
     @staticmethod
     def load(filename=None):
         """ Loads a configuration from an existing file.
-            @param filename: The file to load. If unspecified, 
+            :param filename: The file to load. If unspecified,
                              uses default configuration file.
         """
         if filename is None:
             filename = Config._cfg_filename
 
         # Read configuration file
         with open(filename, 'r') as f:
             Config._config = yaml.load(f.read(), Loader=yaml.SafeLoader)
 
+        if Config._config is None:
+            Config._config = {}
+
         # Add defaults from metadata
         modified = _add_defaults(Config._config,
                                  Config._config_metadata['required'])
         if modified:  # Update file if changed
             Config.save()
 
     @staticmethod
     def load_schema(filename=None):
         """ Loads a configuration schema from an existing file.
-            @param filename: The file to load. If unspecified,
+            :param filename: The file to load. If unspecified,
                              uses default schema file.
         """
         if filename is None:
             filename = Config._metadata_filename
         with open(filename, 'r') as f:
             Config._config_metadata = yaml.load(
                 f.read(), Loader=yaml.SafeLoader)
 
     @staticmethod
     def save(path=None):
         """ Saves the current configuration to a file.
-            @param path: The file to save to. If unspecified,
+            :param path: The file to save to. If unspecified,
                          uses default configuration file.
         """
         if path is None:
             path = Config._cfg_filename
         # Write configuration file
         with open(path, 'w') as f:
             yaml.dump(Config._config, f, default_flow_style=False)
 
     @staticmethod
     def get_metadata(*key_hierarchy):
         """ Returns the configuration specification of a given entry
             from the schema.
-            @param key_hierarchy: A tuple of strings leading to the
+            :param key_hierarchy: A tuple of strings leading to the
                                   configuration entry. 
                                   For example: ('a', 'b', 'c') would be
                                   configuration entry c which is in the
                                   path a->b.
-            @return: Configuration specification as a dictionary.
+            :return: Configuration specification as a dictionary.
         """
         # Traverse the key hierarchy
         current_conf = Config._config_metadata
         for key in key_hierarchy:
             current_conf = current_conf['required'][key]
         return current_conf
 
     @staticmethod
     def get_default(*key_hierarchy):
         """ Returns the default value of a given configuration entry.
             Takes into accound current operating system.
-            @param key_hierarchy: A tuple of strings leading to the
+            :param key_hierarchy: A tuple of strings leading to the
                                   configuration entry. 
                                   For example: ('a', 'b', 'c') would be
                                   configuration entry c which is in the
                                   path a->b.
-            @return: Default configuration value.
+            :return: Default configuration value.
         """
         # Traverse the key hierarchy
         current_conf = Config._config_metadata
         for key in key_hierarchy:
             current_conf = current_conf['required'][key]
         if 'default_' + platform.system() in current_conf:
             return current_conf['default_' + platform.system()]
         return current_conf['default']
 
     @staticmethod
     def get(*key_hierarchy):
         """ Returns the current value of a given configuration entry.
-            @param key_hierarchy: A tuple of strings leading to the
+            :param key_hierarchy: A tuple of strings leading to the
                                   configuration entry. 
                                   For example: ('a', 'b', 'c') would be
                                   configuration entry c which is in the
                                   path a->b.
-            @return: Configuration entry value.
+            :return: Configuration entry value.
         """
         # Environment variable override
         # NOTE: will only work if a specific key is accessed!
         envvar = 'DACE_' + '_'.join(key_hierarchy)
         if envvar in os.environ:
             return os.environ[envvar]
 
@@ -196,40 +199,40 @@
         return current_conf
 
     @staticmethod
     def get_bool(*key_hierarchy):
         """ Returns the current value of a given boolean configuration entry.
             This specialization allows more string types to be converted to 
             boolean, e.g., due to environment variable overrides.
-            @param key_hierarchy: A tuple of strings leading to the
+            :param key_hierarchy: A tuple of strings leading to the
                                   configuration entry. 
                                   For example: ('a', 'b', 'c') would be
                                   configuration entry c which is in the
                                   path a->b.
-            @return: Configuration entry value (as a boolean).
+            :return: Configuration entry value (as a boolean).
         """
         res = Config.get(*key_hierarchy)
         if isinstance(res, bool):
             return res
         return _env2bool(str(res))
 
     @staticmethod
     def append(*key_hierarchy, value=None, autosave=False):
         """ Appends to the current value of a given configuration entry
             and sets it. Example usage: 
             `Config.append('compiler', 'cpu', 'args', value='-fPIC')`
-            @param key_hierarchy: A tuple of strings leading to the
+            :param key_hierarchy: A tuple of strings leading to the
                                   configuration entry. 
                                   For example: ('a', 'b', 'c') would be
                                   configuration entry c which is in the
                                   path a->b.
-            @param value: The value to append.
-            @param autosave: If True, saves the configuration to the file
+            :param value: The value to append.
+            :param autosave: If True, saves the configuration to the file
                              after modification.
-            @return: Current configuration entry value.
+            :return: Current configuration entry value.
         """
         # Traverse the key hierarchy up until the next to last element
         current_conf = Config._config
         for key in key_hierarchy[:-1]:
             current_conf = current_conf[key]
 
         current_conf[key_hierarchy[-1]] += value
@@ -239,21 +242,21 @@
         return current_conf[key_hierarchy[-1]]
 
     @staticmethod
     def set(*key_hierarchy, value=None, autosave=False):
         """ Sets the current value of a given configuration entry.
             Example usage: 
             `Config.set('profiling', value=True)`
-            @param key_hierarchy: A tuple of strings leading to the
+            :param key_hierarchy: A tuple of strings leading to the
                                   configuration entry. 
                                   For example: ('a', 'b', 'c') would be
                                   configuration entry c which is in the
                                   path a->b.
-            @param value: The value to set.
-            @param autosave: If True, saves the configuration to the file
+            :param value: The value to set.
+            :param autosave: If True, saves the configuration to the file
                              after modification.
         """
         # Traverse the key hierarchy up until the next to last element
         current_conf = Config._config
         for key in key_hierarchy[:-1]:
             current_conf = current_conf[key]
```

### Comparing `dace-0.9.0/dace/data.py` & `dace-0.9.5/dace/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,30 +44,30 @@
 
 @make_properties
 class Data(object):
     """ Data type descriptors that can be used as references to memory.
         Examples: Arrays, Streams, custom arrays (e.g., sparse matrices).
     """
 
-    dtype = TypeClassProperty()
-    shape = ShapeProperty()
-    transient = Property(dtype=bool)
+    dtype = TypeClassProperty(default=dtypes.int32)
+    shape = ShapeProperty(default=[])
+    transient = Property(dtype=bool, default=False)
     storage = Property(
         dtype=dace.dtypes.StorageType,
         desc="Storage location",
-        enum=dace.dtypes.StorageType,
+        choices=dace.dtypes.StorageType,
         default=dace.dtypes.StorageType.Default,
         from_string=lambda x: dtypes.StorageType[x])
     location = Property(
         dtype=str,  # Dict[str, symbolic]
         desc='Full storage location identifier (e.g., rank, GPU ID)',
         default='')
     toplevel = Property(
         dtype=bool, desc="Allocate array outside of state", default=False)
-    debuginfo = DebugInfoProperty()
+    debuginfo = DebugInfoProperty(allow_none=True)
 
     def __init__(self, dtype, shape, transient, storage, location, toplevel,
                  debuginfo):
         self.dtype = dtype
         self.shape = shape
         self.transient = transient
         self.storage = storage
@@ -87,25 +87,20 @@
     def _validate(self):
         if any(not isinstance(s, (int, symbolic.SymExpr, symbolic.symbol,
                                   symbolic.sympy.Basic)) for s in self.shape):
             raise TypeError('Shape must be a list or tuple of integer values '
                             'or symbols')
         return True
 
-    def toJSON(self):
-        try:
-            attrs = json.loads(Property.all_properties_to_json(self))
-        except Exception as e:
-            print("Got exception: " + str(e))
-            import traceback
-            traceback.print_exc()
+    def to_json(self):
+        attrs = dace.serialize.all_properties_to_json(self)
 
         retdict = {"type": type(self).__name__, "attributes": attrs}
 
-        return json.dumps(retdict)
+        return retdict
 
     def copy(self):
         raise RuntimeError(
             'Data descriptors are unique and should not be copied')
 
     def is_equivalent(self, other):
         """ Check for equivalence (shape and type) of two data descriptors. """
@@ -119,15 +114,15 @@
         return 'Abstract Data Container, DO NOT USE'
 
 
 @make_properties
 class Scalar(Data):
     """ Data descriptor of a scalar value. """
 
-    allow_conflicts = Property(dtype=bool)
+    allow_conflicts = Property(dtype=bool, default=False)
 
     def __init__(self,
                  dtype,
                  transient=False,
                  storage=dace.dtypes.StorageType.Default,
                  allow_conflicts=False,
                  location='',
@@ -135,21 +130,21 @@
                  debuginfo=None):
         self.allow_conflicts = allow_conflicts
         shape = [1]
         super(Scalar, self).__init__(dtype, shape, transient, storage,
                                      location, toplevel, debuginfo)
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
+    def from_json(json_obj, context=None):
         if json_obj['type'] != "Scalar":
             raise TypeError("Invalid data type")
 
         # Create dummy object
         ret = Scalar(dace.dtypes.int8)
-        Property.set_properties_from_json(ret, json_obj, context=context)
+        dace.serialize.set_properties_from_json(ret, json_obj, context=context)
 
         # Check validity now
         ret.validate()
         return ret
 
     def __repr__(self):
         return 'Scalar (dtype=%s)' % self.dtype
@@ -157,15 +152,19 @@
     def clone(self):
         return Scalar(self.dtype, self.transient, self.storage,
                       self.allow_conflicts, self.location, self.toplevel,
                       self.debuginfo)
 
     @property
     def strides(self):
-        return self.shape
+        return [1]
+
+    @property
+    def total_size(self):
+        return 1
 
     @property
     def offset(self):
         return [0]
 
     def is_equivalent(self, other):
         if not isinstance(other, Scalar):
@@ -210,119 +209,130 @@
                 and obj.storage != dace.dtypes.StorageType.Immaterial):
             raise ValueError("Immaterial array must have immaterial storage, "
                              "but has: {}".format(storage))
         obj.storage = dace.dtypes.StorageType.Immaterial
     obj._materialize_func = val
 
 
+def _prod(sequence):
+    return functools.reduce(lambda a, b: a * b, sequence, 1)
+
+
 @make_properties
 class Array(Data):
     """ Array/constant descriptor (dimensions, type and other properties). """
 
     # Properties
-    allow_conflicts = Property(dtype=bool)
+    allow_conflicts = Property(
+        dtype=bool,
+        default=False,
+        desc='If enabled, allows more than one '
+        'memlet to write to the same memory location without conflict '
+        'resolution.')
+
     # TODO: Should we use a Code property here?
     materialize_func = Property(
         dtype=str, allow_none=True, setter=set_materialize_func)
-    access_order = ListProperty(element_type=int)
-    strides = ListProperty(element_type=symbolic.pystr_to_symbolic)
-    offset = ListProperty(element_type=symbolic.pystr_to_symbolic)
+
+    strides = ListProperty(
+        element_type=symbolic.pystr_to_symbolic,
+        desc='For each dimension, the number of elements to '
+        'skip in order to obtain the next element in '
+        'that dimension.')
+
+    total_size = SymbolicProperty(
+        default=1,
+        desc='The total allocated size of the array. Can be used for'
+        ' padding.')
+
+    offset = ListProperty(
+        element_type=symbolic.pystr_to_symbolic,
+        desc='Initial offset to translate all indices by.')
+
     may_alias = Property(
         dtype=bool,
         default=False,
         desc='This pointer may alias with other pointers in '
         'the same function')
 
     def __init__(self,
                  dtype,
                  shape,
                  materialize_func=None,
                  transient=False,
                  allow_conflicts=False,
                  storage=dace.dtypes.StorageType.Default,
                  location='',
-                 access_order=None,
                  strides=None,
                  offset=None,
                  may_alias=False,
                  toplevel=False,
-                 debuginfo=None):
+                 debuginfo=None,
+                 total_size=None):
 
         super(Array, self).__init__(dtype, shape, transient, storage, location,
                                     toplevel, debuginfo)
 
         if shape is None:
             raise IndexError('Shape must not be None')
 
         self.allow_conflicts = allow_conflicts
         self.materialize_func = materialize_func
         self.may_alias = may_alias
 
-        if access_order is not None:
-            self.access_order = cp.copy(access_order)
-        else:
-            self.access_order = tuple(i for i in range(len(shape)))
-
         if strides is not None:
             self.strides = cp.copy(strides)
         else:
-            self.strides = cp.copy(list(shape))
+            self.strides = [_prod(shape[i + 1:]) for i in range(len(shape))]
+
+        self.total_size = total_size or _prod(shape)
 
         if offset is not None:
             self.offset = cp.copy(offset)
         else:
             self.offset = [0] * len(shape)
 
         self.validate()
 
     def __repr__(self):
         return 'Array (dtype=%s, shape=%s)' % (self.dtype, self.shape)
 
     def clone(self):
         return Array(self.dtype, self.shape, self.materialize_func,
                      self.transient, self.allow_conflicts, self.storage,
-                     self.location, self.access_order, self.strides,
-                     self.offset, self.may_alias, self.toplevel,
-                     self.debuginfo)
+                     self.location, self.strides, self.offset, self.may_alias,
+                     self.toplevel, self.debuginfo, self.total_size)
 
-    def toJSON(self):
-        try:
-            attrs = json.loads(Property.all_properties_to_json(self))
-        except Exception as e:
-            print("Got exception: " + str(e))
-            import traceback
-            traceback.print_exc()
+    def to_json(self):
+        attrs = dace.serialize.all_properties_to_json(self)
 
         # Take care of symbolic expressions
         attrs['strides'] = list(map(str, attrs['strides']))
 
         retdict = {"type": type(self).__name__, "attributes": attrs}
 
-        return json.dumps(retdict)
+        return retdict
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
+    def from_json(json_obj, context=None):
         if json_obj['type'] != "Array":
             raise TypeError("Invalid data type")
 
         # Create dummy object
         ret = Array(dace.dtypes.int8, ())
-        Property.set_properties_from_json(ret, json_obj, context=context)
+        dace.serialize.set_properties_from_json(ret, json_obj, context=context)
         # TODO: This needs to be reworked (i.e. integrated into the list property)
         ret.strides = list(map(symbolic.pystr_to_symbolic, ret.strides))
 
         # Check validity now
         ret.validate()
         return ret
 
     def validate(self):
         super(Array, self).validate()
-        if len(self.access_order) != len(self.shape):
-            raise TypeError('Access order must be the same size as shape')
-
         if len(self.strides) != len(self.shape):
             raise TypeError('Strides must be the same size as shape')
 
         if any(not isinstance(s, (int, symbolic.SymExpr, symbolic.symbol,
                                   symbolic.sympy.Basic))
                for s in self.strides):
             raise TypeError('Strides must be a list or tuple of integer '
@@ -428,98 +438,82 @@
 
 
 @make_properties
 class Stream(Data):
     """ Stream (or stream array) data descriptor. """
 
     # Properties
-    strides = ListProperty(element_type=symbolic.pystr_to_symbolic)
     offset = ListProperty(element_type=symbolic.pystr_to_symbolic)
-    buffer_size = Property(dtype=int, desc="Size of internal buffer.")
+    buffer_size = SymbolicProperty(desc="Size of internal buffer.", default=0)
     veclen = Property(
         dtype=int, desc="Vector length. Memlets must adhere to this.")
 
     def __init__(self,
                  dtype,
                  veclen,
                  buffer_size,
                  shape=None,
                  transient=False,
                  storage=dace.dtypes.StorageType.Default,
                  location='',
-                 strides=None,
                  offset=None,
                  toplevel=False,
                  debuginfo=None):
 
         if shape is None:
             shape = (1, )
 
         self.veclen = veclen
         self.buffer_size = buffer_size
 
-        if strides is not None:
-            if len(strides) != len(shape):
-                raise TypeError('Strides must be the same size as shape')
-            self.strides = cp.copy(strides)
-        else:
-            self.strides = cp.copy(list(shape))
-
         if offset is not None:
             if len(offset) != len(shape):
                 raise TypeError('Offset must be the same size as shape')
             self.offset = cp.copy(offset)
         else:
             self.offset = [0] * len(shape)
 
         super(Stream, self).__init__(dtype, shape, transient, storage,
                                      location, toplevel, debuginfo)
 
-    def toJSON(self):
-        try:
-            attrs = json.loads(Property.all_properties_to_json(self))
-        except Exception as e:
-            print("Got exception: " + str(e))
-            import traceback
-            traceback.print_exc()
-
-        # Take care of symbolic expressions
-        attrs['strides'] = list(map(str, attrs['strides']))
+    def to_json(self):
+        attrs = dace.serialize.all_properties_to_json(self)
 
         retdict = {"type": type(self).__name__, "attributes": attrs}
 
-        return json.dumps(retdict)
+        return retdict
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
+    def from_json(json_obj, context=None):
         if json_obj['type'] != "Stream":
             raise TypeError("Invalid data type")
 
         # Create dummy object
         ret = Stream(dace.dtypes.int8, 1, 1)
-        Property.set_properties_from_json(ret, json_obj, context=context)
-        # TODO: FIXME:
-        # Since the strides are a list-property (normal Property()),
-        # loading from/to string (and, consequently, from/to json)
-        # leads to validation errors (contains Strings/Integers, not sympy symbols).
-        # To fix this, it needs a custom class
-        # For now, this is a workaround:
-        ret.strides = list(map(symbolic.pystr_to_symbolic, ret.strides))
+        dace.serialize.set_properties_from_json(ret, json_obj, context=context)
 
         # Check validity now
         ret.validate()
         return ret
 
     def __repr__(self):
         return 'Stream (dtype=%s, shape=%s)' % (self.dtype, self.shape)
 
+    @property
+    def total_size(self):
+        return _prod(self.shape)
+
+    @property
+    def strides(self):
+        return [_prod(self.shape[i + 1:]) for i in range(len(self.shape))]
+
     def clone(self):
         return Stream(self.dtype, self.veclen, self.buffer_size, self.shape,
-                      self.transient, self.storage, self.location,
-                      self.strides, self.offset, self.toplevel, self.debuginfo)
+                      self.transient, self.storage, self.location, self.offset,
+                      self.toplevel, self.debuginfo)
 
     # Checks for equivalent shape and type
     def is_equivalent(self, other):
         if not isinstance(other, Stream):
             return False
 
         # Test type
@@ -568,20 +562,19 @@
         return [
             d.name if isinstance(d, symbolic.symbol) else str(d)
             for d in self.shape
         ]
 
     def size_string(self):
         return (" * ".join([
-            cppunparse.pyexpr2cpp(dace.symbolic.symstr(s))
-            for s in self.strides
+            cppunparse.pyexpr2cpp(dace.symbolic.symstr(s)) for s in self.shape
         ]))
 
     def is_stream_array(self):
-        return functools.reduce(lambda a, b: a * b, self.strides) != 1
+        return _prod(self.shape) != 1
 
     def covers_range(self, rng):
         if len(rng) != len(self.shape):
             return False
 
         for s, (rb, re, rs) in zip(self.shape, rng):
             # Shape has to be positive
```

### Comparing `dace-0.9.0/dace/frontend/common/op_impl.py` & `dace-0.9.5/dace/frontend/common/op_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,31 +128,29 @@
             actual_dims = [
                 idx for idx, r in enumerate(full_shape)
                 if not (isinstance(r, int) and r == 1)
             ]
             if len(actual_dims) == 0:  # abort
                 actual_dims = [len(full_shape) - 1]
             if isinstance(array, dace.data.Scalar):
-                cloned_array = sdfg.add_array(
+                sdfg.add_array(
                     name=cloned_name,
                     shape=[1],
                     dtype=array.dtype,
                     transient=True,
                     storage=dace.dtypes.StorageType.GPU_Global)
             else:
-                cloned_array = sdfg.add_array(
+                sdfg.add_array(
                     name=cloned_name,
                     shape=[full_shape[d] for d in actual_dims],
                     dtype=array.dtype,
                     materialize_func=array.materialize_func,
                     transient=True,
                     storage=dace.dtypes.StorageType.GPU_Global,
                     allow_conflicts=array.allow_conflicts,
-                    access_order=tuple(
-                        [array.access_order[d] for d in actual_dims]),
                     strides=[array.strides[d] for d in actual_dims],
                     offset=[array.offset[d] for d in actual_dims])
             cloned_arrays[array_node.data] = cloned_name
         cloned_node = type(array_node)(cloned_name)
 
         in_cloned_arraynodes[array_node.data] = cloned_node
     for array_node, memlet in out_arrays_to_clone:
@@ -192,31 +190,29 @@
             actual_dims = [
                 idx for idx, r in enumerate(full_shape)
                 if not (isinstance(r, int) and r == 1)
             ]
             if len(actual_dims) == 0:  # abort
                 actual_dims = [len(full_shape) - 1]
             if isinstance(array, dace.data.Scalar):
-                cloned_array = sdfg.add_array(
+                sdfg.add_array(
                     name=cloned_name,
                     shape=[1],
                     dtype=array.dtype,
                     transient=True,
                     storage=dace.dtypes.StorageType.GPU_Global)
             else:
-                cloned_array = sdfg.add_array(
+                sdfg.add_array(
                     name=cloned_name,
                     shape=[full_shape[d] for d in actual_dims],
                     dtype=array.dtype,
                     materialize_func=array.materialize_func,
                     transient=True,
                     storage=dace.dtypes.StorageType.GPU_Global,
                     allow_conflicts=array.allow_conflicts,
-                    access_order=tuple(
-                        [array.access_order[d] for d in actual_dims]),
                     strides=[array.strides[d] for d in actual_dims],
                     offset=[array.offset[d] for d in actual_dims])
             cloned_arrays[array_node.data] = cloned_name
         cloned_node = type(array_node)(cloned_name)
         cloned_node.setzero = True
 
         out_cloned_arraynodes[array_node.data] = cloned_node
@@ -415,30 +411,30 @@
                           accumulate: bool = False,
                           interchange: bool = True,
                           A_index: Index = None,
                           B_index: Index = None,
                           C_index: Index = None,
                           label: str = None):
     """ Adds a matrix multiplication operation to an existing SDFG state.
-        @param A_src: The source node from which the memlet of matrix A is
+        :param A_src: The source node from which the memlet of matrix A is
                       connected.
-        @param A_node: The Access Node for matrix A.
-        @param B_src: The source node from which the memlet of matrix B is
+        :param A_node: The Access Node for matrix A.
+        :param B_src: The source node from which the memlet of matrix B is
                       connected.
-        @param B_node: The Access Node for matrix B.
-        @param C_dst: The destination node to which the memlet of matrix C is
+        :param B_node: The Access Node for matrix B.
+        :param C_dst: The destination node to which the memlet of matrix C is
                       connected.
-        @param C_node: The Access Node for matrix C.
-        @param accumulate: Whether to accumulate to C or store to it.
-        @param interchange: If True, interchanges the multiplication maps for
+        :param C_node: The Access Node for matrix C.
+        :param accumulate: Whether to accumulate to C or store to it.
+        :param interchange: If True, interchanges the multiplication maps for
                             performance (in some cases).
-        @param A_index: Slice of matrix A to use for multiplication.
-        @param B_index: Slice of matrix B to use for multiplication.
-        @param C_index: Slice of matrix C to use for multiplication.
-        @param label: Optional label for the maps and tasklet.
+        :param A_index: Slice of matrix A to use for multiplication.
+        :param B_index: Slice of matrix B to use for multiplication.
+        :param C_index: Slice of matrix C to use for multiplication.
+        :param label: Optional label for the maps and tasklet.
     """
 
     # Validate input
     sdfg = state.parent
     map_ranges, A_ranges, B_ranges, C_ranges = validate_matrix_multiplication(
         A_node.desc(sdfg).shape,
         B_node.desc(sdfg).shape,
@@ -540,22 +536,22 @@
                             B_dst: Node,
                             B_node: DNode,
                             alpha: str = 'const_pone',
                             label: str = None,
                             conjugate: bool = False):
     """ Adds a matrix transposition operation to an existing SDFG state,
         using CUBLAS as the implementation.
-        @param A_src: The source node from which the memlet of matrix A is
+        :param A_src: The source node from which the memlet of matrix A is
                       connected.
-        @param A_node: The Access Node for matrix A.
-        @param B_dst: The destination node to which the memlet of matrix B is
+        :param A_node: The Access Node for matrix A.
+        :param B_dst: The destination node to which the memlet of matrix B is
                       connected.
-        @param B_node: The Access Node for matrix B.
-        @param alpha: Multiplier for input matrix.
-        @param label: Optional label for the tasklet.
+        :param B_node: The Access Node for matrix B.
+        :param alpha: Multiplier for input matrix.
+        :param label: Optional label for the tasklet.
     """
 
     sdfg = state.parent
 
     # Validate inputs
     A = A_node.desc(sdfg)
     B = B_node.desc(sdfg)
@@ -589,16 +585,16 @@
         );
         '''.format(
             mode=mode,
             btype=_to_blastype(A.dtype.type),
             cutype=_to_cudatype(A.dtype.type),
             rows=A.shape[1],
             cols=A.shape[0],
-            astride=A.strides[1],
-            bstride=B.strides[1],
+            astride=A.strides[0],
+            bstride=B.strides[0],
             alpha=alpha),
         language=dace.dtypes.Language.CPP)
 
     state.add_edge(A_src, None, tasklet, 'a',
                    dace.Memlet.simple(A_node, '0:%s,0:%s' % A.shape))
     state.add_edge(tasklet, 'b', B_dst, None,
                    dace.Memlet.simple(B_node, '0:%s,0:%s' % B.shape))
@@ -619,32 +615,32 @@
                                  beta: str = 'const_zero',
                                  A_index: Index = None,
                                  B_index: Index = None,
                                  C_index: Index = None,
                                  label: str = None):
     """ Adds a matrix multiplication operation to an existing SDFG state,
         using CUBLAS as the implementation.
-        @param A_src: The source node from which the memlet of matrix A is
+        :param A_src: The source node from which the memlet of matrix A is
                       connected.
-        @param A_node: The Access Node for matrix A.
-        @param B_src: The source node from which the memlet of matrix B is
+        :param A_node: The Access Node for matrix A.
+        :param B_src: The source node from which the memlet of matrix B is
                       connected.
-        @param B_node: The Access Node for matrix B.
-        @param C_dst: The destination node to which the memlet of matrix C is
+        :param B_node: The Access Node for matrix B.
+        :param C_dst: The destination node to which the memlet of matrix C is
                       connected.
-        @param C_node: The Access Node for matrix C.
-        @param accumulate: Whether to accumulate to C or store to it.
-        @param interchange: If True, interchanges the multiplication maps for
+        :param C_node: The Access Node for matrix C.
+        :param accumulate: Whether to accumulate to C or store to it.
+        :param interchange: If True, interchanges the multiplication maps for
                             performance (in some cases).
-        @param alpha: Alpha value for GEMM.
-        @param beta: Beta value for GEMM.
-        @param A_index: Slice of matrix A to use for multiplication.
-        @param B_index: Slice of matrix B to use for multiplication.
-        @param C_index: Slice of matrix C to use for multiplication.
-        @param label: Optional label for the maps and tasklet.
+        :param alpha: Alpha value for GEMM.
+        :param beta: Beta value for GEMM.
+        :param A_index: Slice of matrix A to use for multiplication.
+        :param B_index: Slice of matrix B to use for multiplication.
+        :param C_index: Slice of matrix C to use for multiplication.
+        :param label: Optional label for the maps and tasklet.
     """
 
     # Validate input
     sdfg = state.parent
     map_ranges, A_ranges, B_ranges, C_ranges = validate_matrix_multiplication(
         A_node.desc(sdfg).shape,
         B_node.desc(sdfg).shape,
@@ -708,35 +704,35 @@
                                     A_index: Index = None,
                                     B_index: Index = None,
                                     C_index: Index = None,
                                     label: str = None):
     """ Adds a matrix multiplication operation to an existing SDFG state,
         using CUBLAS as the implementation, and providing a separate source
         and destination nodes for the output matrix.
-        @param A_src: The source node from which the memlet of matrix A is
+        :param A_src: The source node from which the memlet of matrix A is
                       connected.
-        @param A_node: The Access Node for matrix A.
-        @param B_src: The source node from which the memlet of matrix B is
+        :param A_node: The Access Node for matrix A.
+        :param B_src: The source node from which the memlet of matrix B is
                       connected.
-        @param B_node: The Access Node for matrix B.
-        @param C_src: The node from which the memlet of matrix C is
+        :param B_node: The Access Node for matrix B.
+        :param C_src: The node from which the memlet of matrix C is
                       connected into the multiplication.
-        @param C_src_node: The input Access Node for matrix C.
-        @param C_dst: The node to which the memlet of matrix C is
+        :param C_src_node: The input Access Node for matrix C.
+        :param C_dst: The node to which the memlet of matrix C is
                       connected out of the multiplication.
-        @param C_dst_node: The output Access Node for matrix C.
-        @param accumulate: Whether to accumulate to C or store to it.
-        @param interchange: If True, interchanges the multiplication maps for
+        :param C_dst_node: The output Access Node for matrix C.
+        :param accumulate: Whether to accumulate to C or store to it.
+        :param interchange: If True, interchanges the multiplication maps for
                             performance (in some cases).
-        @param alpha: Alpha value for GEMM.
-        @param beta: Beta value for GEMM.
-        @param A_index: Slice of matrix A to use for multiplication.
-        @param B_index: Slice of matrix B to use for multiplication.
-        @param C_index: Slice of matrix C to use for multiplication.
-        @param label: Optional label for the maps and tasklet.
+        :param alpha: Alpha value for GEMM.
+        :param beta: Beta value for GEMM.
+        :param A_index: Slice of matrix A to use for multiplication.
+        :param B_index: Slice of matrix B to use for multiplication.
+        :param C_index: Slice of matrix C to use for multiplication.
+        :param label: Optional label for the maps and tasklet.
     """
 
     # Validate input
     sdfg = state.parent
     map_ranges, A_ranges, B_ranges, C_ranges = validate_matrix_multiplication(
         A_node.desc(sdfg).shape,
         B_node.desc(sdfg).shape,
@@ -799,30 +795,30 @@
                               interchange: bool = True,
                               A_index: Index = None,
                               B_index: Index = None,
                               C_index: Index = None,
                               label: str = None):
     """ Adds a matrix multiplication operation to an existing SDFG state,
         using MKL as the implementation.
-        @param A_src: The source node from which the memlet of matrix A is
+        :param A_src: The source node from which the memlet of matrix A is
                       connected.
-        @param A_node: The Access Node for matrix A.
-        @param B_src: The source node from which the memlet of matrix B is
+        :param A_node: The Access Node for matrix A.
+        :param B_src: The source node from which the memlet of matrix B is
                       connected.
-        @param B_node: The Access Node for matrix B.
-        @param C_dst: The destination node to which the memlet of matrix C is
+        :param B_node: The Access Node for matrix B.
+        :param C_dst: The destination node to which the memlet of matrix C is
                       connected.
-        @param C_node: The Access Node for matrix C.
-        @param accumulate: Whether to accumulate to C or store to it.
-        @param interchange: If True, interchanges the multiplication maps for
+        :param C_node: The Access Node for matrix C.
+        :param accumulate: Whether to accumulate to C or store to it.
+        :param interchange: If True, interchanges the multiplication maps for
                             performance (in some cases).
-        @param A_index: Slice of matrix A to use for multiplication.
-        @param B_index: Slice of matrix B to use for multiplication.
-        @param C_index: Slice of matrix C to use for multiplication.
-        @param label: Optional label for the maps and tasklet.
+        :param A_index: Slice of matrix A to use for multiplication.
+        :param B_index: Slice of matrix B to use for multiplication.
+        :param C_index: Slice of matrix C to use for multiplication.
+        :param label: Optional label for the maps and tasklet.
     """
 
     # Validate input
     sdfg = state.parent
     map_ranges, A_ranges, B_ranges, C_ranges = validate_matrix_multiplication(
         A_node.desc(sdfg).shape,
         B_node.desc(sdfg).shape,
```

### Comparing `dace-0.9.0/dace/frontend/common/op_repository.py` & `dace-0.9.5/dace/frontend/common/op_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,35 +32,35 @@
                                     implementation)]
 
 
 @paramdec
 def replaces(func: Callable[..., Tuple[str]], name: str,
              implementation='sdfg'):
     """ Registers a replacement sub-SDFG generator for a function.
-        @param func: A function that receives an SDFG, SDFGState, and the original function
+        :param func: A function that receives an SDFG, SDFGState, and the original function
                      arguments, returning a tuple of array names to connect to the outputs.
-        @param name: Full name (pydoc-compliant, including package) of function to replace.
-        @param implementation: The default implementation to replace the SDFG with.
+        :param name: Full name (pydoc-compliant, including package) of function to replace.
+        :param implementation: The default implementation to replace the SDFG with.
     """
     Replacements._rep[(name, implementation)] = func
     return func
 
 
 @paramdec
 def replaces_operator(func: Callable[[Any, Any, str, str], Tuple[str]],
                       classname: str,
                       optype: str,
                       implementation='sdfg',
                       otherclass: str = None):
     """ Registers a replacement sub-SDFG generator for an operator.
-        @param func: A function that receives an SDFG, SDFGState, and the two operand array names,
+        :param func: A function that receives an SDFG, SDFGState, and the two operand array names,
                      returning a tuple of array names to connect to the outputs.
-        @param classname: The name of the class to implement the operator for (extends dace.Data).
-        @param optype: The type (as string) of the operator to replace (extends ast.operator).
-        @param implementation: The default implementation to replace the SDFG with.
-        @param otherclass: Optional argument defining operators for a second class that
+        :param classname: The name of the class to implement the operator for (extends dace.Data).
+        :param optype: The type (as string) of the operator to replace (extends ast.operator).
+        :param implementation: The default implementation to replace the SDFG with.
+        :param otherclass: Optional argument defining operators for a second class that
                            differs from the first.
     """
     if otherclass is None:
         otherclass = classname
     Replacements._oprep[(classname, otherclass, optype, implementation)] = func
     return func
```

### Comparing `dace-0.9.0/dace/frontend/octave/ast_arrayaccess.py` & `dace-0.9.5/dace/frontend/octave/ast_arrayaccess.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,16 @@
         return (vardef.get_basetype())
 
     def get_dims(self):
         from .ast_matrix import AST_Matrix
         from .ast_loop import AST_ForLoop
         from .ast_values import AST_Constant, AST_Ident
         from .ast_range import AST_RangeExpression
-        # array indexing has many forms/cases in matlab and does not seem to
-        # be fully documented, the idea is to implement the simple things
-        # we are sure about and bail out on anything that looks different
+        # array indexing has many forms/cases in matlab, here we implement
+        # the semantics we are sure about
         dims = []
         if isinstance(self.accdims, list):
             for acc in self.accdims:
                 if isinstance(acc, AST_Constant):
                     dims.append(1)
                 elif isinstance(acc, AST_Matrix):
                     dims.append(len(acc.get_values_row_major()))
```

### Comparing `dace-0.9.0/dace/frontend/octave/ast_assign.py` & `dace-0.9.5/dace/frontend/octave/ast_assign.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/frontend/octave/ast_expression.py` & `dace-0.9.5/dace/frontend/octave/ast_expression.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/frontend/octave/ast_function.py` & `dace-0.9.5/dace/frontend/octave/ast_function.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/frontend/octave/ast_loop.py` & `dace-0.9.5/dace/frontend/octave/ast_loop.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/frontend/octave/ast_matrix.py` & `dace-0.9.5/dace/frontend/octave/ast_matrix.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/frontend/octave/ast_node.py` & `dace-0.9.5/dace/frontend/octave/ast_node.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/frontend/octave/ast_nullstmt.py` & `dace-0.9.5/dace/frontend/octave/ast_nullstmt.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/frontend/octave/ast_range.py` & `dace-0.9.5/dace/frontend/octave/ast_range.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/frontend/octave/ast_values.py` & `dace-0.9.5/dace/frontend/octave/ast_values.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/frontend/octave/lexer.py` & `dace-0.9.5/dace/frontend/octave/lexer.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/frontend/octave/parse.py` & `dace-0.9.5/dace/frontend/octave/parse.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/frontend/operations.py` & `dace-0.9.5/dace/frontend/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 from dace import dtypes
 from dace.config import Config
 
 
 def timethis(program, title, flop_count, f, *args, **kwargs):
     """ Runs a function multiple (`DACE_treps`) times, logs the running times 
         to a file, and prints the median time (with FLOPs if given).
-        @param program: The title of the measurement.
-        @param title: A sub-title of the measurement.
-        @param flop_count: Number of floating point operations in `program`.
+        :param program: The title of the measurement.
+        :param title: A sub-title of the measurement.
+        :param flop_count: Number of floating point operations in `program`.
                            If greater than zero, produces a median FLOPS 
                            report.
-        @param f: The function to measure.
-        @param args: Arguments to invoke the function with.
-        @param kwargs: Keyword arguments to invoke the function with.
-        @return: Latest return value of the function.
+        :param f: The function to measure.
+        :param args: Arguments to invoke the function with.
+        :param kwargs: Keyword arguments to invoke the function with.
+        :return: Latest return value of the function.
     """
 
     start = timer()
     REPS = int(Config.get('treps'))
     times = [start] * (REPS + 1)
     ret = None
     for i in range(REPS):
@@ -59,16 +59,16 @@
     return ret
 
 
 def detect_reduction_type(wcr_str):
     """ Inspects a lambda function and tries to determine if it's one of the 
         built-in reductions that frameworks such as MPI can provide.
 
-        @param wcr_str: A Python string representation of the lambda function.
-        @return: dtypes.ReductionType if detected, dtypes.ReductionType.Custom
+        :param wcr_str: A Python string representation of the lambda function.
+        :return: dtypes.ReductionType if detected, dtypes.ReductionType.Custom
                  if not detected, or None if no reduction is found.
     """
     if wcr_str == '' or wcr_str is None:
         return None
 
     # Get lambda function from string
     wcr = eval(wcr_str)
@@ -112,16 +112,16 @@
 
     return dtypes.ReductionType.Custom
 
 
 def is_op_commutative(wcr_str):
     """ Inspects a custom lambda function and tries to determine whether
         it is symbolically commutative (disregarding data type).
-        @param wcr_str: A string in Python representing a lambda function.
-        @return: True if commutative, False if not, None if cannot be 
+        :param wcr_str: A string in Python representing a lambda function.
+        :return: True if commutative, False if not, None if cannot be
                  determined.
     """
     if wcr_str == '' or wcr_str is None:
         return None
 
     # Get lambda function from string
     wcr = eval(wcr_str)
@@ -138,16 +138,16 @@
 
     return aRb == bRa
 
 
 def is_op_associative(wcr_str):
     """ Inspects a custom lambda function and tries to determine whether
         it is symbolically associative (disregarding data type).
-        @param wcr_str: A string in Python representing a lambda function.
-        @return: True if associative, False if not, None if cannot be 
+        :param wcr_str: A string in Python representing a lambda function.
+        :return: True if associative, False if not, None if cannot be
                  determined.
     """
     if wcr_str == '' or wcr_str is None:
         return None
 
     # Get lambda function from string
     wcr = eval(wcr_str)
```

### Comparing `dace-0.9.0/dace/frontend/python/astnodes.py` & `dace-0.9.5/dace/frontend/python/astnodes.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/frontend/python/astutils.py` & `dace-0.9.5/dace/frontend/python/astutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from typing import Any, Dict, List, Tuple
 
 from dace import dtypes, symbolic
 
 
 def _remove_outer_indentation(src: str):
     """ Removes extra indentation from a source Python function.
-        @param src: Source code (possibly indented).
-        @return: Code after de-indentation.
+        :param src: Source code (possibly indented).
+        :return: Code after de-indentation.
     """
     lines = src.split('\n')
     indentation = len(lines[0]) - len(lines[0].lstrip())
     return '\n'.join([line[indentation:] for line in lines])
 
 
 def function_to_ast(f):
     """ Obtain the source code of a Python function and create an AST.
-        @param f: Python function.
-        @return: A 4-tuple of (AST, function filename, function line-number,
+        :param f: Python function.
+        :return: A 4-tuple of (AST, function filename, function line-number,
                                source code as string).
     """
     try:
         src = inspect.getsource(f)
     # TypeError: X is not a module, class, method, function, traceback, frame,
     # or code object; OR OSError: could not get source code
     except (TypeError, OSError):
@@ -168,16 +168,16 @@
         'Invalid expression, expected tuple of constant numbers or None')
 
 
 def subscript_to_ast_slice(node, without_array=False):
     """ Converts an AST subscript to slice on the form
         (<name>, [<3-tuples of AST nodes>]). If an ast.Name is passed, returns
         (name, None), implying the full range. 
-        @param node: The AST node to convert.
-        @param without_array: If True, returns only the slice. Otherwise,
+        :param node: The AST node to convert.
+        :param without_array: If True, returns only the slice. Otherwise,
                               returns a 2-tuple of (array, range).
     """
 
     result_arr = None
     result_slice = None
 
     if isinstance(node, ast.Name):
```

### Comparing `dace-0.9.0/dace/frontend/python/decorators.py` & `dace-0.9.5/dace/frontend/python/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,28 +23,28 @@
 
 # Dataflow constructs
 @paramdec
 def map(f, rng):
     """ A Map is representation of parallel execution, containing
         an integer set (Python range) for which its contents are run 
         concurrently.
-        @param rng: The map's range.
+        :param rng: The map's range.
     """
     return None
 
 
 @paramdec
 def consume(f, stream, pes):
     """ Consume is a scope, like `Map`, that creates parallel execution.
         Unlike `Map`, it creates a producer-consumer relationship between an
         input stream and the contents. The contents are run by the given number
         of processing elements, who will try to pop elements from the input
         stream until a given quiescence condition is reached. 
-        @param stream: The stream to pop from.
-        @param pes: The number of processing elements to use.
+        :param stream: The stream to pop from.
+        :param pes: The number of processing elements to use.
     """
     return None
 
 
 def tasklet(f):
     """ A general procedure that cannot access any memory apart from incoming
         and outgoing memlets. The DaCe framework cannot analyze these tasklets
@@ -52,27 +52,27 @@
     return None
 
 
 # Control-flow constructs
 @paramdec
 def iterate(f, rng):
     """ A decorator version of a for loop, with a range of `rng`.
-        @param rng: The range of the for loop.
+        :param rng: The range of the for loop.
     """
     return None
 
 
 @paramdec
 def loop(f, cond):
     """ A decorator version of a while loop, with a looping condition `cond`.
-        @param cond: The condition of the while loop.
+        :param cond: The condition of the while loop.
     """
     return None
 
 
 @paramdec
 def conditional(f, cond):
     """ A decorator version of conditional execution, with an if-condition 
         `cond`.
-        @param cond: The condition of the branch.
+        :param cond: The condition of the branch.
     """
     return None
```

### Comparing `dace-0.9.0/dace/frontend/python/ndloop.py` & `dace-0.9.5/dace/frontend/python/ndloop.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ A single generator that creates an N-dimensional for loop in Python. """
 import itertools
-from dace.frontend.python import ndarray
+import numpy as np
 
 # Python 3 compatibility for xrange
 try:
     xxrange = xrange
 except NameError:
     xxrange = range
 
@@ -21,42 +21,42 @@
 
 def tupletoxrange(s):
     """ Helper function that turns a tuple into a range (for iteration). """
     if isinstance(s, int):
         return xxrange(s, s + 1)
 
     ifnone = lambda a, b: b if a is None else a
-    ifscalar = lambda a: a[0] if isinstance(a, ndarray.ndarray) else a
+    ifscalar = lambda a: a[0] if isinstance(a, np.ndarray) else a
     allconds = lambda a, b: ifnone(ifscalar(a), b)
 
     return xxrange(allconds(s[0], 0), ifscalar(s[1]) + 1, allconds(s[2], 1))
 
 
 def NDLoop(ndslice, internal_function, *args, **kwargs):
     """ Wrapped generator that calls an internal function in an N-dimensional 
         for-loop in Python. 
-        @param ndslice: Slice or list of slices (`slice` objects) to loop over.
-        @param internal_function: Function to call in loop.
-        @param *args: Arguments to `internal_function`.
-        @param **kwargs: Keyword arguments to `internal_function`.
-        @return: N-dimensional loop index generator.
+        :param ndslice: Slice or list of slices (`slice` objects) to loop over.
+        :param internal_function: Function to call in loop.
+        :param *args: Arguments to `internal_function`.
+        :param **kwargs: Keyword arguments to `internal_function`.
+        :return: N-dimensional loop index generator.
     """
     if isinstance(ndslice, int) or isinstance(ndslice, slice):
         ndxrange = (slicetoxrange(ndslice), )
     else:
         ndxrange = tuple(slicetoxrange(d) for d in ndslice)
     for indices in itertools.product(*ndxrange):
         internal_function(*(indices + args), **kwargs)
 
 
 def ndrange(slice_list):
     """ Generator that creates an N-dimensional for loop in Python. 
-        @param slice_list: Slice or list of slices (as tuples or `slice`s)
+        :param slice_list: Slice or list of slices (as tuples or `slice`s)
                           to loop over.
-        @return: N-dimensional loop index generator.
+        :return: N-dimensional loop index generator.
     """
     if not isinstance(slice_list, list):
         ndxrange = (tupletoxrange(slice_list), )
     else:
         ndxrange = tuple(tupletoxrange(d) for d in slice_list)
 
     for indices in itertools.product(*ndxrange):
```

### Comparing `dace-0.9.0/dace/frontend/python/newast.py` & `dace-0.9.5/dace/frontend/python/newast.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import ast
 from collections import OrderedDict, namedtuple
 import copy
+from functools import reduce
 import re
 from typing import Any, Dict, List, Tuple, Union, Callable
+import warnings
 
 import dace
 from dace import data, dtypes, subsets, symbolic
 from dace.config import Config
 from dace.frontend.common import op_impl
 from dace.frontend.common import op_repository as oprepo
 from dace.frontend.python import astutils
@@ -86,15 +88,15 @@
             redfunction: Callable[[Any, Any], Any],
             input: str,
             output=None,
             axis=None,
             identity=None):
     # TODO(later): If output is None, derive the output size from the input and create a new node
     if output is None:
-        inarr = until(input, '[')
+        inarr = input
         # Convert axes to tuple
         if axis is not None and not isinstance(axis, (tuple, list)):
             axis = (axis, )
         if axis is not None:
             axis = tuple(pystr_to_symbolic(a) for a in axis)
         input_subset = _parse_memlet_subset(sdfg.arrays[inarr],
                                             ast.parse(input).body[0].value, {})
@@ -107,16 +109,16 @@
             output_subset = copy.deepcopy(input_subset)
             output_subset.pop(axis)
             output_shape = output_subset.size()
         outarr, arr = sdfg.add_temp_transient(
             output_shape, sdfg.arrays[inarr].dtype, sdfg.arrays[inarr].storage)
         output_memlet = Memlet.from_array(outarr, arr)
     else:
-        inarr = until(input, '[')
-        outarr = until(output, '[')
+        inarr = input
+        outarr = output
 
         # Convert axes to tuple
         if axis is not None and not isinstance(axis, (tuple, list)):
             axis = (axis, )
         if axis is not None:
             axis = tuple(pystr_to_symbolic(a) for a in axis)
 
@@ -140,14 +142,129 @@
 
     if output is None:
         return outarr
     else:
         return []
 
 
+def _simple_call(sdfg: SDFG,
+                 state: SDFGState,
+                 inpname: str,
+                 func: str,
+                 restype: dace.typeclass = None):
+    """ Implements a simple call of the form `out = func(inp)`. """
+    inparr = sdfg.arrays[inpname]
+    if restype is None:
+        restype = sdfg.arrays[inpname].dtype
+    outname, outarr = sdfg.add_temp_transient(inparr.shape, restype,
+                                              inparr.storage)
+    num_elements = reduce(lambda x, y: x * y, inparr.shape)
+    if num_elements == 1:
+        inp = state.add_read(inpname)
+        out = state.add_write(outname)
+        tasklet = state.add_tasklet(
+            func, {'__inp'}, {'__out'}, '__out = {f}(__inp)'.format(f=func))
+        state.add_edge(inp, None, tasklet, '__inp',
+                       Memlet.from_array(inpname, inparr))
+        state.add_edge(tasklet, '__out', out, None,
+                       Memlet.from_array(outname, outarr))
+    else:
+        state.add_mapped_tasklet(
+            name=func,
+            map_ranges={
+                '__i%d' % i: '0:%s' % n
+                for i, n in enumerate(inparr.shape)
+            },
+            inputs={
+                '__inp':
+                Memlet.simple(
+                    inpname,
+                    ','.join(['__i%d' % i for i in range(len(inparr.shape))]))
+            },
+            code='__out = {f}(__inp)'.format(f=func),
+            outputs={
+                '__out':
+                Memlet.simple(
+                    outname,
+                    ','.join(['__i%d' % i for i in range(len(inparr.shape))]))
+            },
+            external_edges=True)
+
+    return outname
+
+
+def _complex_to_scalar(complex_type: dace.typeclass):
+    if complex_type is dace.complex64:
+        return dace.float32
+    elif complex_type is dace.complex128:
+        return dace.float64
+    else:
+        return complex_type
+
+
+@oprepo.replaces('exp')
+@oprepo.replaces('dace.exp')
+@oprepo.replaces('numpy.exp')
+def _exp(sdfg: SDFG, state: SDFGState, input: str):
+    return _simple_call(sdfg, state, input, 'exp')
+
+
+@oprepo.replaces('sin')
+@oprepo.replaces('dace.sin')
+@oprepo.replaces('numpy.sin')
+def _sin(sdfg: SDFG, state: SDFGState, input: str):
+    return _simple_call(sdfg, state, input, 'sin')
+
+
+@oprepo.replaces('cos')
+@oprepo.replaces('dace.cos')
+@oprepo.replaces('numpy.cos')
+def _cos(sdfg: SDFG, state: SDFGState, input: str):
+    return _simple_call(sdfg, state, input, 'cos')
+
+
+@oprepo.replaces('sqrt')
+@oprepo.replaces('dace.sqrt')
+@oprepo.replaces('numpy.sqrt')
+def _sqrt(sdfg: SDFG, state: SDFGState, input: str):
+    return _simple_call(sdfg, state, input, 'sqrt')
+
+
+@oprepo.replaces('log')
+@oprepo.replaces('dace.log')
+@oprepo.replaces('numpy.log')
+def _log(sdfg: SDFG, state: SDFGState, input: str):
+    return _simple_call(sdfg, state, input, 'log')
+
+
+@oprepo.replaces('conj')
+@oprepo.replaces('dace.conj')
+@oprepo.replaces('numpy.conj')
+def _conj(sdfg: SDFG, state: SDFGState, input: str):
+    return _simple_call(sdfg, state, input, 'conj')
+
+
+@oprepo.replaces('real')
+@oprepo.replaces('dace.real')
+@oprepo.replaces('numpy.real')
+def _real(sdfg: SDFG, state: SDFGState, input: str):
+    inptype = sdfg.arrays[input].dtype
+    return _simple_call(sdfg, state, input, 'real',
+                        _complex_to_scalar(inptype))
+
+
+@oprepo.replaces('imag')
+@oprepo.replaces('dace.imag')
+@oprepo.replaces('numpy.imag')
+def _imag(sdfg: SDFG, state: SDFGState, input: str):
+    inptype = sdfg.arrays[input].dtype
+    return _simple_call(sdfg, state, input, 'imag',
+                        _complex_to_scalar(inptype))
+
+
 ##############################################################################
 # Python operation replacements ##############################################
 ##############################################################################
 
 
 def _assignop(sdfg: SDFG, state: SDFGState, op1: str, opcode: str,
               opname: str):
@@ -164,38 +281,38 @@
     else:
         write_memlet = Memlet.simple(
             name, ','.join(['__i%d' % i for i in range(len(arr1.shape))]))
     state.add_mapped_tasklet(
         "_%s_" % opname,
         {'__i%d' % i: '0:%s' % s
          for i, s in enumerate(arr1.shape)}, {
-             'in1':
+             '__in1':
              Memlet.simple(
                  op1, ','.join(['__i%d' % i for i in range(len(arr1.shape))]))
          },
-        'out = in1', {'out': write_memlet},
+        '__out = __in1', {'__out': write_memlet},
         external_edges=True)
     return name
 
 
 def _unop(sdfg: SDFG, state: SDFGState, op1: str, opcode: str, opname: str):
     """ Implements a general element-wise array unary operator. """
     arr1 = sdfg.arrays[op1]
 
     name, _ = sdfg.add_temp_transient(arr1.shape, arr1.dtype, arr1.storage)
     state.add_mapped_tasklet(
         "_%s_" % opname,
         {'__i%d' % i: '0:%s' % s
          for i, s in enumerate(arr1.shape)}, {
-             'in1':
+             '__in1':
              Memlet.simple(
                  op1, ','.join(['__i%d' % i for i in range(len(arr1.shape))]))
          },
-        'out = %s in1' % opcode, {
-            'out':
+        '__out = %s __in1' % opcode, {
+            '__out':
             Memlet.simple(
                 name, ','.join(['__i%d' % i for i in range(len(arr1.shape))]))
         },
         external_edges=True)
     return name
 
 
@@ -209,23 +326,23 @@
         raise SyntaxError('Array sizes must match')
 
     name, _ = sdfg.add_temp_transient(arr1.shape, restype, arr1.storage)
     state.add_mapped_tasklet(
         "_%s_" % opname,
         {'__i%d' % i: '0:%s' % s
          for i, s in enumerate(arr1.shape)}, {
-             'in1':
+             '__in1':
              Memlet.simple(
                  op1, ','.join(['__i%d' % i for i in range(len(arr1.shape))])),
-             'in2':
+             '__in2':
              Memlet.simple(
                  op2, ','.join(['__i%d' % i for i in range(len(arr1.shape))]))
          },
-        'out = in1 %s in2' % opcode, {
-            'out':
+        '__out = __in1 %s __in2' % opcode, {
+            '__out':
             Memlet.simple(
                 name, ','.join(['__i%d' % i for i in range(len(arr1.shape))]))
         },
         external_edges=True)
     return name
 
 
@@ -242,25 +359,25 @@
     arr = sdfg.arrays[arrop]
 
     name, _ = sdfg.add_temp_transient(arr.shape, restype, arr.storage)
     state.add_mapped_tasklet(
         "_SA%s_" % opname,
         {'__i%d' % i: '0:%s' % s
          for i, s in enumerate(arr.shape)}, {
-             'in1':
+             '__in1':
              Memlet.simple(scalop, '0'),
-             'in2':
+             '__in2':
              Memlet.simple(
                  arrop, ','.join(['__i%d' % i
                                   for i in range(len(arr.shape))])),
          },
-        'out = %s %s %s' % ('in2' if reverse else 'in1', opcode, 'in1'
-                            if reverse else 'in2'),
+        '__out = %s %s %s' % ('__in2' if reverse else '__in1', opcode, '__in1'
+                              if reverse else '__in2'),
         {
-            'out':
+            '__out':
             Memlet.simple(
                 name, ','.join(['__i%d' % i for i in range(len(arr.shape))]))
         },
         external_edges=True)
     return name
 
 
@@ -431,28 +548,32 @@
 
     arr1 = sdfg.arrays[op1]
     arr2 = sdfg.arrays[op2]
     if (len(arr1.shape) != 2 or len(arr2.shape) != 2
             or arr1.shape[1] != arr2.shape[0]):
         raise SyntaxError('Matrix sizes must match')
 
+    type1 = arr1.dtype.type
+    type2 = arr2.dtype.type
+    restype = dace.DTYPE_TO_TYPECLASS[np.result_type(type1, type2).type]
+
     op3, arr3 = sdfg.add_temp_transient((arr1.shape[0], arr2.shape[1]),
-                                        arr1.dtype, arr1.storage)
+                                        restype, arr1.storage)
 
     state.add_mapped_tasklet(
         '_MatMult_', {
             '__i%d' % i: '0:%s' % s
             for i, s in enumerate(
                 [arr1.shape[0], arr2.shape[1], arr1.shape[1]])
         }, {
-            'a': Memlet.simple(op1, '__i0, __i2'),
-            'b': Memlet.simple(op2, '__i2, __i1')
+            '__a': Memlet.simple(op1, '__i0, __i2'),
+            '__b': Memlet.simple(op2, '__i2, __i1')
         },
-        'c = a * b', {
-            'c':
+        '__c = __a * __b', {
+            '__c':
             Memlet.simple(
                 op3,
                 '__i0, __i1',
                 wcr_str='lambda x, y: x + y',
                 wcr_identity=0)
         },
         external_edges=True)
@@ -469,26 +590,26 @@
 
 ############################################
 
 
 def parse_dace_program(f, argtypes, global_vars, modules, other_sdfgs,
                        constants):
     """ Parses a `@dace.program` function into a _ProgramNode object.
-        @param f: A Python function to parse.
-        @param argtypes: An dictionary of (name, type) for the given
+        :param f: A Python function to parse.
+        :param argtypes: An dictionary of (name, type) for the given
                          function's arguments, which may pertain to data
                          nodes or symbols (scalars).
-        @param global_vars: A dictionary of global variables in the closure
+        :param global_vars: A dictionary of global variables in the closure
                             of `f`.
-        @param modules: A dictionary from an imported module name to the
+        :param modules: A dictionary from an imported module name to the
                         module itself.
-        @param other_sdfgs: Other SDFG and DaceProgram objects in the context
+        :param other_sdfgs: Other SDFG and DaceProgram objects in the context
                             of this function.
-        @param constants: A dictionary from a name to a constant value.
-        @return: Hierarchical tree of `astnodes._Node` objects, where the top
+        :param constants: A dictionary from a name to a constant value.
+        :return: Hierarchical tree of `astnodes._Node` objects, where the top
                  level node is an `astnodes._ProgramNode`.
         @rtype: SDFG
     """
     src_ast, src_file, src_line, src = astutils.function_to_ast(f)
 
     # Resolve symbols to their names
     symrepl = {
@@ -659,18 +780,18 @@
         return pystr_to_symbolic(code)
 
 
 def _pyexpr_to_symbolic(defined_arrays_and_symbols: Dict[str, Any],
                         expr_ast: ast.AST):
     """ Converts a Python AST expression to a DaCe symbolic expression
         with error checks (raises `SyntaxError` on failure).
-        @param defined_arrays_and_symbols: Defined arrays and symbols
+        :param defined_arrays_and_symbols: Defined arrays and symbols
                in the context of this expression.
-        @param expr_ast: The Python AST expression to convert.
-        @return: Symbolic expression.
+        :param expr_ast: The Python AST expression to convert.
+        :return: Symbolic expression.
     """
     # TODO!
     return _inner_eval_ast(defined_arrays_and_symbols, expr_ast)
 
 
 def _ndslice_to_subset(ndslice):
     is_tuple = [isinstance(x, tuple) for x in ndslice]
@@ -851,17 +972,22 @@
             dim = [dim]
         for r in dim:
             if symbolic.contains_sympy_functions(r):
                 return True
     return False
 
 
-def add_indirection_subgraph(sdfg: SDFG, graph: SDFGState, src: nodes.Node,
-                             dst: nodes.Node, memlet: Memlet, local_name: str,
-                             PVisitor):
+def add_indirection_subgraph(sdfg: SDFG,
+                             graph: SDFGState,
+                             src: nodes.Node,
+                             dst: nodes.Node,
+                             memlet: Memlet,
+                             local_name: str,
+                             PVisitor,
+                             output: bool = False):
     """ Replaces the specified edge in the specified graph with a subgraph that
         implements indirection without nested memlet subsets. """
 
     array = sdfg.arrays[memlet.data]
     indirect_inputs = set()
     indirect_outputs = set()
 
@@ -907,105 +1033,225 @@
                     else:
                         rng = list(newsubset[dimidx])
                         rng[i] = rng[i].subs(expr, toreplace)
                         newsubset[dimidx] = tuple(rng)
                         # newsubset[dimidx][i] = r.subs(expr, toreplace)
     #########################
     # Step 2
-    ind_inputs = {'__ind_' + local_name}
-    ind_outputs = {'lookup'}
+    if output:
+        ind_inputs = {'lookup'}
+        ind_outputs = {'__ind_' + local_name}
+    else:
+        ind_inputs = {'__ind_' + local_name}
+        ind_outputs = {'lookup'}
     # Add accesses to inputs
     for arrname, arr_accesses in accesses.items():
         for i in range(len(arr_accesses)):
             ind_inputs.add('index_%s_%d' % (arrname, i))
 
     tasklet = nodes.Tasklet("Indirection", ind_inputs, ind_outputs)
 
+    # Create map if indirected subset is a range
+    ind_entry = None
+    ind_exit = None
+    inp_base_path = [tasklet]
+    out_base_path = [tasklet]
+    if (isinstance(memlet.subset, subsets.Range)
+            and memlet.subset.num_elements() != 1):
+        rng = copy.deepcopy(memlet.subset)
+        nonsqz_dims = rng.squeeze()
+        ind_entry, ind_exit = graph.add_map(
+            'indirection', {
+                '__i%d' % i: '%s:%s+1:%s' % (s, e, t)
+                for i, (s, e, t) in enumerate(rng)
+            })
+        inp_base_path.insert(0, ind_entry)
+        out_base_path.append(ind_exit)
+
     input_index_memlets = []
     for arrname, arr_accesses in accesses.items():
         arr_name = arrname
         for i, access in enumerate(arr_accesses):
             if isinstance(access, (list, tuple)):
                 access = access[0]
             if isinstance(access, sympy.Tuple):
                 access = list(access)
             if not isinstance(access, (list, tuple)):
                 access = [access]
             conn = None
             if PVisitor.nested:
                 arr_rng = dace.subsets.Range([(a, a, 1) for a in access])
-                # arrname, _ = PVisitor._add_read_access(
-                #     arr_name, arr_rng, target=None)
-                arrname = PVisitor._add_read_access(
-                    arr_name, arr_rng, target=None)
+                if output:
+                    arrname = PVisitor._add_write_access(
+                        arr_name, arr_rng, target=None)
+                else:
+                    arrname = PVisitor._add_read_access(
+                        arr_name, arr_rng, target=None)
                 access = [0] * len(access)
                 conn = 'index_%s_%d' % (arr_name, i)
             arr = sdfg.arrays[arrname]
             # Memlet to load the indirection index
             indexMemlet = Memlet(arrname, 1, subsets.Indices(access), 1)
             input_index_memlets.append(indexMemlet)
             read_node = graph.add_read(arrname)
-            if PVisitor.nested:
-                path = [read_node, tasklet]
+            if PVisitor.nested or not isinstance(src, nodes.EntryNode):
+                path = [read_node] + inp_base_path
             else:
-                path = [read_node, src, tasklet]
+                if output:
+                    # TODO: This only works for Maps. Perhaps it should be
+                    # generalized for other pairs of entry/exit nodes.
+                    entry = None
+                    if isinstance(dst, nodes.MapExit):
+                        for node in graph.nodes():
+                            if (isinstance(node, nodes.MapEntry)
+                                    and node.map is dst.map):
+                                entry = node
+                                break
+                    else:
+                        raise NotImplementedError
+                else:
+                    entry = src
+                path = [read_node, entry] + inp_base_path
             graph.add_memlet_path(
                 *path,
                 dst_conn="index_%s_%d" % (arr_name, i),
                 memlet=indexMemlet)
 
     #########################
     # Step 3
     # Create new tasklet that will perform the indirection
-    tasklet.code = "lookup = {arr}[{index}]".format(
+    if output:
+        code = "{arr}[{index}] = lookup"
+    else:
+        code = "lookup = {arr}[{index}]"
+
+    newsubset = [r[0] if isinstance(r, tuple) else r for r in newsubset]
+    if ind_entry:  # Amend newsubset when a range is indirected
+        for i, idx in enumerate(nonsqz_dims):
+            newsubset[idx] = '__i%d' % i
+
+    tasklet.code = code.format(
         arr='__ind_' + local_name,
         index=', '.join([symbolic.symstr(s) for s in newsubset]))
 
     # Create transient variable to trigger the indirect load
-    if memlet.num_accesses == 1:
-        storage = sdfg.add_scalar(
-            '__' + local_name + '_value', array.dtype, transient=True)
+    tmp_name = '__' + local_name + '_value'
+    start_src = None
+    end_dst = None
+    if memlet.num_accesses == 1 and dst is not None:
+        _, storage = sdfg.add_scalar(tmp_name, array.dtype, transient=True)
     else:
-        storage = sdfg.add_array(
-            '__' + local_name + '_value',
-            memlet.bounding_box_size(),
+        rng = copy.deepcopy(memlet.subset)
+        if isinstance(rng, subsets.Range):
+            rng.squeeze()
+        _, storage = sdfg.add_array(
+            tmp_name,
+            rng.bounding_box_size(),
             array.dtype,
             storage=dtypes.StorageType.Default,
             transient=True)
-    indirectRange = subsets.Range([(0, s - 1, 1) for s in storage.shape])
-    # dataNode = nodes.AccessNode('__' + local_name + '_value')
+        # Force creation of transients for range indirection
+        if output:
+            if src:
+                start_src = src
+                src = None
+        else:
+            if dst:
+                end_dst = dst
+                dst = None
+
+    # Create transients when implementing indirection
+    # through slicing or when indirecting a range.
+    if src is None:
+        if start_src:
+            src = graph.add_access(tmp_name)
+        else:
+            src = graph.add_read(tmp_name)
+    elif dst is None:
+        if end_dst:
+            dst = graph.add_access(tmp_name)
+        else:
+            dst = graph.add_write(tmp_name)
+
+    tmp_shape = storage.shape
+    indirectRange = subsets.Range([(0, s - 1, 1) for s in tmp_shape])
+    if ind_entry:  # Amend indirected range
+        indirectRange = ','.join([ind for ind in ind_entry.map.params])
 
     # Create memlet that depends on the full array that we look up in
     fullRange = subsets.Range([(0, s - 1, 1) for s in array.shape])
     fullMemlet = Memlet(memlet.data, memlet.num_accesses, fullRange,
                         memlet.veclen)
 
-    if isinstance(src, nodes.EntryNode):
-        full_read_node = graph.add_read(memlet.data)
-        graph.add_memlet_path(
-            full_read_node,
-            src,
-            tasklet,
-            dst_conn='__ind_' + local_name,
-            memlet=fullMemlet)
-    elif isinstance(src, nodes.AccessNode):
+    if output:
+        if isinstance(dst, nodes.ExitNode):
+            full_write_node = graph.add_write(memlet.data)
+            path = out_base_path + [dst, full_write_node]
+        elif isinstance(dst, nodes.AccessNode):
+            path = out_base_path + [dst]
+        else:
+            raise Exception("Src node type for indirection is invalid.")
         graph.add_memlet_path(
-            src, tasklet, dst_conn='__ind_' + local_name, memlet=fullMemlet)
+            *path, src_conn='__ind_' + local_name, memlet=fullMemlet)
     else:
-        raise Exception("Src node type for indirection is invalid.")
+        if isinstance(src, nodes.EntryNode):
+            full_read_node = graph.add_read(memlet.data)
+            path = [full_read_node, src] + inp_base_path
+        elif isinstance(src, nodes.AccessNode):
+            path = [src] + inp_base_path
+        else:
+            raise Exception("Src node type for indirection is invalid.")
+        graph.add_memlet_path(
+            *path, dst_conn='__ind_' + local_name, memlet=fullMemlet)
 
     # Memlet to store the final value into the transient, and to load it into
     # the tasklet that needs it
     # indirectMemlet = Memlet('__' + local_name + '_value', memlet.num_accesses,
     #                         indirectRange, memlet.veclen)
     # graph.add_edge(tasklet, 'lookup', dataNode, None, indirectMemlet)
 
-    valueMemlet = Memlet('__' + local_name + '_value', memlet.num_accesses,
-                         indirectRange, memlet.veclen)
-    graph.add_edge(tasklet, 'lookup', dst, local_name, valueMemlet)
+    valueMemlet = Memlet(
+        tmp_name,
+        1,  # memlet.num_accesses,
+        indirectRange,
+        memlet.veclen)
+    if output:
+        path = [src] + inp_base_path
+        if isinstance(src, nodes.AccessNode):
+            src_conn = None
+        else:
+            src_conn = local_name
+        graph.add_memlet_path(
+            *path, src_conn=src_conn, dst_conn='lookup', memlet=valueMemlet)
+        # Connect original source to the indirected-range-transient
+        if start_src:
+            if isinstance(start_src, nodes.AccessNode):
+                src_conn = None
+            else:
+                src_conn = local_name
+            graph.add_edge(start_src, src_conn, src, None,
+                           Memlet.from_array(tmp_name, storage))
+    else:
+        path = out_base_path + [dst]
+        if isinstance(dst, nodes.AccessNode):
+            dst_conn = None
+        else:
+            dst_conn = local_name
+        graph.add_memlet_path(
+            *path, src_conn='lookup', dst_conn=dst_conn, memlet=valueMemlet)
+        # Connect original destination to the indirected-range-transient
+        if end_dst:
+            if isinstance(end_dst, nodes.AccessNode):
+                dst_conn = None
+            else:
+                dst_conn = local_name
+            graph.add_edge(dst, None, end_dst, dst_conn,
+                           Memlet.from_array(tmp_name, storage))
+
+    return tmp_name
 
 
 class GlobalResolver(ast.NodeTransformer):
     """ Resolves global constants and lambda expressions if not
         already defined in the given scope. """
 
     def __init__(self, globals: Dict[str, Any]):
@@ -1050,16 +1296,16 @@
                  nested: bool = False,
                  scope_arrays: Dict[str, data.Data] = dict(),
                  scope_vars: Dict[str, str] = dict(),
                  variables: Dict[str, str] = dict(),
                  accesses: Dict[Tuple[str, dace.subsets.Subset, str],
                                 str] = dict()):
         """ Creates an AST parser for tasklets. 
-            @param sdfg: The SDFG to add the tasklet in (used for defined arrays and symbols).
-            @param state: The SDFG state to add the tasklet to.
+            :param sdfg: The SDFG to add the tasklet in (used for defined arrays and symbols).
+            :param state: The SDFG state to add the tasklet to.
         """
         self.sdfg = sdfg
         self.state = state
         self.defined = defined
 
         # For syntax errors
         self.filename = filename
@@ -1086,16 +1332,16 @@
 
         # Disallow keywords
         for stmt in _DISALLOWED_STMTS:
             setattr(self, 'visit_' + stmt, lambda n: _disallow_stmt(self, n))
 
     def parse_tasklet(self, tasklet_ast: TaskletType):
         """ Parses the AST of a tasklet and returns the tasklet node, as well as input and output memlets. 
-            @param tasklet_ast: The Tasklet's Python AST to parse.
-            @return: 3-tuple of (Tasklet node, input memlets, output memlets).
+            :param tasklet_ast: The Tasklet's Python AST to parse.
+            :return: 3-tuple of (Tasklet node, input memlets, output memlets).
             @rtype: Tuple[Tasklet, Dict[str, Memlet], Dict[str, Memlet]]
         """
         # Should return a tasklet object (with connectors)
         self.visit(tasklet_ast)
 
         # Location identifier
         locinfo = dtypes.DebugInfo(tasklet_ast.lineno, tasklet_ast.col_offset,
@@ -1144,15 +1390,18 @@
             squeezed_rng = list(range(len(rng)))
             shape = parent_array.shape
             strides = [parent_array.strides[d] for d in squeezed_rng]
         else:
             squeezed_rng = copy.deepcopy(rng)
             non_squeezed = squeezed_rng.squeeze()
             shape = squeezed_rng.size()
-            strides = [parent_array.strides[d] for d in non_squeezed]
+            if non_squeezed:
+                strides = [parent_array.strides[d] for d in non_squeezed]
+            else:
+                strides = [1]
         dtype = parent_array.dtype
 
         if arr_type is None:
             arr_type = type(parent_array)
         if arr_type == data.Scalar:
             self.sdfg.add_scalar(var_name, dtype)
         elif arr_type == data.Array:
@@ -1172,15 +1421,15 @@
 
         if access_type == 'r':
             if _subset_has_indirection(rng):
                 self.sdfg_inputs[var_name] = (dace.Memlet.from_array(
                     parent_name, parent_array), inner_indices)
             else:
                 self.sdfg_inputs[var_name] = (dace.Memlet(
-                    parent_name,rng.num_elements(), rng, 1), inner_indices)
+                    parent_name, rng.num_elements(), rng, 1), inner_indices)
         else:
             if _subset_has_indirection(rng):
                 self.sdfg_outputs[var_name] = (dace.Memlet.from_array(
                     parent_name, parent_array), inner_indices)
             else:
                 self.sdfg_outputs[var_name] = (dace.Memlet(
                     parent_name, rng.num_elements(), rng, 1), inner_indices)
@@ -1229,15 +1478,18 @@
             rng = dace.subsets.Range(
                 astutils.subscript_to_slice(actual_node, {
                     **self.sdfg.arrays,
                     **self.scope_arrays
                 })[1])
         elif isinstance(node, ast.Subscript):
             actual_node = copy.deepcopy(node)
-            actual_node.value.id = name
+            if isinstance(actual_node.value, ast.Call):
+                actual_node.value.func.id = name
+            else:
+                actual_node.value.id = name
             rng = dace.subsets.Range(
                 astutils.subscript_to_slice(actual_node, {
                     **self.sdfg.arrays,
                     **self.scope_arrays
                 })[1])
         elif isinstance(node, ast.Call):
             rng = dace.subsets.Range.from_array({
@@ -1299,14 +1551,15 @@
                                              rng, 1)
                     if connector in self.inputs or connector in self.outputs:
                         raise DaceSyntaxError(
                             self, node,
                             'Local variable is already a tasklet input or output'
                         )
                     self.inputs[connector] = memlet
+                    return None  # Remove from final tasklet code
                 elif isinstance(node.value.op, ast.RShift):
                     if self.nested:
                         real_name = variables[name]
                         rng = self._get_range(target, real_name)
                         name, squeezed_rng = self._add_write_access(
                             name, rng, target)
                         if squeezed_rng is not None:
@@ -1315,25 +1568,31 @@
                         if name in variables:
                             name = variables[name]
                     node.value.right = self._update_names(
                         node.value.right, name, name_subscript=name_sub)
                     connector, memlet = _parse_memlet(self, node.value.left,
                                                       node.value.right,
                                                       self.sdfg.arrays)
+                    if self.nested and _subset_has_indirection(rng):
+                        memlet = dace.Memlet(memlet.data, rng.num_elements(),
+                                             rng, 1)
                     if self.nested and name in self.sdfg_outputs:
                         out_memlet = self.sdfg_outputs[name][0]
+                        out_memlet.num_accesses = memlet.num_accesses
+                        out_memlet.veclen = memlet.veclen
                         out_memlet.wcr = memlet.wcr
                         out_memlet.wcr_identity = memlet.wcr_identity
                         out_memlet.wcr_conflict = memlet.wcr_conflict
                     if connector in self.inputs or connector in self.outputs:
                         raise DaceSyntaxError(
                             self, node,
                             'Local variable is already a tasklet input or output'
                         )
                     self.outputs[connector] = memlet
+                    return None  # Remove from final tasklet code
         elif isinstance(node.value, ast.Str):
             return self.visit_TopLevelStr(node.value)
 
         return self.generic_visit(node)
 
     # Detect external tasklet code
     def visit_TopLevelStr(self, node: ast.Str):
@@ -1421,15 +1680,16 @@
         self.outputs = {}
 
         # Add symbols
         for k, v in scope_arrays.items():
             if isinstance(v, data.Scalar):
                 self.sdfg.add_symbol(k, v.dtype, override_dtype=True)
         # Add constants
-        self.sdfg.add_constants(constants)
+        for cstname, cstval in constants.items():
+            self.sdfg.add_constant(cstname, cstval)
 
         # Add symbols. TODO: more elegant way
         for arr in scope_arrays.values():
             if arr is None:
                 continue
             for dim in arr.shape:
                 if not hasattr(dim, 'free_symbols'): continue
@@ -1475,14 +1735,18 @@
         # }
         result = {}
         result.update({
             k: self.sdfg.arrays[v]
             for k, v in self.scope_vars.items() if v in self.sdfg.arrays
         })
         result.update({
+            k: self.scope_arrays[v]
+            for k, v in self.scope_vars.items() if v in self.scope_arrays
+        })
+        result.update({
             k: self.sdfg.arrays[v]
             for k, v in self.variables.items() if v in self.sdfg.arrays
         })
         # TODO: Is there a case of a variable-symbol?
         result.update({
             k: self.sdfg.symbols[v]
             for k, v in self.variables.items() if v in self.sdfg.symbols
@@ -1515,16 +1779,16 @@
         return arg
 
     def _decorator_or_annotation_params(
             self, node: ast.FunctionDef) -> List[Tuple[str, Any]]:
         """ Returns a list of parameters, either from the function parameters
             and decorator arguments or parameters and their annotations (type
             hints).
-            @param node: The given function definition node.
-            @return: A list of 2-tuples (name, value).
+            :param node: The given function definition node.
+            :return: A list of 2-tuples (name, value).
         """
         # If the arguments are defined in the decorator
         dec = node.decorator_list[0]
         if 'args' in dir(dec) and len(dec.args) > 0:
             # If it's one argument of the form of ND range, e.g., "_[0:M, 0:N]"
             parg0 = self._parse_arg(dec.args[0])
             if isinstance(parg0, list):
@@ -1599,55 +1863,93 @@
             self._add_dependencies(state, internal_node, None, None, inputs,
                                    outputs)
             self.inputs.update(sdfg_inp)
             self.outputs.update(sdfg_out)
 
         elif dec.startswith('dace.map') or dec.startswith(
                 'dace.consume'):  # Scope or scope+tasklet
-            params = self._decorator_or_annotation_params(node)
-            params, map_inputs = self._parse_map_inputs(
-                node.name, params, node)
-            dummy = False
             if 'map' in dec:
+                params = self._decorator_or_annotation_params(node)
+                params, map_inputs = self._parse_map_inputs(
+                    node.name, params, node)
                 entry, exit = state.add_map(node.name, ndrange=params)
             elif 'consume' in dec:
-                entry, exit = state.add_consume(node.name, **params)
+                (stream_name, stream_elem, PE_tuple, condition,
+                 chunksize) = self._parse_consume_inputs(node)
+                map_inputs = {}
+                entry, exit = state.add_consume(
+                    node.name, PE_tuple, condition, chunksize=chunksize)
 
             if dec.endswith('scope'):  # @dace.mapscope or @dace.consumescope
                 sdfg, inputs, outputs = self._parse_subprogram(node.name, node)
-                internal_node = state.add_nested_sdfg(sdfg, self.sdfg,
-                                                      set(inputs.keys()),
-                                                      set(outputs.keys()))
             else:  # Scope + tasklet (e.g., @dace.map)
-                # internal_node, inputs, outputs, sdfg_inp, sdfg_out = self._parse_tasklet(
-                #     state, node)
-                # dummy = True
                 name = "{}_body".format(entry.label)
-                # name = "{}_{}_{}_body".format(self.sdfg.label, state.label,
-                #                               state.node_id(entry))
-                body, inputs, outputs = self._parse_subprogram(
+                sdfg, inputs, outputs = self._parse_subprogram(
                     name, node, True)
-                internal_node = state.add_nested_sdfg(body, self.sdfg,
-                                                      inputs.keys(),
-                                                      outputs.keys())
+
+            internal_node = state.add_nested_sdfg(sdfg, self.sdfg,
+                                                  set(inputs.keys()),
+                                                  set(outputs.keys()))
+
+            # If consume scope, inject stream inputs to the internal SDFG
+            if 'consume' in dec:
+                self._inject_consume_memlets(dec, entry, inputs, internal_node,
+                                             sdfg, state, stream_elem,
+                                             stream_name)
 
             # Connect internal node with scope/access nodes
             self._add_dependencies(state, internal_node, entry, exit, inputs,
                                    outputs, map_inputs)
-            if dummy:
-                self.inputs.update(sdfg_inp)
-                self.outputs.update(sdfg_out)
 
         elif dec == 'dace.program':  # Nested SDFG
             raise DaceSyntaxError(
                 self, node, 'Nested programs must be '
                 'defined outside existing programs')
         else:
             raise DaceSyntaxError(self, node, 'Unsupported function decorator')
 
+    def _inject_consume_memlets(self, dec, entry, inputs, internal_node, sdfg,
+                                state, stream_elem, stream_name):
+        """ Inject stream inputs to subgraph when creating a consume scope. """
+
+        # Inject element to internal SDFG arrays
+        ntrans = sdfg.temp_data_name()
+        sdfg.add_array(ntrans, [1], self.sdfg.arrays[stream_name].dtype)
+        internal_memlet = dace.Memlet(ntrans, 1, subsets.Indices([0]), 1)
+        external_memlet = dace.Memlet(stream_name, dtypes.DYNAMIC,
+                                      subsets.Indices([0]), 1)
+
+        # Inject to internal tasklet
+        if not dec.endswith('scope'):
+            injected_node_count = 0
+            for s in sdfg.nodes():
+                for n in s.nodes():
+                    if (isinstance(n, nodes.Tasklet)
+                            and not isinstance(n, nodes.EmptyTasklet)):
+                        n.add_in_connector(stream_elem)
+                        rnode = s.add_read(ntrans)
+                        s.add_edge(rnode, None, n, stream_elem,
+                                   internal_memlet)
+                        injected_node_count += 1
+            assert injected_node_count == 1
+
+        # Inject to nested SDFG node
+        internal_node.add_in_connector(ntrans)
+        stream_node = state.add_read(stream_name)
+        state.add_edge_pair(
+            entry,
+            internal_node,
+            stream_node,
+            external_memlet,
+            scope_connector='stream',
+            internal_connector=ntrans)
+
+        # Mark as input so that no extra edges are added
+        inputs[ntrans] = None
+
     def _parse_for_indices(self, node: ast.Expr):
         """Parses the indices of a for-loop statement
         
         Arguments:
             node {ast.Expr} -- Target of ast.For node
         
         Raises:
@@ -1783,23 +2085,24 @@
         return (iterator, ranges)
 
     def _parse_map_inputs(
             self, name: str, params: List[Tuple[str, str]],
             node: ast.AST) -> Tuple[Dict[str, str], Dict[str, Memlet]]:
         """ Parse map parameters for data-dependent inputs, modifying the
             parameter dictionary and returning relevant memlets.
-            @return: A 2-tuple of (parameter dictionary, mapping from connector
+            :return: A 2-tuple of (parameter dictionary, mapping from connector
                      name to memlet).
         """
         new_params = []
         map_inputs = {}
         for k, v in params:
             vsp = list(v.split(':'))
             for i, (val, vid) in enumerate(zip(vsp, 'best')):
-                # Walk through expression, find functions and replace with variables
+                # Walk through expression, find functions and replace with
+                # variables
                 ctr = 0
                 repldict = {}
                 for expr in symbolic.swalk(pystr_to_symbolic(val)):
                     if symbolic.is_sympy_userfunction(expr):
                         # If function contains a function
                         if any(
                                 symbolic.contains_sympy_functions(a)
@@ -1813,54 +2116,112 @@
                         repldict[arr] = newvar
                         # Create memlet
                         args = ','.join([str(a) for a in expr.args])
                         if arr in self.variables:
                             arr = self.variables[arr]
                         if arr not in self.sdfg.arrays:
                             rng = subsets.Range.from_string(args)
-                            # arr, rng = self._add_read_access(arr, rng, node, newvar, data.Scalar)
-                            arr = self._add_read_access(
-                                arr, rng, node, newvar, data.Scalar)
                             args = str(rng)
                         map_inputs[newvar] = Memlet.simple(arr, args)
                         # ','.join([str(a) for a in expr.args]))
                         ctr += 1
                 # Replace functions with new variables
                 for find, replace in repldict.items():
                     val = re.sub(r"%s\(.*?\)" % find, replace, val)
                 vsp[i] = val
 
             new_params.append((k, ':'.join(vsp)))
 
         return new_params, map_inputs
 
+    def _parse_consume_inputs(self, node: ast.FunctionDef
+                              ) -> Tuple[str, str, Tuple[str, str], str, str]:
+        """ Parse consume parameters from AST.
+            :return: A 5-tuple of Stream name, internal stream name,
+                     (PE index, number of PEs), condition, chunk size.
+        """
+
+        # Consume scopes in Python are defined as functions with the following
+        # syntax:
+        # @dace.consume(<stream name>, <number of PEs>[, <quiescence condition>,
+        #               <chunk size>)
+        # def func(<internal stream element name>, <internal PE index name>):
+
+        # Parse decorator
+        dec = node.decorator_list[0]
+        if hasattr(dec, 'args') and len(dec.args) >= 2:
+            stream_name = self.visit(dec.args[0])
+            num_PEs = pystr_to_symbolic(self.visit(dec.args[1]))
+            if len(dec.args) >= 3:
+                # TODO: Does not work if the condition uses arrays
+                condition = astutils.unparse(dec.args[2])
+            else:
+                condition = None  # Run until stream is empty
+            if len(dec.args) >= 4:
+                chunksize = pystr_to_symbolic(self.visit(dec.args[3]))
+            else:
+                chunksize = 1
+        else:
+            raise DaceSyntaxError(
+                self, node, 'Consume scope decorator must '
+                'contain at least two arguments')
+
+        # Parse function
+        if len(node.args.args) != 2:
+            raise DaceSyntaxError(
+                self, node, 'Consume scope function must '
+                'contain two arguments')
+
+        stream_elem, PE_index = tuple(a.arg for a in node.args.args)
+
+        return (stream_name, stream_elem, (PE_index, num_PEs), condition,
+                chunksize)
+
+    def _find_access(self, name: str, rng: subsets.Range, mode: str):
+        for n, r, m in self.accesses:
+            if n == name and m == mode:
+                if r == rng:
+                    return True
+                elif r.covers(rng):
+                    print("WARNING: New access {n}[{rng}] already covered by"
+                          " {n}[{r}]".format(n=name, rng=rng, r=r))
+                elif rng.covers(r):
+                    print("WARNING: New access {n}[{rng}] covers previous"
+                          " access {n}[{r}]".format(n=name, rng=rng, r=r))
+                return False
+
     def _add_dependencies(self,
                           state: SDFGState,
                           internal_node: nodes.CodeNode,
                           entry_node: nodes.EntryNode,
                           exit_node: nodes.ExitNode,
                           inputs: Dict[str, Memlet],
                           outputs: Dict[str, Memlet],
                           map_inputs: Dict[str, Memlet] = None):
 
         # Parse map inputs (for memory-based ranges)
         if map_inputs is not None:
             for conn, memlet in map_inputs.items():
-                read_node = state.add_read(memlet.data)
-                if _subset_has_indirection(memlet.subset):
-                    add_indirection_subgraph(self.sdfg, state, read_node,
-                                             entry_node, memlet, conn, self)
-                    continue
+                if self.nested:
+                    new_name = self._add_read_access(memlet.data,
+                                                     memlet.subset, None)
+                    memlet = Memlet.from_array(new_name,
+                                               self.sdfg.arrays[new_name])
+                else:
+                    new_name = memlet.data
 
+                read_node = state.add_read(new_name)
                 entry_node.add_in_connector(conn)
                 state.add_edge(read_node, None, entry_node, conn, memlet)
 
         # Parse internal node inputs and indirect memory accesses
         if inputs:
             for conn, v in inputs.items():
+                if v is None:  # Input already handled outside
+                    continue
                 if isinstance(v, tuple):
                     memlet, inner_indices = v
                 else:
                     memlet, inner_indices = v, set()
                 if _subset_has_indirection(memlet.subset):
                     read_node = entry_node
                     if entry_node is None:
@@ -1874,41 +2235,43 @@
                 # elif (memlet.data, memlet.subset, 'r') in self.accesses:
                 #     vname = self.accesses[(memlet.data, memlet.subset, 'r')][0]
                 #     memlet = dace.Memlet.from_array(vname, self.sdfg.arrays[vname])
                 if memlet.data not in self.sdfg.arrays:
                     arr = self.scope_arrays[memlet.data]
                     scope_memlet = propagate_memlet(state, memlet, entry_node,
                                                     True, arr)
-                    if (memlet.data, scope_memlet.subset, 'w') in self.accesses:
-                        vname = self.accesses[(memlet.data, scope_memlet.subset, 'w')][0]
-                        memlet = dace.Memlet.from_array(vname, self.sdfg.arrays[vname])
-                    elif (memlet.data, scope_memlet.subset, 'r') in self.accesses:
-                        vname = self.accesses[(memlet.data, scope_memlet.subset, 'r')][0]
-                        memlet = dace.Memlet.from_array(vname, self.sdfg.arrays[vname])
+                    irng = memlet.subset
+                    orng = copy.deepcopy(scope_memlet.subset)
+                    outer_indices = []
+                    for n, (i, o) in enumerate(zip(irng, orng)):
+                        if i == o and n not in inner_indices:
+                            outer_indices.append(n)
+                        elif n not in inner_indices:
+                            inner_indices.add(n)
+                    irng.pop(outer_indices)
+                    orng.pop(outer_indices)
+                    irng.offset(orng, True)
+                    if (memlet.data, scope_memlet.subset,
+                            'w') in self.accesses:
+                        vname = self.accesses[(memlet.data,
+                                               scope_memlet.subset, 'w')][0]
+                        memlet = Memlet.simple(vname, str(irng))
+                    elif (memlet.data, scope_memlet.subset,
+                          'r') in self.accesses:
+                        vname = self.accesses[(memlet.data,
+                                               scope_memlet.subset, 'r')][0]
+                        memlet = Memlet.simple(vname, str(irng))
                     else:
                         name = memlet.data
-                        irng = memlet.subset
-                        orng = copy.deepcopy(scope_memlet.subset)
-                        outer_indices = []
-                        for n, (i, o) in enumerate(zip(irng, orng)):
-                            if i == o and n not in inner_indices:
-                                outer_indices.append(n)
-                            elif n not in inner_indices:
-                                inner_indices.add(n)
-                        # for n in reversed(outer_indices):
-                        #     irng.ranges.pop(n)
-                        #     orng.ranges.pop(n)
-                        irng.pop(outer_indices)
-                        orng.pop(outer_indices)
-                        irng.offset(orng, True)
                         vname = "{c}_in_from_{s}_{n}".format(
                             c=conn,
                             s=self.sdfg.nodes().index(state),
                             n=state.node_id(entry_node))
-                        self.accesses[(name, scope_memlet.subset, 'r')] = (vname, None)
+                        self.accesses[(name, scope_memlet.subset,
+                                       'r')] = (vname, orng)
                         orig_shape = orng.size()
                         shape = [d for d in orig_shape if d != 1]
                         strides = [
                             i for j, i in enumerate(arr.strides)
                             if j not in outer_indices
                         ]
                         strides = [
@@ -1957,46 +2320,59 @@
         else:
             if entry_node is not None:
                 state.add_nedge(entry_node, internal_node, dace.EmptyMemlet())
 
         # Parse internal node outputs
         if outputs:
             for conn, v in outputs.items():
+                if v is None:  # Output already handled outside
+                    continue
                 if isinstance(v, tuple):
                     memlet, inner_indices = v
                 else:
                     memlet, inner_indices = v, set()
+                if _subset_has_indirection(memlet.subset):
+                    write_node = exit_node
+                    if exit_node is None:
+                        write_node = state.add_write(memlet.data)
+                    add_indirection_subgraph(self.sdfg, state, internal_node,
+                                             exit_node, memlet, conn, self,
+                                             True)
+                    continue
+                inner_memlet = memlet
                 if memlet.data not in self.sdfg.arrays:
                     arr = self.scope_arrays[memlet.data]
                     scope_memlet = propagate_memlet(state, memlet, entry_node,
                                                     True, arr)
-                    if (memlet.data, scope_memlet.subset, 'w') in self.accesses:
-                        vname = self.accesses[(memlet.data, scope_memlet.subset, 'w')][0]
-                        memlet = dace.Memlet.from_array(vname, self.sdfg.arrays[vname])
+                    irng = memlet.subset
+                    orng = copy.deepcopy(scope_memlet.subset)
+                    outer_indices = []
+                    for n, (i, o) in enumerate(zip(irng, orng)):
+                        if i == o and n not in inner_indices:
+                            outer_indices.append(n)
+                        elif n not in inner_indices:
+                            inner_indices.add(n)
+                    irng.pop(outer_indices)
+                    orng.pop(outer_indices)
+                    irng.offset(orng, True)
+                    if self._find_access(memlet.data, scope_memlet.subset,
+                                         'w'):
+                        vname = self.accesses[(memlet.data,
+                                               scope_memlet.subset, 'w')][0]
+                        inner_memlet = Memlet.simple(vname, str(irng))
+                        inner_memlet.num_accesses = memlet.num_accesses
+                        inner_memlet.veclen = memlet.veclen
                     else:
                         name = memlet.data
-                        irng = memlet.subset
-                        orng = copy.deepcopy(scope_memlet.subset)
-                        outer_indices = []
-                        for n, (i, o) in enumerate(zip(irng, orng)):
-                            if i == o and n not in inner_indices:
-                                outer_indices.append(n)
-                            elif n not in inner_indices:
-                                inner_indices.add(n)
-                        # for n in reversed(outer_indices):
-                        #     irng.ranges.pop(n)
-                        #     orng.ranges.pop(n)
-                        irng.pop(outer_indices)
-                        orng.pop(outer_indices)
-                        irng.offset(orng, True)
                         vname = "{c}_out_of_{s}_{n}".format(
                             c=conn,
                             s=self.sdfg.nodes().index(state),
                             n=state.node_id(exit_node))
-                        self.accesses[(name, scope_memlet.subset, 'w')] = (vname, None)
+                        self.accesses[(name, scope_memlet.subset,
+                                       'w')] = (vname, orng)
                         orig_shape = orng.size()
                         shape = [d for d in orig_shape if d != 1]
                         strides = [
                             i for j, i in enumerate(arr.strides)
                             if j not in outer_indices
                         ]
                         strides = [
@@ -2012,30 +2388,30 @@
                         if isinstance(memlet.data, data.Stream):
                             self.sdfg.add_stream(vname, dtype)
                         else:
                             self.sdfg.add_array(
                                 vname, shape, dtype, strides=strides)
                         self.outputs[vname] = (scope_memlet, inner_indices)
                         # self.outputs[vname] = (memlet.data, scope_memlet.subset, inner_indices)
-                        memlet.data = vname
+                        inner_memlet.data = vname
                         # memlet.subset.offset(memlet.subset, True, outer_indices)
                 else:
                     vname = memlet.data
                 write_node = state.add_write(vname)
                 if exit_node is not None:
                     state.add_memlet_path(
                         internal_node,
                         exit_node,
                         write_node,
-                        memlet=memlet,
+                        memlet=inner_memlet,
                         src_conn=conn,
                         dst_conn=None)
                 else:
                     state.add_edge(internal_node, conn, write_node, None,
-                                   memlet)
+                                   inner_memlet)
         else:
             if exit_node is not None:
                 state.add_nedge(internal_node, exit_node, dace.EmptyMemlet())
 
     def _recursive_visit(self,
                          body: List[ast.AST],
                          name: str,
@@ -2201,53 +2577,163 @@
         if target_subset.num_elements() != 1:
             if op_subset.num_elements() != 1:
                 op1 = state.add_read(op_name)
                 op2 = state.add_write(target_name)
                 memlet = Memlet(target_name, target_subset.num_elements(),
                                 target_subset, 1)
                 memlet.other_subset = op_subset
-                if op is not None:
-                    memlet.wcr = LambdaProperty.from_string(
-                        'lambda x, y: x {} y'.format(op))
                 state.add_nedge(op1, op2, memlet)
             else:
                 memlet = Memlet.simple(
                     target_name,
                     ','.join(['__i%d' % i for i in range(len(target_subset))]))
                 if op:
                     memlet.wcr = LambdaProperty.from_string(
                         'lambda x, y: x {} y'.format(op))
                 state.add_mapped_tasklet(
                     state.label, {
                         '__i%d' % i: '%s:%s+1:%s' % (start, end, step)
                         for i, (start, end, step) in enumerate(target_subset)
-                    }, {'inp': Memlet.simple(op_name, '%s' % op_subset[0][0])},
-                    'out = inp', {'out': memlet},
+                    },
+                    {'__inp': Memlet.simple(op_name, '%s' % op_subset[0][0])},
+                    '__out = __inp', {'__out': memlet},
                     external_edges=True)
         else:
             if op_subset.num_elements() != 1:
                 raise DaceSyntaxError(
                     self, node, "Incompatible subsets %s and %s" %
                     (target_subset, op_subset))
+            op1 = state.add_read(op_name)
+            op2 = state.add_write(target_name)
+            tasklet = state.add_tasklet(
+                name=state.label,
+                inputs={'__inp'},
+                outputs={'__out'},
+                code='__out = __inp')
+            inp_memlet = Memlet.simple(op_name, '%s' % op_subset[0][0])
+            out_memlet = Memlet.simple(target_name, '%s' % target_subset[0][0])
+            state.add_edge(op1, None, tasklet, '__inp', inp_memlet)
+            state.add_edge(tasklet, '__out', op2, None, out_memlet)
+
+    def _add_aug_assignment(self, node: Union[ast.Assign, ast.AugAssign],
+                            rtarget: Union[str, Tuple[str, subsets.Range]],
+                            wtarget: Union[str, Tuple[str, subsets.Range]],
+                            operand: Union[str, Tuple[str, subsets.Range]],
+                            op: str):
+
+        if isinstance(rtarget, tuple):
+            rtarget_name, rtarget_subset = rtarget
+        else:
+            rtarget_name = rtarget
+            rtarget_array = self.sdfg.arrays[rtarget_name]
+            rtarget_subset = subsets.Range.from_array(rtarget_array)
+        if isinstance(wtarget, tuple):
+            wtarget_name, wtarget_subset = wtarget
+        else:
+            wtarget_name = wtarget
+            wtarget_array = self.sdfg.arrays[wtarget_name]
+            wtarget_subset = subsets.Range.from_array(wtarget_array)
+        if isinstance(operand, tuple):
+            op_name, op_subset = operand
+        else:
+            op_name = operand
+            op_array = self.sdfg.arrays[op_name]
+            op_subset = subsets.Range.from_array(op_array)
+
+        state = self._add_state("assign_{l}_{c}".format(
+            l=node.lineno, c=node.col_offset))
+
+        if wtarget_subset.num_elements() != 1:
+            if op_subset.num_elements() != 1:
+                if wtarget_subset.size() == op_subset.size():
+                    in1_subset = copy.deepcopy(rtarget_subset)
+                    in1_subset.offset(wtarget_subset, True)
+                    in1_memlet = Memlet.simple(
+                        rtarget_name, ','.join([
+                            '__i%d + %d' % (i, s)
+                            for i, (s, _, _) in enumerate(in1_subset)
+                        ]))
+                    in2_subset = copy.deepcopy(op_subset)
+                    in2_subset.offset(wtarget_subset, True)
+                    in2_memlet = Memlet.simple(
+                        op_name, ','.join([
+                            '__i%d + %d' % (i, s)
+                            for i, (s, _, _) in enumerate(in2_subset)
+                        ]))
+                    out_memlet = Memlet.simple(
+                        wtarget_name, ','.join(
+                            ['__i%d' % i for i in range(len(wtarget_subset))]))
+                    state.add_mapped_tasklet(
+                        state.label, {
+                            '__i%d' % i: '%s:%s+1:%s' % (start, end, step)
+                            for i, (start, end,
+                                    step) in enumerate(wtarget_subset)
+                        }, {
+                            '__in1': in1_memlet,
+                            '__in2': in2_memlet
+                        },
+                        '__out = __in1 {op} __in2'.format(op=op),
+                        {'__out': out_memlet},
+                        external_edges=True)
+                else:
+                    op1 = state.add_read(op_name)
+                    op2 = state.add_write(wtarget_name)
+                    memlet = Memlet(wtarget_name,
+                                    wtarget_subset.num_elements(),
+                                    wtarget_subset, 1)
+                    memlet.other_subset = op_subset
+                    if op is not None:
+                        memlet.wcr = LambdaProperty.from_string(
+                            'lambda x, y: x {} y'.format(op))
+                    state.add_nedge(op1, op2, memlet)
             else:
-                op1 = state.add_read(op_name)
-                op2 = state.add_write(target_name)
+                in1_subset = copy.deepcopy(rtarget_subset)
+                in1_subset.offset(wtarget_subset, True)
+                in1_memlet = Memlet.simple(
+                    rtarget_name, ','.join([
+                        '__i%d + %d' % (i, s)
+                        for i, (s, _, _) in enumerate(in1_subset)
+                    ]))
+                in2_memlet = Memlet.simple(op_name, '%s' % op_subset[0][0])
+                out_memlet = Memlet.simple(
+                    wtarget_name, ','.join(
+                        ['__i%d' % i for i in range(len(wtarget_subset))]))
+                state.add_mapped_tasklet(
+                    state.label, {
+                        '__i%d' % i: '%s:%s+1:%s' % (start, end, step)
+                        for i, (start, end, step) in enumerate(wtarget_subset)
+                    }, {
+                        '__in1': in1_memlet,
+                        '__in2': in2_memlet
+                    },
+                    '__out = __in1 {op} __in2'.format(op=op),
+                    {'__out': out_memlet},
+                    external_edges=True)
+        else:
+            if op_subset.num_elements() != 1:
+                raise DaceSyntaxError(
+                    self, node, "Incompatible subsets %s, %s and %s" %
+                    (rtarget_subset, op_subset, wtarget_subset))
+            else:
+                op1 = state.add_read(rtarget_name)
+                op2 = state.add_read(op_name)
+                op3 = state.add_write(wtarget_name)
                 tasklet = state.add_tasklet(
                     name=state.label,
-                    inputs={'inp'},
-                    outputs={'out'},
-                    code='out = inp')
-                inp_memlet = Memlet.simple(op_name, '%s' % op_subset[0][0])
-                out_memlet = Memlet.simple(target_name,
-                                           '%s' % target_subset[0][0])
-                if op is not None:
-                    out_memlet.wcr = LambdaProperty.from_string(
-                        'lambda x, y: x {} y'.format(op))
-                state.add_edge(op1, None, tasklet, 'inp', inp_memlet)
-                state.add_edge(tasklet, 'out', op2, None, out_memlet)
+                    inputs={'__in1', '__in2'},
+                    outputs={'__out'},
+                    code='__out = __in1 {op} __in2'.format(op=op))
+                in1_memlet = Memlet.simple(rtarget_name,
+                                           '%s' % rtarget_subset[0][0])
+                in2_memlet = Memlet.simple(op_name, '%s' % op_subset[0][0])
+                out_memlet = Memlet.simple(wtarget_name,
+                                           '%s' % wtarget_subset[0][0])
+                state.add_edge(op1, None, tasklet, '__in1', in1_memlet)
+                state.add_edge(op2, None, tasklet, '__in2', in2_memlet)
+                state.add_edge(tasklet, '__out', op3, None, out_memlet)
 
     def _get_variable_name(self, node, name):
         if name in self.variables:
             return self.variables[name]
         elif name in self.scope_vars:
             return self.scope_vars[name]
         else:
@@ -2263,48 +2749,53 @@
             new_name: str = None,
             arr_type: data.Data = None) -> str:
         if access_type not in ('r', 'w'):
             raise ValueError("Access type {} is invalid".format(access_type))
         if new_name:
             var_name = new_name
         elif target:
-            var_name = "__tmp_{l}_{c}".format(
-                l=target.lineno, c=target.col_offset)
+            var_name = "__tmp_{l}_{c}_{a}".format(
+                l=target.lineno, c=target.col_offset, a=access_type)
         else:
             var_name = self.sdfg.temp_data_name()
 
         parent_name = self.scope_vars[name]
         parent_array = self.scope_arrays[parent_name]
         squeezed_rng = copy.deepcopy(rng)
-        squeezed_rng.squeeze()
+        non_squeezed = squeezed_rng.squeeze()
         shape = squeezed_rng.size()
         dtype = parent_array.dtype
 
         if arr_type is None:
             arr_type = type(parent_array)
         if arr_type == data.Scalar:
             self.sdfg.add_scalar(var_name, dtype)
         elif arr_type == data.Array:
-            self.sdfg.add_array(
-                var_name, shape, dtype, strides=squeezed_rng.strides())
+            if non_squeezed:
+                strides = [parent_array.strides[d] for d in non_squeezed]
+            else:
+                strides = [1]
+            self.sdfg.add_array(var_name, shape, dtype, strides=strides)
         elif arr_type == data.Stream:
             self.sdfg.add_stream(var_name, dtype)
         else:
             raise NotImplementedError(
                 "Data type {} is not implemented".format(arr_type))
 
         self.accesses[(name, rng, access_type)] = (var_name, squeezed_rng)
+
+        inner_indices = set(non_squeezed)
+
         if access_type == 'r':
-            self.inputs[var_name] = (dace.Memlet(parent_name,
-                                                 rng.num_elements(), rng, 1),
-                                     set())
+            self.inputs[var_name] = (dace.Memlet(
+                parent_name, rng.num_elements(), rng, 1), inner_indices)
         else:
             self.outputs[var_name] = (dace.Memlet(parent_name,
                                                   rng.num_elements(), rng, 1),
-                                      set())
+                                      inner_indices)
 
         return var_name
 
     def _add_read_access(self,
                          name: str,
                          rng: subsets.Range,
                          target: Union[ast.Name, ast.Subscript],
@@ -2400,19 +2891,56 @@
                 true_target.id = true_name
             elif isinstance(target, ast.Subscript):
                 true_target.value.id = true_name
             rng = dace.subsets.Range(
                 astutils.subscript_to_slice(true_target, defined_arrays)[1])
 
             if self.nested:  # Nested SDFG
-                self._add_assignment(node,
-                                     self._add_write_access(name, rng, target),
-                                     result, op)
+                if op:
+                    rtarget = self._add_read_access(name, rng, target)
+                    wtarget = self._add_write_access(name, rng, target)
+                    self._add_aug_assignment(node, rtarget, wtarget, result,
+                                             op)
+                else:
+                    wtarget = self._add_write_access(name, rng, target)
+                    self._add_assignment(node, wtarget, result)
             else:  # Top-level SDFG
-                self._add_assignment(node, (true_name, rng), result, op)
+                output_indirection = None
+                if _subset_has_indirection(rng):
+                    output_indirection = self.sdfg.add_state(
+                        'slice_%s_%d' % (true_name, node.lineno))
+                    wnode = output_indirection.add_write(true_name)
+                    memlet = Memlet.simple(true_name, str(rng))
+                    tmp = self.sdfg.temp_data_name()
+                    wtarget = add_indirection_subgraph(
+                        self.sdfg, output_indirection, None, wnode, memlet,
+                        tmp, self, True)
+                else:
+                    wtarget = (true_name, rng)
+                if op:
+                    if _subset_has_indirection(rng):
+                        self._add_state(
+                            'slice_%s_%d' % (true_name, node.lineno))
+                        rnode = self.last_state.add_read(true_name)
+                        memlet = Memlet.simple(true_name, str(rng))
+                        tmp = self.sdfg.temp_data_name()
+                        rtarget = add_indirection_subgraph(
+                            self.sdfg, self.last_state, rnode, None, memlet,
+                            tmp, self)
+                    else:
+                        rtarget = (true_name, rng)
+                    self._add_aug_assignment(node, rtarget, wtarget, result,
+                                             op)
+                else:
+                    self._add_assignment(node, wtarget, result)
+
+                if output_indirection:
+                    self.sdfg.add_edge(self.last_state, output_indirection,
+                                       dace.graph.edges.InterstateEdge())
+                    self.last_state = output_indirection
 
     def visit_AugAssign(self, node: ast.AugAssign):
 
         self._visit_assign(node, node.target,
                            augassign_ops[type(node.op).__name__])
 
     def _get_keyword_value(self, keywords: List[ast.keyword], arg: str):
@@ -2536,19 +3064,24 @@
         return (shape, dtype)
 
     def _parse_function_arg(self, arg: ast.AST):
         # Obtain a string representation
         return self.visit(arg)
 
     def _is_inputnode(self, sdfg: SDFG, name: str):
+        visited_data = set()
         for state in sdfg.nodes():
+            visited_state_data = set()
             for node in state.nodes():
                 if isinstance(node, nodes.AccessNode) and node.data == name:
-                    if state.out_degree(node) > 0:
+                    visited_state_data.add(node.data)
+                    if (node.data not in visited_data
+                            and state.in_degree(node) == 0):
                         return True
+            visited_data = visited_data.union(visited_state_data)
 
     def _is_outputnode(self, sdfg: SDFG, name: str):
         for state in sdfg.nodes():
             for node in state.nodes():
                 if isinstance(node, nodes.AccessNode) and node.data == name:
                     if state.in_degree(node) > 0:
                         return True
@@ -2596,42 +3129,115 @@
                 }[arg] if isinstance(arg, str) else arg
                                       for aname, arg in args))
             else:
                 raise DaceSyntaxError(
                     self, node, 'Unrecognized SDFG type "%s" in call to "%s"' %
                     (type(func).__name__, funcname))
 
+            # Change transient names
+            for arrname, array in sdfg.arrays.items():
+                if array.transient and arrname[:5] == '__tmp':
+                    if int(arrname[5:]) < self.sdfg._temp_transients:
+                        new_name = sdfg.temp_data_name()
+                        sdfg.replace(arrname, new_name)
+            self.sdfg._temp_transients = max(self.sdfg._temp_transients,
+                                             sdfg._temp_transients)
+
+            slice_state = None
+            output_slices = set()
+            for arg in node.args:
+                if isinstance(arg, ast.Subscript):
+                    slice_state = self.last_state
+                    break
+
             state = self._add_state('call_%s_%d' % (funcname, node.lineno))
             argdict = {
                 conn: Memlet.from_array(arg, self.sdfg.arrays[arg])
                 for conn, arg in args if arg in self.sdfg.arrays
             }
             inputs = {
                 k: v
                 for k, v in argdict.items() if self._is_inputnode(sdfg, k)
             }
             outputs = {
                 k: v
                 for k, v in argdict.items() if self._is_outputnode(sdfg, k)
             }
+            # Unset parent inputs/read accesses that
+            # turn out to be outputs/write accesses.
+            # TODO: Is there a case where some data is both input and output?
+            # TODO: If yes, is it a problem?
+            for memlet in outputs.values():
+                aname = memlet.data
+                rng = memlet.subset
+                access_value = (aname, rng)
+                access_key = _inverse_dict_lookup(self.accesses, access_value)
+                if access_key:
+                    # Delete read access and create write access and output
+                    vname = aname[:-1] + 'w'
+                    name, rng, atype = access_key
+                    if atype == 'r':
+                        del self.accesses[access_key]
+                        access_value = self._add_write_access(
+                            name, rng, node, new_name=vname)
+                        memlet.data = vname
+                if aname in self.inputs.keys():
+                    # Delete input
+                    del self.inputs[aname]
+                # Delete potential input slicing
+                if slice_state:
+                    for n in slice_state.nodes():
+                        if isinstance(n, nodes.AccessNode) and n.data == aname:
+                            for e in slice_state.in_edges(n):
+                                sub = None
+                                for s in node.args:
+                                    if isinstance(s, ast.Subscript):
+                                        if s.value.id == e.src.data:
+                                            sub = s
+                                            break
+                                if not sub:
+                                    raise KeyError("Did not find output "
+                                                   "subscript")
+                                output_slices.add((sub, ast.Name(id=aname)))
+                                slice_state.remove_edge(e)
+                                slice_state.remove_node(e.src)
+                            slice_state.remove_node(n)
+                            break
 
             # Map internal SDFG symbols to external symbols (find_and_replace?)
             for aname, arg in args:
+                if arg in self.sdfg.arrays:
+                    continue
                 if arg in self.sdfg.symbols or not isinstance(arg, str):
                     sdfg.replace(aname, arg)
                 # Disallow memlets/nodes to symbol parameters
                 elif aname in sdfg.symbols:
                     raise DaceSyntaxError(
                         self, node, 'Array nodes cannot be '
                         'passed as scalars to nested SDFG '
                         '(passing "%s" as "%s")' % (aname, arg))
             nsdfg = state.add_nested_sdfg(sdfg, self.sdfg, inputs.keys(),
                                           outputs.keys())
             self._add_dependencies(state, nsdfg, None, None, inputs, outputs)
 
+            if output_slices:
+                assign_node = ast.Assign()
+                targets = []
+                value = []
+                for t, v in output_slices:
+                    targets.append(t)
+                    value.append(v)
+                assign_node = ast.Assign(
+                    targets=ast.Tuple(elts=targets),
+                    value=ast.Tuple(elts=value),
+                    lineno=node.lineno,
+                    col_offset=node.col_offset)
+                return self._visit_assign(assign_node, assign_node.targets,
+                                          None)
+
             # No return values from SDFGs
             return []
 
         # TODO: If the function is a callback, implement it as a tasklet
 
         # Otherwise, try to find a default implementation for the SDFG
         func = oprepo.Replacements.get(funcname, default_impl)
@@ -2678,31 +3284,32 @@
 
             # Create an edge between the two data descriptors
             state = self._add_state('globalmemlet_%d' % node.lineno)
             src_expr = ParseMemlet(self, self.defined, src)
             dst_expr = ParseMemlet(self, self.defined, dst)
             src_name = src_expr.name
             if src_name not in self.sdfg.arrays:
-                src_name = self.variables[src_expr.name]
+                src_name = self._add_read_access(src_name, src_expr.subset,
+                                                 None)
             dst_name = dst_expr.name
             if dst_name not in self.sdfg.arrays:
-                dst_name = self.variables[dst_expr.name]
+                dst_name = self._add_write_access(dst_name, dst_expr.subset,
+                                                  None)
 
             rnode = state.add_read(src_name)
             wnode = state.add_write(dst_name)
             state.add_nedge(
                 rnode, wnode,
                 Memlet(
                     src_name,
                     src_expr.accesses,
-                    src_expr.subset,
+                    subsets.Range.from_array(self.sdfg.arrays[src_name]),
                     1,
                     wcr=dst_expr.wcr,
-                    wcr_identity=dst_expr.wcr_identity,
-                    other_subset=dst_expr.subset))
+                    wcr_identity=dst_expr.wcr_identity))
             return
 
         # Calling reduction or other SDFGs / functions
         elif isinstance(node.value, ast.Call):
             # Handles reduction and calling other SDFGs / DaCe programs
             # self._add_state('call_%d' % node.lineno)
             self.visit_Call(node.value)
@@ -2750,14 +3357,17 @@
         if name in self.variables:
             return self.variables[name]
 
         # If an allowed global, use directly
         if name in self.globals:
             return _inner_eval_ast(self.globals, node)
 
+        if name in self.sdfg.arrays:
+            return name
+
         if name not in self.scope_vars:
             raise DaceSyntaxError(self, node,
                                   'Use of undefined variable "%s"' % name)
         return self.scope_vars[name]
 
     #### Visitors that return arrays
     def visit_Str(self, node: ast.Str):
@@ -2881,16 +3491,14 @@
             print(
                 'WARNING: Operator "%s" is not registered with an %s implementation for'
                 'types %s and %s, falling back to SDFG' %
                 (opname, default_impl, op1type, op2type))
 
         self._add_state('%s_%d' % (type(node).__name__, node.lineno))
         result = func(self, self.sdfg, self.last_state, operand1, operand2)
-        if not isinstance(result, (tuple, list)):
-            return [result]
         return result
 
     def visit_UnaryOp(self, node: ast.UnaryOp):
         return self._visit_op(node, node.operand, None)
 
     def visit_BinOp(self, node: ast.BinOp):
         return self._visit_op(node, node.left, node.right)
@@ -2944,20 +3552,27 @@
             expr: MemletExpr = ParseMemlet(self, self.sdfg.arrays, node)
             arrobj = self.sdfg.arrays[array]
 
             # TODO: Check dimensionality of access and extend as necessary
 
             # Add slicing state
             self._add_state('slice_%s_%d' % (array, node.lineno))
-            other_subset = copy.deepcopy(expr.subset)
-            other_subset.squeeze()
-            tmp, tmparr = self.sdfg.add_temp_transient(
-                other_subset.size(), arrobj.dtype, arrobj.storage)
             rnode = self.last_state.add_read(array)
-            wnode = self.last_state.add_write(tmp)
-            self.last_state.add_nedge(
-                rnode, wnode,
-                Memlet(array, expr.accesses, expr.subset, 1, expr.wcr,
-                       expr.wcr_identity, other_subset))
-            return tmp
+            if _subset_has_indirection(expr.subset):
+                memlet = Memlet(array, expr.accesses, expr.subset, 1, expr.wcr,
+                                expr.wcr_identity)
+                tmp = self.sdfg.temp_data_name()
+                return add_indirection_subgraph(self.sdfg, self.last_state,
+                                                rnode, None, memlet, tmp, self)
+            else:
+                other_subset = copy.deepcopy(expr.subset)
+                other_subset.squeeze()
+                tmp, tmparr = self.sdfg.add_temp_transient(
+                    other_subset.size(), arrobj.dtype, arrobj.storage)
+                wnode = self.last_state.add_write(tmp)
+                self.last_state.add_nedge(
+                    rnode, wnode,
+                    Memlet(array, expr.accesses, expr.subset, 1, expr.wcr,
+                           expr.wcr_identity, other_subset))
+                return tmp
 
     ##################################
```

### Comparing `dace-0.9.0/dace/frontend/python/parser.py` & `dace-0.9.5/dace/frontend/python/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     except AttributeError:
         return inspect.getargspec(f).args
 
 
 def _compile_module(s, name='<string>'):
     """ Compiles a string representing a python module (file or code) and
         returns the resulting global objects as a dictionary mapping name->val.
-        @param name: Optional name for better error message handling.
+        :param name: Optional name for better error message handling.
     """
 
     gen_module = {}
     code = compile(s, name, 'exec')
     exec(code, gen_module)
     return gen_module
 
@@ -88,20 +88,20 @@
 
     return [parse_function(p, *compilation_args) for p in programs]
 
 
 def parse_from_function(function, *compilation_args, strict=None):
     """ Try to parse a DaceProgram object and return the `dace.SDFG` object
         that corresponds to it.
-        @param function: DaceProgram object (obtained from the `@dace.program`
+        :param function: DaceProgram object (obtained from the `@dace.program`
                          decorator).
-        @param compilation_args: Various compilation arguments e.g. dtypes.
-        @param strict: Whether to apply strict transformations or not (None
+        :param compilation_args: Various compilation arguments e.g. dtypes.
+        :param strict: Whether to apply strict transformations or not (None
                        uses configuration-defined value). 
-        @return: The generated SDFG object.
+        :return: The generated SDFG object.
     """
     if not isinstance(function, DaceProgram):
         raise TypeError(
             'Function must be of type dace.frontend.python.DaceProgram')
 
     # Obtain DaCe program as SDFG
     sdfg = function.generate_pdp(*compilation_args)
@@ -125,27 +125,45 @@
 
     # Validate SDFG
     sdfg.validate()
 
     return sdfg
 
 
+def _get_locals_and_globals():
+    """ Retrieves a list of local and global variables four steps up in the
+        stack. This is used to retrieve variables around and defined before
+        @dace.programs for adding symbols. """
+    frame = inspect.currentframe()
+    outer_frame = frame.f_back.f_back.f_back.f_back
+    result = {}
+    # Update globals, then locals
+    result.update(outer_frame.f_globals)
+    result.update(outer_frame.f_locals)
+
+    return result
+
+
 class DaceProgram:
     """ A data-centric program object, obtained by decorating a function with
         `@dace.program`. """
 
     def __init__(self, f, args, kwargs):
         self.f = f
         self.args = args
         self.kwargs = kwargs
         self._name = f.__name__
         self.argnames = _get_argnames(f)
+
+        # NOTE: Important to call this outside list/dict comprehensions
+        global_vars = _get_locals_and_globals()
+
         self.global_vars = {
             k: v
-            for k, v in f.__globals__.items() if dtypes.isallowed(v)
+            for k, v in global_vars.items() if dtypes.isallowed(v)
         }
         if self.argnames is None:
             self.argnames = []
 
     @property
     def name(self):
         return self._name
@@ -155,20 +173,20 @@
         return parse_from_function(self, *args, strict=strict)
 
     def compile(self, *args, strict=None, specialize=None):
         """ Convenience function that parses and compiles a DaCe program. """
         sdfg = parse_from_function(self, *args, strict=strict)
         return sdfg.compile(specialize=specialize)
 
-    def __call__(self, *args, strict=None, specialize=None):
+    def __call__(self, *args, **kwargs):
         """ Convenience function that parses, compiles, and runs a DaCe 
             program. """
-        binaryobj = self.compile(*args, strict=strict, specialize=specialize)
+        binaryobj = self.compile(*args)
         # Add named arguments to the call
-        kwargs = {aname: arg for aname, arg in zip(self.argnames, args)}
+        kwargs.update({aname: arg for aname, arg in zip(self.argnames, args)})
         # Update arguments with symbols in data shapes
         kwargs.update({
             sym: symbolic.symbol(sym).get()
             for arg in args
             for sym in (symbolic.symlist(arg.descriptor.shape) if hasattr(
                 arg, 'descriptor') else [])
         })
@@ -183,16 +201,16 @@
                         except:
                             pass
 
         return binaryobj(**kwargs)
 
     def generate_pdp(self, *compilation_args):
         """ Generates the parsed AST representation of a DaCe program.
-            @param compilation_args: Various compilation arguments e.g., dtypes.
-            @return: A 2-tuple of (program, modules), where `program` is a 
+            :param compilation_args: Various compilation arguments e.g., dtypes.
+            :return: A 2-tuple of (program, modules), where `program` is a
                      `dace.astnodes._ProgramNode` representing the parsed DaCe 
                      program, and `modules` is a dictionary mapping imported 
                      module names to their actual module names (for maintaining
                      import aliases).
         """
         dace_func = self.f
         args = self.args
@@ -226,25 +244,26 @@
 
         # Parse allowed global variables
         # (for inferring types and values in the DaCe program)
         global_vars = copy.copy(self.global_vars)
 
         modules = {
             k: v.__name__
-            for k, v in dace_func.__globals__.items() if dtypes.ismodule(v)
+            for k, v in global_vars.items() if dtypes.ismodule(v)
         }
         modules['builtins'] = ''
 
         # Add symbols as globals with their actual names (sym_0 etc.)
         global_vars.update({
             v.name: v
             for k, v in global_vars.items() if isinstance(v, symbolic.symbol)
         })
 
         # Allow SDFGs and DaceProgram objects
+        # NOTE: These are the globals AT THE TIME OF INVOCATION, NOT DEFINITION
         other_sdfgs = {
             k: v
             for k, v in dace_func.__globals__.items()
             if isinstance(v, (SDFG, DaceProgram))
         }
 
         # Parse AST to create the SDFG
```

### Comparing `dace-0.9.0/dace/frontend/python/simulator.py` & `dace-0.9.5/dace/frontend/python/simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from __future__ import print_function
 import ast
 import copy
 import numpy
 
 from dace import data, symbolic
 from dace.config import Config
-from dace.frontend.python import astnodes, ndloop, ndarray
+from dace.frontend.python import astnodes, ndloop, wrappers
 from dace.frontend.python.astutils import unparse, rname
 from dace.frontend.python.parser import DaceProgram
 
 
 def simulate(dace_program: DaceProgram, *args):
     """ Simulate a DaCe program using Python. 
-        @param dace_program: A program function annotated with `@dace.program`.
-        @param *args: Program arguments to pass.
+        :param dace_program: A program function annotated with `@dace.program`.
+        :param *args: Program arguments to pass.
     """
     pdp, modules = dace_program.generate_pdp()
 
     # Transform the decorated AST into working python code (annotated so
     # that debugging works)
     simulated_ast = SimulatorTransformer(pdp).visit(pdp.ast)
     mod = ast.Module(body=simulated_ast, lineno=1)
@@ -84,15 +84,15 @@
     # Resolve symbols in arguments as well
     newargs = tuple(symbolic.eval(a) for a in args)
     ##################################################################
 
     # Store parameter objects
     pdp.arrayobjs = {
         k: v
-        for k, v in zip(pdp.params, newargs) if isinstance(v, ndarray.ndarray)
+        for k, v in zip(pdp.params, newargs) if isinstance(v, numpy.ndarray)
     }
 
     # Simulate f
     ################################
     # Obtain function object
     gen_module = {}
     gen_module.update(f_globals)
@@ -118,15 +118,15 @@
             key):  # Set object's range every time it is called with a range
         self.range = key
         return self
 
 
 def converttype(argument, cvt_type, argname):
     """ Helper function to convert a scalar argument to its type. """
-    if isinstance(argument, ndarray.ndarray):
+    if isinstance(argument, numpy.ndarray):
         return argument
 
     # Convert type
     converted = cvt_type.type(argument)
 
     # Try to cast back to the original type. If the value has changed
     # (e.g., out of bounds, lost precision), raise exception
```

### Comparing `dace-0.9.0/dace/frontend/tensorflow/tensorflow.py` & `dace-0.9.5/dace/frontend/tensorflow/tensorflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,16 +101,16 @@
 
 _atomic_count = _atomic_counter_generator()
 
 
 class TFSession:
     def __init__(self, name: str = "tfsession", seed: int = None, config=None):
         """ Creates a DaCe Tensorflow session.
-            @param name: (optional) The name of the resulting SDFG.
-            @param seed: (optional) Fix random seed.
+            :param name: (optional) The name of the resulting SDFG.
+            :param seed: (optional) Fix random seed.
         """
         self._internal_session = tf.Session(config=config)
 
         # Set for bookkeeping of already visited nodes
         self.visitedNodes = set()
 
         # Reinit state only used in training mode
@@ -146,27 +146,27 @@
             gpu=False,
             nodes=None,
             output_gradients=False,
     ):
         """ Trains a subgraph for the specified number of iterations and 
             returns requested nodes after training.
             
-            @param optimizer: A TensorFlow tf.Optimizer node.
-            @param initializer: Either a list of global and local initializers
+            :param optimizer: A TensorFlow tf.Optimizer node.
+            :param initializer: Either a list of global and local initializers
                                 or one initializer.
-            @param iterations: Number of training steps.
-            @param feed_dict: Dictionary representing input values and arrays 
+            :param iterations: Number of training steps.
+            :param feed_dict: Dictionary representing input values and arrays
                               to feed in to the evaluator.
-            @param gpu: This boolean should be set if the session is to be run on a GPU.
-            @param nodes: (optional) A TensorFlow node or an iterable 
+            :param gpu: This boolean should be set if the session is to be run on a GPU.
+            :param nodes: (optional) A TensorFlow node or an iterable
                           (e.g. list) of nodes to evaluate.
-            @param output_gradients: A boolean, if set, will output all the gradients passed as the
+            :param output_gradients: A boolean, if set, will output all the gradients passed as the
                                      optimizer arument. This will assume optimizer contains the
                                      list of gradient tensors that will be added to the outputs.
-            @return: A 2-tuple of (varDict, values) - the first is a dictionary
+            :return: A 2-tuple of (varDict, values) - the first is a dictionary
                      of all variables used in the network in arbitrary order,
                      and the second is a tuple of values in the same order as
                      `nodes`.
         """
 
         # Initialize a new SDFG
         self.graph = SDFG(self.graph.name)
@@ -351,22 +351,22 @@
                 gpu,
                 name=None,
                 patterns=[],
                 validate=False,
                 strict=True):
         """ Compiles a subgraph into a callable function, which is equivalent 
             to calling `run()`. 
-            @param nodes: Node or an iterable (e.g. list) of nodes to evaluate.
-            @param name: Name of the SDFG to create, or None for a unique name.
-            @param gpu: set this boolean to True if compilation has to be done for GPU.
-            @param patterns: A list of list of Transformation(s) that should be applied.
-            @param validate: Boolean that decides if validation will take place after
+            :param nodes: Node or an iterable (e.g. list) of nodes to evaluate.
+            :param name: Name of the SDFG to create, or None for a unique name.
+            :param gpu: set this boolean to True if compilation has to be done for GPU.
+            :param patterns: A list of list of Transformation(s) that should be applied.
+            :param validate: Boolean that decides if validation will take place after
                              transformations.
-            @param strict: Should the transformation be strict
-            @return: A function that receives a feed_dict, evaluates the nodes,
+            :param strict: Should the transformation be strict
+            :return: A function that receives a feed_dict, evaluates the nodes,
                      and returns a tuple of values in the same order as nodes.
         """
         from dace.config import Config
 
         # Create a unique name for this session
         if name is None:
             global _LASTSESSION
@@ -571,40 +571,40 @@
             validate=False,
             strict=True,
             name=None,
             winograd=False,
     ):
         """ Evaluates a subgraph and returns a tuple of the evaluated nodes
             (behaves similarly to sess.run).
-            @param nodes: Node or an iterable (e.g. list) of nodes to evaluate.
-            @param feed_dict: Dictionary representing input values and arrays 
+            :param nodes: Node or an iterable (e.g. list) of nodes to evaluate.
+            :param feed_dict: Dictionary representing input values and arrays
                               to feed in to the evaluator.
-            @param name: Name of the SDFG to create, or None for a unique name.
-            @param gpu: This boolean should be set if the session is to be run on a GPU.
-            @param patterns: A list of list of Transformation(s) that should be applied. the outer
+            :param name: Name of the SDFG to create, or None for a unique name.
+            :param gpu: This boolean should be set if the session is to be run on a GPU.
+            :param patterns: A list of list of Transformation(s) that should be applied. the outer
             list is just in-case you want the transformations in a certain sequence.
-            @param validate: Boolean that decides if validation will take place after
+            :param validate: Boolean that decides if validation will take place after
                              transformations.
-            @return: Tuple or dictionary of values in the same order as `nodes`.
+            :return: Tuple or dictionary of values in the same order as `nodes`.
         """
         self.winograd = winograd
         callfunc = self.compile(
             nodes,
             gpu,
             name=name,
             validate=validate,
             strict=strict,
             patterns=transformations,
         )
         return callfunc(feed_dict=feed_dict)
 
     def dfs_nodes(self, source):
         """ Produce nodes in a depth-first-search (DFS) on a TensorFlow graph.
-            @param source: The source node to start from.
-            @return: A generator of nodes in the depth-first-search.       
+            :param source: The source node to start from.
+            :return: A generator of nodes in the depth-first-search.
             @note: Based on http://www.ics.uci.edu/~eppstein/PADS/DFS.py
                     by D. Eppstein, July 2004.
         """
 
         # If source is a list of nodes (or any iterable), start from all
         try:
             iter(source)
@@ -3707,24 +3707,24 @@
                        otherNode,
                        tasklet,
                        inputDims,
                        inputParams,
                        identifier="j"):
         """ Convenience function that adds two memlets for each input of the 
             node: external and internal to a given map.
-            @param inputList: list of inputNodes (DaCe access node)
-            @param otherNode: DaCe node (mostly map_entry)
-            @param tasklet: Normally a tasklet node, but it can also be another 
+            :param inputList: list of inputNodes (DaCe access node)
+            :param otherNode: DaCe node (mostly map_entry)
+            :param tasklet: Normally a tasklet node, but it can also be another
                             mapEntry, for example map in map.
-            @param inputDims: List of list of strings dimension of the 
+            :param inputDims: List of list of strings dimension of the
                               respective input. Example:
                               [["0:5","0:7"],["0:2","0:4"]]  
-            @param inputParams: List of list of strings params of respective 
+            :param inputParams: List of list of strings params of respective
                                 input. Example: [["i0","i1"],["i2","i3"]]
-            @param identifier: This will be used as the base identifier of the
+            :param identifier: This will be used as the base identifier of the
                                 input connector to the tasklet. Default is 'j'  
         """
         state = self.state
         connected_nodes = set()
         for i, inp in enumerate(inputList):
             assert isinstance(inputDims[i], list)
             if inp.data not in connected_nodes:
@@ -3749,31 +3749,31 @@
             wcr=None,
             wcr_identity=None,
             identifier="out",
             wcr_conflict=True,
     ):
         """ Convenience function that adds two memlets for each output of the 
             node: external and internal to a given map.
-            @param outputList: list of outputNodes (DaCe access node)
-            @param otherNode: DaCe node (mostly map_entry)
-            @param tasklet: Normally a tasklet node, but it can also be another 
+            :param outputList: list of outputNodes (DaCe access node)
+            :param otherNode: DaCe node (mostly map_entry)
+            :param tasklet: Normally a tasklet node, but it can also be another
                             mapEntry, for example map in map.
-            @param outputDims: List of list of strings dimension of the 
+            :param outputDims: List of list of strings dimension of the
                                respective output. Example:
                                [["0:5","0:7"],["0:2","0:4"]]  
-            @param outputParams: List of list of strings params of respective 
+            :param outputParams: List of list of strings params of respective
                                  output. Example: [["i0","i1"],["i2","i3"]]  
-            @param wcr: (optional) Write-conflict resolution function (as 
+            :param wcr: (optional) Write-conflict resolution function (as
                         string).
-            @param wcr_identity: (optional) Identity element for write-conflict
+            :param wcr_identity: (optional) Identity element for write-conflict
                                  resolution.
-            @param identifier: This is the base identifier for the out connector
+            :param identifier: This is the base identifier for the out connector
                                 of the tasklet. Default value is "out". If there are
                                 multiple out connectors, each is numbered from zero.
-            @param wcr_conflict: (optional) If False, specifies that this
+            :param wcr_conflict: (optional) If False, specifies that this
                                  write-conflict resolution does not incur an
                                  atomic operation.
         """
 
         connected_nodes = set()
 
         state = self.state
@@ -3807,16 +3807,16 @@
             else:
                 state.add_edge(tasklet, None, otherNode, None, innerMemlet)
 
     def create_and_add_input_node(self, inp):
         """ Creates a DaCe access node for each input of `inp`, adds it to the 
             state, and returns it.
             If the node already exists, returns the pre-existing node.
-            @param inp: tf.Operation
-            @return: A 3-tuple of (input DaCe access node, 
+            :param inp: tf.Operation
+            :return: A 3-tuple of (input DaCe access node,
                                    list of parameter strings,
                                    list of dimension strings).
         """
 
         state = self.state
         # Get DaCe name of the operation
         label = string_builder(inp.name)
@@ -3843,16 +3843,16 @@
 
         return inputNode, params, dims
 
     def create_and_add_output_node(self, node):
         """ Creates a DaCe access node for each output of `node`, adds it to 
             the state, and returns it.
             If the node already exists, returns the pre-existing node.
-            @param node: tf.Operation
-            @return: List of DaCe access node.
+            :param node: tf.Operation
+            :return: List of DaCe access node.
         """
         outputList = []
         state = self.state
         for count, out in enumerate(node.outputs):
             label = string_builder(out.name)
             if "?" in str(_tensorshape(out)):
                 raise ValueError("Invalid shape {} for tensor {}".format(
@@ -3871,18 +3871,18 @@
                     label, shape, dtype, toplevel=True)
             outputList.append(outputNode)
         return outputList
 
     def reinitCR(self, inp, params, dims, identity):
         """ Adds a reinitialization map to a `reinit` state, setting inputs
             to their initial values. Only used in training mode.
-            @param inp: DaCe access node.
-            @param params: List of string parameters to `inp`.
-            @param dims: List of strings dimensions of `inp`.
-            @param identity: Identity value of the CR node (as a string)
+            :param inp: DaCe access node.
+            :param params: List of string parameters to `inp`.
+            :param dims: List of strings dimensions of `inp`.
+            :param identity: Identity value of the CR node (as a string)
         """
 
         if self.training:
             # Swap current state and reinitState
             self.state, self.reinitState = self.reinitState, self.state
             node = inp
             state = self.state
@@ -3916,22 +3916,22 @@
             pass
 
     def inputPadding(self, node, inpnode, inp, outputSize, kernelSize, strides,
                      inputDims):
         """ Zero-pads the input to fit the outputSize.
             WARNING: This function assumes the height and width of the output is the
             same (which is reasonable for deep learning).
-            @param node: tf.Operation
-            @param inpnode: DaCe access node to pad
-            @param inp: input node descriptor
-            @param outputSize: Output size. (int like)
-            @param kernelSize: Kernel size.
-            @param strides: Strides.
-            @param inputDims: List of strings (e.g.["0:N","0:M"]).
-            @return: A 2-tuple (output DaCe access node with padded input,
+            :param node: tf.Operation
+            :param inpnode: DaCe access node to pad
+            :param inp: input node descriptor
+            :param outputSize: Output size. (int like)
+            :param kernelSize: Kernel size.
+            :param strides: Strides.
+            :param inputDims: List of strings (e.g.["0:N","0:M"]).
+            :return: A 2-tuple (output DaCe access node with padded input,
                                 list of dimension strings of the padded data).
         """
         state = self.state
         paddingUp = 0
         paddingDown = 0
         label = inpnode.label
         inputSize = inp.shape[1]
@@ -3989,31 +3989,31 @@
         # self.add_out_memlets([output], mapExit, tasklet, [outputDims],
         #                    [outputParams])
         return output, outputDims
 
     def get_default_params(self, tensor, start=0, identifier="i"):
         """ Returns the default parameters of a tensor starting at `start`,
             e.g., ["i0","i1",...].
-            @param tensor: tf.Tensor.
-            @param start: Starting position for the iteration.
-            @param identifier: The base identifier for the parameters. Default is 'i'
-            @return: List of parameters as strings ["i0",i"1",...].
+            :param tensor: tf.Tensor.
+            :param start: Starting position for the iteration.
+            :param identifier: The base identifier for the parameters. Default is 'i'
+            :return: List of parameters as strings ["i0",i"1",...].
         """
         params = []
         shape = _tensorshape(tensor)
         if shape == 1:
             shape = [1]
         for i, dim in enumerate(shape, start):
             params.append(identifier + str(i))
         return params
 
     def get_default_dims(self, tensor):
         """ Returns the default dimensions of a tensor e.g., ["0:N","0:M"]
-            @param tensor: tf.Tensor.
-            @return: List of dimensions as strings ["0:N","0:M"]
+            :param tensor: tf.Tensor.
+            :return: List of dimensions as strings ["0:N","0:M"]
         """
         dims = []
         shape = _tensorshape(tensor)
         if shape == 1:
             shape = [1]
         for dim in shape:
             dims.append("0:" + str(dim))
```

### Comparing `dace-0.9.0/dace/frontend/tensorflow/winograd.py` & `dace-0.9.5/dace/frontend/tensorflow/winograd.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,26 +410,26 @@
 
 
 def winograd_convolution(dace_session, tf_node):
     debugNodes = []
     state = dace_session.state
     add_cublas_cusolver(dace_session.graph)
     #############Add constants for transformation matrices###############
-    dace_session.graph.add_constants({'Btrans': bt})
-    dace_session.graph.add_constants({'B': b})
+    dace_session.graph.add_constant('Btrans', bt)
+    dace_session.graph.add_constant('B', b)
     bNode = 'B'
     bTransposeNode = 'Btrans'
 
-    dace_session.graph.add_constants({'G': g})
-    dace_session.graph.add_constants({'Gtrans': gt})
+    dace_session.graph.add_constant('G', g)
+    dace_session.graph.add_constant('Gtrans', gt)
     gNode = 'G'
     gTransposeNode = 'Gtrans'
 
-    dace_session.graph.add_constants({'Atrans': at})
-    dace_session.graph.add_constants({'A': a})
+    dace_session.graph.add_constant('Atrans', at)
+    dace_session.graph.add_constant('A', a)
     aNode = 'A'
     aTransposeNode = 'Atrans'
 
     inputNodes = []
     inputParams = []
     inputDims = []
     for _inp in tf_node.inputs:
```

### Comparing `dace-0.9.0/dace/graph/dot.py` & `dace-0.9.5/dace/graph/dot.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
             ["{}=\"{}\"".format(key, value)
              for key, value in opts.items()]) + "];") if opts else ";"))
 
 
 def draw_edge(sdfg, graph, edge, **extraOpts):
     srcName = 's%d_%d' % (sdfg.node_id(graph), graph.node_id(edge.src))
     dstName = 's%d_%d' % (sdfg.node_id(graph), graph.node_id(edge.dst))
-
     return draw_edge_explicit(srcName, dstName, edge, sdfg, graph)
 
 
 def draw_interstate_edge(sdfg, src_graph, dst_graph, edge, **extraOpts):
     srcName = 's%d_%d' % (sdfg.node_id(src_graph), src_graph.node_id(edge.src))
     dstName = 's%d_%d' % (sdfg.node_id(dst_graph), dst_graph.node_id(edge.dst))
     if isinstance(edge, gr.MultiConnectorEdge):
@@ -84,32 +83,32 @@
         code = code.format(name=name)
         # Input connectors
         code += '<TR><TD BORDER="0"><TABLE BORDER="0" CELLBORDER="0" CELLSPACING="-8" CELLPADDING="0"><TR>'
         code += '<TD WIDTH="20"></TD>'
         connector_code = []
         for conn in sorted(obj.in_connectors):
             connector_code.append(
-                '<TD PORT="in_{conn}" BORDER="1" CELLPADDING="1"><FONT POINT-SIZE="10">{conn}</FONT></TD>'.
-                format(conn=conn))
+                '<TD PORT="in_{conn}" BORDER="1" CELLPADDING="1"><FONT POINT-SIZE="10">{conn}</FONT></TD>'
+                .format(conn=conn))
         code += '<TD WIDTH="20"></TD>'.join(connector_code)
         code += '<TD WIDTH="20"></TD></TR></TABLE></TD></TR>'
 
         # Contents
         html_label = html.escape(opts['label'][1:-1])
         code += '<TR><TD BORDER="0" CELLPADDING="15" COLOR="black">{label}</TD></TR>'.format(
             label=html_label)
 
         # Output connectors
         code += '<TR><TD BORDER="0"><TABLE BORDER="0" CELLBORDER="0" CELLSPACING="-8" CELLPADDING="0"><TR>'
         code += '<TD WIDTH="20"></TD>'
         connector_code = []
         for conn in sorted(obj.out_connectors):
             connector_code.append(
-                '<TD PORT="out_{conn}" BORDER="1" CELLPADDING="1"><FONT POINT-SIZE="10">{conn}</FONT></TD>'.
-                format(conn=conn))
+                '<TD PORT="out_{conn}" BORDER="1" CELLPADDING="1"><FONT POINT-SIZE="10">{conn}</FONT></TD>'
+                .format(conn=conn))
         code += '<TD WIDTH="20"></TD>'.join(connector_code)
         code += '<TD WIDTH="20"></TD></TR></TABLE></TD></TR>'
 
         # Footer
         code += '</TABLE>>'
 
         filtered_opts = {k: v for k, v in opts.items() if k != 'label'}
```

### Comparing `dace-0.9.0/dace/graph/edges.py` & `dace-0.9.5/dace/graph/edges.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 import ast
 import copy
 import enum
 import re
 
 import dace
-from dace import dtypes
+from dace import symbolic
 from dace.graph.graph import Edge
 from dace.frontend.python import astutils
 from dace.properties import Property, CodeProperty, make_properties
 
 
 def assignments_from_string(astr):
-    """ Returns a dictionary of assignments from a semicolon-delimited 
+    """ Returns a dictionary of assignments from a semicolon-delimited
         string of expressions. """
 
     result = {}
     for aitem in astr.split(';'):
         aitem = aitem.strip()
         m = re.search(r'([^=\s]+)\s*=\s*([^=]+)', aitem)
         result[m.group(1)] = m.group(2)
 
     return result
 
 
 def assignments_to_string(assdict):
-    """ Returns a semicolon-delimited string from a dictionary of assignment 
+    """ Returns a semicolon-delimited string from a dictionary of assignment
         expressions. """
     return '; '.join(['%s=%s' % (k, v) for k, v in assdict.items()])
 
 
 @make_properties
 class InterstateEdge(object):
-    """ An SDFG state machine edge. These edges can contain a condition     
+    """ An SDFG state machine edge. These edges can contain a condition
         (which may include data accesses for data-dependent decisions) and
         zero or more assignments of values to inter-state variables (e.g.,
         loop iterates).
     """
 
     assignments = Property(
         dtype=dict,
         desc="Assignments to perform upon transition (e.g., 'x=x+1; y = 0')",
         from_string=assignments_from_string,
         to_string=assignments_to_string)
-    condition = CodeProperty(desc="Transition condition")
+    condition = CodeProperty(
+        desc="Transition condition", default=ast.parse("1").body[0])
 
     def __init__(self, condition=None, assignments=None):
 
         if condition is None:
             condition = ast.parse("1").body[0]
 
         if assignments is None:
@@ -56,41 +57,40 @@
         self.assignments = assignments
 
         self._dotOpts = {"minlen": 3, "color": "blue", "fontcolor": "blue"}
 
     def is_unconditional(self):
         """ Returns True if the state transition is unconditional. """
         return (self.condition is None or InterstateEdge.condition.to_string(
-            self.condition).strip() == "1")
+            self.condition).strip() == "1" or self.condition.as_string == "")
 
     def condition_sympy(self):
         cond_ast = self.condition
         return symbolic.pystr_to_symbolic(astutils.unparse(cond_ast))
 
     def condition_symbols(self):
         return dace.symbolic.symbols_in_ast(self.condition[0])
 
-    def toJSON(self, parent=None):
-        import json
+    def to_json(self, parent=None):
         ret = {
             'type': type(self).__name__,
-            'attributes': json.loads(Property.all_properties_to_json(self)),
+            'attributes': dace.serialize.all_properties_to_json(self),
             'label': self.label
         }
 
-        return json.dumps(ret)
+        return ret
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
+    def from_json(json_obj, context=None):
         if json_obj['type'] != "InterstateEdge":
             raise TypeError("Invalid data type")
 
         # Create dummy object
         ret = InterstateEdge()
-        Property.set_properties_from_json(ret, json_obj, context=context)
+        dace.serialize.set_properties_from_json(ret, json_obj, context=context)
 
         return ret
 
     @property
     def label(self):
         assignments = ','.join(
             ['%s=%s' % (k, v) for k, v in self.assignments.items()])
@@ -103,15 +103,15 @@
             return assignments
 
         # Edge with condition only (no assignment)
         if len(self.assignments) == 0:
             return astutils.unparse(self.condition)
 
         # Edges with assigments and conditions
-        return assignments + '; ' + astutils.unparse(self.condition)
+        return astutils.unparse(self.condition) + '; ' + assignments
 
     @property
     def dotOpts(self):
         result = {}
         result.update(self._dotOpts)
         result.update({'label': self.label})
         return result
@@ -162,55 +162,55 @@
 class ControlFlow:
     pass
 
 
 @make_properties
 class LoopAssignment(ControlFlow):
 
-    scope = Property(dtype=LoopScope)
-    edge = Property(dtype=Edge)
+    scope = Property(dtype=LoopScope, allow_none=True)
+    edge = Property(dtype=Edge, allow_none=True)
 
     def __init__(self, scope, edge, *args, **kwargs):
         self.scope = scope
         self.edge = edge
         scope.assignment = self
         super().__init__(*args, **kwargs)
 
 
 @make_properties
 class LoopEntry(ControlFlow):
 
-    scope = Property(dtype=LoopScope)
-    edge = Property(dtype=Edge)
+    scope = Property(dtype=LoopScope, allow_none=True)
+    edge = Property(dtype=Edge, allow_none=True)
 
     def __init__(self, scope, edge, *args, **kwargs):
         self.scope = scope
         self.edge = edge
         scope.entry = self
         super().__init__(*args, **kwargs)
 
 
 @make_properties
 class LoopExit(ControlFlow):
 
-    scope = Property(dtype=LoopScope)
-    edge = Property(dtype=Edge)
+    scope = Property(dtype=LoopScope, allow_none=True)
+    edge = Property(dtype=Edge, allow_none=True)
 
     def __init__(self, scope, edge, *args, **kwargs):
         self.scope = scope
         self.edge = edge
         scope.exit = self
         super().__init__(*args, **kwargs)
 
 
 @make_properties
 class LoopBack(ControlFlow):
 
-    scope = Property(dtype=LoopScope)
-    edge = Property(dtype=Edge)
+    scope = Property(dtype=LoopScope, allow_none=True)
+    edge = Property(dtype=Edge, allow_none=True)
 
     def __init__(self, scope, edge, *args, **kwargs):
         self.scope = scope
         self.edge = edge
         scope.back = self
         super().__init__(*args, **kwargs)
 
@@ -223,69 +223,69 @@
 LoopScope = make_properties(LoopScope)
 
 
 # Extra meta-object binding together then and else scopes.
 # make_properties will be called after adding cyclic class reference members
 class IfThenElse:
 
-    entry = Property()
-    exit = Property()
+    entry = Property(allow_none=True)
+    exit = Property(allow_none=True)
 
     def __init__(self, entry, exit):
         self.entry = entry
         self.exit = exit
         self.then_scope = None
         self.else_scope = None
 
 
 @make_properties
 class IfEntry(ControlFlow):
 
-    scope = Property(dtype=ControlFlowScope)
-    edge = Property(dtype=Edge)
+    scope = Property(dtype=ControlFlowScope, allow_none=True)
+    edge = Property(dtype=Edge, allow_none=True)
 
     def __init__(self, scope, edge, *args, **kwargs):
         self.scope = scope
         self.edge = edge
         scope.entry = self
         super().__init__(*args, **kwargs)
 
 
 @make_properties
 class IfExit(ControlFlow):
 
-    scope = Property(dtype=ControlFlowScope)
-    edge = Property(dtype=Edge)
+    scope = Property(dtype=ControlFlowScope, allow_none=True)
+    edge = Property(dtype=Edge, allow_none=True)
 
     def __init__(self, scope, edge, *args, **kwargs):
         self.scope = scope
         self.edge = edge
         scope.exit = self
         super().__init__(*args, **kwargs)
 
 
 @make_properties
 class IfThenScope(ControlFlowScope):
 
-    if_then_else = Property(dtype=IfThenElse)
+    if_then_else = Property(dtype=IfThenElse, allow_none=True)
     entry = Property(dtype=IfEntry, allow_none=True)
     exit = Property(dtype=IfExit, allow_none=True)
 
     def __init__(self, if_then_else, *args, **kwargs):
         self.if_then_else = if_then_else
         if_then_else.then_scope = self
         self.entry = None
         self.exit = None
         super().__init__(*args, **kwargs)
 
 
 @make_properties
 class IfElseScope(ControlFlowScope):
 
-    if_then_else = Property(dtype=IfThenElse)
+    if_then_else = Property(dtype=IfThenElse, allow_none=True)
     entry = Property(dtype=IfEntry, allow_none=True)
     exit = Property(dtype=IfExit, allow_none=True)
 
     def __init__(self, if_then_else, *args, **kwargs):
         self.if_then_else = if_then_else
         if_then_else.else_scope = self
         self.entry = None
```

### Comparing `dace-0.9.0/dace/graph/graph.py` & `dace-0.9.5/dace/graph/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """ Graph and multigraph implementations for DaCe. """
 
 from collections import deque, OrderedDict
 import itertools
 import networkx as nx
 from dace.dtypes import deduplicate
 from dace.properties import Property
-import json
+import dace.serialize
 
 
 class NodeNotFoundError(Exception):
     pass
 
 
 class EdgeNotFoundError(Exception):
     pass
 
 
+@dace.serialize.serializable
 class Edge(object):
     def __init__(self, src, dst, data):
         self._src = src
         self._dst = dst
         self._data = data
 
     @property
@@ -35,31 +36,31 @@
         return self._data
 
     def __iter__(self):
         yield self._src
         yield self._dst
         yield self._data
 
-    def toJSON(self, parent_graph):
+    def to_json(self, parent_graph):
         # Slight hack to preserve the old format (attributes should not behave like this)
-        memlet_ret = json.loads(self.data.toJSON(parent_graph))
+        memlet_ret = self.data.to_json(parent_graph)
         ret = {
             'type': type(self).__name__,
             'attributes': {
                 'data':
                 memlet_ret  #TODO: FIXME: Why is data() not a Property instance? (Would need MemletProperty class)
             },
             'src': str(parent_graph.node_id(self.src)),
             'dst': str(parent_graph.node_id(self.dst)),
         }
 
-        return json.dumps(ret)
+        return ret
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
+    def from_json(json_obj, context=None):
         if json_obj['type'] != "Edge":
             raise TypeError("Invalid data type")
 
         ret = Edge(json_obj['src'], json_obj['dst'],
                    json_obj['attributes']['data'])
 
         return ret
@@ -68,42 +69,44 @@
     def __len__():
         return 3
 
     def reverse(self):
         self._src, self._dst = self._dst, self._src
 
 
+@dace.serialize.serializable
 class MultiEdge(Edge):
     def __init__(self, src, dst, data, key):
         super(MultiEdge, self).__init__(src, dst, data)
         self._key = key
 
     @property
     def key(self):
         return self._key
 
 
+@dace.serialize.serializable
 class MultiConnectorEdge(MultiEdge):
     def __init__(self, src, src_conn, dst, dst_conn, data, key):
         super(MultiConnectorEdge, self).__init__(src, dst, data, key)
         self._src_conn = src_conn
         self._dst_conn = dst_conn
 
-    def toJSON(self, parent_graph):
-        ret = json.loads(super(MultiConnectorEdge, self).toJSON(parent_graph))
+    def to_json(self, parent_graph):
+        ret = super().to_json(parent_graph)
 
         ret['dst_connector'] = self.dst_conn
         ret['src_connector'] = self.src_conn
 
         ret['type'] = "MultiConnectorEdge"
 
-        return json.dumps(ret)
+        return ret
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
+    def from_json(json_obj, context=None):
 
         sdfg = context['sdfg_state']
         if sdfg is None:
             raise Exception("parent_graph must be defined for this method")
         data = json_obj['attributes']['data']
         src_nid = json_obj['src']
         dst_nid = json_obj['dst']
@@ -144,27 +147,27 @@
         yield self._data
 
     @staticmethod
     def __len__():
         return 5
 
 
+@dace.serialize.serializable
 class Graph(object):
     def _not_implemented_error(self):
         return NotImplementedError("Not implemented for " + str(type(self)))
 
-    def toJSON(self):
-        import json
+    def to_json(self):
         ret = {
             'type': type(self).__name__,
-            'attributes': json.loads(Property.all_properties_to_json(self)),
-            'nodes': [json.loads(n.toJSON(self)) for n in self.nodes()],
-            'edges': [json.loads(e.toJSON(self)) for e in self.edges()],
+            'attributes': dace.serialize.all_properties_to_json(self),
+            'nodes': [n.to_json(self) for n in self.nodes()],
+            'edges': [e.to_json(self) for e in self.edges()],
         }
-        return json.dumps(ret)
+        return ret
 
     def nodes(self):
         """Returns an iterable to internal graph nodes."""
         raise self._not_implemented_error()
 
     def edges(self):
         """Returns an iterable to internal graph edges."""
@@ -360,14 +363,15 @@
 
     def all_simple_paths(self, source_node, dest_node):
         """ Finds all simple paths (with no repeating nodes) from source_node
             to dest_node """
         return nx.all_simple_paths(self._nx, source_node, dest_node)
 
 
+@dace.serialize.serializable
 class SubgraphView(Graph):
     def __init__(self, graph, subgraph_nodes):
         self._graph = graph
         self._subgraph_nodes = subgraph_nodes
         self._parallel_parent = None
 
     def is_parallel(self):
@@ -449,15 +453,20 @@
 
     def is_directed(self):
         return self._graph.is_directed()
 
     def is_multigraph(self):
         return self._graph.is_multigraph()
 
+    @property
+    def graph(self):
+        return self._graph
+
 
+@dace.serialize.serializable
 class DiGraph(Graph):
     def __init__(self):
         self._nx = nx.DiGraph()
 
     def nodes(self):
         return self._nx.nodes()
 
@@ -553,14 +562,15 @@
     def remove_edge(self, edge):
         self._nx.remove_edge(edge[0], edge[1], edge.key)
 
     def is_multigraph(self):
         return True
 
 
+@dace.serialize.serializable
 class OrderedDiGraph(Graph):
     """ Directed graph where nodes and edges are returned in the order they
         were added. """
 
     def __init__(self):
         self._nx = nx.DiGraph()
         # {node: ({in edge: None}, {out edges: None})}
```

### Comparing `dace-0.9.0/dace/graph/labeling.py` & `dace-0.9.5/dace/graph/labeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -592,16 +592,16 @@
     """
     for state in sdfg.nodes():
         _propagate_labels(state, sdfg)
 
 
 def _propagate_labels(g, sdfg):
     """ Propagates memlets throughout one SDFG state. 
-        @param g: The state to propagate in.
-        @param sdfg: The SDFG in which the state is situated.
+        :param g: The state to propagate in.
+        :param sdfg: The SDFG in which the state is situated.
         @note: This is an in-place operation on the SDFG state.
     """
     patterns = MemletPattern.patterns()
 
     # Algorithm:
     # 1. Start propagating information from tasklets outwards (their edges
     #    are hardcoded).
@@ -669,34 +669,37 @@
         ]
         external_edges = [
             e for e in dfg_state.out_edges(node)
             if e.src_conn and e.src_conn.startswith('OUT_')
         ]
 
     for edge in external_edges:
-        internal_edge = next(
-            e for e in internal_edges if e.data.data == edge.data.data)
-        new_memlet = propagate_memlet(dfg_state, internal_edge.data, node,
-                                      True)
+        if isinstance(edge.data, EmptyMemlet):
+            new_memlet = EmptyMemlet()
+        else:
+            internal_edge = next(
+                e for e in internal_edges if e.data.data == edge.data.data)
+            new_memlet = propagate_memlet(dfg_state, internal_edge.data, node,
+                                          True)
         edge._data = new_memlet
 
 
 # External API
 def propagate_memlet(dfg_state,
                      memlet: Memlet,
                      scope_node: nodes.EntryNode,
                      union_inner_edges: bool,
                      arr=None):
     """ Tries to propagate a memlet through a scope (computes the image of 
         the memlet function applied on an integer set of, e.g., a map range) 
         and returns a new memlet object.
-        @param dfg_state: An SDFGState object representing the graph.
-        @param memlet: The memlet adjacent to the scope node from the inside.
-        @param scope_node: A scope entry or exit node.
-        @param union_inner_edges: True if the propagation should take other
+        :param dfg_state: An SDFGState object representing the graph.
+        :param memlet: The memlet adjacent to the scope node from the inside.
+        :param scope_node: A scope entry or exit node.
+        :param union_inner_edges: True if the propagation should take other
                                   neighboring internal memlets within the same
                                   scope into account.
     """
     if isinstance(scope_node, nodes.EntryNode):
         entry_node = scope_node
         neighboring_edges = dfg_state.out_edges(scope_node)
     elif isinstance(scope_node, nodes.ExitNode):
@@ -704,25 +707,29 @@
         neighboring_edges = dfg_state.in_edges(scope_node)
     else:
         raise TypeError('Trying to propagate through a non-scope node')
     if isinstance(memlet, EmptyMemlet):
         return EmptyMemlet()
 
     sdfg = dfg_state.parent
+    scope_node_symbols = set(
+        conn for conn in scope_node.in_connectors
+        if not conn.startswith('IN_'))
     defined_vars = [
         symbolic.pystr_to_symbolic(s)
         for s in (sdfg.symbols_defined_at(scope_node, dfg_state).keys())
+        if s not in scope_node_symbols
     ]
 
     # Find other adjacent edges within the connected to the scope node
     # and union their subsets
     if union_inner_edges:
         aggdata = [
             e.data for e in neighboring_edges
-            if e.data.data == arr and e.data != memlet
+            if e.data.data == memlet.data and e.data != memlet
         ]
     else:
         aggdata = []
 
     aggdata.append(memlet)
 
     if arr is None:
@@ -787,13 +794,14 @@
 
     # Number of accesses in the propagated memlet is the sum of the internal
     # number of accesses times the size of the map range set
     new_memlet.num_accesses = (
         sum(m.num_accesses for m in aggdata) * functools.reduce(
             lambda a, b: a * b, scope_node.map.range.size(), 1))
     if any(m.num_accesses == -1 for m in aggdata):
-        memlet.num_accesses = -1
-    elif symbolic.issymbolic(memlet.num_accesses) and any(
-            s not in defined_vars for s in memlet.num_accesses.free_symbols):
-        memlet.num_accesses = -1
+        new_memlet.num_accesses = -1
+    elif symbolic.issymbolic(new_memlet.num_accesses) and any(
+            s not in defined_vars
+            for s in new_memlet.num_accesses.free_symbols):
+        new_memlet.num_accesses = -1
 
     return new_memlet
```

### Comparing `dace-0.9.0/dace/graph/nodes.py` & `dace-0.9.5/dace/graph/nodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """ Contains classes implementing the different types of nodes of the stateful
     dataflow multigraph representation. """
 
 import ast
 from copy import deepcopy as dcpy
 import itertools
+import dace.serialize
 from typing import Set
 from dace.graph import dot, graph
 from dace.frontend.python.astutils import unparse
 from dace.properties import (
     Property, CodeProperty, LambdaProperty, ParamsProperty, RangeProperty,
     DebugInfoProperty, SetProperty, make_properties, indirect_properties,
     DataProperty, SymbolicProperty, ListProperty, SDFGReferenceProperty)
 from dace.frontend.operations import detect_reduction_type
 from dace import data, subsets as sbs, dtypes
-import json
 
 # -----------------------------------------------------------------------------
 
 
 @make_properties
 class Node(object):
     """ Base node class. """
@@ -36,90 +36,96 @@
             return self.label
         else:
             return type(self).__name__
 
     def validate(self, sdfg, state):
         pass
 
-    def toJSON(self, parent):
+    def to_json(self, parent):
         labelstr = str(self)
         typestr = str(type(self).__name__)
 
         scope_entry_node = parent.entry_node(self)
         if scope_entry_node is not None:
             ens = parent.exit_nodes(parent.entry_node(self))
             scope_exit_nodes = [str(parent.node_id(x)) for x in ens]
             scope_entry_node = str(parent.node_id(scope_entry_node))
         else:
             scope_entry_node = None
             scope_exit_nodes = []
 
+        # The scope exit of an entry node is the matching exit node
+        if isinstance(self, EntryNode):
+            scope_exit_nodes = [
+                str(parent.node_id(x)) for x in parent.exit_nodes(self)
+            ]
+
         retdict = {
             "type": typestr,
             "label": labelstr,
-            "attributes": json.loads(Property.all_properties_to_json(self)),
+            "attributes": dace.serialize.all_properties_to_json(self),
             "id": parent.node_id(self),
             "scope_entry": scope_entry_node,
             "scope_exits": scope_exit_nodes
         }
-        return json.dumps(retdict)
+        return retdict
 
     def __repr__(self):
         return type(self).__name__ + ' (' + self.__str__() + ')'
 
     def add_in_connector(self, connector_name: str):
         """ Adds a new input connector to the node. The operation will fail if
-            a connector (either input or output) with the same name already 
+            a connector (either input or output) with the same name already
             exists in the node.
 
-            @param connector_name: The name of the new connector.
-            @return: True if the operation is successful, otherwise False.
+            :param connector_name: The name of the new connector.
+            :return: True if the operation is successful, otherwise False.
         """
 
         if (connector_name in self.in_connectors
                 or connector_name in self.out_connectors):
             return False
         connectors = self.in_connectors
         connectors.add(connector_name)
         self.in_connectors = connectors
         return True
 
     def add_out_connector(self, connector_name: str):
         """ Adds a new output connector to the node. The operation will fail if
-            a connector (either input or output) with the same name already 
+            a connector (either input or output) with the same name already
             exists in the node.
 
-            @param connector_name: The name of the new connector.
-            @return: True if the operation is successful, otherwise False.
+            :param connector_name: The name of the new connector.
+            :return: True if the operation is successful, otherwise False.
         """
 
         if (connector_name in self.in_connectors
                 or connector_name in self.out_connectors):
             return False
         connectors = self.out_connectors
         connectors.add(connector_name)
         self.out_connectors = connectors
         return True
 
     def remove_in_connector(self, connector_name: str):
         """ Removes an input connector from the node.
-            @param connector_name: The name of the connector to remove.
-            @return: True if the operation was successful.
+            :param connector_name: The name of the connector to remove.
+            :return: True if the operation was successful.
         """
 
         if connector_name in self.in_connectors:
             connectors = self.in_connectors
             connectors.remove(connector_name)
             self.in_connectors = connectors
         return True
 
     def remove_out_connector(self, connector_name: str):
         """ Removes an output connector from the node.
-            @param connector_name: The name of the connector to remove.
-            @return: True if the operation was successful.
+            :param connector_name: The name of the connector to remove.
+            :return: True if the operation was successful.
         """
 
         if connector_name in self.out_connectors:
             connectors = self.out_connectors
             connectors.remove(connector_name)
             self.out_connectors = connectors
         return True
@@ -135,15 +141,15 @@
                 cconn = conn[4:]
             else:
                 continue
             try:
                 curconn = int(cconn)
                 if curconn >= next_number:
                     next_number = curconn + 1
-            except TypeError:  # not integral
+            except (TypeError, ValueError):  # not integral
                 continue
         return next_number
 
     def next_connector(self) -> str:
         """ Returns the next unused connector ID (as a string). Used for
             filling connectors when adding edges to scopes. """
         return str(self._next_connector_int())
@@ -158,15 +164,15 @@
 
 
 @make_properties
 class AccessNode(Node):
     """ A node that accesses data in the SDFG. Denoted by a circular shape. """
 
     access = Property(
-        enum=dtypes.AccessType,
+        choices=dtypes.AccessType,
         desc="Type of access to this array",
         default=dtypes.AccessType.ReadWrite)
     setzero = Property(dtype=bool, desc="Initialize to zero", default=False)
     debuginfo2 = DebugInfoProperty()
     data = DataProperty(desc="Data (array, stream, scalar) to access")
 
     def __init__(self,
@@ -179,17 +185,17 @@
         self.debuginfo2 = debuginfo
         self.access = access
         if not isinstance(data, str):
             raise TypeError('Data for AccessNode must be a string')
         self.data = data
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
+    def from_json(json_obj, context=None):
         ret = AccessNode("Nodata")
-        Property.set_properties_from_json(ret, json_obj, context=context)
+        dace.serialize.set_properties_from_json(ret, json_obj, context=context)
         return ret
 
     def __deepcopy__(self, memo):
         node = object.__new__(AccessNode)
         node._access = self._access
         node._data = self._data
         node._setzero = self._setzero
@@ -226,44 +232,44 @@
             raise KeyError('Array "%s" not found in SDFG' % self.data)
 
 
 # ------------------------------------------------------------------------------
 
 
 class CodeNode(Node):
-    """ A node that contains runnable code with acyclic external data 
-        dependencies. May either be a tasklet or a nested SDFG, and 
+    """ A node that contains runnable code with acyclic external data
+        dependencies. May either be a tasklet or a nested SDFG, and
         denoted by an octagonal shape. """
     pass
 
 
 @make_properties
 class Tasklet(CodeNode):
     """ A node that contains a tasklet: a functional computation procedure
-        that can only access external data specified using connectors. 
-        
-        Tasklets may be implemented in Python, C++, or any supported 
-        language by the code generator. 
+        that can only access external data specified using connectors.
+
+        Tasklets may be implemented in Python, C++, or any supported
+        language by the code generator.
     """
 
     label = Property(dtype=str, desc="Name of the tasklet")
-    code = CodeProperty(desc="Tasklet code")
+    code = CodeProperty(desc="Tasklet code", default="")
     code_global = CodeProperty(
         desc="Global scope code needed for tasklet execution", default="")
     code_init = CodeProperty(
         desc="Extra code that is called on DaCe runtime initialization",
         default="")
     code_exit = CodeProperty(
         desc="Extra code that is called on DaCe runtime cleanup", default="")
     location = Property(
         dtype=str, desc="Tasklet execution location descriptor")
     debuginfo = DebugInfoProperty()
 
     instrument = Property(
-        enum=dtypes.InstrumentationType,
+        choices=dtypes.InstrumentationType,
         desc="Measure execution statistics with given method",
         default=dtypes.InstrumentationType.No_Instrumentation)
 
     def __init__(self,
                  label,
                  inputs=None,
                  outputs=None,
@@ -289,17 +295,17 @@
         self.debuginfo = debuginfo
 
     @property
     def language(self):
         return self._code['language']
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
+    def from_json(json_obj, context=None):
         ret = Tasklet("dummylabel")
-        Property.set_properties_from_json(ret, json_obj, context=context)
+        dace.serialize.set_properties_from_json(ret, json_obj, context=context)
         return ret
 
     @property
     def name(self):
         return self._label
 
     def draw_node(self, sdfg, graph):
@@ -318,65 +324,67 @@
     def __str__(self):
         if not self.label:
             return "--Empty--"
         else:
             return self.label
 
 
+@make_properties
 class EmptyTasklet(Tasklet):
     """ A special tasklet that contains no code. Used for filling empty states
         in an SDFG. """
 
     def __init__(self, label=""):
         super(EmptyTasklet, self).__init__(label)
 
     def draw_node(self, sdfg, graph):
         return dot.draw_node(sdfg, graph, self, style="invis", shape="octagon")
 
     def validate(self, sdfg, state):
         pass
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
+    def from_json(json_obj, context=None):
         ret = EmptyTasklet("dummylabel")
-        Property.set_properties_from_json(ret, json_obj, context=context)
+        dace.serialize.set_properties_from_json(ret, json_obj, context=context)
         return ret
 
 
 # ------------------------------------------------------------------------------
 
 
 @make_properties
 class NestedSDFG(CodeNode):
     """ An SDFG state node that contains an SDFG of its own, runnable using
         the data dependencies specified using its connectors.
 
         It is encouraged to use nested SDFGs instead of coarse-grained tasklets
         since they are analyzable with respect to transformations.
-        
+
         @note: A nested SDFG cannot create recursion (one of its parent SDFGs).
     """
 
     label = Property(dtype=str, desc="Name of the SDFG")
     # NOTE: We cannot use SDFG as the type because of an import loop
-    sdfg = SDFGReferenceProperty(dtype=graph.OrderedDiGraph, desc="The SDFG")
+    sdfg = SDFGReferenceProperty(desc="The SDFG", allow_none=True)
     schedule = Property(
         dtype=dtypes.ScheduleType,
         desc="SDFG schedule",
-        enum=dtypes.ScheduleType,
-        from_string=lambda x: dtypes.ScheduleType[x])
+        choices=dtypes.ScheduleType,
+        from_string=lambda x: dtypes.ScheduleType[x],
+        default=dtypes.ScheduleType.Default)
     location = Property(dtype=str, desc="SDFG execution location descriptor")
     debuginfo = DebugInfoProperty()
     is_collapsed = Property(
         dtype=bool,
         desc="Show this node/scope/state as collapsed",
         default=False)
 
     instrument = Property(
-        enum=dtypes.InstrumentationType,
+        choices=dtypes.InstrumentationType,
         desc="Measure execution statistics with given method",
         default=dtypes.InstrumentationType.No_Instrumentation)
 
     def __init__(self,
                  label,
                  sdfg,
                  inputs: Set[str],
@@ -390,27 +398,29 @@
         self.label = label
         self.sdfg = sdfg
         self.schedule = schedule
         self.location = location
         self.debuginfo = debuginfo
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
+    def from_json(json_obj, context=None):
         from dace import SDFG  # Avoid import loop
 
         # We have to load the SDFG first.
         ret = NestedSDFG("nolabel", SDFG('nosdfg'), set(), set())
 
-        Property.set_properties_from_json(ret, json_obj, context)
+        dace.serialize.set_properties_from_json(ret, json_obj, context)
 
         if context and 'sdfg_state' in context:
             ret.sdfg.parent = context['sdfg_state']
         if context and 'sdfg' in context:
             ret.sdfg.parent_sdfg = context['sdfg']
 
+        ret.sdfg.update_sdfg_list([])
+
         return ret
 
     def draw_node(self, sdfg, graph):
         return dot.draw_node(sdfg, graph, self, shape="doubleoctagon")
 
     def __str__(self):
         if not self.label:
@@ -453,30 +463,41 @@
     def validate(self, sdfg, state):
         self.map.validate(sdfg, state, self)
 
 
 # ------------------------------------------------------------------------------
 
 
+@dace.serialize.serializable
 class MapEntry(EntryNode):
-    """ Node that opens a Map scope. 
+    """ Node that opens a Map scope.
         @see: Map
     """
 
     def __init__(self, map, dynamic_inputs=None):
         super(MapEntry, self).__init__(dynamic_inputs or set())
         if map is None:
             raise ValueError("Map for MapEntry can not be None.")
         self._map = map
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
+    def from_json(json_obj, context=None):
         m = Map("", [], [])
         ret = MapEntry(map=m)
-        Property.set_properties_from_json(ret, json_obj, context=context)
+
+        try:
+            # Set map reference to map exit
+            nid = int(json_obj['scope_exits'][0])
+            exit_node = context['sdfg_state'].node(nid)
+            exit_node.map = m
+        except IndexError:  # Exit node has a higher node ID
+            # Connection of the scope nodes handled in MapExit
+            pass
+
+        dace.serialize.set_properties_from_json(ret, json_obj, context=context)
         return ret
 
     @property
     def map(self):
         return self._map
 
     @map.setter
@@ -488,32 +509,39 @@
             return dot.draw_node(sdfg, graph, self, shape="hexagon")
         return dot.draw_node(sdfg, graph, self, shape="trapezium")
 
     def __str__(self):
         return str(self.map)
 
 
+@dace.serialize.serializable
 class MapExit(ExitNode):
     """ Node that closes a Map scope.
         @see: Map
     """
 
     def __init__(self, map):
         super(MapExit, self).__init__()
         if map is None:
             raise ValueError("Map for MapExit can not be None.")
         self._map = map
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
-        # Set map reference to map entry
-        entry_node = context['sdfg_state'].node(int(json_obj['scope_entry']))
+    def from_json(json_obj, context=None):
+        try:
+            # Set map reference to map entry
+            entry_node = context['sdfg_state'].node(
+                int(json_obj['scope_entry']))
+
+            ret = MapExit(map=entry_node.map)
+        except IndexError:  # Entry node has a higher ID than exit node
+            # Connection of the scope nodes handled in MapEntry
+            ret = MapExit(Map('_', [], []))
 
-        ret = MapExit(map=entry_node.map)
-        Property.set_properties_from_json(ret, json_obj, context=context)
+        dace.serialize.set_properties_from_json(ret, json_obj, context=context)
 
         return ret
 
     @property
     def map(self):
         return self._map
 
@@ -539,42 +567,44 @@
     def __str__(self):
         return str(self.map)
 
 
 @make_properties
 class Map(object):
     """ A Map is a two-node representation of parametric graphs, containing
-        an integer set by which the contents (nodes dominated by an entry 
+        an integer set by which the contents (nodes dominated by an entry
         node and post-dominated by an exit node) are replicated.
-        
+
         Maps contain a `schedule` property, which specifies how the scope
         should be scheduled (execution order). Code generators can use the
         schedule property to generate appropriate code, e.g., GPU kernels.
     """
 
     # List of (editable) properties
     label = Property(dtype=str, desc="Label of the map")
     params = ParamsProperty(desc="Mapped parameters")
-    range = RangeProperty(desc="Ranges of map parameters")
+    range = RangeProperty(
+        desc="Ranges of map parameters", default=sbs.Range([]))
     schedule = Property(
         dtype=dtypes.ScheduleType,
         desc="Map schedule",
-        enum=dtypes.ScheduleType,
-        from_string=lambda x: dtypes.ScheduleType[x])
+        choices=dtypes.ScheduleType,
+        from_string=lambda x: dtypes.ScheduleType[x],
+        default=dtypes.ScheduleType.Default)
     is_async = Property(dtype=bool, desc="Map asynchronous evaluation")
     unroll = Property(dtype=bool, desc="Map unrolling")
     flatten = Property(dtype=bool, desc="Map loop flattening")
     debuginfo = DebugInfoProperty()
     is_collapsed = Property(
         dtype=bool,
         desc="Show this node/scope/state as collapsed",
         default=False)
 
     instrument = Property(
-        enum=dtypes.InstrumentationType,
+        choices=dtypes.InstrumentationType,
         desc="Measure execution statistics with given method",
         default=dtypes.InstrumentationType.No_Instrumentation)
 
     def __init__(self,
                  label,
                  params,
                  ndrange,
@@ -615,33 +645,44 @@
 
 # Indirect Map properties to MapEntry and MapExit
 MapEntry = indirect_properties(Map, lambda obj: obj.map)(MapEntry)
 
 # ------------------------------------------------------------------------------
 
 
+@dace.serialize.serializable
 class ConsumeEntry(EntryNode):
-    """ Node that opens a Consume scope. 
+    """ Node that opens a Consume scope.
         @see: Consume
     """
 
     def __init__(self, consume, dynamic_inputs=None):
         super(ConsumeEntry, self).__init__(dynamic_inputs or set())
         if consume is None:
             raise ValueError("Consume for ConsumeEntry can not be None.")
         self._consume = consume
         self._map_depth = 0
         self.add_in_connector('IN_stream')
         self.add_out_connector('OUT_stream')
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
+    def from_json(json_obj, context=None):
         c = Consume("", ['i', 1], None)
         ret = ConsumeEntry(consume=c)
-        Property.set_properties_from_json(ret, json_obj, context=context)
+
+        try:
+            # Set map reference to map exit
+            nid = int(json_obj['scope_exits'][0])
+            exit_node = context['sdfg_state'].node(nid)
+            exit_node.consume = c
+        except IndexError:  # Exit node has a higher node ID
+            # Connection of the scope nodes handled in ConsumeExit
+            pass
+
+        dace.serialize.set_properties_from_json(ret, json_obj, context=context)
         return ret
 
     @property
     def map(self):
         return self._consume.as_map()
 
     @property
@@ -659,32 +700,38 @@
         return dot.draw_node(
             sdfg, graph, self, shape="trapezium", style='dashed')
 
     def __str__(self):
         return str(self.consume)
 
 
+@dace.serialize.serializable
 class ConsumeExit(ExitNode):
-    """ Node that closes a Consume scope. 
+    """ Node that closes a Consume scope.
         @see: Consume
     """
 
     def __init__(self, consume):
         super(ConsumeExit, self).__init__()
         if consume is None:
             raise ValueError("Consume for ConsumeExit can not be None.")
         self._consume = consume
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
-        # Set map reference to entry node
-        entry_node = context['sdfg_state'].node(int(json_obj['scope_entry']))
+    def from_json(json_obj, context=None):
+        try:
+            # Set consume reference to entry node
+            entry_node = context['sdfg_state'].node(
+                int(json_obj['scope_entry']))
+            ret = ConsumeExit(consume=entry_node.consume)
+        except IndexError:  # Entry node has a higher ID than exit node
+            # Connection of the scope nodes handled in ConsumeEntry
+            ret = ConsumeExit(Consume("", ['i', 1], None))
 
-        ret = ConsumeExit(consume=entry_node.consume)
-        Property.set_properties_from_json(ret, json_obj, context=context)
+        dace.serialize.set_properties_from_json(ret, json_obj, context=context)
         return ret
 
     @property
     def map(self):
         return self._consume.as_map()
 
     @property
@@ -713,43 +760,44 @@
 
     def __str__(self):
         return str(self.consume)
 
 
 @make_properties
 class Consume(object):
-    """ Consume is a scope, like `Map`, that is a part of the parametric 
-        graph extension of the SDFG. It creates a producer-consumer 
+    """ Consume is a scope, like `Map`, that is a part of the parametric
+        graph extension of the SDFG. It creates a producer-consumer
         relationship between the input stream and the scope subgraph. The
         subgraph is scheduled to a given number of processing elements
         for processing, and they will try to pop elements from the input
         stream until a given quiescence condition is reached. """
 
     # Properties
     label = Property(dtype=str, desc="Name of the consume node")
     pe_index = Property(dtype=str, desc="Processing element identifier")
-    num_pes = SymbolicProperty(desc="Number of processing elements")
+    num_pes = SymbolicProperty(desc="Number of processing elements", default=1)
     condition = CodeProperty(desc="Quiescence condition", allow_none=True)
     schedule = Property(
         dtype=dtypes.ScheduleType,
         desc="Consume schedule",
-        enum=dtypes.ScheduleType,
-        from_string=lambda x: dtypes.ScheduleType[x])
+        choices=dtypes.ScheduleType,
+        from_string=lambda x: dtypes.ScheduleType[x],
+        default=dtypes.ScheduleType.Default)
     chunksize = Property(
         dtype=int,
         desc="Maximal size of elements to consume at a time",
         default=1)
     debuginfo = DebugInfoProperty()
     is_collapsed = Property(
         dtype=bool,
         desc="Show this node/scope/state as collapsed",
         default=False)
 
     instrument = Property(
-        enum=dtypes.InstrumentationType,
+        choices=dtypes.InstrumentationType,
         desc="Measure execution statistics with given method",
         default=dtypes.InstrumentationType.No_Instrumentation)
 
     def as_map(self):
         """ Compatibility function that allows to view the consume as a map,
             mainly in memlet propagation. """
         return Map(self.label, [self.pe_index],
@@ -795,31 +843,32 @@
                                    lambda obj: obj.consume)(ConsumeEntry)
 
 # ------------------------------------------------------------------------------
 
 
 @make_properties
 class Reduce(Node):
-    """ An SDFG node that reduces an N-dimensional array to an 
+    """ An SDFG node that reduces an N-dimensional array to an
         (N-k)-dimensional array, with a list of axes to reduce and
         a reduction binary function. """
 
     # Properties
     axes = ListProperty(element_type=int, allow_none=True)
-    wcr = LambdaProperty()
+    wcr = LambdaProperty(default='lambda a,b: a')
     identity = Property(dtype=object, allow_none=True)
     schedule = Property(
         dtype=dtypes.ScheduleType,
         desc="Reduction execution policy",
-        enum=dtypes.ScheduleType,
-        from_string=lambda x: dtypes.ScheduleType[x])
+        choices=dtypes.ScheduleType,
+        from_string=lambda x: dtypes.ScheduleType[x],
+        default=dtypes.ScheduleType.Default)
     debuginfo = DebugInfoProperty()
 
     instrument = Property(
-        enum=dtypes.InstrumentationType,
+        choices=dtypes.InstrumentationType,
         desc="Measure execution statistics with given method",
         default=dtypes.InstrumentationType.No_Instrumentation)
 
     def __init__(self,
                  wcr,
                  axes,
                  wcr_identity=None,
@@ -832,17 +881,17 @@
         self.schedule = schedule
         self.debuginfo = debuginfo
 
     def draw_node(self, sdfg, state):
         return dot.draw_node(sdfg, state, self, shape="invtriangle")
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
+    def from_json(json_obj, context=None):
         ret = Reduce("(lambda a, b: (a + b))", None)
-        Property.set_properties_from_json(ret, json_obj, context=context)
+        dace.serialize.set_properties_from_json(ret, json_obj, context=context)
         return ret
 
     def __str__(self):
         # Autodetect reduction type
         redtype = detect_reduction_type(self.wcr)
         if redtype == dtypes.ReductionType.Custom:
             wcrstr = unparse(ast.parse(self.wcr).body[0].value.body)
```

### Comparing `dace-0.9.0/dace/graph/nxutil.py` & `dace-0.9.5/dace/graph/nxutil.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 def node_path_graph(*args):
     """ Generates a path graph passing through the input nodes.
 
         The function generates a graph using as nodes the input arguments.
         Subsequently, it creates a path passing through all the nodes, in
         the same order as they were given in the function input.
 
-        @param *args: Variable number of nodes or a list of nodes.
-        @return: A directed graph based on the input arguments.
+        :param *args: Variable number of nodes or a list of nodes.
+        :return: A directed graph based on the input arguments.
         @rtype: gr.OrderedDiGraph
     """
 
     # 1. Create new networkx directed graph.
     path = gr.OrderedDiGraph()
     # 2. Place input nodes in a list.
     if len(args) == 1 and isinstance(args[0], list):
@@ -106,19 +106,19 @@
     """ Produce nodes in a depth-first topological ordering.
 
     The function produces nodes in a depth-first topological ordering
     (DFS to make sure maps are visited properly), with the condition
     that each node visited had all its predecessors visited. Applies
     for DAGs only.
 
-    @param G: An input DiGraph (assumed acyclic).
-    @param sources: (optional) node or list of nodes that
+    :param G: An input DiGraph (assumed acyclic).
+    :param sources: (optional) node or list of nodes that
                     specify starting point(s) for depth-first search and return
                     edges in the component reachable from source.
-    @return: A generator of edges in the lastvisit depth-first-search.
+    :return: A generator of edges in the lastvisit depth-first-search.
 
     @note: Based on http://www.ics.uci.edu/~eppstein/PADS/DFS.py
     by D. Eppstein, July 2004.
 
     @note: If a source is not specified then a source is chosen arbitrarily and
     repeatedly until all components in the graph are searched.
 
@@ -214,19 +214,19 @@
         except StopIteration:
             queue.popleft()
 
 
 def traverse_sdfg_scope(G, source, yield_edges=True):
     """ Traverse an SDFG scope (nodes dominated by a ScopeEntry and 
         post-dominated by a ScopeExit). 
-        @param G: Input graph (assumed SDFGState).
-        @param source: Source node.
-        @param yield_edges: If True, returned generator yields edges
+        :param G: Input graph (assumed SDFGState).
+        :param source: Source node.
+        :param yield_edges: If True, returned generator yields edges
                             as well as nodes.
-        @return: A generator that iterates over the scope nodes (or edges).
+        :return: A generator that iterates over the scope nodes (or edges).
     """
 
     if not isinstance(source, nodes.EntryNode):
         raise SyntaxError('Source should be an entry node')
 
     visited = set()
     visited.add(source)
@@ -422,18 +422,18 @@
 
         The function finds all edges in the graph that have node A as their
         destination. It then creates a new edge for each one found,
         using the same source nodes and data, but node B as the destination.
         Afterwards, it deletes the edges found and inserts the new ones into 
         the graph.
 
-        @param graph: The graph upon which the edge transformations will be 
+        :param graph: The graph upon which the edge transformations will be
                       applied.  
-        @param node_a: The original destination of the edges.  
-        @param node_b: The new destination of the edges to be transformed. 
+        :param node_a: The original destination of the edges.
+        :param node_b: The new destination of the edges to be transformed.
     """
 
     # Create new incoming edges to node B, by copying the incoming edges to
     # node A and setting their destination to node B.
     edges = list(graph.in_edges(node_a))
     for e in edges:
         # Delete the incoming edges to node A from the graph.
@@ -466,18 +466,18 @@
 
         The function finds all edges in the graph that have node A as their 
         source. It then creates a new edge for each one found, using the same 
         destination nodes and data, but node B as the source. Afterwards, it 
         deletes the edges
         found and inserts the new ones into the graph.
 
-        @param graph: The graph upon which the edge transformations will be 
+        :param graph: The graph upon which the edge transformations will be
                       applied.
-        @param node_a: The original source of the edges to be transformed.
-        @param node_b: The new source of the edges to be transformed.
+        :param node_a: The original source of the edges to be transformed.
+        :param node_b: The new source of the edges to be transformed.
     """
 
     # Create new outgoing edges from node B, by copying the outgoing edges from
     # node A and setting their source to node B.
     edges = list(graph.out_edges(node_a))
     for e in edges:
         # Delete the outgoing edges from node A from the graph.
@@ -502,27 +502,27 @@
 
 def find_source_nodes(graph):
     """ Finds the source nodes of a graph.
 
         The function finds the source nodes of a graph, i.e. the nodes with 
         zero in-degree.
 
-        @param graph: The graph whose source nodes are being searched for.
-        @return: A list of the source nodes found.
+        :param graph: The graph whose source nodes are being searched for.
+        :return: A list of the source nodes found.
     """
     return [n for n in graph.nodes() if graph.in_degree(n) == 0]
 
 
 def find_sink_nodes(graph):
     """ Finds the sink nodes of a graph.
 
         The function finds the sink nodes of a graph, i.e. the nodes with zero out-degree.
 
-        @param graph: The graph whose sink nodes are being searched for.
-        @return: A list of the sink nodes found.
+        :param graph: The graph whose sink nodes are being searched for.
+        :return: A list of the sink nodes found.
     """
     return [n for n in graph.nodes() if graph.out_degree(n) == 0]
 
 
 def replace_subgraph(graph: dace.graph.graph.OrderedDiGraph,
                      old: dace.graph.graph.OrderedDiGraph,
                      new: dace.graph.graph.OrderedDiGraph):
@@ -533,19 +533,19 @@
         'new' subgraph. Both the 'old' and the 'new' subgraphs must have 
         unique source and sink nodes. Graph edges incoming to the source of 
         the 'old' subgraph have their destination changed to the source of 
         the 'new subgraph. Likewise, graph edges outgoing from the sink of 
         the 'old subgraph have their source changed to the sink of the 'new' 
         subgraph.
 
-        @param graph: The graph upon which the replacement will be applied.
-        @param old: The subgraph to be replaced.
-        @param new: The replacement subgraph.
+        :param graph: The graph upon which the replacement will be applied.
+        :param old: The subgraph to be replaced.
+        :param new: The replacement subgraph.
 
-        @return: True if the replacement succeeded, otherwise False.
+        :return: True if the replacement succeeded, otherwise False.
     """
 
     # 1. Find the source node of 'old' subgraph.
     # 1.1. Retrieve the source nodes of the 'old' subgraph.
     old_source_nodes = find_source_nodes(old)
     # 1.2. Verify the existence of a unique source in the 'old' subgraph.
     if len(old_source_nodes) != 1:
@@ -611,50 +611,49 @@
     operation is valid. """
 
     outer_map = outer_map_entry.map
     inner_map = inner_map_entry.map
 
     # Create merged map by inheriting attributes from outer map and using
     # the merge functions for parameters and ranges.
-    merged_map = dace.graph.nodes.Map(
-        label='_merged_' + outer_map.label + '_' + inner_map.label,
-        params=param_merge(outer_map.params, inner_map.params),
-        ndrange=range_merge(outer_map.range, inner_map.range),
-        schedule=outer_map.schedule,
-        unroll=outer_map.unroll,
-        is_async=outer_map.is_async,
-        flatten=outer_map.flatten,
-        debuginfo=outer_map.debuginfo)
+    merged_map = copy.deepcopy(outer_map)
+    merged_map.label = 'merged_' + outer_map.label
+    merged_map.params = param_merge(outer_map.params, inner_map.params)
+    merged_map.range = range_merge(outer_map.range, inner_map.range)
 
     merged_entry = dace.graph.nodes.MapEntry(merged_map)
     merged_entry.in_connectors = outer_map_entry.in_connectors
     merged_entry.out_connectors = outer_map_entry.out_connectors
 
     merged_exit = dace.graph.nodes.MapExit(merged_map)
     merged_exit.in_connectors = outer_map_exit.in_connectors
     merged_exit.out_connectors = outer_map_exit.out_connectors
 
     graph.add_nodes_from([merged_entry, merged_exit])
 
     # Redirect inner in edges.
     inner_in_edges = graph.out_edges(inner_map_entry)
     for edge in graph.edges_between(outer_map_entry, inner_map_entry):
-        in_conn_num = edge.dst_conn[3:]
-        out_conn = 'OUT_' + in_conn_num
+        if edge.dst_conn is None:  # Empty memlets
+            out_conn = None
+        else:
+            out_conn = 'OUT_' + edge.dst_conn[3:]
         inner_edge = [e for e in inner_in_edges if e.src_conn == out_conn][0]
         graph.remove_edge(edge)
         graph.remove_edge(inner_edge)
         graph.add_edge(merged_entry, edge.src_conn, inner_edge.dst,
                        inner_edge.dst_conn, inner_edge.data)
 
     # Redirect inner out edges.
     inner_out_edges = graph.in_edges(inner_map_exit)
     for edge in graph.edges_between(inner_map_exit, outer_map_exit):
-        out_conn_num = edge.src_conn[4:]
-        in_conn = 'IN_' + out_conn_num
+        if edge.src_conn is None:  # Empty memlets
+            in_conn = None
+        else:
+            in_conn = 'IN_' + edge.src_conn[4:]
         inner_edge = [e for e in inner_out_edges if e.dst_conn == in_conn][0]
         graph.remove_edge(edge)
         graph.remove_edge(inner_edge)
         graph.add_edge(inner_edge.src, inner_edge.src_conn, merged_exit,
                        edge.dst_conn, inner_edge.data)
 
     # Redirect outer edges.
```

### Comparing `dace-0.9.0/dace/jupyter.py` & `dace-0.9.5/dace/jupyter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 """ Jupyter Notebook support for DaCe. """
 
 import os
 
 
 # From https://stackoverflow.com/a/39662359/6489142
-def _isnotebook():
+def isnotebook():
     try:
         shell = get_ipython().__class__.__name__
         if shell == 'ZMQInteractiveShell':
             return True  # Jupyter notebook or qtconsole
         elif shell == 'TerminalInteractiveShell':
             return False  # Terminal running IPython
         else:
             return False  # Other type (?)
     except NameError:
         return False  # Probably standard Python interpreter
 
 
-# Code that runs on "import dace"
-if _isnotebook():
-    from IPython.display import display, HTML
-
+def preamble():
     # Emit javascript headers for SDFG renderer
     sdfv_deps = [
         'renderer_dir/dagre.js', 'renderer_dir/global_vars.js',
         'renderer_elements.js', 'sdfg_utils.js', 'renderer.js'
     ]
     result = ''
 
     # Load dependencies
     root_path = os.path.join(
-        os.path.dirname(os.path.abspath(__file__)), '..', 'diode', 'client')
+        os.path.dirname(os.path.abspath(__file__)), '..', 'diode', 'webclient')
     for dep in sdfv_deps:
         file = os.path.join(root_path, dep)
         with open(file, 'r') as fp:
             result += '<script>%s</script>\n' % fp.read()
 
     # Rely on internet connection for Material icons
     result += '<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">'
 
     # Run this code once
-    display(HTML(result))
+    return result
+
+
+# Code that runs on "import dace"
+if isnotebook():
+    from IPython.display import display, HTML
+    display(HTML(preamble()))
```

### Comparing `dace-0.9.0/dace/memlet.py` & `dace-0.9.5/dace/memlet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import ast
 from functools import reduce
 import operator
-import copy as cp
+from typing import List
 
-import json
 import dace
-from dace import data as dt, subsets, symbolic, dtypes
+import dace.serialize
+from dace import subsets, dtypes
 from dace.frontend.operations import detect_reduction_type
 from dace.frontend.python.astutils import unparse
-from dace.properties import (
-    Property, make_properties, DataProperty, ShapeProperty, SubsetProperty,
-    SymbolicProperty, TypeClassProperty, DebugInfoProperty, LambdaProperty)
+from dace.properties import (Property, make_properties, DataProperty,
+                             SubsetProperty, SymbolicProperty,
+                             DebugInfoProperty, LambdaProperty)
 
 
 @make_properties
 class Memlet(object):
     """ Data movement object. Represents the data, the subset moved, and the
         manner it is reindexed (`other_subset`) into the destination.
         If there are multiple conflicting writes, this object also specifies
         how they are resolved with a lambda function.
     """
 
     # Properties
     veclen = Property(dtype=int, desc="Vector length")
-    num_accesses = SymbolicProperty()
-    subset = SubsetProperty()
+    num_accesses = SymbolicProperty(default=0)
+    subset = SubsetProperty(default=subsets.Range([]))
     other_subset = SubsetProperty(allow_none=True)
     data = DataProperty()
     debuginfo = DebugInfoProperty()
     wcr = LambdaProperty(allow_none=True)
     wcr_identity = Property(dtype=object, default=None, allow_none=True)
     wcr_conflict = Property(dtype=bool, default=True)
     allow_oob = Property(
@@ -41,48 +41,48 @@
                  vector_length,
                  wcr=None,
                  wcr_identity=None,
                  other_subset=None,
                  debuginfo=None,
                  wcr_conflict=True):
         """ Constructs a Memlet.
-            @param data: The data object or name to access. B{Note:} this
+            :param data: The data object or name to access. B{Note:} this
                          parameter will soon be deprecated.
             @type data: Either a string of the data descriptor name or an
                         AccessNode.
-            @param num_accesses: The number of times that the moved data
+            :param num_accesses: The number of times that the moved data
                                  will be subsequently accessed. If
                                  `dace.dtypes.DYNAMIC` (-1),
                                  designates that the number of accesses is
                                  unknown at compile time.
-            @param subset: The subset of `data` that is going to be accessed.
-            @param vector_length: The length of a single unit of access to
-                                  the data (used for vectorization 
+            :param subset: The subset of `data` that is going to be accessed.
+            :param vector_length: The length of a single unit of access to
+                                  the data (used for vectorization
                                   optimizations).
-            @param wcr: A lambda function specifying how write-conflicts
+            :param wcr: A lambda function specifying how write-conflicts
                         are resolved. The syntax of the lambda function receives two elements: `current` value and `new` value,
                         and returns the value after resolution. For example,
                         summation is `lambda cur, new: cur + new`.
-            @param wcr_identity: Identity value used for the first write 
+            :param wcr_identity: Identity value used for the first write
                                  conflict. B{Note:} this parameter will soon
                                  be deprecated.
-            @param other_subset: The reindexing of `subset` on the other 
+            :param other_subset: The reindexing of `subset` on the other
                                  connected data.
-            @param debuginfo: Source-code information (e.g., line, file) 
+            :param debuginfo: Source-code information (e.g., line, file)
                               used for debugging.
-            @param wcr_conflict: If False, forces non-locked conflict 
+            :param wcr_conflict: If False, forces non-locked conflict
                                  resolution when generating code. The default
-                                 is to let the code generator infer this 
+                                 is to let the code generator infer this
                                  information from the SDFG.
         """
 
         # Properties
-        self.num_accesses = num_accesses  # type: sympy math
+        self.num_accesses = num_accesses  # type: sympy.expr.Expr
         self.subset = subset  # type: subsets.Subset
-        self.veclen = vector_length  # type: int (in elements, default 1)
+        self.veclen = vector_length  # type: int
         if hasattr(data, 'data'):
             data = data.data
         self.data = data  # type: str
 
         # Annotates memlet with _how_ writing is performed in case of conflict
         self.wcr = wcr
         self.wcr_identity = wcr_identity
@@ -90,80 +90,75 @@
 
         # The subset of the other endpoint we are copying from/to (note:
         # carries the dimensionality of the other endpoint too!)
         self.other_subset = other_subset
 
         self.debuginfo = debuginfo
 
-    def toJSON(self, parent_graph=None):
-        try:
-            attrs = json.loads(Property.all_properties_to_json(self))
-        except Exception as e:
-            print("Got exception: " + str(e))
-            import traceback
-            traceback.print_exc()
+    def to_json(self, parent_graph=None):
+        attrs = dace.serialize.all_properties_to_json(self)
 
         retdict = {"type": "Memlet", "label": str(self), "attributes": attrs}
 
-        return json.dumps(retdict)
+        return retdict
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
+    def from_json(json_obj, context=None):
         if json_obj['type'] != "Memlet":
             raise TypeError("Invalid data type")
 
         # Create dummy object
         ret = Memlet("", dace.dtypes.DYNAMIC, None, 1)
-        Property.set_properties_from_json(ret, json_obj, context=context)
+        dace.serialize.set_properties_from_json(ret, json_obj, context=context)
 
         return ret
 
     @staticmethod
     def simple(data,
                subset_str,
                veclen=1,
                wcr_str=None,
                wcr_identity=None,
                other_subset_str=None,
                wcr_conflict=True,
                num_accesses=None,
                debuginfo=None):
         """ Constructs a Memlet from string-based expressions.
-            @param data: The data object or name to access. B{Note:} this
+            :param data: The data object or name to access. B{Note:} this
                          parameter will soon be deprecated.
             @type data: Either a string of the data descriptor name or an
                         AccessNode.
-            @param subset_str: The subset of `data` that is going to 
+            :param subset_str: The subset of `data` that is going to
                                be accessed in string format. Example: '0:N'.
-            @param veclen: The length of a single unit of access to
+            :param veclen: The length of a single unit of access to
                            the data (used for vectorization optimizations).
-            @param wcr_str: A lambda function (as a string) specifying 
-                            how write-conflicts are resolved. The syntax 
+            :param wcr_str: A lambda function (as a string) specifying
+                            how write-conflicts are resolved. The syntax
                             of the lambda function receives two elements:
                             `current` value and `new` value,
-                            and returns the value after resolution. For 
-                            example, summation is 
+                            and returns the value after resolution. For
+                            example, summation is
                             `'lambda cur, new: cur + new'`.
-            @param wcr_identity: Identity value used for the first write 
+            :param wcr_identity: Identity value used for the first write
                                  conflict. B{Note:} this parameter will soon
                                  be deprecated.
-            @param other_subset_str: The reindexing of `subset` on the other 
+            :param other_subset_str: The reindexing of `subset` on the other
                                      connected data (as a string).
-            @param wcr_conflict: If False, forces non-locked conflict 
+            :param wcr_conflict: If False, forces non-locked conflict
                                  resolution when generating code. The default
-                                 is to let the code generator infer this 
+                                 is to let the code generator infer this
                                  information from the SDFG.
-            @param num_accesses: The number of times that the moved data
+            :param num_accesses: The number of times that the moved data
                                  will be subsequently accessed. If
                                  `dace.dtypes.DYNAMIC` (-1),
                                  designates that the number of accesses is
                                  unknown at compile time.
-            @param debuginfo: Source-code information (e.g., line, file) 
+            :param debuginfo: Source-code information (e.g., line, file)
                               used for debugging.
-                                 
+
         """
         subset = SubsetProperty.from_string(subset_str)
         if num_accesses is not None:
             na = num_accesses
         else:
             na = subset.num_elements()
 
@@ -191,16 +186,16 @@
             other_subset=other_subset,
             wcr_conflict=wcr_conflict,
             debuginfo=debuginfo)
 
     @staticmethod
     def from_array(dataname, datadesc):
         """ Constructs a Memlet that transfers an entire array's contents.
-            @param dataname: The name of the data descriptor in the SDFG.
-            @param datadesc: The data descriptor object.
+            :param dataname: The name of the data descriptor in the SDFG.
+            :param datadesc: The data descriptor object.
             @type datadesc: Data.
         """
         range = subsets.Range.from_array(datadesc)
         return Memlet(dataname, range.num_elements(), range, 1)
 
     def __hash__(self):
         return hash((self.data, self.num_accesses, self.subset, self.veclen,
@@ -227,19 +222,19 @@
         return self.subset.bounding_box_size()
 
     def validate(self, sdfg, state):
         if self.data is not None and self.data not in sdfg.arrays:
             raise KeyError('Array "%s" not found in SDFG' % self.data)
 
     def __label__(self, sdfg, state):
-        """ Returns a string representation of the memlet for display in a 
+        """ Returns a string representation of the memlet for display in a
             graph.
 
-            @param sdfg: The SDFG in which the memlet resides.
-            @param state: An SDFGState object in which the memlet resides.
+            :param sdfg: The SDFG in which the memlet resides.
+            :param state: An SDFGState object in which the memlet resides.
         """
         if self.data is None:
             return self._label(None)
         return self._label(sdfg.arrays[self.data].shape)
 
     def __str__(self):
         return self._label(None)
@@ -294,7 +289,43 @@
 
 class EmptyMemlet(Memlet):
     """ A memlet without data. Primarily used for connecting nodes to scopes
         without transferring data to them. """
 
     def __init__(self):
         super(EmptyMemlet, self).__init__(None, 0, None, 1)
+
+
+class MemletTree(object):
+    """ A tree of memlet edges.
+
+        Since memlets can form paths through scope nodes, and since these
+        paths can split in "OUT_*" connectors, a memlet edge can be extended
+        to a memlet tree. The tree is always rooted at the outermost-scope node,
+        which can mean that it forms a tree of directed edges going forward
+        (in the case where memlets go through scope-entry nodes) or backward
+        (through scope-exit nodes).
+
+        Memlet trees can be used to obtain all edges pertaining to a single
+        memlet using the `memlet_tree` function in SDFGState. This collects
+        all siblings of the same edge and their children, for instance if
+        multiple inputs from the same access node are used.
+    """
+
+    def __init__(
+            self, edge, parent=None, children=None
+    ):  # type: (dace.graph.graph.MultiConnectorEdge, MemletTree, List[MemletTree]) -> None
+        self.edge = edge
+        self.parent = parent
+        self.children = children or []
+
+    def __iter__(self):
+        if self.parent is not None:
+            yield from self.parent
+            return
+
+        def traverse(node):
+            yield node.edge
+            for child in node.children:
+                yield from traverse(child)
+
+        yield from traverse(self)
```

### Comparing `dace-0.9.0/dace/properties.py` & `dace-0.9.5/dace/properties.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import ast
 import astunparse
+import enum
 from collections import OrderedDict
 import copy
 from dace.frontend.python.astutils import unparse
 import itertools
+import json
 import pydoc
 import re
 import sympy as sp
 import numpy as np
 import dace.subsets as sbs
 import dace
+import dace.serialize
 from dace.symbolic import pystr_to_symbolic
 from dace.dtypes import DebugInfo
-import json
 
 ###############################################################################
 # External interface to guarantee correct usage
 ###############################################################################
 
 
 def set_property_from_string(prop, obj, string, sdfg=None, from_json=False):
@@ -56,17 +58,14 @@
 
 class PropertyError(Exception):
     """Exception type for errors related to internal functionality of
     these properties."""
     pass
 
 
-json_store_metadata = True
-
-
 class Property:
     """ Class implementing properties of DaCe objects that conform to strong
     typing, and allow conversion to and from strings to be edited. """
 
     def __init__(
             self,
             getter=None,
@@ -74,124 +73,115 @@
             dtype=None,
             default=None,
             from_string=None,
             to_string=None,
             from_json=None,
             to_json=None,
             meta_to_json=None,
-            enum=None,  # Values must be present in this enum
+            choices=None,  # Values must be present in this enum
             unmapped=False,  # Don't enforce 1:1 mapping with a member variable
             allow_none=False,
             indirected=False,  # This property belongs to a different class
             category='General',
             desc=""):
 
         self._getter = getter
         self._setter = setter
         self._dtype = dtype
         self._default = default
+
+        if allow_none is False and default is None:
+            try:
+                self._default = dtype()
+            except TypeError:
+                if hasattr(self, 'dtype'):
+                    try:
+                        self._default = self.dtype()
+                    except TypeError:
+                        raise TypeError(
+                            'Default not properly defined for property')
+                else:
+                    raise TypeError(
+                        'Default not properly defined for property')
+
+        if choices is not None:
+            for choice in choices:
+                if dtype is None:
+                    dtype = type(choice)
+                if not isinstance(choice, dtype):
+                    raise TypeError("All choices must be an instance of dtype")
+
         if from_string is not None:
             self._from_string = from_string
-        elif enum is not None:
-            self._from_string = lambda s: enum[s]
+        elif choices is not None:
+            self._from_string = lambda s: choices[s]
         else:
             self._from_string = self.dtype
+
         if to_string is not None:
             self._to_string = to_string
-        elif enum is not None:
-            self._to_string = lambda val: val._name_
+        elif choices is not None:
+            self._to_string = lambda val: val.__name__
         else:
             self._to_string = str
+
         if from_json is None:
-            import json
 
-            def tmp(x, sdfg=None):
-                if self.dtype == bool:
-                    return json.loads(x)
-                elif self.dtype is None:
-                    # Return without type cast.
-                    return self.from_string(json.loads(x))
-                if self.dtype == dict or self.dtype == object:
-                    # Treat special types (e.g. dict)
-                    return json.loads(x, object_hook=Property.json_loader)
-
-                pre = json.loads(x, object_hook=Property.json_loader)
-                if pre is None:
-                    return None
-                return self.from_string(pre)
+            def f(obj, *args, **kwargs):
+                if isinstance(obj, str) and self._from_string is not None:
+                    # The serializer does not know about this property, so if
+                    # we can convert using our to_string method, do that here
+                    return self._from_string(obj)
+                # Otherwise ship off to the serializer, telling it which type
+                # it's dealing with as a sanity check
+                return dace.serialize.from_json(
+                    obj, *args, known_type=dtype, **kwargs)
 
-            self._from_json = tmp
+            self._from_json = f
         else:
             self._from_json = from_json
-        if to_json is None:
-            import json
-
-            # We have to add an indirection
-            # (if just returning the output of to_string, one could not always parse it back)
-            def tmp(x):
-                if x is not None:
-                    if self.dtype == bool:
-                        return json.dumps(x)
-                    elif self.dtype is None:
-                        # Return without type cast.
-                        return json.dumps(None
-                                          if x is None else self.to_string(x))
-                    elif self.dtype == dict:
-                        # Treat special types (e.g. dict)
-                        typecast = dict(x)
-                        return json.dumps(
-                            None if x is None else typecast,
-                            default=Property.json_dumper)
-                    elif self.dtype == tuple:
-                        typecast = tuple(x)
-                        return json.dumps(
-                            None if x is None else typecast,
-                            default=Property.json_dumper)
-                    elif self.dtype == list:
-                        typecast = list(x)
-                        return json.dumps(
-                            None if x is None else typecast,
-                            default=Property.json_dumper)
-                    elif self.dtype == object:
-                        # Not treating this - go away.
-                        return json.dumps(x)
 
-                return json.dumps(None if x is None else self.to_string(x))
-
-            self._to_json = tmp
+        if to_json is None:
+            self._to_json = dace.serialize.to_json
         else:
             self._to_json = to_json
+
         if meta_to_json is None:
-            import json
 
             def tmp_func(self):
                 typestr = self.typestring()
 
                 _default = self.to_json(self.default)
 
                 mdict = {
-                    "type": typestr,
+                    "metatype": typestr,
                     "desc": self.desc,
                     "category": self.category,
-                    "default": json.loads(_default),
+                    "default": _default,
                 }
                 if self.indirected:
                     mdict['indirected'] = True
-                return json.dumps(mdict)
+                return mdict
 
             self._meta_to_json = tmp_func
         else:
             self._meta_to_json = meta_to_json
 
-        self._enum = enum
+        self._choices = choices
         self._unmapped = unmapped
         self._allow_none = allow_none
         self._indirected = indirected
         self._desc = desc
         self._category = category
+        if desc is not None and len(desc) > 0:
+            self.__doc__ = desc
+        elif self.dtype is not None:
+            self.__doc__ = "Object property of type %s" % self.dtype.__name__
+        else:
+            self.__doc__ = "Object property of type %s" % type(self).__name__
 
     def __get__(self, obj, objtype=None):
         if obj is None:
             # Called on the class rather than an instance, so return the
             # property object itself
             return self
         # If a custom getter is specified, use it
@@ -229,18 +219,19 @@
                     "from_string method of the property.".format(
                         self.attr_name, self.dtype))
             raise TypeError(
                 "Invalid type \"{}\" for property {}: expected {}".format(
                     type(val).__name__, self.attr_name, self.dtype.__name__))
         # If the value has not yet been set, we cannot pass it to the enum
         # function. Fail silently if this happens
-        if self.enum is not None and isinstance(self.enum, (list, tuple, set)):
-            if val not in self.enum:
-                raise ValueError("Value {} not present in enum: {}".format(
-                    val, self.enum))
+        if self.choices is not None and isinstance(self.choices,
+                                                   (list, tuple, set)):
+            if val not in self.choices:
+                raise ValueError("Value {} not present in choices: {}".format(
+                    val, self.choices))
         setattr(obj, "_" + self.attr_name, val)
 
     # Python Properties of this Property class
 
     @property
     def getter(self):
         return self._getter
@@ -264,15 +255,15 @@
     def typestring(self):
         typestr = ""
         try:
             typestr = self.dtype.__name__
         except:
             # Try again, it might be an enum
             try:
-                typestr = self.enum.__name__
+                typestr = self.choices.__name__
             except:
                 try:
                     typestr = type(self).__name__
                 except:
                     typestr = 'None'
         return typestr
 
@@ -307,16 +298,16 @@
     @property
     def meta_to_json(self):
         """ Returns a function to export meta information (type, description, default value).
         """
         return self._meta_to_json
 
     @property
-    def enum(self):
-        return self._enum
+    def choices(self):
+        return self._choices
 
     @property
     def unmapped(self):
         return self._unmapped
 
     @property
     def indirected(self):
@@ -332,144 +323,23 @@
 
     @staticmethod
     def add_none_pair(dict_in):
         dict_in[None] = None
         return dict_in
 
     @staticmethod
-    def all_properties_to_json(object_with_properties, options=None):
-        options = options or dict(no_meta=not json_store_metadata)
-        retdict = {}
-        for x, v in object_with_properties.properties():
-            # The following loads is intended: This is a nested object.
-            # If loads() is not used, every element would be a string, and loading the resulting string is hard.
-            t = x.to_json(v)
-            retdict[x.attr_name] = json.loads(t)
-
-            # Add the meta elements decoupled from key/value to facilitate value usage
-            # (The meta is only used when rendering the values)
-            if not options['no_meta']:
-                retdict['_meta_' + x.attr_name] = json.loads(x.meta_to_json(x))
-
-        # Stringify using the default interface
-        return json.dumps(retdict)
-
-    @staticmethod
-    def set_properties_from_json(object_with_properties,
-                                 json_obj,
-                                 context=None):
-        try:
-            attrs = json_obj['attributes']
-        except:
-            attrs = json_obj
-
-        # Apply properties
-        ps = dict(object_with_properties.__properties__)
-        for tmp, _v in ps.items():
-            pname = tmp
-            try:
-                val = attrs[pname]
-            except:
-                continue
-
-            # Some properties only work when converted back from string.
-            try:
-                stringified = json.dumps(val, default=Property.json_dumper)
-                newval = _v.from_json(stringified, context)
-                setattr(object_with_properties, tmp, newval)
-            except Exception as e:
-                import traceback
-                traceback.print_exc()
-                #TODO: Maybe log this...
-                raise e
-
-    @staticmethod
     def get_property_element(object_with_properties, name):
         # Get the property object (as it may have more options than available by exposing the value)
         ps = dict(object_with_properties.__properties__)
         for tmp, _v in ps.items():
             pname = tmp
             if pname == name:
                 return _v
         return None
 
-    @staticmethod
-    def json_dumper(obj):
-        if hasattr(obj, 'toJSON'):
-            # Try the toJSON-methods by default
-            tmp = json.loads(obj.toJSON())
-            return tmp
-        elif isinstance(obj, np.ndarray):
-            # Special case for external structures (numpy arrays)
-            return NumpyLoader.toJSON_object(obj)
-        else:
-            # If not available, go for the default str() representation
-            return str(obj)
-
-    @staticmethod
-    def known_types():
-        import dace.data
-        return {
-            "Array": dace.data.Array,
-            "Scalar": dace.data.Scalar,
-            "Stream": dace.data.Stream,
-            "AccessNode": dace.graph.nodes.AccessNode,
-            "MapEntry": dace.graph.nodes.MapEntry,
-            "MapExit": dace.graph.nodes.MapExit,
-            "Reduce": dace.graph.nodes.Reduce,
-            "ConsumeEntry": dace.graph.nodes.ConsumeEntry,
-            "ConsumeExit": dace.graph.nodes.ConsumeExit,
-            "Tasklet": dace.graph.nodes.Tasklet,
-            "EmptyTasklet": dace.graph.nodes.EmptyTasklet,
-            "NestedSDFG": dace.graph.nodes.NestedSDFG,
-            "Memlet": dace.memlet.Memlet,
-            "MultiConnectorEdge": dace.graph.graph.MultiConnectorEdge,
-            "InterstateEdge": dace.graph.edges.InterstateEdge,
-            "Edge": dace.graph.graph.Edge,
-            "SDFG": dace.sdfg.SDFG,
-            "SDFGState": dace.sdfg.SDFGState,
-
-            # Data types (Note: Types must be qualified, as properties also have type subelements)
-            "subsets.Range": dace.subsets.Range,
-            "subsets.Indices": dace.subsets.Indices,
-            "pointer": dace.dtypes.pointer,
-            "callback": dace.dtypes.callback,
-            "struct": dace.dtypes.struct,
-            "ndarray": NumpyLoader
-        }
-
-    @staticmethod
-    def json_loader(obj, context=None):
-        if not isinstance(obj, dict):
-            return obj
-        attr_type = None
-        if "attributes" in obj:
-            tmp = obj['attributes']
-            if isinstance(tmp, dict):
-                if "type" in tmp:
-                    attr_type = tmp['type']
-            else:
-                # The object was consumed previously
-                try:
-                    obj['type']
-                except KeyError:
-                    return tmp
-                # If a type is available, the parent element must also be parsed accordingly
-
-        try:
-            t = obj['type']
-        except KeyError:
-            t = attr_type
-
-        if t in Property.known_types():
-            return (Property.known_types()[t]).fromJSON_object(
-                obj, context=context)
-
-        return obj
-
 
 ###############################################################################
 # Decorator for objects with properties
 ###############################################################################
 
 
 def _property_generator(instance):
@@ -477,15 +347,15 @@
         if hasattr(instance, "_" + name):
             yield prop, getattr(instance, "_" + name)
         else:
             yield prop, getattr(instance, name)
 
 
 def make_properties(cls):
-    """ A decorator for objects that adds support and checks for strongly-typed 
+    """ A decorator for objects that adds support and checks for strongly-typed
         properties (which use the Property class).
     """
 
     # Extract all Property members of the class
     properties = OrderedDict([(name, prop)
                               for name, prop in cls.__dict__.items()
                               if isinstance(prop, Property)])
@@ -518,16 +388,17 @@
             # Only assign our own properties, so we don't overwrite what's been
             # set by the base class
             if hasattr(obj, name):
                 raise PropertyError(
                     "Property {} already assigned in {}".format(
                         name,
                         type(obj).__name__))
-            if not prop.indirected and prop.default is not None:
-                setattr(obj, name, prop.default)
+            if not prop.indirected:
+                if prop.allow_none or prop.default is not None:
+                    setattr(obj, name, prop.default)
         # Now call vanilla __init__, which can initialize members
         init(obj, *args, **kwargs)
         # Assert that all properties have been set
         for name, prop in properties.items():
             try:
                 getattr(obj, name)
             except AttributeError:
@@ -543,14 +414,17 @@
                     "{} : Variable {} is neither a Property nor "
                     "an internal variable (prefixed with \"_\")".format(
                         str(type(obj)), name))
 
     # Replace the __init__ method
     cls.__init__ = initialize_properties
 
+    # Register our type with the serialization framework
+    cls = dace.serialize.serializable(cls)
+
     return cls
 
 
 def indirect_property(cls, f, prop, override):
 
     # Make a copy of the original property, but override its getter and setter
     prop_name = prop.attr_name
@@ -594,44 +468,42 @@
     """ Property type for ordered dicts
     """
 
     def to_json(self, d):
 
         # The ordered dict is more of a list than a dict.
         retlist = [{k: v} for k, v in d.items()]
-        return json.dumps(retlist, default=Property.json_dumper)
+        return retlist
 
     @staticmethod
-    def from_json(s, sdfg=None):
+    def from_json(obj, sdfg=None):
 
-        obj = json.loads(s, object_hook=Property.json_loader)
         # This is expected to be a list (a JSON dict does not guarantee an order,
         # although it would often be lexicographically ordered by key name)
 
-        import collections
-        ret = collections.OrderedDict()
+        ret = OrderedDict()
         for x in obj:
             ret[list(x.keys())[0]] = list(x.values())[0]
 
         return ret
 
 
 class ListProperty(Property):
     """ Property type for lists.
     """
 
     def __init__(self, element_type, *args, **kwargs):
         """
         Create a List property with a uniform element type.
-        @param element_type: The type of each element in the list, or a function
+        :param element_type: The type of each element in the list, or a function
                              that converts an element to the wanted type (e.g.,
                              `dace.symbolic.pystr_to_symbolic` for symbolic
                              expressions)
-        @param args: Other arguments (inherited from Property).
-        @param kwargs: Other keyword arguments (inherited from Property).
+        :param args: Other arguments (inherited from Property).
+        :param kwargs: Other keyword arguments (inherited from Property).
         """
 
         kwargs['dtype'] = list
         super().__init__(*args, **kwargs)
         self.element_type = element_type
 
     def __set__(self, obj, val):
@@ -643,53 +515,58 @@
 
     @staticmethod
     def to_string(l):
         return str(l)
 
     def to_json(self, l):
         if l is None:
-            return json.dumps(l)
-
+            return None
+        # If element knows how to convert itself, let it
+        if hasattr(self.element_type, "to_json"):
+            return [elem.to_json() for elem in l]
         # If elements are one of the JSON basic types, use directly
         if self.element_type in (int, float, list, tuple, dict):
-            return json.dumps(l, default=Property.json_dumper)
+            return l
         # Otherwise, convert to strings
-        return json.dumps(list(map(str, l)))
+        return list(map(str, l))
 
     @staticmethod
     def from_string(s):
         return list(s)
 
-    def from_json(self, s, sdfg=None):
-        data = json.loads(s, object_hook=Property.json_loader)
+    def from_json(self, data, sdfg=None):
         if data is None:
             return data
         if not isinstance(data, list):
             raise TypeError('ListProperty expects a list input, got %s' % data)
-
+        # If element knows how to convert itself, let it
+        if hasattr(self.element_type, "from_json"):
+            return [self.element_type.from_json(elem) for elem in data]
         # Type-checks (casts) to the element type
         return list(map(self.element_type, data))
 
 
 ###############################################################################
 # Custom properties
 ###############################################################################
 
 
 class SDFGReferenceProperty(Property):
     def to_json(self, obj):
-        if obj is None: return 'null'
-
-        return json.dumps(obj.toJSON())  # Make a string of a JSON
+        if obj is None:
+            return None
+        return dace.serialize.dumps(obj.to_json())  # Make a string of a JSON
 
-    def from_json(self, s, context=None):
-        if s == "null": return None
+    def from_json(self, obj, context=None):
+        if obj is None:
+            return None
 
         # Parse the string of the JSON back into an SDFG object
-        return dace.SDFG.fromJSON_object(json.loads(json.loads(s)))
+        # Need to use regular json.loads instead of dace.serialize.dumps
+        return dace.SDFG.from_json(json.loads(obj), context)
 
 
 class RangeProperty(Property):
     """ Custom Property type for `dace.graph.subset.Range` members. """
 
     def __set__(self, obj, value):
         if isinstance(value, list):
@@ -704,32 +581,23 @@
     def to_string(obj):
         return sbs.Range.ndslice_to_string(obj)
 
     @staticmethod
     def from_string(s):
         return sbs.Range.from_string(s)
 
-    def to_json(self, obj):
-        if obj is None:
-            return "null"
-        # to_string is not enough - it does not preserve all information
-
-        return obj.toJSON()
-
-    def from_json(self, s, sdfg=None):
-        from dace.subsets import Range
-
-        if s == "null": return None
-
-        return Range.fromJSON(s)
-
 
 class DebugInfoProperty(Property):
     """ Custom Property type for DebugInfo members. """
 
+    def __init__(self, **kwargs):
+        if 'default' not in kwargs:
+            kwargs['default'] = DebugInfo(0, 0, 0, 0)
+        super().__init__(dtype=DebugInfo, **kwargs)
+
     @property
     def dtype(self):
         return DebugInfo
 
     @property
     def allow_none(self):
         return True
@@ -781,33 +649,14 @@
         if m is not None:
             ec = m.group(1)
             info_available = True
         if info_available:
             di = DebugInfo(f, sl, sc, el, ec)
         return di
 
-    def to_json(self, s):
-        if not isinstance(s, DebugInfo):
-            return json.dumps(None)
-        nval = {
-            "filename": s.filename,
-            "start_line": s.start_line,
-            "end_line": s.end_line,
-            "start_col": s.start_column,
-            "end_col": s.end_column
-        }
-        return json.dumps(nval)
-
-    def from_json(self, s, sdfg=None):
-        s = json.loads(s)
-        if s is None: return None
-
-        return DebugInfo(s['start_line'], s['start_col'], s['end_line'],
-                         s['end_col'], s['filename'])
-
 
 class ParamsProperty(Property):
     """ Property for list of parameters, such as parameters for a Map. """
 
     @property
     def dtype(self):
         return list
@@ -820,19 +669,18 @@
     def from_string(s):
         return [
             sp.Symbol(m.group(0))
             for m in re.finditer("[a-zA-Z_][a-zA-Z0-9_]*", s)
         ]
 
     def to_json(self, l):
-        return json.dumps(l, default=Property.json_dumper)
+        return l
 
     def from_json(self, l, sdfg=None):
-        return json.loads(
-            l, object_hook=lambda x: Property.json_loader(l, sdfg))
+        return l
 
 
 class SetProperty(Property):
     """Property for a set of elements of one type, e.g., connectors. """
 
     def __init__(
             self,
@@ -855,15 +703,15 @@
             setter=setter,
             dtype=set,
             default=default,
             from_string=from_string,
             to_string=to_string,
             from_json=from_json,
             to_json=to_json,
-            enum=None,
+            choices=None,
             unmapped=unmapped,
             allow_none=allow_none,
             desc=desc,
             **kwargs)
         self._element_type = element_type
 
     @property
@@ -875,19 +723,18 @@
         return str(l)
 
     @staticmethod
     def from_string(s):
         return [eval(i) for i in re.sub("[\{\}\(\)\[\]]", "", s).split(",")]
 
     def to_json(self, l):
-        return json.dumps(list(sorted(l)))
+        return list(sorted(l))
 
     def from_json(self, l, sdfg=None):
-        import json
-        return set(json.loads(l))
+        return set(l)
 
     def __get__(self, obj, objtype=None):
         # Copy to avoid changes in the set at callee to be reflected in
         # the node directly
         return set(super(SetProperty, self).__get__(obj, objtype))
 
     def __set__(self, obj, val):
@@ -907,35 +754,35 @@
 
 class LambdaProperty(Property):
     """ Custom Property type that accepts a lambda function, with conversions
         to and from strings. """
 
     @property
     def dtype(self):
-        return str
+        return None
 
     @staticmethod
     def from_string(s):
         return ast.parse(s).body[0].value
 
     @staticmethod
     def to_string(obj):
         if obj is None:
             return 'lambda: None'
         if isinstance(obj, str):
             return unparse(ast.parse(obj))
         return unparse(obj)
 
     def to_json(self, obj):
-        if obj is None: return 'null'
-        return json.dumps(LambdaProperty.to_string(obj))
+        if obj is None: return None
+        return LambdaProperty.to_string(obj)
 
     def from_json(self, s, sdfg=None):
-        if s == 'null': return None
-        return LambdaProperty.from_string(json.loads(s))
+        if s == None: return None
+        return LambdaProperty.from_string(s)
 
     def __set__(self, obj, val):
         if val is not None:
             if isinstance(val, str):
                 self.from_string(val)  # Check that from_string doesn't fail
             elif isinstance(val, ast.Lambda):
                 val = self.to_string(val)  # Store as string internally
@@ -951,22 +798,22 @@
     """
 
     def __set__(self, obj, val):
         if val is not None:
             super(SubgraphProperty, self).__set__(obj, val)
 
     def to_json(self, obj):
-        return json.dumps(str(obj))
+        return str(obj)
 
     def from_json(self, s, sdfg=None):
         return None
 
 
 class CodeBlock(list):
-    """ Helper class that represents AST code blocks for `CodeProperty`, 
+    """ Helper class that represents AST code blocks for `CodeProperty`,
         implemented as a list with an extra _as_string property. The object
         also stores the original string, allowing us to preserve comments and
         formatting from user input.
     """
 
     def __init__(self, *args, **kwargs):
         self._as_string = ""
@@ -997,27 +844,26 @@
         except:
             pass
         return tmp
 
     def to_json(self, obj):
         lang = dace.dtypes.Language.Python
         if obj is None:
-            return json.dumps(obj)
+            return None
 
         if isinstance(obj, dict):
             lang = obj['language']
 
         ret = {
             'string_data': CodeProperty.to_string(obj),
             'language': lang.name
         }
-        return json.dumps(ret)
+        return ret
 
-    def from_json(self, l, sdfg=None):
-        tmp = json.loads(l)
+    def from_json(self, tmp, sdfg=None):
 
         if tmp is None:
             return None
 
         try:
             lang = tmp['language']
         except:
@@ -1057,15 +903,15 @@
     def to_string(obj):
         if isinstance(obj, dict):
             # The object has annotated language in this case; ignore the language for this operation
             obj = obj['code_or_block']
         if isinstance(obj, str):
             return obj
         # Grab the originally parsed string if any
-        if obj._as_string is not None and obj._as_string != "":
+        if hasattr(obj, "_as_string") and obj._as_string:
             return obj._as_string
         # It's probably good enough to assume that there is an original string
         # if the language was not Python, so we just throw the string to the
         # astunparser.
         return unparse(obj)
 
     def __get__(self, obj, val):
@@ -1145,22 +991,21 @@
         return None
 
     @property
     def allow_none(self):
         return True
 
     def __set__(self, obj, val):
+        if isinstance(val, str):
+            val = self.from_string(val)
         if (val is not None and not isinstance(val, sbs.Range)
                 and not isinstance(val, sbs.Indices)):
-            try:
-                val = self.from_string(val)
-            except SyntaxError:
-                raise TypeError(
-                    "Subset property must be either Range or Indices: got {}".
-                    format(type(val).__name__))
+            raise TypeError(
+                "Subset property must be either Range or Indices: got {}".
+                format(type(val).__name__))
         super(SubsetProperty, self).__set__(obj, val)
 
     @staticmethod
     def from_string(s):
         if s is None or s == 'None' or len(s) == 0:
             return None
         ranges = sbs.Range.from_string(s)
@@ -1177,25 +1022,22 @@
             return sbs.Indices.__str__(val)
         elif val is None:
             return 'None'
         raise TypeError
 
     def to_json(self, val):
         if val is None:
-            return 'null'
+            return None
         try:
-            return val.toJSON()
-        except:
-            return json.dumps(SubsetProperty.to_string(val))
+            return val.to_json()
+        except AttributeError:
+            return SubsetProperty.to_string(val)
 
     def from_json(self, val, sdfg=None):
-        if val == 'null':
-            return None
-        obj = json.loads(val, object_hook=Property.json_loader)
-        return obj
+        return dace.serialize.from_json(val)
 
 
 class SymbolicProperty(Property):
     """ Custom Property type that accepts integers or Sympy expressions. """
 
     @property
     def dtype(self):
@@ -1221,30 +1063,30 @@
         # Go through sympy once to reorder factors
         return str(pystr_to_symbolic(str(obj), simplify=False))
 
 
 class DataProperty(Property):
     """ Custom Property type that represents a link to a data descriptor.
         Needs the SDFG to be passed as an argument to `from_string` and
-        `enum`. """
+        `choices`. """
 
     def __init__(self, desc='', default=None, **kwargs):
         # Data can be None when no data is flowing, e.g., on a memlet with a
         # map that has no external inputs
         return super().__init__(
             dtype=str, allow_none=True, desc=desc, default=default, **kwargs)
 
     def typestring(self):
         return "DataProperty"
 
     @staticmethod
-    def enum(sdfg=None):
+    def choices(sdfg=None):
         if sdfg is None:
             raise TypeError("Must pass SDFG as second argument to "
-                            "enum method of ArrayProperty")
+                            "choices method of ArrayProperty")
         return list(sdfg.arrays.keys())
 
     @staticmethod
     def from_string(s, sdfg=None):
         if sdfg is None:
             raise TypeError("Must pass SDFG as second argument to "
                             "from_string method of ArrayProperty")
@@ -1254,20 +1096,22 @@
 
     @staticmethod
     def to_string(obj):
         return str(obj)
 
     def to_json(self, obj):
         if obj is None:
-            return "null"
-        return json.dumps(str(obj))
+            return None
+        return str(obj)
 
     def from_json(self, s, context=None):
-        sdfg = context['sdfg']
-        s = json.loads(s)
+        if isinstance(context, dace.SDFG):
+            sdfg = context
+        else:
+            sdfg = context['sdfg']
         if sdfg is None:
             raise TypeError("Must pass SDFG as second argument")
         if s not in sdfg.arrays:
             if s is None:
                 # This is fine
                 #return "null" # Every SDFG has a 'null' element
                 return None
@@ -1315,31 +1159,30 @@
 
     @staticmethod
     def to_string(obj):
         return ", ".join(map(str, obj))
 
     def to_json(self, obj):
         if obj is None:
-            return json.dumps(obj)
-        return json.dumps([*map(str, obj)])
+            return None
+        return list(map(str, obj))
 
-    def from_json(self, s, sdfg=None):
-        d = json.loads(s)
+    def from_json(self, d, sdfg=None):
         if d is None:
             return None
         return tuple([dace.symbolic.pystr_to_symbolic(m) for m in d])
 
     def __set__(self, obj, val):
         if isinstance(val, list):
             val = tuple(val)
         super(ShapeProperty, self).__set__(obj, val)
 
 
 class TypeProperty(Property):
-    """ Custom Property type that finds a type according to the input string. 
+    """ Custom Property type that finds a type according to the input string.
     """
 
     @property
     def dtype(self):
         return type
 
     @staticmethod
@@ -1347,14 +1190,23 @@
         dtype = pydoc.locate(s)
         if dtype is None:
             raise ValueError("No type \"{}\" found.".format(s))
         if not isinstance(dtype, type):
             raise ValueError("Object \"{}\" is not a type.".format(dtype))
         return dtype
 
+    @staticmethod
+    def from_json(obj, context=None):
+        if obj is None:
+            return None
+        if isinstance(obj, str):
+            return TypeProperty.from_string(obj)
+        else:
+            raise TypeError("Cannot parse type from: {}".format(obj))
+
 
 class TypeClassProperty(Property):
     """ Custom property type for memory as defined in dace.types,
         e.g. `dace.float32`. """
 
     @property
     def dtype(self):
@@ -1369,42 +1221,21 @@
 
     @staticmethod
     def to_string(obj):
         return obj.to_string()
 
     def to_json(self, obj):
         if obj is None:
-            return json.dumps(obj)
-        return obj.dtype.toJSON()
-
-    def from_json(self, s, sdfg=None):
-        d = json.loads(s, object_hook=Property.json_loader)
-        if d is None:
             return None
-        if isinstance(d, str):
-            return TypeClassProperty.from_string(d)
-        elif isinstance(d, dace.typeclass):
-            return d
-        else:
-            raise TypeError('Unrecognized typeclass object: %s' % d)
-
-
-class NumpyLoader(object):
-    """ Helper class to load/store numpy arrays from JSON. """
+        return obj.dtype.to_json()
 
     @staticmethod
-    def fromJSON_object(json_obj, context=None):
-        if json_obj['type'] != 'ndarray':
-            raise TypeError('Object is not a numpy ndarray')
-
-        if 'dtype' in json_obj:
-            return np.array(json_obj['data'], dtype=json_obj['dtype'])
-
-        return np.array(json_obj['data'])
-
-    @staticmethod
-    def toJSON_object(obj):
-        return {
-            'type': 'ndarray',
-            'data': obj.tolist(),
-            'dtype': str(obj.dtype)
-        }
+    def from_json(obj, context=None):
+        if obj is None:
+            return None
+        elif isinstance(obj, str):
+            return TypeClassProperty.from_string(obj)
+        elif isinstance(obj, dict):
+            # Let the deserializer handle this
+            return dace.serialize.from_json(obj)
+        else:
+            raise TypeError("Cannot parse type from: {}".format(obj))
```

### Comparing `dace-0.9.0/dace/sdfg.py` & `dace-0.9.5/dace/sdfg.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,48 +4,52 @@
 import errno
 import itertools
 from inspect import getframeinfo, stack
 import os
 import pickle, json
 from pydoc import locate
 import random
+import shutil
 import sys
-from typing import Any, Dict, Set, Tuple, List, Union
+from typing import Any, Dict, List, Optional, Set, Tuple, Type, Union
 import warnings
 import numpy as np
 import sympy as sp
 
 import dace
-from dace import data as dt, memlet as mm, subsets as sbs, dtypes, properties, symbolic
+import dace.serialize
+from dace import (data as dt, memlet as mm, subsets as sbs, dtypes, properties,
+                  symbolic)
 from dace.config import Config
-from dace.frontend.python import ndarray
+from dace.frontend.python import wrappers
 from dace.frontend.python.astutils import ASTFindReplace
 from dace.graph import edges as ed, nodes as nd, labeling
 from dace.graph.labeling import propagate_memlet, propagate_labels_sdfg
 from dace.data import validate_name
-from dace.graph import dot, nxutil
+from dace.graph import dot
 from dace.graph.graph import (OrderedDiGraph, OrderedMultiDiConnectorGraph,
                               SubgraphView, Edge, MultiConnectorEdge)
-from dace.properties import make_properties, Property, CodeProperty, OrderedDictProperty
+from dace.properties import (make_properties, Property, CodeProperty,
+                             OrderedDictProperty)
 
 
 def getcaller() -> Tuple[str, int]:
     """ Returns the file and line of the function that called the current
         function (the one that calls getcaller()).
-        @return: 2-tuple of file and line.
+        :return: 2-tuple of file and line.
     """
     caller = getframeinfo(stack()[2][0])
     return (caller.filename, caller.lineno)
 
 
 def getdebuginfo(old_dinfo=None) -> dtypes.DebugInfo:
     """ Returns a DebugInfo object for the position that called this function.
-        @param old_dinfo: Another DebugInfo object that will override the
+        :param old_dinfo: Another DebugInfo object that will override the
                           return value of this function
-        @return: DebugInfo containing line number and calling file.
+        :return: DebugInfo containing line number and calling file.
     """
     if old_dinfo is not None:
         return old_dinfo
 
     caller = getframeinfo(stack()[2][0])
     return dtypes.DebugInfo(caller.lineno, 0, caller.lineno, 0,
                             caller.filename)
@@ -145,157 +149,169 @@
             )
         else:
             edgestr = ""
 
         return "%s (at state %s%s)" % (self.message, str(state.label), edgestr)
 
 
+def _arrays_to_json(arrays):
+    if arrays is None:
+        return None
+    return {k: dace.serialize.to_json(v) for k, v in arrays.items()}
+
+
+def _arrays_from_json(obj, context=None):
+    if obj is None:
+        return {}
+    return {k: dace.serialize.from_json(v, context) for k, v in obj.items()}
+
+
 @make_properties
 class SDFG(OrderedDiGraph):
     """ The main intermediate representation of code in DaCe.
 
         A Stateful DataFlow multiGraph (SDFG) is a directed graph of directed
         acyclic multigraphs (i.e., where two nodes can be connected by more
         than one edge). The top-level directed graph represents a state
         machine, where edges can contain state transition conditions and
         assignments (see the `InterstateEdge` class documentation). The nested
         acyclic multigraphs represent dataflow, where nodes may represent data
         regions in memory, tasklets, or parametric graph scopes (see
-        `dace.graph.nodes` for a full list of available node types); edges in the multigraph represent data movement using memlets, as described in the `Memlet` class documentation.
+        `dace.graph.nodes` for a full list of available node types); edges in
+        the multigraph represent data movement using memlets, as described in
+        the `Memlet` class documentation.
     """
 
     #arg_types = Property(dtype=dict, default={}, desc="Formal parameter list")
     arg_types = OrderedDictProperty(default={}, desc="Formal parameter list")
     constants_prop = Property(
         dtype=dict, default={}, desc="Compile-time constants")
-    _arrays = Property(dtype=dict, desc="Data descriptors for this SDFG",
-                        to_json=lambda x: json.dumps({k: v for k, v in x.items() if k is not None}, default=Property.json_dumper) if x is not None else "null",
-                        from_json=lambda s, sdfg=None: Property.add_none_pair(json.loads(s, object_hook=Property.json_loader)) if s != "null" else None)
+    _arrays = Property(
+        dtype=dict,
+        desc="Data descriptors for this SDFG",
+        to_json=_arrays_to_json,
+        from_json=_arrays_from_json)
 
     global_code = CodeProperty(
         desc=
         "Code generated in a global scope on the frame-code generated file.",
         default="")
     init_code = CodeProperty(
         desc="Code generated in the `__dapp_init` function.", default="")
     exit_code = CodeProperty(
         desc="Code generated in the `__dapp_exit` function.", default="")
 
     def __init__(self,
                  name: str,
                  arg_types: Dict[str, dt.Data] = None,
-                 constants: Dict[str, Any] = None,
+                 constants: Dict[str, Tuple[dt.Data, Any]] = None,
                  propagate: bool = True,
                  parent=None):
         """ Constructs a new SDFG.
-            @param name: Name for the SDFG (also used as the filename for
+            :param name: Name for the SDFG (also used as the filename for
                          the compiled shared library).
-            @param symbols: Additional dictionary of symbol names -> types that the SDFG
+            :param symbols: Additional dictionary of symbol names -> types that the SDFG
                             defines, apart from symbolic data sizes.
-            @param propagate: If False, disables automatic propagation of
+            :param propagate: If False, disables automatic propagation of
                               memlet subsets from scopes outwards. Saves
                               processing time but disallows certain
                               transformations.
-            @param parent: The parent SDFG or SDFG state (for nested SDFGs).
+            :param parent: The parent SDFG or SDFG state (for nested SDFGs).
         """
         super(SDFG, self).__init__()
         self._name = name
         if name is not None and not validate_name(name):
             raise InvalidSDFGError('Invalid SDFG name "%s"' % name, self, None)
 
-        #if not isinstance(arg_types, collections.OrderedDict):
-        #    raise TypeError
-
-        #self._arg_types = arg_types  # OrderedDict(str, typeclass)
-        #self._constants = constants  # type: Dict[str, Any]
         self.arg_types = arg_types or collections.OrderedDict()
-        self.constants_prop = constants or {}
+        self.constants_prop = {}
+        if constants is not None:
+            for cstname, (cst_dtype, cstval) in constants.items():
+                self.add_constant(cstname, cstval, cst_dtype)
 
         self._propagate = propagate
         self._parent = parent
         self._symbols = {}  # type: Dict[str, dtypes.typeclass]
         self._parent_sdfg = None
         self._sdfg_list = [self]
         self._instrumented_parent = (
             False
         )  # Same as above. This flag is needed to know if the parent is instrumented (it's possible for a parent to be serial and instrumented.)
         self._start_state = None
-        self._arrays = {None: None}  # type: Dict[str, dt.Array]
+        self._arrays = {}  # type: Dict[str, dt.Array]
         self.global_code = ''
         self.init_code = ''
         self.exit_code = ''
 
         # Counter to make it easy to create temp transients
         self._temp_transients = 0
 
         # Counter to resolve name conflicts
         self._orig_name = name
         self._num = 0
 
-    def toJSON(self):
+    def to_json(self):
         """ Serializes this object to JSON format.
             :return: A string representing the JSON-serialized SDFG.
         """
-        import json
-        tmp = super(SDFG, self).toJSON()
-        tmp = json.loads(tmp)
+        tmp = super().to_json()
 
         # Inject the undefined symbols
-        tmp['undefined_symbols'] = self.undefined_symbols(True)
-        tmp['scalar_parameters'] = self.scalar_parameters(True)
+        tmp['undefined_symbols'] = [
+            (k, v.to_json())
+            for k, v in sorted(self.undefined_symbols(True).items())
+        ]
+        tmp['scalar_parameters'] = [(k, v.to_json()) for k, v in sorted(
+            self.scalar_parameters(True), key=lambda x: x[0])]
 
         tmp['attributes']['name'] = self.name
 
-        # Re-encode
-        return json.dumps(tmp, default=Property.json_dumper)
+        return tmp
 
     @classmethod
-    def fromJSON_object(cls, json_obj, context_info={'sdfg': None}):
+    def from_json(cls, json_obj, context_info={'sdfg': None}):
+
         _type = json_obj['type']
         if _type != cls.__name__:
             raise TypeError("Class type mismatch")
 
         attrs = json_obj['attributes']
         nodes = json_obj['nodes']
         edges = json_obj['edges']
 
-        import json
-
         ret = SDFG(
             name=attrs['name'],
-            arg_types=json.loads(
-                json.dumps(attrs['arg_types']),
-                object_hook=properties.Property.json_loader),
-            constants=json.loads(
-                json.dumps(attrs['constants_prop']),
-                object_hook=properties.Property.json_loader),
+            arg_types=dace.serialize.loads(
+                dace.serialize.dumps(attrs['arg_types'])),
+            constants=dace.serialize.loads(
+                dace.serialize.dumps(attrs['constants_prop'])),
             parent=context_info['sdfg'])
 
-        Property.set_properties_from_json(ret, json_obj)
+        dace.serialize.set_properties_from_json(
+            ret, json_obj, ignore_properties={'constants_prop'})
 
-        import copy
         for n in nodes:
             nci = copy.deepcopy(context_info)
             nci['sdfg'] = ret
 
-            state = SDFGState.fromJSON_object(n, nci)
+            state = SDFGState.from_json(n, context=nci)
             ret.add_node(state)
 
         for e in edges:
-            e = json.loads(json.dumps(e), object_hook=Property.json_loader)
+            e = dace.serialize.loads(dace.serialize.dumps(e))
             ret.add_edge(ret.node(int(e.src)), ret.node(int(e.dst)), e.data)
 
         # Redefine symbols
-        for k, v in json_obj['undefined_symbols'].items():
-            v = Property.known_types()[v['type']].fromJSON_object(v)
-            symbolic.symbol(k, v.dtype)
+        for k, v in json_obj['undefined_symbols']:
+            v = dace.serialize.from_json(v)
+            symbolic.symbol(k, v.dtype, override_dtype=True)
 
         for k, v in json_obj['scalar_parameters']:
-            v = Property.known_types()[v['type']].fromJSON_object(v)
-            ret.add_symbol(k, v.dtype)
+            v = dace.serialize.from_json(v)
+            ret.add_symbol(k, v.dtype, override_dtype=True)
 
         ret.validate()
 
         return ret
 
         # Counter to make it easy to create temp transients
         self._temp_transients = 0
@@ -320,17 +336,17 @@
         if dataname in self._symbols:
             return self._symbols[dataname]
         raise KeyError(
             'Data descriptor with name "%s" not found in SDFG' % dataname)
 
     def replace(self, name: str, new_name: str):
         """ Finds and replaces all occurrences of a symbol or array name in SDFG.
-            @param name: Name to find.
-            @param new_name: Name to replace.
-            @raise FileExistsError: If name and new_name already exist as data descriptors or symbols.
+            :param name: Name to find.
+            :param new_name: Name to replace.
+            :raise FileExistsError: If name and new_name already exist as data descriptors or symbols.
         """
 
         def replace_dict(d, old, new):
             if old in d:
                 if new in d:
                     raise FileExistsError('"%s" already exists in SDFG' % new)
                 d[new] = d[old]
@@ -355,73 +371,61 @@
 
         # Replace in states
         for state in self.nodes():
             state.replace(name, new_name)
 
     def add_symbol(self, name, stype, override_dtype=False):
         """ Adds a symbol to the SDFG.
-            @param name: Symbol name.
-            @param stype: Symbol type.
-            @param override_dtype: If True, overrides existing symbol type in
+            :param name: Symbol name.
+            :param stype: Symbol type.
+            :param override_dtype: If True, overrides existing symbol type in
                                    symbol registry.
         """
         if name in self._symbols:
             raise FileExistsError('Symbol "%s" already exists in SDFG' % name)
         if not isinstance(stype, dtypes.typeclass):
             stype = dtypes.DTYPE_TO_TYPECLASS[stype]
 
         symbolic.symbol(name, stype, override_dtype=override_dtype)
         self._symbols[name] = stype
 
     @property
     def start_state(self):
         """ Returns the starting state of this SDFG. """
+        source_nodes = self.source_nodes()
+        if len(source_nodes) == 1:
+            return source_nodes[0]
         if self._start_state is None:
-            return self.source_nodes()[0]
+            raise ValueError('Ambiguous or undefined starting state for SDFG')
 
         return self.node(self._start_state)
 
     def set_start_state(self, state_id):
         """ Manually sets the starting state of this SDFG.
-            @param state_id: The node ID (use `node_id(state)`) of the
+            :param state_id: The node ID (use `node_id(state)`) of the
                              state to set.
         """
         if state_id < 0 or state_id >= len(self.nodes()):
             raise ValueError("Invalid state ID")
         self._start_state = state_id
 
-    #@property
-    #def global_code(self):
-    #    """ Returns C++ code, generated in a global scope on the frame-code generated file. """
-    #    return self._global_code
-
     def set_global_code(self, cpp_code: str):
         """ Sets C++ code that will be generated in a global scope on the frame-code generated file. """
         self.global_code = {
             'code_or_block': cpp_code,
             'language': dace.dtypes.Language.CPP
         }
 
-    #@property
-    #def init_code(self):
-    #    """ Returns C++ code, generated in the `__dapp_init` function. """
-    #    return self._init_code
-
     def set_init_code(self, cpp_code: str):
         """ Sets C++ code, generated in the `__dapp_init` function. """
         self.init_code = {
             'code_or_block': cpp_code,
             'language': dace.dtypes.Language.CPP
         }
 
-    #@property
-    #def exit_code(self):
-    #    """ Returns C++ code, generated in the `__dapp_exit` function. """
-    #    return self._exit_code
-
     def set_exit_code(self, cpp_code: str):
         """ Sets C++ code, generated in the `__dapp_exit` function. """
         self.exit_code = {
             'code_or_block': cpp_code,
             'language': dace.dtypes.Language.CPP
         }
 
@@ -431,16 +435,16 @@
     def set_instrumented_parent(self):
         self._instrumented_parent = (
             True
         )  # When this is set: Under no circumstances try instrumenting this (or any transitive children)
 
     def remove_data(self, name, validate=True):
         """ Removes a data descriptor from the SDFG.
-            @param name: The name of the data descriptor to remove.
-            @param validate: If True, verifies that there are no access
+            :param name: The name of the data descriptor to remove.
+            :param validate: If True, verifies that there are no access
                              nodes that are using this data descriptor
                              prior to removing it.
         """
         # Verify first that there are no access nodes that use this data
         if validate:
             for state in self.nodes():
                 for node in state.nodes():
@@ -467,16 +471,16 @@
 
     @property
     def sdfg_list(self):
         return self._sdfg_list
 
     def set_sourcecode(self, code, lang=None):
         """ Set the source code of this SDFG (for IDE purposes).
-            @param code: A string of source code.
-            @param lang: A string representing the language of the source code,
+            :param code: A string of source code.
+            :param lang: A string representing the language of the source code,
                          for syntax highlighting and completion.
         """
         self.sourcecode = {'code_or_block': code, 'language': lang}
 
     @property
     def name(self):
         """ The name of this SDFG. """
@@ -496,43 +500,53 @@
 
     @property
     def label(self):
         """ The name of this SDFG. """
         #return self._name
         return self.name
 
-    #@property
-    #def arg_types(self):
-    #    return self._arg_types
-
     @property
     def constants(self):
         """ A dictionary of compile-time constants defined in this SDFG. """
         result = {}
         # Merge with parent's constants
         if self._parent_sdfg is not None:
             result.update(self._parent_sdfg.constants)
 
-        #result.update(self._constants)
-        result.update(self.constants_prop)
+        def cast(dtype: dt.Data, value: Any):
+            """ Cast a value to the given data type. """
+            if isinstance(dtype, dt.Array):
+                return value
+            elif isinstance(dtype, dt.Scalar):
+                return dtype.dtype(value)
+            raise TypeError('Unsupported data type %s' % dtype)
+
+        result.update({k: cast(*v) for k, v in self.constants_prop.items()})
         return result
 
-    def add_constants(self, new_constants: Dict[str, Any]):
-        """ Adds new compile-time constants to this SDFG.
-            @param new_constants: Dictionary of new constants to add.
-        """
-        #self._constants.update(new_constants)
-        self.constants_prop.update(new_constants)
-
-    def reset_constants(self, constants: Dict[str, Any]):
-        """ Resets compile-time constants of this SDFG to a given dictionary.
-            @param constants: Dictionary of new constants to set.
-        """
-        #self._constants = constants
-        self.constants_prop = constants
+    def add_constant(self, name: str, value: Any, dtype: dt.Data = None):
+        """ Adds/updates a new compile-time constant to this SDFG. A constant
+            may either be a scalar or a numpy ndarray thereof.
+            :param name: The name of the constant.
+            :param value: The constant value.
+            :param dtype: Optional data type of the symbol, or None to deduce
+                          automatically.
+        """
+
+        def get_type(obj):
+            if isinstance(obj, np.ndarray):
+                return dt.Array(
+                    dtypes.DTYPE_TO_TYPECLASS[obj.dtype.type], shape=obj.shape)
+            elif isinstance(obj, dtypes.typeclass):
+                return dt.Scalar(type(obj))
+            elif type(obj) in dtypes.DTYPE_TO_TYPECLASS:
+                return dt.Scalar(dtypes.DTYPE_TO_TYPECLASS[type(obj)])
+            raise TypeError('Unrecognized constant type: %s' % type(obj))
+
+        self.constants_prop[name] = (dtype or get_type(value), value)
 
     @property
     def propagate(self):
         return self._propagate
 
     @propagate.setter
     def propagate(self, propagate: bool):
@@ -555,33 +569,33 @@
     @parent_sdfg.setter
     def parent_sdfg(self, value):
         self._parent_sdfg = value
 
     def add_node(self, node, is_start_state=False):
         """ Adds a new node to the SDFG. Must be an SDFGState or a subclass
             thereof.
-            @param node: The node to add.
-            @param is_start_state: If True, sets this node as the starting
+            :param node: The node to add.
+            :param is_start_state: If True, sets this node as the starting
                                    state.
         """
         if not isinstance(node, SDFGState):
             raise TypeError("Expected SDFGState, got " + str(type(node)))
 
         # If no start state has been defined, define to be the first state
         if is_start_state == True:
             self._start_state = len(self.nodes())
 
         return super(SDFG, self).add_node(node)
 
     def add_edge(self, u, v, edge):
         """ Adds a new edge to the SDFG. Must be an InterstateEdge or a
             subclass thereof.
-            @param u: Source node.
-            @param v: Destination node.
-            @param edge: The edge to add.
+            :param u: Source node.
+            :param v: Destination node.
+            :param edge: The edge to add.
         """
         if not isinstance(u, SDFGState):
             raise TypeError("Expected SDFGState, got: {}".format(
                 type(u).__name__))
         if not isinstance(v, SDFGState):
             raise TypeError("Expected SDFGState, got: {}".format(
                 type(v).__name__))
@@ -601,14 +615,24 @@
             either the SDFG (for states) or a DFG (nodes). """
         all_nodes = []
         for node in self.nodes():
             all_nodes.append((node, self))
             all_nodes += node.all_nodes_recursive()
         return all_nodes
 
+    def all_edges_recursive(self):
+        """ Iterate over all edges in this SDFG, including state edges,
+            inter-state edges, and recursively edges within nested SDFGs,
+            returning tuples on the form (edge, parent), where the parent is
+            either the SDFG (for states) or a DFG (nodes). """
+        all_edges = [(e, self) for e in self.edges()]
+        for node in self.nodes():
+            all_edges += node.all_edges_recursive()
+        return all_edges
+
     def arrays_recursive(self):
         """ Iterate over all arrays in this SDFG, including arrays within
             nested SDFGs. Yields 3-tuples of (sdfg, array name, array)."""
         for aname, arr in self.arrays.items():
             yield self, aname, arr
         for state in self.nodes():
             for node in state.nodes():
@@ -639,14 +663,20 @@
             for s in edge_data.condition_symbols():
                 used[s] = dt.Scalar(symbolic.symbol(s).dtype)
         for state in self.nodes():
             a, u = state.interstate_symbols()
             assigned.update(a)
             used.update(u)
 
+        assigned = collections.OrderedDict([(k, v)
+                                            for k, v in assigned.items()
+                                            if not k.startswith('__dace')])
+        used = collections.OrderedDict(
+            [(k, v) for k, v in used.items() if not k.startswith('__dace')])
+
         return assigned, used
 
     def scalar_parameters(self, include_constants):
         """ Returns all scalar data arguments to the SDFG (this excludes
             symbols used to define array sizes)."""
         return [
             (name, dt.Scalar(stype)) for name, stype in self._symbols.items()
@@ -748,15 +778,16 @@
         return iteration_variables, subset_symbols
 
     def all_symbols(self, include_constants):
         """ Returns all symbols used in this SDFG, including scalar parameters
             to the SDFG, loop iteration variables, array sizes and variables
             used in interstate edges. """
         symbols = collections.OrderedDict(
-            (name, data) for name, data in self.scalar_parameters())
+            (name, data)
+            for name, data in self.scalar_parameters(include_constants))
         symbols.update(self.data_symbols(True))
         assigned, used = self.interstate_symbols()
         symbols.update(used)
         iteration_variables, subset_symbols = self.scope_symbols()
         symbols.update(subset_symbols)
         symbols.update(iteration_variables)
         if include_constants:
@@ -842,20 +873,20 @@
                 arg_list[key] = val
 
         return arg_list
 
     def signature_arglist(self, with_types=True, for_call=False):
         """ Returns a list of arguments necessary to call this SDFG,
             formatted as a list of C definitions.
-            @param with_types: If True, includes argment types in the result.
-            @param for_call: If True, returns arguments that can be used when
+            :param with_types: If True, includes argument types in the result.
+            :param for_call: If True, returns arguments that can be used when
                              calling the SDFG. This means that immaterial data
                              will generate "nullptr" arguments instead of the
                              argument names.
-            @return: A list of strings. For example: `['float *A', 'int b']`.
+            :return: A list of strings. For example: `['float *A', 'int b']`.
         """
         arg_list = self.arglist()
 
         signature_args = []
         for name, arg_type in arg_list.items():
             if isinstance(arg_type, dace.data.Data):
                 signature_args.append(
@@ -864,35 +895,35 @@
             else:
                 raise TypeError("Unsupported argument type")
 
         return signature_args
 
     def signature(self, with_types=True, for_call=False):
         """ Returns a C/C++ signature of this SDFG, used when generating code.
-            @param with_types: If True, includes argument types (can be used
+            :param with_types: If True, includes argument types (can be used
                                for a function prototype). If False, only
                                include argument names (can be used for function
                                calls).
-            @param for_call: If True, returns arguments that can be used when
+            :param for_call: If True, returns arguments that can be used when
                              calling the SDFG. This means that immaterial data
                              will generate "nullptr" arguments instead of the
                              argument names.
         """
         return ", ".join(self.signature_arglist(with_types, for_call))
 
     def draw_to_file(self,
                      filename="sdfg.dot",
                      fill_connectors=True,
                      recursive=True):
         """ Draws the SDFG to a GraphViz (.dot) file.
-            @param filename: The file to draw the SDFG to (will be written to
+            :param filename: The file to draw the SDFG to (will be written to
                              '_dotgraphs/<filename>').
-            @param fill_connectors: Whether to fill missing scope (e.g., "IN_")
+            :param fill_connectors: Whether to fill missing scope (e.g., "IN_")
                                     connectors prior to drawing the graph.
-            @param recursive: If True, also draws nested SDFGs.
+            :param recursive: If True, also draws nested SDFGs.
         """
         if fill_connectors:
             self.fill_scope_connectors()
 
         try:
             os.makedirs("_dotgraphs")
         # Python 2.x does not have FileExistsError
@@ -912,15 +943,15 @@
                         node.sdfg.draw_to_file(
                             filename=node.sdfg.name + "_" + filename,
                             recursive=True)
 
     def draw(self):
         """ Creates a GraphViz representation of the full SDFG, including all
             states and transitions.
-            @return: A string representing the SDFG in .dot format.
+            :return: A string representing the SDFG in .dot format.
         """
 
         nodes = []
 
         # Redirect all edges between states to point at the boundaries
         edges = []
         for ind, edge in enumerate(self.edges()):
@@ -1016,23 +1047,31 @@
             "    compound=true;\n" + "    newrank=true;\n" +
             "\n    ".join(nodes + edges) + "\n" + "\n".join(clusters) + "\n}")
 
     # TODO(later): Also implement the "_repr_svg_" method for static output
     def _repr_html_(self):
         """ HTML representation of the SDFG, used mainly for Jupyter
             notebooks. """
+        from dace.jupyter import isnotebook, preamble
+
+        result = ''
+        if not isnotebook():
+            result = preamble()
+
         # Create renderer canvas and load SDFG
-        result = """
+        result += """
 <div id="contents_{uid}" style="position: relative; resize: vertical; overflow: auto"></div>
 <script>
     var sdfg_{uid} = {sdfg};
-    var renderer_{uid} = new SDFGRenderer(parse_sdfg(sdfg_{uid}), 
+    var renderer_{uid} = new SDFGRenderer(parse_sdfg(sdfg_{uid}),
         document.getElementById('contents_{uid}'));
 </script>""".format(
-            sdfg=json.dumps(self.toJSON()),
+            # Dumping to a string so that Jupyter Javascript can parse it
+            # recursively
+            sdfg=dace.serialize.dumps(dace.serialize.dumps(self.to_json())),
             uid=random.randint(0, sys.maxsize - 1))
 
         return result
 
     def transients(self):
         """ Returns a dictionary mapping transient data descriptors to their
             parent scope entry node, or None if top-level (i.e., exists in
@@ -1059,24 +1098,32 @@
         return result
 
     def shared_transients(self):
         """ Returns a list of transient data that appears in more than one
             state. """
         seen = {}
         shared = []
+
+        # If a transient is present in an inter-state edge, it is shared
+        for interstate_edge in self.edges():
+            for sym in interstate_edge.data.condition_symbols():
+                if sym in self.arrays and self.arrays[sym].transient:
+                    seen[sym] = interstate_edge
+                    shared.append(sym)
+
+        # If transient is accessed in more than one state, it is shared
         for state in self.nodes():
             for node in state.nodes():
                 if isinstance(node,
                               nd.AccessNode) and node.desc(self).transient:
-                    # If transient is accessed in more than one state, it is a
-                    # shared transient
                     if node.desc(self).toplevel or (node.data in seen and
                                                     seen[node.data] != state):
                         shared.append(node.data)
                     seen[node.data] = state
+
         return dtypes.deduplicate(shared)
 
     def input_arrays(self):
         """ Returns a list of input arrays that need to be fed into the SDFG.
         """
         result = []
         for state in self.nodes():
@@ -1095,61 +1142,66 @@
                 if isinstance(node, nd.AccessNode):
                     if node not in result:
                         result.append(node)
         return result
 
     def save(self, filename: str, use_pickle=False, with_metadata=False):
         """ Save this SDFG to a file.
-            @param filename: File name to save to.
-            @param use_pickle: Use Python pickle as the SDFG format (default:
+            :param filename: File name to save to.
+            :param use_pickle: Use Python pickle as the SDFG format (default:
                                JSON).
-            @param with_metadata: Save property metadata (e.g. name,
+            :param with_metadata: Save property metadata (e.g. name,
                                   description). False or True override current
                                   option, whereas None keeps default
         """
+        try:
+            os.makedirs(os.path.dirname(filename), exist_ok=True)
+        except (FileNotFoundError, FileExistsError):
+            pass
+
         if use_pickle:
             with open(filename, "wb") as fp:
                 symbolic.SympyAwarePickler(fp).dump(self)
         else:
             if with_metadata is not None:
-                old_meta = dace.properties.json_store_metadata
-                dace.properties.json_store_metadata = with_metadata
+                old_meta = dace.serialize.JSON_STORE_METADATA
+                dace.serialize.JSON_STORE_METADATA = with_metadata
             with open(filename, "w") as fp:
-                fp.write(self.toJSON())
+                fp.write(dace.serialize.dumps(self.to_json()))
             if with_metadata is not None:
-                dace.properties.json_store_metadata = old_meta
+                dace.serialize.JSON_STORE_METADATA = old_meta
 
     @staticmethod
     def from_file(filename: str):
         """ Constructs an SDFG from a file.
-            @param filename: File name to load SDFG from.
-            @return: An SDFG.
+            :param filename: File name to load SDFG from.
+            :return: An SDFG.
         """
         with open(filename, "rb") as fp:
             firstbyte = fp.read(1)
             fp.seek(0)
             if firstbyte == b'{':  # JSON file
                 sdfg_json = json.load(fp)
-                sdfg = SDFG.fromJSON_object(sdfg_json)
+                sdfg = SDFG.from_json(sdfg_json)
             else:  # Pickle
                 sdfg = symbolic.SympyAwareUnpickler(fp).load()
 
             if not isinstance(sdfg, SDFG):
                 raise TypeError("Loaded file is not an SDFG (loaded "
                                 "type: %s)" % type(sdfg).__name__)
             return sdfg
 
     # Dynamic SDFG creation API
     ##############################
     def add_state(self, label=None, is_start_state=False):
         """ Adds a new SDFG state to this graph and returns it.
-            @param label: State label.
-            @param is_start_state: If True, resets SDFG starting state to this
+            :param label: State label.
+            :param is_start_state: If True, resets SDFG starting state to this
                                    state.
-            @return: A new SDFGState object.
+            :return: A new SDFGState object.
         """
         if label is None or any([s.label == label for s in self.nodes()]):
             i = len(self)
             base = "state" if label is None else label
             while True:
                 # Append a number. If the state already exists, increment the
                 # number until it doesn't
@@ -1159,39 +1211,50 @@
                 else:
                     break
         state = SDFGState(label, self)
 
         self.add_node(state, is_start_state=is_start_state)
         return state
 
-    def add_array(
-            self,
-            name: str,
-            shape,
-            dtype,
-            storage=dtypes.StorageType.Default,
-            materialize_func=None,
-            transient=False,
-            strides=None,
-            offset=None,
-            toplevel=False,
-            debuginfo=None,
-            allow_conflicts=False,
-            access_order=None,
-    ):
+    def _find_new_name(self, name: str):
+        """ Tries to find a new name by adding an underscore and a number. """
+        index = 0
+        while (name + ('_%d' % index)) in self._arrays:
+            index += 1
+
+        return name + ('_%d' % index)
+
+    def add_array(self,
+                  name: str,
+                  shape,
+                  dtype,
+                  storage=dtypes.StorageType.Default,
+                  materialize_func=None,
+                  transient=False,
+                  strides=None,
+                  offset=None,
+                  toplevel=False,
+                  debuginfo=None,
+                  allow_conflicts=False,
+                  total_size=None,
+                  find_new_name=False):
         """ Adds an array to the SDFG data descriptor store. """
 
         if not isinstance(name, str):
             raise TypeError(
                 "Array name must be a string. Got %s" % type(name).__name__)
 
         # If exists, fail
         if name in self._arrays:
-            raise NameError('Array or Stream with name "%s" already exists '
-                            "in SDFG" % name)
+            if not find_new_name:
+                raise NameError(
+                    'Array or Stream with name "%s" already exists '
+                    "in SDFG" % name)
+            else:
+                name = self._find_new_name(name)
 
         # convert strings to int if possible
         newshape = []
         for s in shape:
             try:
                 newshape.append(int(s))
             except:
@@ -1203,222 +1266,231 @@
 
         desc = dt.Array(
             dtype,
             shape,
             storage=storage,
             materialize_func=materialize_func,
             allow_conflicts=allow_conflicts,
-            access_order=access_order,
             transient=transient,
             strides=strides,
             offset=offset,
             toplevel=toplevel,
             debuginfo=debuginfo,
-        )
+            total_size=total_size)
 
         self._arrays[name] = desc
-        return desc
+        return name, desc
 
-    def add_stream(
-            self,
-            name: str,
-            dtype,
-            veclen=1,
-            buffer_size=1,
-            shape=(1, ),
-            storage=dtypes.StorageType.Default,
-            transient=False,
-            strides=None,
-            offset=None,
-            toplevel=False,
-            debuginfo=None,
-    ):
+    def add_stream(self,
+                   name: str,
+                   dtype,
+                   veclen=1,
+                   buffer_size=1,
+                   shape=(1, ),
+                   storage=dtypes.StorageType.Default,
+                   transient=False,
+                   offset=None,
+                   toplevel=False,
+                   debuginfo=None,
+                   find_new_name=False):
         """ Adds a stream to the SDFG data descriptor store. """
         if not isinstance(name, str):
             raise TypeError(
                 "Stream name must be a string. Got %s" % type(name).__name__)
 
         # If exists, fail
         if name in self._arrays:
-            raise NameError('Array or Stream with name "%s" already exists '
-                            "in SDFG" % name)
+            if not find_new_name:
+                raise NameError(
+                    'Array or Stream with name "%s" already exists '
+                    "in SDFG" % name)
+            else:
+                name = self._find_new_name(name)
 
         if isinstance(dtype, type) and dtype in dtypes._CONSTANT_TYPES[:-1]:
             dtype = dtypes.typeclass(dtype)
 
         desc = dt.Stream(
             dtype,
             veclen,
             buffer_size,
             shape=shape,
             storage=storage,
             transient=transient,
-            strides=strides,
             offset=offset,
             toplevel=toplevel,
             debuginfo=debuginfo,
         )
 
         self._arrays[name] = desc
-        return desc
+        return name, desc
 
-    def add_scalar(
-            self,
-            name: str,
-            dtype,
-            storage=dtypes.StorageType.Default,
-            transient=False,
-            toplevel=False,
-            debuginfo=None,
-    ):
+    def add_scalar(self,
+                   name: str,
+                   dtype,
+                   storage=dtypes.StorageType.Default,
+                   transient=False,
+                   toplevel=False,
+                   debuginfo=None,
+                   find_new_name=False):
         """ Adds a scalar to the SDFG data descriptor store. """
         if not isinstance(name, str):
             raise TypeError(
                 "Scalar name must be a string. Got %s" % type(name).__name__)
         # If exists, fail
         if name in self._arrays:
-            raise NameError('Array or Stream with name "%s" already exists '
-                            "in SDFG" % name)
+            if not find_new_name:
+                raise NameError(
+                    'Array or Stream with name "%s" already exists '
+                    "in SDFG" % name)
+            else:
+                name = self._find_new_name(name)
 
         if isinstance(dtype, type) and dtype in dtypes._CONSTANT_TYPES[:-1]:
             dtype = dtypes.typeclass(dtype)
 
         desc = dt.Scalar(
             dtype,
             storage=storage,
             transient=transient,
             toplevel=toplevel,
             debuginfo=debuginfo,
         )
 
         self._arrays[name] = desc
-        return desc
+        return name, desc
 
-    def add_transient(
-            self,
-            name,
-            shape,
-            dtype,
-            storage=dtypes.StorageType.Default,
-            materialize_func=None,
-            strides=None,
-            offset=None,
-            toplevel=False,
-            debuginfo=None,
-            allow_conflicts=False,
-            access_order=None,
-    ):
+    def add_transient(self,
+                      name,
+                      shape,
+                      dtype,
+                      storage=dtypes.StorageType.Default,
+                      materialize_func=None,
+                      strides=None,
+                      offset=None,
+                      toplevel=False,
+                      debuginfo=None,
+                      allow_conflicts=False,
+                      total_size=None,
+                      find_new_name=False):
         """ Convenience function to add a transient array to the data
             descriptor store. """
         return self.add_array(
             name,
             shape,
             dtype,
             storage,
             materialize_func,
             True,
             strides,
             offset,
             toplevel=toplevel,
-            debuginfo=None,
+            debuginfo=debuginfo,
             allow_conflicts=allow_conflicts,
-            access_order=access_order,
-        )
+            total_size=total_size,
+            find_new_name=find_new_name)
 
     def temp_data_name(self):
         """ Returns a temporary data descriptor name that can be used in this SDFG. """
 
         name = '__tmp%d' % self._temp_transients
         while name in self._arrays:
             self._temp_transients += 1
             name = '__tmp%d' % self._temp_transients
+        self._temp_transients += 1
 
         return name
 
     def add_temp_transient(self,
                            shape,
                            dtype,
                            storage=dtypes.StorageType.Default,
                            materialize_func=None,
                            strides=None,
                            offset=None,
                            toplevel=False,
                            debuginfo=None,
                            allow_conflicts=False,
-                           access_order=None):
+                           total_size=None):
         """ Convenience function to add a transient array with a temporary name to the data
             descriptor store. """
-        name = self.temp_data_name()
-
-        return name, self.add_array(
-            name,
+        return self.add_array(
+            self.temp_data_name(),
             shape,
             dtype,
             storage,
             materialize_func,
             True,
             strides,
             offset,
             toplevel=toplevel,
-            debuginfo=None,
+            debuginfo=debuginfo,
             allow_conflicts=allow_conflicts,
-            access_order=access_order)
+            total_size=total_size)
 
-    def add_datadesc(self, name: str, datadesc: dt.Data):
+    def add_datadesc(self, name: str, datadesc: dt.Data, find_new_name=False):
         """ Adds an existing data descriptor to the SDFG array store.
-            @param name: Name to use.
-            @param datadesc: Data descriptor to add.
+            :param name: Name to use.
+            :param datadesc: Data descriptor to add.
+            :param find_new_name: If True and data descriptor with this name
+                                  exists, finds a new name to add.
+            :return: Name of the new data descriptor
         """
         if not isinstance(name, str):
             raise TypeError("Data descriptor name must be a string. Got %s" %
                             type(name).__name__)
         # If exists, fail
         if name in self._arrays:
-            raise NameError('Array or Stream with name "%s" already exists '
-                            "in SDFG" % name)
+            if find_new_name:
+                name = self._find_new_name(name)
+            else:
+                raise NameError(
+                    'Array or Stream with name "%s" already exists '
+                    "in SDFG" % name)
         self._arrays[name] = datadesc
+        return name
 
     def add_loop(
             self,
             before_state,
             loop_state,
             after_state,
             loop_var: str,
             initialize_expr: str,
             condition_expr: str,
             increment_expr: str,
             loop_end_state=None,
     ):
-        """ Helper function that adds a looping state machine around a 
+        """ Helper function that adds a looping state machine around a
             given state (or sequence of states).
-            @param before_state: The state after which the loop should
+            :param before_state: The state after which the loop should
                                  begin, or None if the loop is the first
                                  state (creates an empty state).
-            @param loop_state: The state that begins the loop. See also
+            :param loop_state: The state that begins the loop. See also
                                `loop_end_state` if the loop is multi-state.
-            @param after_state: The state that should be invoked after
-                                the loop ends, or None if the program 
+            :param after_state: The state that should be invoked after
+                                the loop ends, or None if the program
                                 should terminate (creates an empty state).
-            @param loop_var: A name of an inter-state variable to use
+            :param loop_var: A name of an inter-state variable to use
                              for the loop. If None, `initialize_expr`
                              and `increment_expr` must be None.
-            @param initialize_expr: A string expression that is assigned
+            :param initialize_expr: A string expression that is assigned
                                     to `loop_var` before the loop begins.
                                     If None, does not define an expression.
-            @param condition_expr: A string condition that occurs every
-                                   loop iteration. If None, loops forever 
+            :param condition_expr: A string condition that occurs every
+                                   loop iteration. If None, loops forever
                                    (undefined behavior).
-            @param increment_expr: A string expression that is assigned to
+            :param increment_expr: A string expression that is assigned to
                                    `loop_var` after every loop iteration.
                                     If None, does not define an expression.
-            @param loop_end_state: If the loop wraps multiple states, the
+            :param loop_end_state: If the loop wraps multiple states, the
                                    state where the loop iteration ends.
-                                   If None, sets the end state to 
+                                   If None, sets the end state to
                                    `loop_state` as well.
-            @return: A 3-tuple of (`before_state`, generated loop guard state,
+            :return: A 3-tuple of (`before_state`, generated loop guard state,
                                    `after_state`).
         """
         from dace.frontend.python.astutils import negate_expr  # Avoid import loops
 
         # Argument checks
         if loop_var is None and (initialize_expr or increment_expr):
             raise ValueError("Cannot initalize or increment an empty loop"
@@ -1459,16 +1531,16 @@
     # SDFG queries
     ##############################
 
     def find_state(self, state_id_or_label):
         """ Finds a state according to its ID (if integer is provided) or
             label (if string is provided).
 
-            @param state_id_or_label: State ID (if int) or label (if str).
-            @return: An SDFGState object.
+            :param state_id_or_label: State ID (if int) or label (if str).
+            :return: An SDFGState object.
         """
 
         if isinstance(state_id_or_label, str):
             for s in self.nodes():
                 if s.label == state_id_or_label:
                     return s
             raise LookupError("State %s not found" % state_id_or_label)
@@ -1479,26 +1551,26 @@
                 "state_id_or_label is not an int nor string: {}".format(
                     state_id_or_label))
 
     def find_node(self, state_id_or_label, node_id_or_label):
         """ Finds a node within a state according to its ID (if integer is
             provided) or label (if string is provided).
 
-            @param state_id_or_label: State ID (if int) or label (if str).
-            @param node_id_or_label:  Node ID (if int) or label (if str)
+            :param state_id_or_label: State ID (if int) or label (if str).
+            :param node_id_or_label:  Node ID (if int) or label (if str)
                                       within the given state.
-            @return: A nodes.Node object.
+            :return: A nodes.Node object.
         """
         state = self.find_state(state_id_or_label)
         return state.find_node(node_id_or_label)
 
     def specialize(self, additional_symbols=None, specialize_all_symbols=True):
         """ Sets symbolic values in this SDFG to constants.
-            @param additional_symbols: Additional values to specialize.
-            @param specialize_all_symbols: If True, raises an
+            :param additional_symbols: Additional values to specialize.
+            :param specialize_all_symbols: If True, raises an
                    UnboundLocalError if at least one of the symbols in the
                    SDFG is unset.
         """
         syms = {}
         additional_symbols = additional_symbols or {}
         undefined_symbols = self.undefined_symbols(False)
         # scalar_arguments = self.scalar_parameters(False)
@@ -1518,26 +1590,29 @@
             # If symbols are passed, extract the value. If constants are
             # passed, use them directly.
             name: val.get() if isinstance(val, dace.symbolic.symbol) else val
             for name, val in additional_symbols.items()
         })
 
         # Update constants
-        self.constants_prop.update(syms)
+        for k, v in syms.items():
+            self.add_constant(k, v)
 
-    def compile(self, specialize=None, optimizer=None):
+    def compile(self, specialize=None, optimizer=None, output_file=None):
         """ Compiles a runnable binary from this SDFG.
 
-            @param specialize: If True, specializes all symbols to their
+            :param specialize: If True, specializes all symbols to their
                                defined values as constants. If None, uses
                                configuration setting.
-            @param optimizer: If defines a valid class name, it will be called
+            :param optimizer: If defines a valid class name, it will be called
                               during compilation to transform the SDFG as
                               necessary. If None, uses configuration setting.
-            @return: A callable CompiledSDFG object.
+            :param output_file: If not None, copies the output library file to
+                                the specified path.
+            :return: A callable CompiledSDFG object.
         """
 
         # Importing these outside creates an import loop
         from dace.codegen import codegen, compiler
 
         if Config.get_bool("compiler", "use_cache"):
             # Try to see if a cached version of the binary exists
@@ -1565,36 +1640,45 @@
                 "optimizer", "autospecialize")) or specialize == True:
             sdfg.specialize()
 
         # Optimize SDFG using the CLI or external hooks
         optclass = _get_optimizer_class(optimizer)
         if optclass is not None:
             opt = optclass(sdfg)
-            sdfg = opt.optimize(debugprint=Config.get_bool("debugprint"))
+            sdfg = opt.optimize()
+
+        sdfg.save(os.path.join('_dotgraphs', 'program.sdfg'))
 
         # Generate code for the program by traversing the SDFG state by state
         program_objects = codegen.generate_code(sdfg)
 
         # Generate the program folder and write the source files
         program_folder = compiler.generate_program_folder(
             self, program_objects, os.path.join(".dacecache", sdfg.name))
 
         # Compile the code and get the shared library path
         shared_library = compiler.configure_and_compile(program_folder)
 
+        # If provided, save output to path or filename
+        if output_file is not None:
+            if os.path.isdir(output_file):
+                output_file = os.path.join(output_file,
+                                           os.path.basename(shared_library))
+            shutil.copyfile(shared_library, output_file)
+
         # Get the function handle
         return compiler.get_program_handle(shared_library, sdfg)
 
     def argument_typecheck(self, args, kwargs, types_only=False):
         """ Checks if arguments and keyword arguments match the SDFG
             types. Raises RuntimeError otherwise.
 
-            @raise RuntimeError: Argument count mismatch.
-            @raise TypeError: Argument type mismatch.
-            @raise NotImplementedError: Unsupported argument type.
+            :raise RuntimeError: Argument count mismatch.
+            :raise TypeError: Argument type mismatch.
+            :raise NotImplementedError: Unsupported argument type.
         """
         expected_args = self.arglist()
         num_args_passed = len(args) + len(kwargs)
         num_args_expected = len(expected_args)
         if num_args_passed < num_args_expected:
             expected_kwargs = list(expected_args.keys())[len(args):]
             missing_args = [k for k in expected_kwargs if k not in kwargs]
@@ -1628,16 +1712,15 @@
                 desc = dt.create_datadescriptor(passed)
                 if not expected.is_equivalent(desc):
                     raise TypeError("Type mismatch for argument: "
                                     "expected %s, got %s" % (expected, desc))
                 else:
                     continue
             if isinstance(expected, dace.data.Array):
-                if (not isinstance(passed, ndarray.ndarray)
-                        and not isinstance(passed, np.ndarray)):
+                if not isinstance(passed, np.ndarray):
                     raise TypeError("Type mismatch for argument {}: "
                                     "expected array type, got {}".format(
                                         arg, type(passed)))
             elif (isinstance(expected, dace.data.Scalar)
                   or isinstance(expected, dace.dtypes.typeclass)):
                 if (not dace.dtypes.isconstant(passed)
                         and not isinstance(passed, dace.symbolic.symbol)):
@@ -1694,49 +1777,53 @@
 
     def validate(self) -> None:
         """ Verifies the correctness of an SDFG by applying multiple tests.
 
             Raises an InvalidSDFGError with the erroneous node/edge
             on failure.
         """
-        # SDFG-level checks
-        if not validate_name(self.name):
-            raise InvalidSDFGError("Invalid name", self, None)
-
-        if len(self.source_nodes()) > 1 and self._start_state is None:
-            raise InvalidSDFGError("Starting state undefined", self, None)
-
-        if len(set([s.label for s in self.nodes()])) != len(self.nodes()):
-            raise InvalidSDFGError("Found multiple states with the same name",
-                                   self, None)
-
-        # Validate array names
-        for name in self._arrays.keys():
-            if name is not None and not validate_name(name):
-                raise InvalidSDFGError("Invalid array name %s" % name, self,
-                                       None)
-
-        # Check every state separately
-        for sid, state in enumerate(self.nodes()):
-            state.validate(self, sid)
-
-        # Interstate edge checks
-        for eid, edge in enumerate(self.edges()):
-
-            # Name validation
-            if len(edge.data.assignments) > 0:
-                for assign in edge.data.assignments.keys():
-                    if not validate_name(assign):
-                        raise InvalidSDFGInterstateEdgeError(
-                            "Invalid interstate symbol name %s" % assign, self,
-                            eid)
+        try:
+            # SDFG-level checks
+            if not validate_name(self.name):
+                raise InvalidSDFGError("Invalid name", self, None)
+
+            if len(self.source_nodes()) > 1 and self._start_state is None:
+                raise InvalidSDFGError("Starting state undefined", self, None)
+
+            if len(set([s.label for s in self.nodes()])) != len(self.nodes()):
+                raise InvalidSDFGError(
+                    "Found multiple states with the same name", self, None)
+
+            # Validate array names
+            for name in self._arrays.keys():
+                if name is not None and not validate_name(name):
+                    raise InvalidSDFGError("Invalid array name %s" % name,
+                                           self, None)
+
+            # Check every state separately
+            for sid, state in enumerate(self.nodes()):
+                state.validate(self, sid)
+
+            # Interstate edge checks
+            for eid, edge in enumerate(self.edges()):
+
+                # Name validation
+                if len(edge.data.assignments) > 0:
+                    for assign in edge.data.assignments.keys():
+                        if not validate_name(assign):
+                            raise InvalidSDFGInterstateEdgeError(
+                                "Invalid interstate symbol name %s" % assign,
+                                self, eid)
 
-        # TODO: Check interstate edges with undefined symbols
+            # TODO: Check interstate edges with undefined symbols
 
-        pass
+        except InvalidSDFGError:
+            # If the SDFG is invalid, save it
+            self.save(os.path.join('_dotgraphs', 'invalid.sdfg'))
+            raise
 
     def is_valid(self) -> bool:
         """ Returns True if the SDFG is verified correctly (using `validate`).
         """
         try:
             self.validate()
         except InvalidSDFGError:
@@ -1746,52 +1833,74 @@
     def apply_strict_transformations(self, validate=True):
         """ Applies safe transformations (that will surely increase the
             performance) on the SDFG. For example, this fuses redundant states
             (safely) and removes redundant arrays.
 
             B{Note:} This is an in-place operation on the SDFG.
         """
-        from dace.transformation.dataflow import RedundantArray
-        from dace.transformation.interstate import StateFusion
-        from dace.transformation.interstate import InlineSDFG
+        from dace.transformation.dataflow import RedundantArray, MergeArrays
+        from dace.transformation.interstate import StateFusion, InlineSDFG
 
-        strict_transformations = (StateFusion, RedundantArray, InlineSDFG)
+        strict_transformations = [
+            StateFusion, RedundantArray, MergeArrays, InlineSDFG
+        ]
 
         self.apply_transformations(
             strict_transformations, validate=validate, strict=True)
 
     def apply_transformations(self,
-                              patterns,
-                              validate=True,
-                              strict=False,
-                              states=None):
+                              patterns: Union[Type, List[Type]],
+                              validate: bool = True,
+                              strict: bool = False,
+                              states: Optional[List[Any]] = None,
+                              apply_once: bool = False,
+                              properties: Dict[str, Any] = None):
         """ This function applies transformations as given in the argument
-            patterns. """
+            patterns. Operates in-place.
+            :param patterns: A Transformation class or a list thereof to apply.
+            :param validate: If True, validates after every transformation.
+            :param strict: If True, operates in strict transformation mode.
+            :param states: If not None, specifies a subset of states to
+                           apply transformations on.
+            :param apply_once: If True, applies the first found transformation
+                               and returns. Otherwise, applies until no further
+                               transformations are found.
+            :param properties: Properties to set when applying transformations.
+        """
         # Avoiding import loops
         from dace.transformation import optimizer
+        from dace.transformation.pattern_matching import Transformation
+
+        if isinstance(patterns, type) and issubclass(patterns, Transformation):
+            patterns = [patterns]
 
         # Apply strict state fusions greedily.
         opt = optimizer.SDFGOptimizer(self, inplace=True)
         applied = True
         applied_transformations = collections.defaultdict(int)
         while applied:
             applied = False
             # Find and apply immediately
             for match in opt.get_pattern_matches(
                     strict=strict, patterns=patterns, states=states):
                 sdfg = self.sdfg_list[match.sdfg_id]
+                if properties is not None:
+                    for prop_name, prop_val in properties.items():
+                        setattr(match, prop_name, prop_val)
                 match.apply(sdfg)
                 applied_transformations[type(match).__name__] += 1
                 if validate:
                     self.fill_scope_connectors()
                     self.validate()
                 applied = True
                 break
+            if apply_once and applied:
+                break
 
-        if Config.get_bool('debugprint'):
+        if Config.get_bool('debugprint') and len(applied_transformations) > 0:
             print('Applied {}.'.format(', '.join([
                 '%d %s' % (v, k) for k, v in applied_transformations.items()
             ])))
 
     def apply_gpu_transformations(self,
                                   states=None,
                                   validate=True,
@@ -1808,18 +1917,18 @@
 
         patterns = [GPUTransformLocalStorage]
         self.apply_transformations(
             patterns, validate=validate, strict=strict, states=states)
 
     def generate_code(self, specialize=None):
         """ Generates code from this SDFG and returns it.
-            @param specialize: If True, specializes all set symbols to their
+            :param specialize: If True, specializes all set symbols to their
                                values in the generated code. If None,
                                uses default configuration value.
-            @return: A list of `CodeObject` objects containing the generated
+            :return: A list of `CodeObject` objects containing the generated
                       code of different files and languages.
         """
 
         # Import loop "fix"
         from dace.codegen import codegen
 
         ################################
@@ -1850,19 +1959,19 @@
 class MemletTrackingView(object):
     """ A mixin class that enables tracking memlets in directed acyclic multigraphs. """
 
     def memlet_path(self,
                     edge: MultiConnectorEdge) -> List[MultiConnectorEdge]:
         """ Given one edge, returns a list of edges representing a path
             between its source and sink nodes. Used for memlet tracking.
-    
+
             @note: Behavior is undefined when there is more than one path
                    involving this edge.
-            @param edge: An edge within this state.
-            @return: A list of edges from a source node to a destination node.
+            :param edge: An edge within this state.
+            :return: A list of edges from a source node to a destination node.
             """
         result = [edge]
 
         # Obtain the full state (to work with paths that trace beyond a scope)
         state = self._graph
 
         # If empty memlet, return itself as the path
@@ -1902,81 +2011,104 @@
                     e for e in state.out_edges(curedge.dst)
                     if e.src_conn == "OUT_" + curedge.dst_conn[3:])
                 result.append(next_edge)
                 curedge = next_edge
 
         return result
 
-    def memlet_tree(self,
-                    edge: MultiConnectorEdge) -> List[MultiConnectorEdge]:
-        """ Given one edge, returns a list of edges representing a tree
-            between its node source(s) and sink(s). Used for memlet tracking.
-    
-            @param edge: An edge within this state.
-            @return: A list of edges from source nodes to destination nodes
-                     (in arbitrary order) that pass through the given edge.
+    def memlet_tree(self, edge: MultiConnectorEdge) -> mm.MemletTree:
+        """ Given one edge, returns a tree of edges between its node source(s)
+            and sink(s). Used for memlet tracking.
+
+            :param edge: An edge within this state.
+            :return: A tree of edges whose root is the source/sink node
+                     (depending on direction) and associated children edges.
             """
-        result = {}
+        propagate_forward = False
+        propagate_backward = False
+        if ((isinstance(edge.src, nd.EntryNode) and edge.src_conn is not None)
+                or
+            (isinstance(edge.dst, nd.EntryNode) and edge.dst_conn is not None
+             and edge.dst_conn.startswith('IN_'))):
+            propagate_forward = True
+        if ((isinstance(edge.src, nd.ExitNode) and edge.src_conn is not None)
+                or
+            (isinstance(edge.dst, nd.ExitNode) and edge.dst_conn is not None)):
+            propagate_backward = True
+
+        # If either both are False (no scopes involved) or both are True
+        # (invalid SDFG), we return only the current edge as a degenerate tree
+        if propagate_forward == propagate_backward:
+            return mm.MemletTree(edge)
 
         # Obtain the full state (to work with paths that trace beyond a scope)
         state = self._graph
 
-        # If empty memlet, return itself as the path
-        if edge.src_conn is None and edge.dst_conn is None and edge.data.data is None:
-            return [edge]
+        # Find tree root
+        curedge = edge
+        if propagate_forward:
+            while (isinstance(curedge.src, nd.EntryNode)
+                   and curedge.src_conn is not None):
+                assert curedge.src_conn.startswith('OUT_')
+                cname = curedge.src_conn[4:]
+                curedge = next(
+                    e for e in state.in_edges(curedge.src)
+                    if e.dst_conn == 'IN_%s' % cname)
+        elif propagate_backward:
+            while (isinstance(curedge.dst, nd.ExitNode)
+                   and curedge.dst_conn is not None):
+                assert curedge.dst_conn.startswith('IN_')
+                cname = curedge.dst_conn[3:]
+                curedge = next(
+                    e for e in state.out_edges(curedge.dst)
+                    if e.src_conn == 'OUT_%s' % cname)
+        tree_root = mm.MemletTree(curedge)
 
-        # Obtain original path
-        path = self.memlet_path(edge)
-        result.update({state.edge_id(e): e for e in path})
+        # Collect children (recursively)
+        def add_children(treenode):
+            if propagate_forward:
+                if not (isinstance(treenode.edge.dst, nd.EntryNode)
+                        and treenode.edge.dst_conn
+                        and treenode.edge.dst_conn.startswith('IN_')):
+                    return
+                conn = treenode.edge.dst_conn[3:]
+                treenode.children = [
+                    mm.MemletTree(e, parent=treenode)
+                    for e in state.out_edges(treenode.edge.dst)
+                    if e.src_conn == 'OUT_%s' % conn
+                ]
+            elif propagate_backward:
+                if (not isinstance(treenode.edge.src, nd.ExitNode)
+                        or treenode.edge.src_conn is None):
+                    return
+                conn = treenode.edge.src_conn[4:]
+                treenode.children = [
+                    mm.MemletTree(e, parent=treenode)
+                    for e in state.in_edges(treenode.edge.src)
+                    if e.dst_conn == 'IN_%s' % conn
+                ]
 
-        num = len(path)
+            for child in treenode.children:
+                add_children(child)
 
-        # Add edges from branching memlet paths
-        for i, curedge in enumerate(path):
-            # Trace through scopes using OUT_# -> IN_#
-            if i > 0 and isinstance(curedge.src, (nd.EntryNode, nd.ExitNode)):
-                if curedge.src_conn is None:
-                    raise ValueError(
-                        "Source connector cannot be None for {}".format(
-                            curedge.src))
-                assert curedge.src_conn.startswith("OUT_")
+        # Start from root node (obtained from above parent traversal)
+        add_children(tree_root)
 
-                # Check for neighboring edges
-                for e in state.out_edges(curedge.src):
-                    if e == curedge:
-                        continue
-                    if e.src_conn == curedge.src_conn:
-                        extra_path = self.memlet_path(e)
-                        result.update(
-                            {state.edge_id(ee): ee
-                             for ee in extra_path})
-
-            # Trace through scopes using IN_# -> OUT_#
-            if i < num - 1 and isinstance(curedge.dst,
-                                          (nd.EntryNode, nd.ExitNode)):
-                if curedge.dst_conn is None:
-                    raise ValueError(
-                        "Destination connector cannot be None for {}".format(
-                            curedge.dst))
-
-                # Map variables are last edges in memlet paths, so this can only
-                # be an edge that enters/exits the scope
-                assert curedge.dst_conn.startswith("IN_")
-
-                # Check for neighboring edges
-                for e in state.in_edges(curedge.dst):
-                    if e == curedge:
-                        continue
-                    if e.dst_conn == curedge.dst_conn:
-                        extra_path = self.memlet_path(e)
-                        result.update(
-                            {state.edge_id(ee): ee
-                             for ee in extra_path})
+        # Find edge in tree
+        def traverse(node):
+            if node.edge == edge:
+                return node
+            for child in node.children:
+                res = traverse(child)
+                if res is not None:
+                    return res
+            return None
 
-        return list(result.values())
+        # Return node that corresponds to current edge
+        return traverse(tree_root)
 
 
 class ScopeSubgraphView(SubgraphView, MemletTrackingView):
     """ An extension to SubgraphView that enables the creation of scope
         dictionaries in subgraphs and free symbols. """
 
     def __init__(self, graph, subgraph_nodes):
@@ -1991,44 +2123,50 @@
         """ Clears the cached results for the scope_dict function.
 
             For use when the graph mutates (e.g., new edges/nodes, deletions).
         """
         self._scope_dict_toparent_cached = None
         self._scope_dict_tochildren_cached = None
 
-    def scope_dict(self, node_to_children=False, return_ids=False):
+    def scope_dict(self,
+                   node_to_children=False,
+                   return_ids=False,
+                   validate=True):
         """ Returns a dictionary that segments an SDFG state into
             entry-node/exit-node scopes.
 
-            @param node_to_children: If False (default), returns a mapping
+            :param node_to_children: If False (default), returns a mapping
                                      of each node to its parent scope
                                      (ScopeEntry) node. If True, returns a
                                      mapping of each parent node to a list of
                                      children nodes.
-            @type node_to_children: bool
-            @param return_ids: Return node ID numbers instead of node objects.
-            @type return_ids: bool
-            @return: The mapping from a node to its parent scope node, or the
+            :type node_to_children: bool
+            :param return_ids: Return node ID numbers instead of node objects.
+            :type return_ids: bool
+            :param validate: Ensure that the graph is not malformed when
+                 computing dictionary.
+            :return: The mapping from a node to its parent scope node, or the
                      mapping from a node to a list of children nodes.
-            @rtype: dict(Node, Node) or dict(Node, list(Node))
+            :rtype: dict(Node, Node) or dict(Node, list(Node))
         """
         result = None
         if not node_to_children and self._scope_dict_toparent_cached is not None:
             result = copy.copy(self._scope_dict_toparent_cached)
         elif node_to_children and self._scope_dict_tochildren_cached is not None:
             result = copy.copy(self._scope_dict_tochildren_cached)
 
         if result is None:
             result = {}
             node_queue = collections.deque(self.source_nodes())
             eq = _scope_dict_inner(self, node_queue, None, node_to_children,
                                    result)
 
             # Sanity check
-            assert len(eq) == 0
+            if validate:
+                assert len(eq) == 0
 
             # Cache result
             if node_to_children:
                 self._scope_dict_tochildren_cached = result
             else:
                 self._scope_dict_toparent_cached = result
 
@@ -2090,14 +2228,21 @@
         all_nodes = []
         for node in self.nodes():
             all_nodes.append((node, self))
             if isinstance(node, dace.graph.nodes.NestedSDFG):
                 all_nodes += node.sdfg.all_nodes_recursive()
         return all_nodes
 
+    def all_edges_recursive(self):
+        all_edges = [(e, self) for e in self.edges()]
+        for node in self.nodes():
+            if isinstance(node, dace.graph.nodes.NestedSDFG):
+                all_edges += node.sdfg.all_edges_recursive()
+        return all_edges
+
 
 # TODO: Use mixin for SDFGState and ScopeSubgraphView for scope dict
 @make_properties
 class SDFGState(OrderedMultiDiConnectorGraph, MemletTrackingView):
     """ An acyclic dataflow multigraph in an SDFG, corresponding to a
         single state in the SDFG state machine. """
 
@@ -2108,23 +2253,23 @@
 
     nosync = Property(
         dtype=bool,
         default=False,
         desc="Do not synchronize at the end of the state")
 
     instrument = Property(
-        enum=dtypes.InstrumentationType,
+        choices=dtypes.InstrumentationType,
         desc="Measure execution statistics with given method",
         default=dtypes.InstrumentationType.No_Instrumentation)
 
     def __init__(self, label=None, sdfg=None, debuginfo=None):
         """ Constructs an SDFG state.
-            @param label: Name for the state (optional).
-            @param sdfg: A reference to the parent SDFG.
-            @param debuginfo: Source code locator for debugging.
+            :param label: Name for the state (optional).
+            :param sdfg: A reference to the parent SDFG.
+            :param debuginfo: Source code locator for debugging.
         """
         super(SDFGState, self).__init__()
         self._label = label
         self._parent = sdfg
         self._graph = self  # Allowing MemletTrackingView mixin to work
         self._clear_scopedict_cache()
         self._debuginfo = debuginfo
@@ -2180,16 +2325,16 @@
 
     def set_label(self, label):
         self._label = label
 
     def replace(self, name: str, new_name: str):
         """ Finds and replaces all occurrences of a symbol or array in this
             state.
-            @param name: Name to find.
-            @param new_name: Name to replace.
+            :param name: Name to find.
+            :param new_name: Name to replace.
         """
         replace(self, name, new_name)
 
     def add_node(self, node):
         if not isinstance(node, nd.Node):
             raise TypeError("Expected Node, got " + str(type(node)) + " (" +
                             str(node) + ")")
@@ -2221,26 +2366,36 @@
         return super(SDFGState, self).add_edge(u, u_connector, v, v_connector,
                                                memlet)
 
     def remove_edge(self, edge):
         self._clear_scopedict_cache()
         super(SDFGState, self).remove_edge(edge)
 
+    def remove_edge_and_connectors(self, edge):
+        self._clear_scopedict_cache()
+        super(SDFGState, self).remove_edge(edge)
+        if edge.src_conn in edge.src.out_connectors:
+            edge.src._out_connectors.remove(edge.src_conn)
+        if edge.dst_conn in edge.dst.in_connectors:
+            edge.dst._in_connectors.remove(edge.dst_conn)
+
     def all_nodes_recursive(self):
         all_nodes = []
         for node in self.nodes():
             all_nodes.append((node, self))
             if isinstance(node, dace.graph.nodes.NestedSDFG):
                 all_nodes += node.sdfg.all_nodes_recursive()
         return all_nodes
 
-    def defined_symbols_at(self, sdfg, node):
-        """ Returns all symbols available to a given node, including map and
-           state transition variables. """
-        return sdfg.defined_symbols_at(node, state=self)
+    def all_edges_recursive(self):
+        all_edges = [(e, self) for e in self.edges()]
+        for node in self.nodes():
+            if isinstance(node, dace.graph.nodes.NestedSDFG):
+                all_edges += node.sdfg.all_edges_recursive()
+        return all_edges
 
     def data_symbols(self):
         """ Returns all symbols used in data nodes. """
         return data_symbols(self)
 
     def scope_symbols(self):
         """ Returns all symbols defined by scopes within this state. """
@@ -2260,83 +2415,77 @@
 
     def memlets_for_array(self, arrayname):
         return [e for e in self.edges() if e[3].data == arrayname]
 
     def draw_node(self, graph):
         return dot.draw_node(graph, self, shape="Msquare")
 
-    def toJSON(self, parent=None):
-        import json
+    def to_json(self, parent=None):
         ret = {
             'type':
             type(self).__name__,
             'label':
             self.name,
             'id':
             parent.node_id(self) if parent is not None else None,
             'collapsed':
             self.is_collapsed,
             'scope_dict': {
                 k: sorted(v)
-                for k, v in self.scope_dict(
-                    node_to_children=True, return_ids=True).items()
+                for k, v in sorted(
+                    self.scope_dict(node_to_children=True, return_ids=True)
+                    .items())
             },
-            'nodes': [json.loads(n.toJSON(self)) for n in self.nodes()],
+            'nodes': [n.to_json(self) for n in self.nodes()],
             'edges': [
-                json.loads(e.toJSON(self)) for e in sorted(
+                e.to_json(self) for e in sorted(
                     self.edges(),
                     key=lambda e: (e.src_conn or '', e.dst_conn or ''))
             ],
             'attributes':
-            json.loads(Property.all_properties_to_json(self)),
+            dace.serialize.all_properties_to_json(self),
         }
 
-        return json.dumps(ret)
+        return ret
 
     @classmethod
-    def fromJSON_object(cls, json_obj, context_info={'sdfg': None}):
+    def from_json(cls, json_obj, context={'sdfg': None}):
         """ Loads the node properties, label and type into a dict.
-            @param json_obj: The object containing information about this node.
+            :param json_obj: The object containing information about this node.
                              NOTE: This may not be a string!
-            @return: An SDFGState instance constructed from the passed data
+            :return: An SDFGState instance constructed from the passed data
         """
 
         _type = json_obj['type']
         if _type != cls.__name__:
             raise Exception("Class type mismatch")
 
         attrs = json_obj['attributes']
         nodes = json_obj['nodes']
         edges = json_obj['edges']
 
         ret = SDFGState(
-            label=json_obj['label'], sdfg=context_info['sdfg'], debuginfo=None)
+            label=json_obj['label'], sdfg=context['sdfg'], debuginfo=None)
 
         rec_ci = {
-            'sdfg':
-            context_info['sdfg'],
-            'sdfg_state':
-            ret,
-            'callback':
-            context_info['callback'] if 'callback' in context_info else None
+            'sdfg': context['sdfg'],
+            'sdfg_state': ret,
+            'callback': context['callback'] if 'callback' in context else None
         }
-        Property.set_properties_from_json(ret, json_obj, rec_ci)
+        dace.serialize.set_properties_from_json(ret, json_obj, rec_ci)
 
-        import json
         for n in nodes:
-            nret = json.loads(
-                json.dumps(n),
-                object_hook=lambda x: Property.json_loader(x, rec_ci))
+            nret = dace.serialize.loads(
+                dace.serialize.dumps(n), context=rec_ci)
             ret.add_node(nret)
 
         # Connect using the edges
         for e in edges:
-            eret = json.loads(
-                json.dumps(e),
-                object_hook=lambda x: Property.json_loader(x, rec_ci))
+            eret = dace.serialize.loads(
+                dace.serialize.dumps(e), context=rec_ci)
 
             ret.add_edge(eret.src, eret.src_conn, eret.dst, eret.dst_conn,
                          eret.data)
 
         # Fix potentially broken scopes
         for n in nodes:
             if isinstance(n, dace.graph.nodes.MapExit):
@@ -2401,44 +2550,49 @@
             return copy.copy(self._scope_leaves_cached)
         st = self.scope_tree()
         self._scope_leaves_cached = [
             scope for scope in st.values() if len(scope.children) == 0
         ]
         return copy.copy(self._scope_leaves_cached)
 
-    def scope_dict(self, node_to_children=False, return_ids=False):
+    def scope_dict(self,
+                   node_to_children=False,
+                   return_ids=False,
+                   validate=True):
         """ Returns a dictionary that segments an SDFG state into
             entry-node/exit-node scopes.
 
-            @param node_to_children: If False (default), returns a mapping
+            :param node_to_children: If False (default), returns a mapping
                                      of each node to its parent scope
                                      (ScopeEntry) node. If True, returns a
                                      mapping of each parent node to a list of
                                      children nodes.
-            @type node_to_children: bool
-            @param return_ids: Return node ID numbers instead of node objects.
-            @type return_ids: bool
-            @return: The mapping from a node to its parent scope node, or the
+            :type node_to_children: bool
+            :param return_ids: Return node ID numbers instead of node objects.
+            :type return_ids: bool
+            :param validate: Ensure that the graph is not malformed when
+                             computing dictionary.
+            :return: The mapping from a node to its parent scope node, or the
                      mapping from a node to a list of children nodes.
-            @rtype: dict(Node, Node) or dict(Node, list(Node))
+            :rtype: dict(Node, Node) or dict(Node, list(Node))
         """
         result = None
         if not node_to_children and self._scope_dict_toparent_cached is not None:
             result = copy.copy(self._scope_dict_toparent_cached)
         elif node_to_children and self._scope_dict_tochildren_cached is not None:
             result = copy.copy(self._scope_dict_tochildren_cached)
 
         if result is None:
             result = {}
             node_queue = collections.deque(self.source_nodes())
             eq = _scope_dict_inner(self, node_queue, None, node_to_children,
                                    result)
 
             # Sanity check
-            if len(eq) != 0:
+            if validate and len(eq) != 0:
                 raise RuntimeError("Leftover nodes in queue: {}".format(eq))
 
             # Cache result
             if node_to_children:
                 self._scope_dict_tochildren_cached = result
             else:
                 self._scope_dict_toparent_cached = result
@@ -2482,44 +2636,44 @@
         ]
 
     # Dynamic SDFG creation API
     ##############################
     def add_read(self, array_or_stream_name: str,
                  debuginfo=None) -> nd.AccessNode:
         """ Adds a read-only access node to this SDFG state.
-            @param array_or_stream_name: The name of the array/stream.
-            @return: An array access node.
+            :param array_or_stream_name: The name of the array/stream.
+            :return: An array access node.
         """
         debuginfo = getdebuginfo(debuginfo)
         node = nd.AccessNode(
             array_or_stream_name,
             dtypes.AccessType.ReadOnly,
             debuginfo=debuginfo)
         self.add_node(node)
         return node
 
     def add_write(self, array_or_stream_name: str,
                   debuginfo=None) -> nd.AccessNode:
         """ Adds a write-only access node to this SDFG state.
-            @param array_or_stream_name: The name of the array/stream.
-            @return: An array access node.
+            :param array_or_stream_name: The name of the array/stream.
+            :return: An array access node.
         """
         debuginfo = getdebuginfo(debuginfo)
         node = nd.AccessNode(
             array_or_stream_name,
             dtypes.AccessType.WriteOnly,
             debuginfo=debuginfo)
         self.add_node(node)
         return node
 
     def add_access(self, array_or_stream_name: str,
                    debuginfo=None) -> nd.AccessNode:
         """ Adds a general (read/write) access node to this SDFG state.
-            @param array_or_stream_name: The name of the array/stream.
-            @return: An array access node.
+            :param array_or_stream_name: The name of the array/stream.
+            :return: An array access node.
         """
         debuginfo = getdebuginfo(debuginfo)
         node = nd.AccessNode(
             array_or_stream_name,
             dtypes.AccessType.ReadWrite,
             debuginfo=debuginfo)
         self.add_node(node)
@@ -2567,19 +2721,17 @@
             debuginfo=None,
     ):
         """ Adds a nested SDFG to the SDFG state. """
         if name is None:
             name = sdfg.label
         debuginfo = getdebuginfo(debuginfo)
 
-        if sdfg.parent is not None and sdfg.parent != parent:
-            raise ValueError('SDFG "{}" already has a parent'.format(
-                sdfg.label))
         sdfg.parent = self
-        sdfg._parent_sdfg = parent
+        sdfg._parent_sdfg = self.parent
+
         sdfg.update_sdfg_list([])
 
         s = nd.NestedSDFG(
             name,
             sdfg,
             inputs,
             outputs,
@@ -2612,23 +2764,23 @@
     def add_map(
             self,
             name,
             ndrange: Dict[str, str],
             schedule=dtypes.ScheduleType.Default,
             unroll=False,
             debuginfo=None,
-    ) -> Tuple[nd.Node]:
+    ) -> Tuple[nd.MapEntry, nd.MapExit]:
         """ Adds a map entry and map exit.
-            @param name:      Map label
-            @param ndrange:   Mapping between range variable names and their
+            :param name:      Map label
+            :param ndrange:   Mapping between range variable names and their
                               subsets (parsed from strings)
-            @param schedule:  Map schedule type
-            @param unroll:    True if should unroll the map in code generation
+            :param schedule:  Map schedule type
+            :param unroll:    True if should unroll the map in code generation
 
-            @return: (map_entry, map_exit) node 2-tuple
+            :return: (map_entry, map_exit) node 2-tuple
         """
         debuginfo = getdebuginfo(debuginfo)
         map = self._map_from_ndrange(
             name, schedule, unroll, ndrange, debuginfo=debuginfo)
         map_entry = nd.MapEntry(map)
         map_exit = nd.MapExit(map)
         self.add_nodes_from([map_entry, map_exit])
@@ -2638,27 +2790,27 @@
             self,
             name,
             elements: Tuple[str, str],
             condition: str = None,
             schedule=dtypes.ScheduleType.Default,
             chunksize=1,
             debuginfo=None,
-    ) -> Tuple[nd.Node]:
+    ) -> Tuple[nd.ConsumeEntry, nd.ConsumeExit]:
         """ Adds consume entry and consume exit nodes.
-            @param name:      Label
-            @param elements:  A 2-tuple signifying the processing element
+            :param name:      Label
+            :param elements:  A 2-tuple signifying the processing element
                               index and number of total processing elements
-            @param condition: Quiescence condition to finish consuming, or
+            :param condition: Quiescence condition to finish consuming, or
                               None (by default) to consume until the stream
                               is empty for the first time. If false, will
                               consume forever.
-            @param schedule:  Consume schedule type
-            @param chunksize: Maximal number of elements to consume at a time
+            :param schedule:  Consume schedule type
+            :param chunksize: Maximal number of elements to consume at a time
 
-            @return: (consume_entry, consume_exit) node 2-tuple
+            :return: (consume_entry, consume_exit) node 2-tuple
         """
         if len(elements) != 2:
             raise TypeError("Elements must be a 2-tuple of "
                             "(PE_index, num_PEs)")
         pe_tuple = (elements[0],
                     properties.SymbolicProperty.from_string(elements[1]))
 
@@ -2688,36 +2840,36 @@
             code_global="",
             code_init="",
             code_exit="",
             location="-1",
             language=dtypes.Language.Python,
             debuginfo=None,
             external_edges=False,
-    ) -> Tuple[nd.Node]:
+    ) -> Tuple[nd.Tasklet, nd.MapEntry, nd.MapExit]:
         """ Convenience function that adds a map entry, tasklet, map exit,
             and the respective edges to external arrays.
-            @param name:       Tasklet (and wrapping map) name
-            @param map_ranges: Mapping between variable names and their
+            :param name:       Tasklet (and wrapping map) name
+            :param map_ranges: Mapping between variable names and their
                                subsets
-            @param inputs:     Mapping between input local variable names and
+            :param inputs:     Mapping between input local variable names and
                                their memlets
-            @param code:       Code (written in `language`)
-            @param outputs:    Mapping between output local variable names and
+            :param code:       Code (written in `language`)
+            :param outputs:    Mapping between output local variable names and
                                their memlets
-            @param schedule:   Map schedule
-            @param unroll_map: True if map should be unrolled in code
+            :param schedule:   Map schedule
+            :param unroll_map: True if map should be unrolled in code
                                generation
-            @param code_global: (optional) Global code (outside functions)
-            @param language:   Programming language in which the code is
+            :param code_global: (optional) Global code (outside functions)
+            :param language:   Programming language in which the code is
                                written
-            @param debuginfo:  Debugging information (mostly for DIODE)
-            @param external_edges: Create external access nodes and connect
+            :param debuginfo:  Debugging information (mostly for DIODE)
+            :param external_edges: Create external access nodes and connect
                                    them with memlets automatically
 
-            @return: tuple of (tasklet, map_entry, map_exit)
+            :return: tuple of (tasklet, map_entry, map_exit)
         """
         map_name = name + "_map"
         debuginfo = getdebuginfo(debuginfo)
         tasklet = nd.Tasklet(
             name,
             set(inputs.keys()),
             set(outputs.keys()),
@@ -2813,22 +2965,22 @@
             wcr,
             axes,
             wcr_identity=None,
             schedule=dtypes.ScheduleType.Default,
             debuginfo=None,
     ):
         """ Adds a reduction node.
-            @param wcr: A lambda function representing the reduction operation
-            @param axes: A tuple of axes to reduce the input memlet from, or
+            :param wcr: A lambda function representing the reduction operation
+            :param axes: A tuple of axes to reduce the input memlet from, or
                          None for all axes
-            @param wcr_identity: If not None, initializes output memlet values
+            :param wcr_identity: If not None, initializes output memlet values
                                  with this value
-            @param schedule: Reduction schedule type
+            :param schedule: Reduction schedule type
 
-            @return: A Reduce node
+            :return: A Reduce node
         """
         debuginfo = getdebuginfo(debuginfo)
         result = nd.Reduce(
             wcr, axes, wcr_identity, schedule, debuginfo=debuginfo)
         self.add_node(result)
         return result
 
@@ -2847,33 +2999,33 @@
             exit).
 
             The internal memlet (connecting to the internal node) has to be
             specified. If external_memlet (i.e., connecting to the node out
             of the scope) is not specified, it is propagated automatically
             using internal_memlet and the scope.
 
-            @param scope_node: A scope node (for example, map exit) to add
+            :param scope_node: A scope node (for example, map exit) to add
                                edges around.
-            @param internal_node: The node within the scope to connect to. If
+            :param internal_node: The node within the scope to connect to. If
                                   `scope_node` is an entry node, this means
                                   the node connected to the outgoing edge,
                                   else incoming.
-            @param external_node: The node out of the scope to connect to.
-            @param internal_memlet: The memlet on the edge to/from
+            :param external_node: The node out of the scope to connect to.
+            :param internal_memlet: The memlet on the edge to/from
                                     internal_node.
-            @param external_memlet: The memlet on the edge to/from
+            :param external_memlet: The memlet on the edge to/from
                                     external_node (optional, will propagate
                                     internal_memlet if not specified).
-            @param scope_connector: A scope connector name (or a unique
+            :param scope_connector: A scope connector name (or a unique
                                     number if not specified).
-            @param internal_connector: The connector on internal_node to
+            :param internal_connector: The connector on internal_node to
                                        connect to.
-            @param external_connector: The connector on external_node to
+            :param external_connector: The connector on external_node to
                                        connect to.
-            @return: A 2-tuple representing the (internal, external) edges.
+            :return: A 2-tuple representing the (internal, external) edges.
         """
         if not isinstance(scope_node, (nd.EntryNode, nd.ExitNode)):
             raise ValueError("scope_node is not a scope entry/exit")
 
         # Autodetermine scope connector ID
         if scope_connector is None:
             # Pick out numbered connectors that do not lead into the scope range
@@ -2941,22 +3093,22 @@
                         *path_nodes,
                         memlet=None,
                         src_conn=None,
                         dst_conn=None):
         """ Adds a path of memlet edges between the given nodes, propagating
             from the given innermost memlet.
 
-            @param *path_nodes: Nodes participating in the path (in the given
+            :param *path_nodes: Nodes participating in the path (in the given
                                 order).
-            @keyword memlet: (mandatory) The memlet at the innermost scope
+            :keyword memlet: (mandatory) The memlet at the innermost scope
                              (e.g., the incoming memlet to a tasklet (last
                              node), or an outgoing memlet from an array
                              (first node), followed by scope exits).
-            @keyword src_conn: Connector at the beginning of the path.
-            @keyword dst_conn: Connector at the end of the path.
+            :keyword src_conn: Connector at the beginning of the path.
+            :keyword dst_conn: Connector at the end of the path.
         """
         if memlet is None:
             raise TypeError("Innermost memlet cannot be None")
         if len(path_nodes) < 2:
             raise ValueError("Memlet path must consist of at least 2 nodes")
 
         src_node = path_nodes[0]
@@ -2969,23 +3121,24 @@
             for i in range(len(path_nodes) - 1)
         ]
 
         if not isinstance(memlet, dace.memlet.Memlet):
             raise TypeError("Expected Memlet, got: {}".format(
                 type(memlet).__name__))
 
-        if scope_contains_scope(self.scope_dict(), src_node, dst_node):
+        sdict = self.scope_dict(validate=False)
+        if scope_contains_scope(sdict, src_node, dst_node):
             propagate_forward = False
         else:  # dst node's scope is higher than src node, propagate out
             propagate_forward = True
 
         # Innermost edge memlet
         cur_memlet = memlet
 
-        # Verify that connectors exists
+        # Verify that connectors exist
         if (not isinstance(memlet, dace.memlet.EmptyMemlet)
                 and hasattr(edges[0].src, "out_connectors")
                 and isinstance(edges[0].src, nd.CodeNode) and
             (src_conn is None or src_conn not in edges[0].src.out_connectors)):
             raise ValueError("Output connector {} does not exist in {}".format(
                 src_conn, edges[0].src.label))
         if (not isinstance(memlet, dace.memlet.EmptyMemlet)
@@ -3006,24 +3159,21 @@
                          ("IN_" + edge.dst.next_connector()))
             else:
                 sconn = (src_conn if i == len(edges) - 1 else
                          ("OUT_" + edge.src.next_connector()))
                 dconn = dst_conn if i == 0 else (
                     "IN_" + edge.dst.last_connector())
 
-            # If edge with current data already exists, replace it with
-            # our newly propagated one
-            existing_edges = [
-                e for e in self.edges_between(edge.src, edge.dst)
-                if isinstance(e.src, (nd.EntryNode, nd.ExitNode))
-                and isinstance(e.dst, (nd.EntryNode, nd.ExitNode))
-            ]
-            for e in existing_edges:
-                if e.data.data == cur_memlet.data:
-                    self.remove_edge(e)
+            if isinstance(cur_memlet, dace.memlet.EmptyMemlet):
+                if propagate_forward:
+                    sconn = src_conn if i == 0 else None
+                    dconn = dst_conn if i == len(edges) - 1 else None
+                else:
+                    sconn = src_conn if i == len(edges) - 1 else None
+                    dconn = dst_conn if i == 0 else None
 
             # Modify edge to match memlet path
             edge._src_conn = sconn
             edge._dst_conn = dconn
             edge._data = cur_memlet
 
             # Add connectors to edges
@@ -3037,31 +3187,33 @@
                     edge.dst.add_in_connector(dconn)
                 if sconn is not None:
                     edge.src.add_out_connector(sconn)
 
             # Propagate current memlet to produce the next one
             if i < len(edges) - 1:
                 snode = edge.dst if propagate_forward else edge.src
-                cur_memlet = propagate_memlet(self, cur_memlet, snode, True)
+                if not isinstance(cur_memlet, dace.memlet.EmptyMemlet):
+                    cur_memlet = propagate_memlet(self, cur_memlet, snode,
+                                                  True)
 
     # DEPRECATED FUNCTIONS
     ######################################
-    def add_array(
-            self,
-            name,
-            shape,
-            dtype,
-            storage=dtypes.StorageType.Default,
-            materialize_func=None,
-            transient=False,
-            strides=None,
-            offset=None,
-            toplevel=False,
-            debuginfo=None,
-    ):
+    def add_array(self,
+                  name,
+                  shape,
+                  dtype,
+                  storage=dtypes.StorageType.Default,
+                  materialize_func=None,
+                  transient=False,
+                  strides=None,
+                  offset=None,
+                  toplevel=False,
+                  debuginfo=None,
+                  total_size=None,
+                  find_new_name=False):
         """ @attention: This function is deprecated. """
         warnings.warn(
             'The "SDFGState.add_array" API is deprecated, please '
             'use "SDFG.add_array" and "SDFGState.add_access"',
             DeprecationWarning)
         # Workaround to allow this legacy API
         if name in self.parent._arrays:
@@ -3073,27 +3225,27 @@
             storage,
             materialize_func,
             transient,
             strides,
             offset,
             toplevel,
             debuginfo,
-        )
+            find_new_name=find_new_name,
+            total_size=total_size)
         return self.add_access(name, debuginfo)
 
     def add_stream(
             self,
             name,
             dtype,
             veclen=1,
             buffer_size=1,
             shape=(1, ),
             storage=dtypes.StorageType.Default,
             transient=False,
-            strides=None,
             offset=None,
             toplevel=False,
             debuginfo=None,
     ):
         """ @attention: This function is deprecated. """
         warnings.warn(
             'The "SDFGState.add_stream" API is deprecated, please '
@@ -3106,15 +3258,14 @@
             name,
             dtype,
             veclen,
             buffer_size,
             shape,
             storage,
             transient,
-            strides,
             offset,
             toplevel,
             debuginfo,
         )
         return self.add_access(name, debuginfo)
 
     def add_scalar(
@@ -3134,48 +3285,47 @@
         # Workaround to allow this legacy API
         if name in self.parent._arrays:
             del self.parent._arrays[name]
         self.parent.add_scalar(name, dtype, storage, transient, toplevel,
                                debuginfo)
         return self.add_access(name, debuginfo)
 
-    def add_transient(
-            self,
-            name,
-            shape,
-            dtype,
-            storage=dtypes.StorageType.Default,
-            materialize_func=None,
-            strides=None,
-            offset=None,
-            toplevel=False,
-            debuginfo=None,
-    ):
+    def add_transient(self,
+                      name,
+                      shape,
+                      dtype,
+                      storage=dtypes.StorageType.Default,
+                      materialize_func=None,
+                      strides=None,
+                      offset=None,
+                      toplevel=False,
+                      debuginfo=None,
+                      total_size=None):
         """ @attention: This function is deprecated. """
         return self.add_array(
             name,
             shape,
             dtype,
             storage,
             materialize_func,
             True,
             strides,
             offset,
             toplevel,
             debuginfo,
-        )
+            total_size=total_size)
 
     # SDFG queries
     ######################################
     def find_node(self, node_id_or_label):
         """ Finds a node according to its ID (if integer is
             provided) or label (if string is provided).
 
-            @param node_id_or_label  Node ID (if int) or label (if str)
-            @return A nodes.Node object
+            :param node_id_or_label  Node ID (if int) or label (if str)
+            :return A nodes.Node object
         """
 
         if isinstance(node_id_or_label, str):
             for n in self.nodes():
                 if n.label == node_id_or_label:
                     return n
             raise LookupError("Node %s not found" % node_id_or_label)
@@ -3207,15 +3357,15 @@
                 # Append input connectors and get mapping of connectors to data
                 for edge in self.in_edges(node):
                     if edge.dst_conn is not None and edge.dst_conn.startswith(
                             "IN_"):
                         conn_to_data[edge.data.data] = edge.dst_conn[3:]
 
                     # We're only interested in edges without connectors
-                    if edge.dst_conn is not None:
+                    if edge.dst_conn is not None or edge.data.data is None:
                         continue
                     edge._dst_conn = "IN_" + str(num_inputs + 1)
                     node._in_connectors.add(edge.dst_conn)
                     conn_to_data[edge.data.data] = num_inputs + 1
 
                     num_inputs += 1
 
@@ -3241,15 +3391,15 @@
                 # Append output connectors and get mapping of connectors to data
                 for edge in self.out_edges(node):
                     if edge.src_conn is not None and edge.src_conn.startswith(
                             "OUT_"):
                         conn_to_data[edge.data.data] = edge.src_conn[4:]
 
                     # We're only interested in edges without connectors
-                    if edge.src_conn is not None:
+                    if edge.src_conn is not None or edge.data.data is None:
                         continue
                     edge._src_conn = "OUT_" + str(num_outputs + 1)
                     node._out_connectors.add(edge.src_conn)
                     conn_to_data[edge.data.data] = num_outputs + 1
 
                     num_outputs += 1
 
@@ -3285,14 +3435,16 @@
                 and sdfg.out_degree(self) == 0):
             raise InvalidSDFGError("Unreachable state", sdfg, state_id)
 
         for nid, node in enumerate(self.nodes()):
             # Node validation
             try:
                 node.validate(sdfg, self)
+            except InvalidSDFGError:
+                raise
             except Exception as ex:
                 raise InvalidSDFGNodeError(
                     "Node validation failed: " + str(ex), sdfg, state_id, nid)
 
             # Isolated nodes
             ########################################
             if self.in_degree(node) + self.out_degree(node) == 0:
@@ -3474,14 +3626,16 @@
 
         # Memlet checks
         scope = self.scope_dict()
         for eid, e in enumerate(self.edges()):
             # Edge validation
             try:
                 e.data.validate(sdfg, self)
+            except InvalidSDFGError:
+                raise
             except Exception as ex:
                 raise InvalidSDFGEdgeError(
                     "Edge validation failed: " + str(ex), sdfg, state_id, eid)
 
             # For every memlet, obtain its full path in the DFG
             path = self.memlet_path(e)
             src_node = path[0].src
@@ -3824,48 +3978,68 @@
 
 
 def scope_symbols(dfg):
     """ Returns all symbols used in scopes within the given DFG, separated
         into (iteration variables, symbols used in subsets). """
     iteration_variables = collections.OrderedDict()
     subset_symbols = collections.OrderedDict()
+    sdict = dfg.scope_dict()
     for n in dfg.nodes():
+        # TODO(later): Refactor to method on Node objects
         if isinstance(n, dace.graph.nodes.NestedSDFG):
             iv, ss = n.sdfg.scope_symbols()
             iteration_variables.update(iv)
             subset_symbols.update(ss)
             continue
         if not isinstance(n, dace.graph.nodes.EntryNode):
             continue
         if isinstance(n, dace.graph.nodes.MapEntry):
+            # Collect dynamic map range symbols from parent scopes
+            dynamic_symbols = set()
+            parent = n
+            while parent is not None:
+                dynamic_symbols |= parent.in_connectors
+                parent = sdict[parent]
+
             for param in n.params:
                 iteration_variables[param] = dt.Scalar(
                     symbolic.symbol(param).dtype)
             for dim in n.map.range:
                 try:
                     for i in dim:
                         if isinstance(i, sp.Expr):
-                            subset_symbols.update((k.name, dt.Scalar(k.dtype))
-                                                  for k in i.free_symbols)
+                            subset_symbols.update(
+                                (k.name, dt.Scalar(k.dtype))
+                                for k in i.free_symbols
+                                if k.name not in dynamic_symbols)
                 except TypeError:  # X object is not iterable
                     if isinstance(dim, sp.Expr):
-                        result.update((k.name, dt.Scalar(k.dtype))
-                                      for k in dim.free_symbols)
+                        subset_symbols.update((k.name, dt.Scalar(k.dtype))
+                                              for k in dim.free_symbols
+                                              if k.name not in dynamic_symbols)
                     else:
                         raise TypeError(
                             "Unexpected map range type for {}: {}".format(
                                 n.map,
                                 type(n.map.range).__name__))
         elif isinstance(n, dace.graph.nodes.ConsumeEntry):
+            # Collect dynamic map range symbols from parent scopes
+            dynamic_symbols = set()
+            parent = n
+            while parent is not None:
+                dynamic_symbols |= parent.in_connectors
+                parent = sdict[parent]
+
             # Add PE index as iteration variable
             iteration_variables[n.consume.pe_index] = dt.Scalar(
                 symbolic.symbol(n.consume.pe_index).dtype)
             if isinstance(n.consume.num_pes, sp.Expr):
                 subset_symbols.update((k.name, dt.Scalar(k.dtype))
-                                      for k in n.consume.num_pes.free_symbols)
+                                      for k in n.consume.num_pes.free_symbols
+                                      if k.name not in dynamic_symbols)
         else:
             raise TypeError("Unsupported entry node type: {}".format(
                 type(n).__name__))
     return iteration_variables, subset_symbols
 
 
 def data_symbols(dfg):
@@ -3920,28 +4094,37 @@
     defined |= {
         n.data
         for n, scope in obj.all_nodes_recursive()
         if (isinstance(n, dace.graph.nodes.AccessNode) and (
             scope.parent is None and n.desc(scope).transient or scope.parent))
     }
     symbols = collections.OrderedDict(
-        (key, value) for key, value in symbols.items() if key not in defined)
+        (key, value) for key, value in symbols.items()
+        if key not in defined and not key.startswith('__dace'))
     return symbols
 
 
 def interstate_symbols(dfg):
     """ Returns all symbols used in interstate edges in nested SDFGs within
         this state. """
     assigned = collections.OrderedDict()
     used = collections.OrderedDict()
     for node in dfg.nodes():
         if isinstance(node, dace.graph.nodes.NestedSDFG):
             a, u = node.sdfg.interstate_symbols()
             assigned.update(a)
+
+            # Filter used symbols if they belong to SDFG input/output connectors
+            u = {
+                k: v
+                for k, v in u.items()
+                if k not in (node.in_connectors | node.out_connectors)
+            }
             used.update(u)
+
     return assigned, used
 
 
 def top_level_transients(dfg):
     """ Iterate over top-level transients (i.e., ones that exist in multiple
         states or scopes) of the passed dataflow graph. """
     sdfg = dfg.parent
@@ -3968,62 +4151,63 @@
             continue
         if node.data in visited:
             continue
         visited.add(node.data)
         yield node.data
 
 
+def _transients_in_scope(sdfg, scope, scope_dict):
+    return set(node.data
+               for node in scope_dict[scope.entry if scope else scope]
+               if isinstance(node, nd.AccessNode)
+               and sdfg.arrays[node.data].transient)
+
+
 def local_transients(sdfg, dfg, entry_node):
     """ Returns transients local to the scope defined by the specified entry
         node in the dataflow graph. """
-    scope_dict = dfg.scope_dict(node_to_children=False)
-    shared_transients = set(sdfg.shared_transients())
-    in_scope = set()
-    out_scope = set()
-    for node in dfg.nodes():
-        if not isinstance(node, nd.AccessNode):
-            continue
-        if not node.desc(sdfg).transient:
-            continue
-        if node.data in shared_transients:
-            continue
-        if scope_dict[node] == entry_node:
-            in_scope.add(node.data)
-        else:
-            # Since nodes can appear in multiple places, make sure it's not
-            # present anywhere else by keeping track of transients not in this
-            # scope
-            out_scope.add(node.data)
-    transients = dtypes.deduplicate([
-        n.data for n in dfg.nodes()
-        if isinstance(n, dace.graph.nodes.AccessNode) and n.data in in_scope
-        and n.data not in out_scope
-    ])
-    return transients
+    state: SDFGState = dfg._graph
+    scope_dict = state.scope_dict(node_to_children=True)
+    scope_tree = state.scope_tree()
+    current_scope = scope_tree[entry_node]
 
+    # Start by setting shared transients as defined
+    defined_transients = set(sdfg.shared_transients())
 
-def compile(function_or_sdfg, *args, specialize=None):
+    # Get access nodes in current scope
+    transients = _transients_in_scope(sdfg, current_scope, scope_dict)
+
+    # Add transients defined in parent scopes
+    while current_scope is not None:
+        current_scope = current_scope.parent
+        defined_transients.update(
+            _transients_in_scope(sdfg, current_scope, scope_dict))
+
+    return sorted(list(transients - defined_transients))
+
+
+def compile(function_or_sdfg, *args, **kwargs):
     """ Obtain a runnable binary from a Python (@dace.program) function. """
     if isinstance(function_or_sdfg, dace.frontend.python.parser.DaceProgram):
         sdfg = dace.frontend.python.parser.parse_from_function(
-            function_or_sdfg, *args)
+            function_or_sdfg, *args, **kwargs)
     elif isinstance(function_or_sdfg, SDFG):
         sdfg = function_or_sdfg
     else:
         raise TypeError("Unsupported function type")
-    return sdfg.compile(specialize=specialize)
+    return sdfg.compile(**kwargs)
 
 
 def is_devicelevel(sdfg: SDFG, state: SDFGState, node: dace.graph.nodes.Node):
     """ Tests whether a node in an SDFG is contained within GPU device-level
         code.
-        @param sdfg: The SDFG in which the node resides.
-        @param state: The SDFG state in which the node resides.
-        @param node: The node in question
-        @return: True if node is in device-level code, False otherwise.
+        :param sdfg: The SDFG in which the node resides.
+        :param state: The SDFG state in which the node resides.
+        :param node: The node in question
+        :return: True if node is in device-level code, False otherwise.
     """
     while sdfg is not None:
         sdict = state.scope_dict()
         scope = sdict[node]
         while scope is not None:
             if scope.schedule in dtypes.GPU_SCHEDULES:
                 return True
@@ -4043,17 +4227,17 @@
     return False
 
 
 def replace(subgraph: Union[SDFGState, ScopeSubgraphView, SubgraphView],
             name: str, new_name: str):
     """ Finds and replaces all occurrences of a symbol or array in the given
         subgraph.
-        @param subgraph: The given graph or subgraph to replace in.
-        @param name: Name to find.
-        @param new_name: Name to replace.
+        :param subgraph: The given graph or subgraph to replace in.
+        :param name: Name to find.
+        :param new_name: Name to replace.
     """
     symrepl = {
         symbolic.symbol(name):
         symbolic.symbol(new_name) if isinstance(new_name, str) else new_name
     }
 
     def replsym(symlist):
@@ -4095,50 +4279,67 @@
 
 
 def is_array_stream_view(sdfg: SDFG, dfg: SDFGState, node: nd.AccessNode):
     """ Test whether a stream is directly connected to an array. """
 
     # Test all memlet paths from the array. If the path goes directly
     # to/from a stream, construct a stream array view
+    all_source_paths = []
     source_paths = []
+    all_sink_paths = []
     sink_paths = []
     for e in dfg.in_edges(node):
         src_node = dfg.memlet_path(e)[0].src
         # Append empty path to differentiate between a copy and an array-view
         if isinstance(src_node, nd.CodeNode):
-            source_paths.append(None)
+            all_source_paths.append(None)
         # Append path from source node
         if isinstance(src_node, nd.AccessNode) and isinstance(
                 src_node.desc(sdfg), dt.Array):
             source_paths.append(src_node)
     for e in dfg.out_edges(node):
         sink_node = dfg.memlet_path(e)[-1].dst
 
         # Append empty path to differentiate between a copy and an array-view
         if isinstance(sink_node, nd.CodeNode):
-            sink_paths.append(None)
+            all_sink_paths.append(None)
         # Append path to sink node
         if isinstance(sink_node, nd.AccessNode) and isinstance(
                 sink_node.desc(sdfg), dt.Array):
             sink_paths.append(sink_node)
 
+    all_sink_paths.extend(sink_paths)
+    all_source_paths.extend(source_paths)
+
     # Special case: stream can be represented as a view of an array
-    if ((len(source_paths) > 0 and len(sink_paths) == 1)
-            or (len(sink_paths) > 0 and len(source_paths) == 1)):
+    if ((len(all_source_paths) > 0 and len(sink_paths) == 1)
+            or (len(all_sink_paths) > 0 and len(source_paths) == 1)):
         # TODO: What about a source path?
         arrnode = sink_paths[0]
         # Only works if the stream itself is not an array of streams
         if list(node.desc(sdfg).shape) == [1]:
             node.desc(sdfg).sink = arrnode.data  # For memlet generation
             arrnode.desc(
                 sdfg).src = node.data  # TODO: Move src/sink to node, not array
             return True
     return False
 
 
+def dynamic_map_inputs(state: SDFGState,
+                       map_entry: nd.MapEntry) -> List[MultiConnectorEdge]:
+    return [
+        e for e in state.in_edges(map_entry)
+        if e.dst_conn and not e.dst_conn.startswith('IN_')
+    ]
+
+
+def has_dynamic_map_inputs(state: SDFGState, map_entry: nd.MapEntry) -> bool:
+    return len(dynamic_map_inputs(state, map_entry)) > 0
+
+
 def _get_optimizer_class(class_override):
     """ Imports and returns a class string defined in the configuration
         (under "optimizer.interface") or overridden in the input
         class_override argument. Empty string, False, or failure to find the
         class skips the process.
 
         @note: This method uses pydoc to locate the class.
```

### Comparing `dace-0.9.0/dace/subsets.py` & `dace-0.9.5/dace/subsets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import dace.serialize
 from dace import data, symbolic, dtypes
 import re
 import sympy as sp
 from functools import reduce
 from sympy.core.sympify import SympifyError
 import warnings
 
@@ -39,14 +40,15 @@
 
 
 def _tuple_to_symexpr(val):
     return (symbolic.SymExpr(val[0], val[1])
             if isinstance(val, tuple) else symbolic.pystr_to_symbolic(val))
 
 
+@dace.serialize.serializable
 class Range(Subset):
     """ Subset defined in terms of a fixed range. """
 
     def __init__(self, ranges):
         parsed_ranges = []
         parsed_tiles = []
         for r in ranges:
@@ -58,16 +60,15 @@
             if len(r) == 3:
                 parsed_tiles.append(symbolic.pystr_to_symbolic(1))
             else:
                 parsed_tiles.append(symbolic.pystr_to_symbolic(r[3]))
         self.ranges = parsed_ranges
         self.tile_sizes = parsed_tiles
 
-    def toJSON(self):
-        import json
+    def to_json(self):
         ret = []
 
         def a2s(obj):
             if isinstance(obj, symbolic.SymExpr):
                 return {'main': str(obj.expr), 'approx': str(obj.approx)}
             else:
                 return str(obj)
@@ -77,29 +78,23 @@
             ret.append({
                 'start': a2s(start),
                 'end': a2s(end),
                 'step': a2s(step),
                 'tile': a2s(tile)
             })
 
-        return json.dumps({'type': 'subsets.Range', 'ranges': ret})
+        return {'type': 'Range', 'ranges': ret}
 
     @staticmethod
-    def fromJSON(obj, context=None):
-        import json
-        obj = json.loads(obj)
-
-        return Range.fromJSON_object(obj, context)
-
-    @staticmethod
-    def fromJSON_object(obj, context=None):
-        if obj['type'] != 'subsets.Range':
-            raise TypeError(
-                "fromJSON of class `Range` called on json with type %s (expected 'subsets.Range')"
-                % obj['type'])
+    def from_json(obj, context=None):
+        if not isinstance(obj, dict):
+            raise TypeError("Expected dict, got {}".format(type(obj)))
+        if obj['type'] != 'Range':
+            raise TypeError("from_json of class \"Range\" called on json "
+                            "with type %s (expected 'Range')" % obj['type'])
 
         ranges = obj['ranges']
         tuples = []
 
         def p2s(x):
             pts = symbolic.pystr_to_symbolic
             if isinstance(x, str):
@@ -111,15 +106,15 @@
             tuples.append((p2s(r['start']), p2s(r['end']), p2s(r['step']),
                            p2s(r['tile'])))
 
         return Range(tuples)
 
     @staticmethod
     def from_array(array):
-        """ Constructs a range that covers the full array given as input. 
+        """ Constructs a range that covers the full array given as input.
             @type array: dace.data.Data """
         return Range([(0, s - 1, 1) for s in array.shape])
 
     def __hash__(self):
         return hash(tuple(r for r in self.ranges))
 
     def __add__(self, other):
@@ -173,20 +168,20 @@
         return [_expr(x[1]) for x in self.ranges]
         # return [(sp.floor((iMax - iMin) / step) - 1) * step
         #        for iMin, iMax, step in self.ranges]
 
     def coord_at(self, i):
         """ Returns the offseted coordinates of this subset at
             the given index tuple.
-            
+
             For example, the range [2:10:2] at index 2 would return 6 (2+2*2).
-            
-            @param i: A tuple of the same dimensionality as subset.dims() or
+
+            :param i: A tuple of the same dimensionality as subset.dims() or
                       subset.data_dims().
-            @return: Absolute coordinates for index i (length equal to
+            :return: Absolute coordinates for index i (length equal to
                      `data_dims()`, may be larger than `dims()`).
         """
         tiles = sum(1 if ts != 1 else 0 for ts in self.tile_sizes)
         if len(i) != len(self.ranges) and len(i) != len(self.ranges) + tiles:
             raise ValueError('Invalid dimensionality of input tuple (expected'
                              ' %d, got %d)' % (len(self.ranges), len(i)))
 
@@ -196,34 +191,32 @@
 
         i = i[:len(self.ranges)]
 
         return tuple(
             _expr(rb) + k * _expr(rs)
             for k, (rb, _, rs) in zip(i, self.ranges)) + tuple(ti)
 
-    def at(self, i, global_shape):
+    def at(self, i, strides):
         """ Returns the absolute index (1D memory layout) of this subset at
             the given index tuple.
-            
+
             For example, the range [2:10:2] at index 2 would return 6 (2+2*2).
-            
-            @param i: A tuple of the same dimensionality as subset.dims() or
+
+            :param i: A tuple of the same dimensionality as subset.dims() or
                       subset.data_dims().
-            @param global_shape: The full size of the set that we are 
-                                 subsetting (e.g., full array strides/padded 
-                                 shape).
-            @return: Absolute 1D index at coordinate i.
+            :param strides: The strides of the array we are subsetting.
+            :return: Absolute 1D index at coordinate i.
         """
         coord = self.coord_at(i)
 
         # Return i0 + i1*size0 + i2*size1*size0 + ....
         # Cancel out stride since we determine the initial offset only here
         return sum(
             _expr(s) * _expr(astr) / _expr(rs) for s, (_, _, rs), astr in zip(
-                coord, self.ranges, self.absolute_strides(global_shape)))
+                coord, self.ranges, self.absolute_strides(strides)))
 
     def data_dims(self):
         return (
             sum(1 if (re - rb + 1) != 1 else 0
                 for rb, re, _ in self.ranges) + sum(1 if ts != 1 else 0
                                                     for ts in self.tile_sizes))
 
@@ -243,19 +236,17 @@
 
     def absolute_strides(self, global_shape):
         """ Returns a list of strides for advancing one element in each
             dimension. Size of the list is equal to `data_dims()`, which may
             be larger than `dims()` depending on tile sizes. """
         # ..., stride2*size1*size0, stride1*size0, stride0, ..., tile strides
         return [
-            rs * reduce(sp.mul.Mul, global_shape[i + 1:], 1)
-            for i, (_, _, rs) in enumerate(self.ranges)
+            rs * global_shape[i] for i, (_, _, rs) in enumerate(self.ranges)
         ] + [
-            reduce(sp.mul.Mul, global_shape[i + 1:], 1)
-            for i, ts in enumerate(self.tile_sizes) if ts != 1
+            global_shape[i] for i, ts in enumerate(self.tile_sizes) if ts != 1
         ]
 
     def strides(self):
         return [rs for _, _, rs in self.ranges]
 
     @staticmethod
     def _range_pystr(range):
@@ -270,15 +261,15 @@
         for dim in self.ranges:
             for d in dim:
                 result.update(set(symbolic.symlist(d)))
         return result
 
     def reorder(self, order):
         """ Re-orders the dimensions in-place according to a permutation list.
-            @param order: List or tuple of integers from 0 to self.dims() - 1,
+            :param order: List or tuple of integers from 0 to self.dims() - 1,
                           indicating the desired order of the dimensions.
         """
         new_ranges = [self.ranges[o] for o in order]
         self.ranges = new_ranges
 
     @staticmethod
     def dim_to_string(d, t=1):
@@ -494,15 +485,14 @@
         shape = self.size()
         non_ones = [i for i, d in enumerate(shape) if d != 1]
         squeezed_ranges = [self.ranges[i] for i in non_ones]
         squeezed_tsizes = [self.tile_sizes[i] for i in non_ones]
         if not squeezed_ranges:
             squeezed_ranges = [(0, 0, 1)]
             squeezed_tsizes = [1]
-            non_ones = [len(shape) - 1]
         self.ranges = squeezed_ranges
         self.tile_sizes = squeezed_tsizes
         self.offset(self, True)
         return non_ones
 
     def unsqueeze(self, axes):
         for axis in sorted(axes):
@@ -522,14 +512,15 @@
         self.ranges = new_ranges
         self.tile_sizes = new_tsizes
 
     def string_list(self):
         return Range.ndslice_to_string_list(self.ranges, self.tile_sizes)
 
 
+@dace.serialize.serializable
 class Indices(Subset):
     """ A subset of one element representing a single index in an
         N-dimensional data descriptor. """
 
     def __init__(self, indices):
         if indices is None or len(indices) == 0:
             raise TypeError('Expected an array of index expressions: got empty'
@@ -538,41 +529,28 @@
             raise TypeError("Expected collection of index expression: got str")
         if isinstance(indices, tuple):
             self.indices = symbolic.SymExpr(indices[0], indices[1])
         else:
             self.indices = symbolic.pystr_to_symbolic(indices)
         self.tile_sizes = [1]
 
-    def toJSON(self):
-        import json
-
+    def to_json(self):
         def a2s(obj):
             if isinstance(obj, symbolic.SymExpr):
                 return str(obj.expr)
             else:
                 return str(obj)
 
-        return json.dumps({
-            'type': 'subsets.Indices',
-            'indices': [*map(a2s, self.indices)]
-        })
-
-    @staticmethod
-    def fromJSON(obj, context=None):
-        import json
-        obj = json.loads(obj)
-
-        return Indices.fromJSON_object(obj, context)
+        return {'type': 'Indices', 'indices': list(map(a2s, self.indices))}
 
     @staticmethod
-    def fromJSON_object(obj, context=None):
-        if obj['type'] != 'subsets.Indices':
-            raise TypeError(
-                "fromJSON of class `Indices` called on json with type %s (expected 'subsets.Indices')"
-                % obj['type'])
+    def from_json(obj, context=None):
+        if obj['type'] != 'Indices':
+            raise TypeError("from_json of class \"Indices\" called on json "
+                            "with type %s (expected 'Indices')" % obj['type'])
 
         #return Indices(symbolic.SymExpr(obj['indices']))
         return Indices([*map(symbolic.pystr_to_symbolic, obj['indices'])])
 
     def __hash__(self):
         return hash(tuple(i for i in self.indices))
 
@@ -610,40 +588,37 @@
         for i, off in enumerate(other.min_element()):
             self.indices[i] += mult * off
 
     def coord_at(self, i):
         """ Returns the offseted coordinates of this subset at
             the given index tuple.
             For example, the range [2:10:2] at index 2 would return 6 (2+2*2).
-            @param i: A tuple of the same dimensionality as subset.dims().
-            @return: Absolute coordinates for index i.
+            :param i: A tuple of the same dimensionality as subset.dims().
+            :return: Absolute coordinates for index i.
         """
         if len(i) != len(self.indices):
             raise ValueError('Invalid dimensionality of input tuple (expected'
                              ' %d, got %d)' % (len(self.indices), len(i)))
         if any([k != 0 for k in i]):
             raise ValueError('Value out of bounds')
 
         return tuple(r for r in self.indices)
 
-    def at(self, i, global_shape):
+    def at(self, i, strides):
         """ Returns the absolute index (1D memory layout) of this subset at
             the given index tuple.
             For example, the range [2:10::2] at index 2 would return 6 (2+2*2).
-            @param i: A tuple of the same dimensionality as subset.dims().
-            @param global_shape: The full size of the set that we are 
-                                 subsetting (e.g., full array strides/padded 
-                                 shape).
-            @return: Absolute 1D index at coordinate i.
+            :param i: A tuple of the same dimensionality as subset.dims().
+            :param strides: The strides of the array we are subsetting.
+            :return: Absolute 1D index at coordinate i.
         """
         coord = self.coord_at(i)
 
         # Return i0 + i1*size0 + i2*size1*size0 + ....
-        return sum(s * reduce(sp.mul.Mul, global_shape[i + 1:], 1)
-                   for i, s in enumerate(coord))
+        return sum(s * strides[i] for i, s in enumerate(coord))
 
     def pystr(self):
         return str(self.indices)
 
     def __str__(self):
         return ", ".join(map(str, self.indices))
 
@@ -678,29 +653,34 @@
             return False
         if len(self.indices) != len(other.indices):
             return False
         return all([i == o_i for i, o_i in zip(self.indices, other.indices)])
 
     def reorder(self, order):
         """ Re-orders the dimensions in-place according to a permutation list.
-            @param order: List or tuple of integers from 0 to self.dims() - 1,
+            :param order: List or tuple of integers from 0 to self.dims() - 1,
                           indicating the desired order of the dimensions.
         """
         new_indices = [self.indices[o] for o in order]
         self.indices = new_indices
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def ndrange(self):
         return [(i, i, 1) for i in self.indices]
 
     def compose(self, other):
         raise TypeError('Index subsets cannot be composed with other subsets')
 
+    def squeeze(self):
+        num_dim = len(self.indices)
+        self.indices = [0]
+        return [num_dim - 1]
+
     def unsqueeze(self, axes):
         for axis in sorted(axes):
             self.indices.insert(axis, 0)
 
 
 def bounding_box_union(subset_a: Subset, subset_b: Subset) -> Range:
     """ Perform union by creating a bounding-box of two subsets. """
@@ -714,17 +694,17 @@
     return Range(result)
 
 
 def union(subset_a: Subset, subset_b: Subset) -> Subset:
     """ Compute the union of two Subset objects.
         If the subsets are not of the same type, degenerates to bounding-box
         union.
-        @param subset_a: The first subset.
-        @param subset_b: The second subset.
-        @return: A Subset object whose size is at least the union of the two
+        :param subset_a: The first subset.
+        :param subset_b: The second subset.
+        :return: A Subset object whose size is at least the union of the two
                  inputs. If union failed, returns None.
     """
     try:
         if type(subset_a) != type(subset_b):
             return bounding_box_union(subset_a, subset_b)
         elif subset_a is not None and subset_b is None:
             return subset_a
```

### Comparing `dace-0.9.0/dace/symbolic.py` & `dace-0.9.5/dace/symbolic.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,15 +456,15 @@
     """ Returns the symbol name if symbol, otherwise the value as a string. """
     if isinstance(val, symbol):
         return val.name
     return str(val)
 
 
 def sympy_to_dace(exprs, symbol_map=None):
-    """ Convert all `sympy.Symbol`s to DaCe symbols, according to 
+    """ Convert all `sympy.Symbol`s to DaCe symbols, according to
         `symbol_map`. """
     repl = {}
     symbol_map = symbol_map or {}
 
     oneelem = False
     try:
         exprs_iter = iter(exprs)
@@ -504,39 +504,46 @@
     for arg in expr.args:
         if not enter_functions and is_sympy_userfunction(arg):
             yield arg
             continue
         yield from swalk(arg)
 
 
+_builtin_userfunctions = {
+    'int_floor', 'int_ceil', 'min', 'Min', 'max', 'Max', 'not', 'Not'
+}
+
+
 def contains_sympy_functions(expr):
     """ Returns True if expression contains Sympy functions. """
     if is_sympy_userfunction(expr):
+        if str(expr.func) in _builtin_userfunctions:
+            return False
         return True
     for arg in expr.args:
         if contains_sympy_functions(arg):
             return True
     return False
 
 
 def sympy_numeric_fix(expr):
-    """ Fix for printing out integers as floats with ".00000000". 
+    """ Fix for printing out integers as floats with ".00000000".
         Converts the float constants in a given expression to integers. """
     if not isinstance(expr, sympy.Basic):
         if int(expr) == expr:
             return int(expr)
         return expr
 
     if isinstance(expr, sympy.Number) and expr == int(expr):
         return int(expr)
     return expr
 
 
-def sympy_ceiling_fix(expr):
-    """ Fix for SymPy printing out reciprocal values when they should be 
+def sympy_intdiv_fix(expr):
+    """ Fix for SymPy printing out reciprocal values when they should be
         integral in "ceiling/floor" sympy functions.
     """
     nexpr = expr
     if not isinstance(expr, sympy.Basic):
         return expr
 
     # The properties avoid matching the silly case "ceiling(N/32)" as
@@ -577,20 +584,41 @@
                 processed += 1
                 continue
             m = ceil.match(sympy.ceiling(a * int_ceil(c, d)))
             if m is not None:
                 nexpr = nexpr.subs(ceil, m[a] * int_ceil(m[c], m[d]))
                 processed += 1
                 continue
+        for floor in nexpr.find(sympy.floor):
+            # Simple floor
+            m = floor.match(sympy.floor(a / b))
+            if m is not None:
+                nexpr = nexpr.subs(floor, int_floor(m[a], m[b]))
+                processed += 1
+                continue
+            # Floor of floor: "floor(floor(c/d) / b)"
+            m = floor.match(sympy.floor(int_floor(c, d) / b))
+            if m is not None:
+                nexpr = nexpr.subs(floor, int_floor(
+                    int_floor(m[c], m[d]), m[b]))
+                processed += 1
+                continue
+            # Floor of floor: "floor(a / floor(c/d))"
+            m = floor.match(sympy.floor(a / int_floor(c, d)))
+            if m is not None:
+                nexpr = nexpr.subs(floor, int_floor(m[a], int_floor(
+                    m[c], m[d])))
+                processed += 1
+                continue
 
     return nexpr
 
 
 def sympy_divide_fix(expr):
-    """ Fix SymPy printouts where integer division such as "tid/2" turns 
+    """ Fix SymPy printouts where integer division such as "tid/2" turns
         into ".5*tid".
     """
     nexpr = expr
     if not isinstance(expr, sympy.Basic):
         return expr
 
     int_floor = sympy.Function('int_floor')
@@ -672,15 +700,15 @@
         return s.replace('Min', 'min').replace('Max', 'max')
 
     if isinstance(sym, SymExpr):
         return symstr(sym.expr)
 
     try:
         sym = sympy_numeric_fix(sym)
-        sym = sympy_ceiling_fix(sym)
+        sym = sympy_intdiv_fix(sym)
         sym = sympy_divide_fix(sym)
 
         sstr = DaceSympyPrinter().doprint(sym)
 
         if isinstance(sym,
                       symbol) or isinstance(sym, sympy.Symbol) or isinstance(
                           sym, sympy.Number) or dtypes.isconstant(sym):
@@ -704,29 +732,29 @@
     # Create symbols
     for sname, (stype, assumptions) in slist.items():
         symbol(sname, stype, **assumptions)
     return pystr_to_symbolic(s)
 
 
 class SympyAwarePickler(pickle.Pickler):
-    """ Custom Pickler class that safely saves SymPy expressions 
+    """ Custom Pickler class that safely saves SymPy expressions
         with function definitions in expressions (e.g., int_ceil).
     """
 
     def persistent_id(self, obj):
         if isinstance(obj, sympy.Basic):
             # Save sympy expression as srepr
             return ("DaCeSympyExpression", _spickle(obj))
         else:
             # Pickle everything else normally
             return None
 
 
 class SympyAwareUnpickler(pickle.Unpickler):
-    """ Custom Unpickler class that safely restores SymPy expressions 
+    """ Custom Unpickler class that safely restores SymPy expressions
         with function definitions in expressions (e.g., int_ceil).
     """
 
     def persistent_load(self, pid):
         type_tag, value = pid
         if type_tag == "DaCeSympyExpression":
             return _sunpickle(value)
```

### Comparing `dace-0.9.0/dace/transformation/dataflow/__init__.py` & `dace-0.9.5/dace/transformation/dataflow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 from .map_collapse import MapCollapse
 from .map_for_loop import MapToForLoop
 from .map_interchange import MapInterchange
 from .map_fusion import MapFusion
 
 # Data movement
 from .strip_mining import StripMining
-from .tiling import OrthogonalTiling
+from .tiling import MapTiling
 from .vectorization import Vectorization
 
 # Data-related
-from .stream_transient import StreamTransient, InLocalStorage, OutLocalStorage
+from .stream_transient import StreamTransient
+from .local_storage import InLocalStorage, OutLocalStorage
 from .reduce_expansion import ReduceExpansion
+from .double_buffering import DoubleBuffering
 
 # Complexity reduction
 from .redundant_array import RedundantArray
 from .redundant_array_copying import (
     RedundantArrayCopying, RedundantArrayCopying2, RedundantArrayCopying3)
+from .merge_arrays import MergeArrays
 
 # TensorFlow-specific transformations
 from .tensorflow_redundant_array import TensorflowRedundantArray
 
 # Device-related
 from .copy_to_device import CopyToDevice
 from .gpu_transform import GPUTransformMap
 from .gpu_transform_local_storage import GPUTransformLocalStorage
-from .fpga_transform import FPGATransformMap
 from .mpi import MPITransformMap
```

### Comparing `dace-0.9.0/dace/transformation/dataflow/copy_to_device.py` & `dace-0.9.5/dace/transformation/dataflow/copy_to_device.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,79 +21,103 @@
 
 
 @properties.make_properties
 class CopyToDevice(pattern_matching.Transformation):
     """ Implements the copy-to-device transformation, which copies a nested
         SDFG and its dependencies to a given device.
 
-        The transformation changes all data storage types of a nested SDFG to 
+        The transformation changes all data storage types of a nested SDFG to
         the given `storage` property, and creates new arrays and copies around
         the nested SDFG to that storage.
     """
 
     _nested_sdfg = nodes.NestedSDFG("", graph.OrderedDiGraph(), set(), set())
 
     storage = properties.Property(
         dtype=dtypes.StorageType,
         desc="Nested SDFG storage",
-        enum=dtypes.StorageType,
+        choices=dtypes.StorageType,
         from_string=lambda x: dtypes.StorageType[x],
         default=dtypes.StorageType.Default)
 
     @staticmethod
     def annotates_memlets():
         return True
 
     @staticmethod
     def expressions():
         return [nxutil.node_path_graph(CopyToDevice._nested_sdfg)]
 
     @staticmethod
     def can_be_applied(graph, candidate, expr_index, sdfg, strict=False):
+        nested_sdfg = graph.nodes()[candidate[CopyToDevice._nested_sdfg]]
+
+        for edge in graph.all_edges(nested_sdfg):
+            # Stream inputs/outputs not allowed
+            path = graph.memlet_path(edge)
+            if ((isinstance(path[0].src, nodes.AccessNode)
+                 and isinstance(sdfg.arrays[path[0].src.data], data.Stream)) or
+                (isinstance(path[-1].dst, nodes.AccessNode)
+                 and isinstance(sdfg.arrays[path[-1].dst.data], data.Stream))):
+                return False
+            # WCR outputs with arrays are not allowed
+            if (edge.data.wcr is not None
+                    and edge.data.subset.num_elements() != 1):
+                return False
+
         return True
 
     @staticmethod
     def match_to_str(graph, candidate):
         nested_sdfg = graph.nodes()[candidate[CopyToDevice._nested_sdfg]]
         return nested_sdfg.label
 
     def apply(self, sdfg):
         state = sdfg.nodes()[self.state_id]
         nested_sdfg = state.nodes()[self.subgraph[CopyToDevice._nested_sdfg]]
         storage = self.storage
+        created_arrays = set()
 
         for _, edge in enumerate(state.in_edges(nested_sdfg)):
 
             src, src_conn, dst, dst_conn, memlet = edge
             dataname = memlet.data
+            if dataname is None:
+                continue
             memdata = sdfg.arrays[dataname]
 
-            if isinstance(memdata, data.Array):
-                new_data = sdfg.add_array(
-                    'device_' + dataname + '_in',
-                    memdata.dtype, [
-                        symbolic.overapproximate(r)
-                        for r in memlet.bounding_box_size()
-                    ],
-                    transient=True,
-                    storage=storage)
-            elif isinstance(memdata, data.Scalar):
-                new_data = sdfg.add_scalar(
-                    'device_' + dataname + '_in',
-                    memdata.dtype,
-                    transient=True,
-                    storage=storage)
-            else:
-                raise NotImplementedError
+            name = 'device_' + dataname + '_in'
+            if name not in created_arrays:
+                if isinstance(memdata, data.Array):
+                    name, _ = sdfg.add_array(
+                        'device_' + dataname + '_in',
+                        shape=[
+                            symbolic.overapproximate(r)
+                            for r in memlet.bounding_box_size()
+                        ],
+                        dtype=memdata.dtype,
+                        transient=True,
+                        storage=storage,
+                        find_new_name=True)
+                elif isinstance(memdata, data.Scalar):
+                    name, _ = sdfg.add_scalar(
+                        'device_' + dataname + '_in',
+                        dtype=memdata.dtype,
+                        transient=True,
+                        storage=storage,
+                        find_new_name=True)
+                else:
+                    raise NotImplementedError
+                created_arrays.add(name)
 
-            data_node = nodes.AccessNode('device_' + dataname + '_in')
+            data_node = nodes.AccessNode(name)
 
             to_data_mm = dcpy(memlet)
             from_data_mm = dcpy(memlet)
-            from_data_mm.data = 'device_' + dataname + '_in'
+            from_data_mm.data = name
             offset = []
             for ind, r in enumerate(memlet.subset):
                 offset.append(r[0])
                 if isinstance(memlet.subset[ind], tuple):
                     begin = memlet.subset[ind][0] - r[0]
                     end = memlet.subset[ind][1] - r[0]
                     step = memlet.subset[ind][2]
@@ -105,39 +129,46 @@
             state.add_edge(src, src_conn, data_node, None, to_data_mm)
             state.add_edge(data_node, None, dst, dst_conn, from_data_mm)
 
         for _, edge in enumerate(state.out_edges(nested_sdfg)):
 
             src, src_conn, dst, dst_conn, memlet = edge
             dataname = memlet.data
+            if dataname is None:
+                continue
             memdata = sdfg.arrays[dataname]
 
-            if isinstance(memdata, data.Array):
-                new_data = data.Array(
-                    'device_' + dataname + '_out',
-                    memdata.dtype, [
-                        symbolic.overapproximate(r)
-                        for r in memlet.bounding_box_size()
-                    ],
-                    transient=True,
-                    storage=storage)
-            elif isinstance(memdata, data.Scalar):
-                new_data = sdfg.add_scalar(
-                    'device_' + dataname + '_out',
-                    memdata.dtype,
-                    transient=True,
-                    storage=storage)
-            else:
-                raise NotImplementedError
+            name = 'device_' + dataname + '_out'
+            if name not in created_arrays:
+                if isinstance(memdata, data.Array):
+                    name, _ = sdfg.add_array(
+                        name,
+                        shape=[
+                            symbolic.overapproximate(r)
+                            for r in memlet.bounding_box_size()
+                        ],
+                        dtype=memdata.dtype,
+                        transient=True,
+                        storage=storage,
+                        find_new_name=True)
+                elif isinstance(memdata, data.Scalar):
+                    name, _ = sdfg.add_scalar(
+                        name,
+                        dtype=memdata.dtype,
+                        transient=True,
+                        storage=storage)
+                else:
+                    raise NotImplementedError
+                created_arrays.add(name)
 
-            data_node = nodes.AccessNode('device_' + dataname + '_out')
+            data_node = nodes.AccessNode(name)
 
             to_data_mm = dcpy(memlet)
             from_data_mm = dcpy(memlet)
-            to_data_mm.data = 'device_' + dataname + '_out'
+            to_data_mm.data = name
             offset = []
             for ind, r in enumerate(memlet.subset):
                 offset.append(r[0])
                 if isinstance(memlet.subset[ind], tuple):
                     begin = memlet.subset[ind][0] - r[0]
                     end = memlet.subset[ind][1] - r[0]
                     step = memlet.subset[ind][2]
```

### Comparing `dace-0.9.0/dace/transformation/dataflow/fpga_transform.py` & `dace-0.9.5/dace/transformation/dataflow/fpga_transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,49 +99,51 @@
         # Second, create a FPGA clone of each array
         cloned_arrays = {}
         in_cloned_arraynodes = {}
         out_cloned_arraynodes = {}
         for array_node in in_arrays_to_clone:
             array = array_node.desc(sdfg)
             if array_node.data in cloned_arrays:
-                cloned_array = cloned_arrays[array_node.data]
+                pass
+            elif 'fpga_' + array_node.data in sdfg.arrays:
+                pass
             else:
-                cloned_array = sdfg.add_array(
+                sdfg.add_array(
                     'fpga_' + array_node.data,
-                    array.dtype,
-                    array.shape,
+                    dtype=array.dtype,
+                    shape=array.shape,
                     materialize_func=array.materialize_func,
                     transient=True,
                     storage=dtypes.StorageType.FPGA_Global,
                     allow_conflicts=array.allow_conflicts,
-                    access_order=array.access_order,
                     strides=array.strides,
                     offset=array.offset)
                 cloned_arrays[array_node.data] = 'fpga_' + array_node.data
-            cloned_node = type(array_node)(cloned_array)
+            cloned_node = nodes.AccessNode('fpga_' + array_node.data)
 
             in_cloned_arraynodes[array_node.data] = cloned_node
         for array_node in out_arrays_to_clone:
             array = array_node.desc(sdfg)
             if array_node.data in cloned_arrays:
-                cloned_array = cloned_arrays[array_node.data]
+                pass
+            elif 'fpga_' + array_node.data in sdfg.arrays:
+                pass
             else:
-                cloned_array = sdfg.add_array(
+                sdfg.add_array(
                     'fpga_' + array_node.data,
-                    array.dtype,
-                    array.shape,
+                    dtype=array.dtype,
+                    shape=array.shape,
                     materialize_func=array.materialize_func,
                     transient=True,
                     storage=dtypes.StorageType.FPGA_Global,
                     allow_conflicts=array.allow_conflicts,
-                    access_order=array.access_order,
                     strides=array.strides,
                     offset=array.offset)
                 cloned_arrays[array_node.data] = 'fpga_' + array_node.data
-            cloned_node = type(array_node)(cloned_array)
+            cloned_node = nodes.AccessNode('fpga_' + array_node.data)
 
             out_cloned_arraynodes[array_node.data] = cloned_node
 
         # Third, connect the cloned arrays to the originals
         # TODO(later): Shift indices and create only the necessary sub-arrays
         for array_name, node in in_cloned_arraynodes.items():
             graph.add_node(node)
@@ -171,8 +173,8 @@
                     and edge.data.data in cloned_arrays):
                 edge.data.data = cloned_arrays[edge.data.data]
 
     def modifies_graph(self):
         return True
 
 
-pattern_matching.Transformation.register_pattern(FPGATransformMap)
+# pattern_matching.Transformation.register_pattern(FPGATransformMap)
```

### Comparing `dace-0.9.0/dace/transformation/dataflow/gpu_transform.py` & `dace-0.9.5/dace/transformation/interstate/fpga_transform_state.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,264 +1,276 @@
-""" Contains the GPU Transform Map transformation. """
+""" Contains inter-state transformations of an SDFG to run on an FPGA. """
 
-import copy
-import itertools
-
-from dace import data, dtypes, sdfg as sd, subsets as sbs, symbolic
-from dace.graph import nodes, nxutil
+import dace
+from dace import data, memlet, dtypes, sdfg as sd, subsets
+from dace.graph import edges, nodes, nxutil
 from dace.transformation import pattern_matching
-from dace.properties import Property, make_properties
-from dace.config import Config
-
 
-@make_properties
-class GPUTransformMap(pattern_matching.Transformation):
-    """ Implements the GPUTransformMap transformation.
 
-        Converts a single map to a GPU-scheduled map and creates GPU arrays
-        outside it, generating CPU<->GPU memory copies automatically.
-    """
+def fpga_update(sdfg, state, depth):
+    scope_dict = state.scope_dict()
+    for node in state.nodes():
+        if (isinstance(node, nodes.AccessNode)
+                and node.desc(sdfg).storage == dtypes.StorageType.Default):
+            nodedesc = node.desc(sdfg)
+            if depth >= 2:
+                nodedesc.storage = dtypes.StorageType.FPGA_Local
+            else:
+                if scope_dict[node]:
+                    nodedesc.storage = dtypes.StorageType.FPGA_Local
+                else:
+                    nodedesc.storage = dtypes.StorageType.FPGA_Global
+        if (hasattr(node, "schedule")
+                and node.schedule == dace.dtypes.ScheduleType.Default):
+            node.schedule = dace.dtypes.ScheduleType.FPGA_Device
+        if isinstance(node, nodes.NestedSDFG):
+            for s in node.sdfg.nodes():
+                fpga_update(node.sdfg, s, depth + 1)
 
-    _maps_transformed = 0
-    _arrays_removed = 0
 
-    fullcopy = Property(
-        desc="Copy whole arrays rather than used subset",
-        dtype=bool,
-        default=False)
+class FPGATransformState(pattern_matching.Transformation):
+    """ Implements the FPGATransformState transformation. """
 
-    _map_entry = nodes.MapEntry(nodes.Map("", [], []))
-    _reduce = nodes.Reduce('lambda: None', None)
+    _state = sd.SDFGState()
 
     @staticmethod
     def expressions():
-        return [
-            nxutil.node_path_graph(GPUTransformMap._map_entry),
-            nxutil.node_path_graph(GPUTransformMap._reduce)
-        ]
+        return [nxutil.node_path_graph(FPGATransformState._state)]
 
     @staticmethod
     def can_be_applied(graph, candidate, expr_index, sdfg, strict=False):
-        if expr_index == 0:
-            map_entry = graph.nodes()[candidate[GPUTransformMap._map_entry]]
+        state = graph.nodes()[candidate[FPGATransformState._state]]
+
+        # TODO: Support most of these cases
+        for edge, graph in state.all_edges_recursive():
+            # Code->Code memlets are disallowed (for now)
+            if (isinstance(edge.src, nodes.CodeNode)
+                    and isinstance(edge.dst, nodes.CodeNode)):
+                return False
+
+        for node, graph in state.all_nodes_recursive():
+            # Consume scopes are currently unsupported
+            if isinstance(node, (nodes.ConsumeEntry, nodes.ConsumeExit)):
+                return False
+
+            # Streams have strict conditions due to code generator limitations
+            if (isinstance(node, nodes.AccessNode)
+                    and isinstance(sdfg.arrays[node.data], data.Stream)):
+                nodedesc = graph.parent.arrays[node.data]
+                sdict = graph.scope_dict()
+                if nodedesc.storage in [
+                        dtypes.StorageType.CPU_Heap,
+                        dtypes.StorageType.CPU_Pinned,
+                        dtypes.StorageType.CPU_Stack
+                ]:
+                    return False
+
+                # Cannot allocate FIFO from CPU code
+                if sdict[node] is None:
+                    return False
+
+                # Arrays of streams cannot have symbolic size on FPGA
+                if dace.symbolic.issymbolic(nodedesc.total_size,
+                                            graph.parent.constants):
+                    return False
+
+                # Streams cannot be unbounded on FPGA
+                if nodedesc.buffer_size < 1:
+                    return False
+
+        for node in state.nodes():
+
+            if (isinstance(node, nodes.AccessNode)
+                    and node.desc(sdfg).storage != dtypes.StorageType.Default):
+                return False
+
+            if not isinstance(node, nodes.MapEntry):
+                continue
+
+            map_entry = node
             candidate_map = map_entry.map
 
-            # Map schedules that are disallowed to transform to GPUs
+            # No more than 3 dimensions
+            if candidate_map.range.dims() > 3: return False
+
+            # Map schedules that are disallowed to transform to FPGAs
             if (candidate_map.schedule == dtypes.ScheduleType.MPI
                     or candidate_map.schedule == dtypes.ScheduleType.GPU_Device
+                    or
+                    candidate_map.schedule == dtypes.ScheduleType.FPGA_Device
                     or candidate_map.schedule ==
                     dtypes.ScheduleType.GPU_ThreadBlock):
                 return False
 
-            # Recursively check parent for GPU schedules
-            sdict = graph.scope_dict()
+            # Recursively check parent for FPGA schedules
+            sdict = state.scope_dict()
             current_node = map_entry
             while current_node is not None:
                 if (current_node.map.schedule == dtypes.ScheduleType.GPU_Device
                         or current_node.map.schedule ==
-                        dtypes.ScheduleType.GPU_ThreadBlock):
-                    return False
-                current_node = sdict[current_node]
-
-            # Ensure that map does not include internal arrays that are allocated
-            # on non-default space
-            subgraph = graph.scope_subgraph(map_entry)
-            for node in subgraph.nodes():
-                if (isinstance(node, nodes.AccessNode) and
-                        node.desc(sdfg).storage != dtypes.StorageType.Default
-                        and node.desc(sdfg).storage !=
-                        dtypes.StorageType.Register):
-                    return False
-
-            return True
-        elif expr_index == 1:
-            reduce = graph.nodes()[candidate[GPUTransformMap._reduce]]
-
-            # Map schedules that are disallowed to transform to GPUs
-            if (reduce.schedule == dtypes.ScheduleType.MPI
-                    or reduce.schedule == dtypes.ScheduleType.GPU_Device
-                    or reduce.schedule == dtypes.ScheduleType.GPU_ThreadBlock):
-                return False
-
-            # Recursively check parent for GPU schedules
-            sdict = graph.scope_dict()
-            current_node = sdict[reduce]
-            while current_node is not None:
-                if (current_node.map.schedule == dtypes.ScheduleType.GPU_Device
+                        dtypes.ScheduleType.FPGA_Device
                         or current_node.map.schedule ==
                         dtypes.ScheduleType.GPU_ThreadBlock):
                     return False
                 current_node = sdict[current_node]
 
-            return True
+        return True
 
     @staticmethod
     def match_to_str(graph, candidate):
-        if GPUTransformMap._reduce in candidate:
-            return str(graph.nodes()[candidate[GPUTransformMap._reduce]])
-        else:
-            map_entry = graph.nodes()[candidate[GPUTransformMap._map_entry]]
-            return str(map_entry)
+        state = graph.nodes()[candidate[FPGATransformState._state]]
+
+        return state.label
 
     def apply(self, sdfg):
-        graph = sdfg.nodes()[self.state_id]
-        if self.expr_index == 0:
-            cnode = graph.nodes()[self.subgraph[GPUTransformMap._map_entry]]
-            node_schedprop = cnode.map
-            exit_nodes = graph.exit_nodes(cnode)
-        else:
-            cnode = graph.nodes()[self.subgraph[GPUTransformMap._reduce]]
-            node_schedprop = cnode
-            exit_nodes = [cnode]
-
-        # Change schedule
-        node_schedprop._schedule = dtypes.ScheduleType.GPU_Device
-        if Config.get_bool("debugprint"):
-            GPUTransformMap._maps_transformed += 1
-
-        gpu_storage_types = [
-            dtypes.StorageType.GPU_Global,
-            dtypes.StorageType.GPU_Shared,
-            dtypes.StorageType.GPU_Stack  #, dtypes.StorageType.CPU_Pinned
-        ]
-
-        #######################################################
-        # Add GPU copies of CPU arrays (i.e., not already on GPU)
-
-        # First, understand which arrays to clone
-        all_out_edges = []
-        for enode in exit_nodes:
-            all_out_edges.extend(list(graph.out_edges(enode)))
-        in_arrays_to_clone = set()
-        out_arrays_to_clone = set()
-        out_streamarrays = {}
-        for e in graph.in_edges(cnode):
-            data_node = sd.find_input_arraynode(graph, e)
-            if isinstance(data_node.desc(sdfg), data.Scalar):
-                continue
-            if data_node.desc(sdfg).storage not in gpu_storage_types:
-                in_arrays_to_clone.add(data_node)
-        for e in all_out_edges:
-            data_node = sd.find_output_arraynode(graph, e)
-            if isinstance(data_node.desc(sdfg), data.Scalar):
-                continue
-            if data_node.desc(sdfg).storage not in gpu_storage_types:
-                # Stream directly connected to an array
-                if sd.is_array_stream_view(sdfg, graph, data_node):
-                    datadesc = data_node.desc(sdfg)
-                    if datadesc.transient is False:
-                        raise TypeError('Non-transient stream-array view are '
-                                        'unsupported')
-                    # Add parent node to clone
-                    out_arrays_to_clone.add(graph.out_edges(data_node)[0].dst)
-                    out_streamarrays[graph.out_edges(data_node)[0]
-                                     .dst] = data_node
+        state = sdfg.nodes()[self.subgraph[FPGATransformState._state]]
 
-                    # Do not clone stream
+        # Find source/sink (data) nodes
+        input_nodes = nxutil.find_source_nodes(state)
+        output_nodes = nxutil.find_sink_nodes(state)
+
+        fpga_data = {}
+
+        # Input nodes may also be nodes with WCR memlets
+        # We have to recur across nested SDFGs to find them
+        wcr_input_nodes = set()
+        stack = []
+
+        for node, graph in state.all_nodes_recursive():
+            if isinstance(node, dace.graph.nodes.AccessNode):
+                for e in graph.all_edges(node):
+                    if e.data.wcr is not None:
+                        # This is an output node with wcr
+                        # find the target in the parent sdfg
+
+                        # following the structure State->SDFG->State-> SDFG
+                        # from the current_state we have to go two levels up
+                        parent_state = graph.parent.parent
+                        if parent_state is not None:
+                            for parent_edges in parent_state.edges():
+                                if parent_edges.src_conn == e.dst.data or (
+                                        isinstance(parent_edges.dst,
+                                                   dace.graph.nodes.AccessNode)
+                                        and
+                                        e.dst.data == parent_edges.dst.data):
+                                    # This must be copied to device
+                                    input_nodes.append(parent_edges.dst)
+                                    wcr_input_nodes.add(parent_edges.dst)
+
+        if input_nodes:
+            # create pre_state
+            pre_state = sd.SDFGState('pre_' + state.label, sdfg)
+
+            for node in input_nodes:
+                if (not isinstance(node, dace.graph.nodes.AccessNode)
+                        or not isinstance(node.desc(sdfg), dace.data.Array)):
+                    # Only transfer array nodes
+                    # TODO: handle streams
                     continue
 
-                out_arrays_to_clone.add(data_node)
-        if Config.get_bool("debugprint"):
-            GPUTransformMap._arrays_removed += len(in_arrays_to_clone) + len(
-                out_arrays_to_clone)
-
-        # Second, create a GPU clone of each array
-        cloned_arrays = {}
-        in_cloned_arraynodes = {}
-        out_cloned_arraynodes = {}
-        for array_node in in_arrays_to_clone:
-            array = array_node.desc(sdfg)
-            if array_node.data in cloned_arrays:
-                cloned_array = cloned_arrays[array_node.data]
-            else:
-                cloned_array = array.clone()
-                cloned_array.storage = dtypes.StorageType.GPU_Global
-                cloned_array.transient = True
-                sdfg.add_datadesc('gpu_' + array_node.data, cloned_array)
-                cloned_arrays[array_node.data] = 'gpu_' + array_node.data
-            cloned_node = type(array_node)('gpu_' + array_node.data)
-
-            in_cloned_arraynodes[array_node.data] = cloned_node
-        for array_node in out_arrays_to_clone:
-            array = array_node.desc(sdfg)
-            if array_node.data in cloned_arrays:
-                cloned_array = cloned_arrays[array_node.data]
-            else:
-                cloned_array = array.clone()
-                cloned_array.storage = dtypes.StorageType.GPU_Global
-                cloned_array.transient = True
-                sdfg.add_datadesc('gpu_' + array_node.data, cloned_array)
-                cloned_arrays[array_node.data] = 'gpu_' + array_node.data
-            cloned_node = type(array_node)('gpu_' + array_node.data)
-
-            out_cloned_arraynodes[array_node.data] = cloned_node
-
-        # Third, connect the cloned arrays to the originals
-        # TODO(later): Shift indices and create only the necessary sub-arrays
-        for array_name, node in in_cloned_arraynodes.items():
-            graph.add_node(node)
-            for edge in graph.in_edges(cnode):
-                if edge.data.data == array_name:
-                    graph.remove_edge(edge)
-                    newmemlet = copy.copy(edge.data)
-                    newmemlet.data = node.data
-                    graph.add_edge(node, edge.src_conn, edge.dst,
-                                   edge.dst_conn, newmemlet)
-
-                    if self.fullcopy:
-                        edge.data.subset = sbs.Range.from_array(
-                            node.desc(sdfg))
-                    edge.data.other_subset = edge.data.subset
-                    graph.add_edge(edge.src, None, node, None, edge.data)
-        for array_name, node in out_cloned_arraynodes.items():
-            graph.add_node(node)
-            for edge in all_out_edges:
-                if edge.data.data == array_name:
-                    graph.remove_edge(edge)
-                    newmemlet = copy.copy(edge.data)
-                    newmemlet.data = node.data
-                    graph.add_edge(edge.src, edge.src_conn, node,
-                                   edge.dst_conn, newmemlet)
-                    edge.data.wcr = None
-                    if self.fullcopy:
-                        edge.data.subset = sbs.Range.from_array(
-                            node.desc(sdfg))
-                    edge.data.other_subset = edge.data.subset
-                    graph.add_edge(node, None, edge.dst, None, edge.data)
-
-        # Reconnect stream-arrays
-        for array_node, streamnode in out_streamarrays.items():
-            # Set stream storage to GPU
-            streamnode.desc(sdfg).storage = dtypes.StorageType.GPU_Global
-
-            cloned_node = out_cloned_arraynodes[array_node.data]
-
-            e = graph.out_edges(streamnode)[0]
-            graph.remove_edge(e)
-            newmemlet = copy.copy(e.data)
-            newmemlet.data = cloned_node.data
-            # stream -> cloned array
-            graph.add_edge(e.src, e.src_conn, cloned_node, e.dst_conn,
-                           newmemlet)
-            # cloned array -> array
-            graph.add_nedge(cloned_node, array_node, e.data)
-
-        # Fourth, replace memlet arrays as necessary
-        if self.expr_index == 0:
-            scope_subgraph = graph.scope_subgraph(cnode)
-            for edge in scope_subgraph.edges():
-                if (edge.data.data is not None
-                        and edge.data.data in cloned_arrays):
-                    edge.data.data = cloned_arrays[edge.data.data]
+                array = node.desc(sdfg)
+                if node.data in fpga_data:
+                    fpga_array = fpga_data[node.data]
+                elif node not in wcr_input_nodes:
+                    fpga_array = sdfg.add_array(
+                        'fpga_' + node.data,
+                        array.shape,
+                        array.dtype,
+                        materialize_func=array.materialize_func,
+                        transient=True,
+                        storage=dtypes.StorageType.FPGA_Global,
+                        allow_conflicts=array.allow_conflicts,
+                        strides=array.strides,
+                        offset=array.offset)
+                    fpga_data[node.data] = fpga_array
+
+                pre_node = pre_state.add_read(node.data)
+                pre_fpga_node = pre_state.add_write('fpga_' + node.data)
+                full_range = subsets.Range(
+                    [(0, s - 1, 1) for s in array.shape])
+                mem = memlet.Memlet(node.data, full_range.num_elements(),
+                                    full_range, 1)
+                pre_state.add_edge(pre_node, None, pre_fpga_node, None, mem)
+
+                if node not in wcr_input_nodes:
+                    fpga_node = state.add_read('fpga_' + node.data)
+                    nxutil.change_edge_src(state, node, fpga_node)
+                    state.remove_node(node)
+
+            sdfg.add_node(pre_state)
+            nxutil.change_edge_dest(sdfg, state, pre_state)
+            sdfg.add_edge(pre_state, state, edges.InterstateEdge())
+
+        if output_nodes:
+
+            post_state = sd.SDFGState('post_' + state.label, sdfg)
+
+            for node in output_nodes:
+                if (not isinstance(node, dace.graph.nodes.AccessNode)
+                        or not isinstance(node.desc(sdfg), dace.data.Array)):
+                    # Only transfer array nodes
+                    # TODO: handle streams
+                    continue
 
-    def modifies_graph(self):
-        return True
+                array = node.desc(sdfg)
+                if node.data in fpga_data:
+                    fpga_array = fpga_data[node.data]
+                else:
+                    fpga_array = sdfg.add_array(
+                        'fpga_' + node.data,
+                        array.shape,
+                        array.dtype,
+                        materialize_func=array.materialize_func,
+                        transient=True,
+                        storage=dtypes.StorageType.FPGA_Global,
+                        allow_conflicts=array.allow_conflicts,
+                        strides=array.strides,
+                        offset=array.offset)
+                    fpga_data[node.data] = fpga_array
+                # fpga_node = type(node)(fpga_array)
+
+                post_node = post_state.add_write(node.data)
+                post_fpga_node = post_state.add_read('fpga_' + node.data)
+                full_range = subsets.Range(
+                    [(0, s - 1, 1) for s in array.shape])
+                mem = memlet.Memlet('fpga_' + node.data,
+                                    full_range.num_elements(), full_range, 1)
+                post_state.add_edge(post_fpga_node, None, post_node, None, mem)
+
+                fpga_node = state.add_write('fpga_' + node.data)
+                nxutil.change_edge_dest(state, node, fpga_node)
+                state.remove_node(node)
+
+            sdfg.add_node(post_state)
+            nxutil.change_edge_src(sdfg, state, post_state)
+            sdfg.add_edge(state, post_state, edges.InterstateEdge())
+
+        veclen_ = 1
+
+        # propagate vector info from a nested sdfg
+        for src, src_conn, dst, dst_conn, mem in state.edges():
+            # need to go inside the nested SDFG and grab the vector length
+            if isinstance(dst, dace.graph.nodes.NestedSDFG):
+                # this edge is going to the nested SDFG
+                for inner_state in dst.sdfg.states():
+                    for n in inner_state.nodes():
+                        if isinstance(n, dace.graph.nodes.AccessNode
+                                      ) and n.data == dst_conn:
+                            # assuming all memlets have the same vector length
+                            veclen_ = inner_state.all_edges(n)[0].data.veclen
+            if isinstance(src, dace.graph.nodes.NestedSDFG):
+                # this edge is coming from the nested SDFG
+                for inner_state in src.sdfg.states():
+                    for n in inner_state.nodes():
+                        if isinstance(n, dace.graph.nodes.AccessNode
+                                      ) and n.data == src_conn:
+                            # assuming all memlets have the same vector length
+                            veclen_ = inner_state.all_edges(n)[0].data.veclen
+
+            if mem.data is not None and mem.data in fpga_data:
+                mem.data = 'fpga_' + mem.data
+                mem.veclen = veclen_
 
-    @staticmethod
-    def print_debuginfo():
-        print("Automatically cloned {} arrays for the GPU.".format(
-            GPUTransformMap._arrays_removed))
-        print("Automatically changed {} maps for the GPU.".format(
-            GPUTransformMap._maps_transformed))
+        fpga_update(sdfg, state, 0)
 
 
-pattern_matching.Transformation.register_pattern(GPUTransformMap)
+pattern_matching.Transformation.register_stateflow_pattern(FPGATransformState)
```

### Comparing `dace-0.9.0/dace/transformation/dataflow/gpu_transform_local_storage.py` & `dace-0.9.5/dace/transformation/dataflow/gpu_transform_local_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,18 @@
             if (candidate_map.schedule == dtypes.ScheduleType.MPI
                     or candidate_map.schedule == dtypes.ScheduleType.GPU_Device
                     or candidate_map.schedule ==
                     dtypes.ScheduleType.GPU_ThreadBlock or
                     candidate_map.schedule == dtypes.ScheduleType.Sequential):
                 return False
 
+            # Dynamic map ranges cannot become kernels
+            if sd.has_dynamic_map_inputs(graph, map_entry):
+                return False
+
             # Recursively check parent for GPU schedules
             sdict = graph.scope_dict()
             current_node = map_entry
             while current_node is not None:
                 if (current_node.map.schedule == dtypes.ScheduleType.GPU_Device
                         or current_node.map.schedule ==
                         dtypes.ScheduleType.GPU_ThreadBlock):
@@ -104,14 +108,22 @@
             for node in subgraph.nodes():
                 if (isinstance(node, nodes.AccessNode) and
                         node.desc(sdfg).storage != dtypes.StorageType.Default
                         and node.desc(sdfg).storage !=
                         dtypes.StorageType.Register):
                     return False
 
+            # If one of the outputs is a stream, do not match
+            map_exit = graph.exit_nodes(map_entry)[0]
+            for edge in graph.out_edges(map_exit):
+                dst = graph.memlet_path(edge)[-1].dst
+                if (isinstance(dst, nodes.AccessNode)
+                        and isinstance(sdfg.arrays[dst.data], data.Stream)):
+                    return False
+
             return True
         elif expr_index == 1:
             reduce = graph.nodes()[candidate[GPUTransformLocalStorage._reduce]]
 
             # Map schedules that are disallowed to transform to GPUs
             if (reduce.schedule == dtypes.ScheduleType.MPI
                     or reduce.schedule == dtypes.ScheduleType.GPU_Device
@@ -239,31 +251,39 @@
                 actual_dims = [
                     idx for idx, r in enumerate(full_shape)
                     if not (isinstance(r, int) and r == 1)
                 ]
                 if len(actual_dims) == 0:  # abort
                     actual_dims = [len(full_shape) - 1]
                 if isinstance(array, data.Scalar):
-                    cloned_array = sdfg.add_array(
+                    sdfg.add_array(
                         name=cloned_name,
                         shape=[1],
                         dtype=array.dtype,
                         transient=True,
                         storage=dtypes.StorageType.GPU_Global)
+                elif isinstance(array, data.Stream):
+                    sdfg.add_stream(
+                        name=cloned_name,
+                        dtype=array.dtype,
+                        shape=[full_shape[d] for d in actual_dims],
+                        veclen=array.veclen,
+                        buffer_size=array.buffer_size,
+                        storage=dtypes.StorageType.GPU_Global,
+                        transient=True,
+                        offset=[array.offset[d] for d in actual_dims])
                 else:
-                    cloned_array = sdfg.add_array(
+                    sdfg.add_array(
                         name=cloned_name,
                         shape=[full_shape[d] for d in actual_dims],
                         dtype=array.dtype,
                         materialize_func=array.materialize_func,
                         transient=True,
                         storage=dtypes.StorageType.GPU_Global,
                         allow_conflicts=array.allow_conflicts,
-                        access_order=tuple(
-                            [array.access_order[d] for d in actual_dims]),
                         strides=[array.strides[d] for d in actual_dims],
                         offset=[array.offset[d] for d in actual_dims],
                     )
                 cloned_arrays[array_node.data] = cloned_name
             cloned_node = type(array_node)(cloned_name)
 
             in_cloned_arraynodes[array_node.data] = cloned_node
@@ -304,31 +324,39 @@
                 actual_dims = [
                     idx for idx, r in enumerate(full_shape)
                     if not (isinstance(r, int) and r == 1)
                 ]
                 if len(actual_dims) == 0:  # abort
                     actual_dims = [len(full_shape) - 1]
                 if isinstance(array, data.Scalar):
-                    cloned_array = sdfg.add_array(
+                    sdfg.add_array(
                         name=cloned_name,
                         shape=[1],
                         dtype=array.dtype,
                         transient=True,
                         storage=dtypes.StorageType.GPU_Global)
+                elif isinstance(array, data.Stream):
+                    sdfg.add_stream(
+                        name=cloned_name,
+                        dtype=array.dtype,
+                        shape=[full_shape[d] for d in actual_dims],
+                        veclen=array.veclen,
+                        buffer_size=array.buffer_size,
+                        storage=dtypes.StorageType.GPU_Global,
+                        transient=True,
+                        offset=[array.offset[d] for d in actual_dims])
                 else:
-                    cloned_array = sdfg.add_array(
+                    sdfg.add_array(
                         name=cloned_name,
                         shape=[full_shape[d] for d in actual_dims],
                         dtype=array.dtype,
                         materialize_func=array.materialize_func,
                         transient=True,
                         storage=dtypes.StorageType.GPU_Global,
                         allow_conflicts=array.allow_conflicts,
-                        access_order=tuple(
-                            [array.access_order[d] for d in actual_dims]),
                         strides=[array.strides[d] for d in actual_dims],
                         offset=[array.offset[d] for d in actual_dims],
                     )
                 cloned_arrays[array_node.data] = cloned_name
             cloned_node = type(array_node)(cloned_name)
             cloned_node.setzero = True
 
@@ -400,15 +428,15 @@
                                     begin = r[0] - offset[ind]
                                     end = r[1] - offset[ind]
                                     step = r[2]
                                     newsubset[ind] = (begin, end, step)
                                 else:
                                     newsubset[ind] = (
                                         r - offset[ind],
-                                        r - offset[ind] + 1,
+                                        r - offset[ind],
                                         1,
                                     )
                             memlet.subset = type(edge.data.subset)(
                                 [r for r in newsubset if r is not None])
                         memlet.data = node.data
 
                     if self.fullcopy:
@@ -485,15 +513,15 @@
                                     begin = r[0] - offset[ind]
                                     end = r[1] - offset[ind]
                                     step = r[2]
                                     newsubset[ind] = (begin, end, step)
                                 else:
                                     newsubset[ind] = (
                                         r - offset[ind],
-                                        r - offset[ind] + 1,
+                                        r - offset[ind],
                                         1,
                                     )
                             memlet.subset = type(edge.data.subset)(
                                 [r for r in newsubset if r is not None])
                         memlet.data = node.data
 
                     edge.data.wcr = None
```

### Comparing `dace-0.9.0/dace/transformation/dataflow/map_collapse.py` & `dace-0.9.5/dace/transformation/dataflow/map_collapse.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Contains classes that implement the map-collapse transformation. """
 
 from copy import deepcopy as dcpy
+from dace.symbolic import symlist
 from dace.graph import nodes, nxutil
 from dace.transformation import pattern_matching
 from dace.properties import make_properties
 
 
 @make_properties
 class MapCollapse(pattern_matching.Transformation):
@@ -30,34 +31,46 @@
     def can_be_applied(graph, candidate, expr_index, sdfg, strict=False):
         # Check the edges between the entries of the two maps.
         outer_map_entry = graph.nodes()[candidate[
             MapCollapse._outer_map_entry]]
         inner_map_entry = graph.nodes()[candidate[
             MapCollapse._inner_map_entry]]
 
+        # Check that inner map range is independent of outer range
+        map_deps = set()
+        for s in inner_map_entry.map.range:
+            map_deps |= set(map(str, symlist(s)))
+        if any(dep in outer_map_entry.map.params for dep in map_deps):
+            return False
+
         # Check that the destination of all the outgoing edges
         # from the outer map's entry is the inner map's entry.
         for _src, _, dest, _, _ in graph.out_edges(outer_map_entry):
             if dest != inner_map_entry:
                 return False
 
         # Check that the source of all the incoming edges
         # to the inner map's entry is the outer map's entry.
-        for src, _, _dest, _, _ in graph.in_edges(inner_map_entry):
+        for src, _, _, dst_conn, memlet in graph.in_edges(inner_map_entry):
             if src != outer_map_entry:
                 return False
 
-        # Check the edges between the exits of the two maps.
-        inner_map_exits = graph.exit_nodes(inner_map_entry)
-        outer_map_exits = graph.exit_nodes(outer_map_entry)
-        if len(inner_map_exits) > 1 or len(outer_map_exits) > 1:
-            return False
+            # Check that dynamic input range memlets are independent of
+            # first map range
+            if dst_conn is not None and not dst_conn.startswith('IN_'):
+                memlet_deps = set()
+                for s in memlet.subset:
+                    memlet_deps |= set(map(str, symlist(s)))
+                if any(dep in outer_map_entry.map.params
+                       for dep in memlet_deps):
+                    return False
 
-        inner_map_exit = inner_map_exits[0]
-        outer_map_exit = outer_map_exits[0]
+        # Check the edges between the exits of the two maps.
+        inner_map_exit = graph.exit_nodes(inner_map_entry)[0]
+        outer_map_exit = graph.exit_nodes(outer_map_entry)[0]
 
         # Check that the destination of all the outgoing edges
         # from the inner map's exit is the outer map's exit.
         for _src, _, dest, _, _ in graph.out_edges(inner_map_exit):
             if dest != outer_map_exit:
                 return False
```

### Comparing `dace-0.9.0/dace/transformation/dataflow/map_dim_interchange.py` & `dace-0.9.5/dace/transformation/dataflow/map_dim_interchange.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """ Contains an implementation of the map-dimension-interchange transformation.
 """
 
 from dace.graph import nodes, nxutil
-from dace.properties import ShapeProperty
+from dace.properties import ShapeProperty, make_properties
 from dace.transformation import pattern_matching as pm
 
 
 @make_properties
 class MapDimInterchange(pm.Transformation):
     """ Implements the map-dimension-interchange pattern.
 
         Map-dimension-interchange re-orders the dimensions of a map.
     """
 
-    _map_entry = nodes.MapEntry(None)
+    _map_entry = nodes.MapEntry(nodes.Map("", [], []))
 
     order = ShapeProperty()
 
     @staticmethod
     def expressions():
         return [nxutil.node_path_graph(MapDimInterchange._map_entry)]
```

### Comparing `dace-0.9.0/dace/transformation/dataflow/map_interchange.py` & `dace-0.9.5/dace/transformation/dataflow/map_interchange.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Implements the map interchange transformation. """
 
 from copy import deepcopy as dcpy
 import dace
 from dace.graph import nodes, nxutil
+from dace.symbolic import symlist
 from dace.transformation import pattern_matching
 from dace.properties import make_properties
 
 
 @make_properties
 class MapInterchange(pattern_matching.Transformation):
     """ Implements the map-interchange transformation.
@@ -22,36 +23,51 @@
         return [
             nxutil.node_path_graph(MapInterchange._outer_map_entry,
                                    MapInterchange._inner_map_entry)
         ]
 
     @staticmethod
     def can_be_applied(graph, candidate, expr_index, sdfg, strict=False):
-        # TODO: Add matching condition that the map variables are independent
-        # of each other.
         # TODO: Assuming that the subsets on the edges between the two map
         # entries/exits are the union of separate inner subsets, is it possible
         # that inverting these edges breaks the continuity of union? What about
         # the opposite?
 
         # Check the edges between the entries of the two maps.
         outer_map_entry = graph.nodes()[candidate[
             MapInterchange._outer_map_entry]]
         inner_map_entry = graph.nodes()[candidate[
             MapInterchange._inner_map_entry]]
+
+        # Check that inner map range is independent of outer range
+        map_deps = set()
+        for s in inner_map_entry.map.range:
+            map_deps |= set(map(str, symlist(s)))
+        if any(dep in outer_map_entry.map.params for dep in map_deps):
+            return False
+
         # Check that the destination of all the outgoing edges
         # from the outer map's entry is the inner map's entry.
         for e in graph.out_edges(outer_map_entry):
             if e.dst != inner_map_entry:
                 return False
         # Check that the source of all the incoming edges
         # to the inner map's entry is the outer map's entry.
         for e in graph.in_edges(inner_map_entry):
             if e.src != outer_map_entry:
                 return False
+            # Check that dynamic input range memlets are independent of
+            # first map range
+            if e.dst_conn and not e.dst_conn.startswith('IN_'):
+                memlet_deps = set()
+                for s in e.data.subset:
+                    memlet_deps |= set(map(str, symlist(s)))
+                if any(dep in outer_map_entry.map.params
+                       for dep in memlet_deps):
+                    return False
 
         # Check the edges between the exits of the two maps.
         inner_map_exits = graph.exit_nodes(inner_map_entry)
         outer_map_exits = graph.exit_nodes(outer_map_entry)
         inner_map_exit = inner_map_exits[0]
         outer_map_exit = outer_map_exits[0]
```

### Comparing `dace-0.9.0/dace/transformation/dataflow/mapreduce.py` & `dace-0.9.5/dace/transformation/dataflow/mapreduce.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import copy
 from dace import data as dt, dtypes, subsets, symbolic
 from dace.memlet import Memlet
 from dace.graph import nodes, nxutil
 from dace.sdfg import SDFGState
 from dace.transformation import pattern_matching as pm
 from dace.properties import ShapeProperty
+from typing import List, Optional
 
 
 class MapReduceFusion(pm.Transformation):
     """ Implements the map-reduce-fusion transformation.
         Fuses a map with an immediately following reduction, where the array
         between the map and the reduction is not used anywhere else.
     """
@@ -148,14 +149,27 @@
         #        if map_range[1] != symbolic.pystr_to_symbolic(
         #                reduce.outslice[axis_after_reduce[dim]][1]):
         #            return False  # Range check (output axis)
         #    else:
         #        if map_range[1] != symbolic.pystr_to_symbolic(reduce.inslice[dim][1]):
         #            return False  # Range check (reduction axis)
 
+        # Map-Reduce
+        if expr_index == 2:
+            tasklet = graph.nodes()[candidate[MapReduceFusion._tasklet]]
+            tmem = next(
+                e for e in graph.edges_between(tasklet, tmap_exit)
+                if e.data.data == in_array.data).data
+            reduce_node = rmap_entry
+
+            # If memlet already has WCR and it is different from reduce node,
+            # do not match
+            if tmem.wcr is not None and tmem.wcr != reduce_node.wcr:
+                return False
+
         # Verify that reduction ranges match tasklet map
         tout_memlet = graph.in_edges(in_array)[0].data
         rin_memlet = graph.out_edges(in_array)[0].data
         if tout_memlet.subset != rin_memlet.subset:
             return False
 
         return True
@@ -169,17 +183,20 @@
         else:
             reduce = candidate[MapReduceFusion._rmap_in_cr]
 
         return ' -> '.join(str(node) for node in [tasklet, map_exit, reduce])
 
     @staticmethod
     def find_memlet_map_permutation(memlet: Memlet, map: nodes.Map):
-        perm = [None] * len(memlet.subset)
+        perm: List[int] = [None] * len(memlet.subset)
         indices = set()
         for i, dim in enumerate(memlet.subset):
+            if len(set(symbolic.symlist(dim)) & set(map.params)) == 0:
+                perm[i] = -1
+                continue
             if isinstance(memlet.subset, subsets.Range):
                 if memlet.subset.ranges[i][0] != memlet.subset.ranges[i][1]:
                     raise RuntimeError('Range found in MapReduceFusion')
                 dim = memlet.subset.ranges[i][0]
 
             for j, mapdim in enumerate(map.params):
                 if symbolic.pystr_to_symbolic(
@@ -227,37 +244,43 @@
     @staticmethod
     def find_permutation_reduce(tasklet_map: nodes.Map,
                                 reduce_node: nodes.Reduce, graph: SDFGState,
                                 tmem: Memlet):
 
         in_memlet = graph.in_edges(reduce_node)[0].data
         out_memlet = graph.out_edges(reduce_node)[0].data
-        assert len(tasklet_map.range) == in_memlet.subset.dims()
+        unrelated_axes = [
+            i for i, s in enumerate(tmem.subset)
+            if len(set(symbolic.symlist(s)) & set(tasklet_map.params)) == 0
+        ]
+
+        assert (len(tasklet_map.range) == in_memlet.subset.dims() -
+                len(unrelated_axes))
 
         # Find permutation between tasklet-exit memlet and tasklet map
         tmem_perm = MapReduceFusion.find_memlet_map_permutation(
             tmem, tasklet_map)
         mapred_perm = []
 
-        # Match map ranges with reduce ranges
+        # Match map ranges with reduce axes
         unavailable_ranges = set()
         for i, tmap_rng in enumerate(tasklet_map.range):
             found = False
 
             for j, in_rng in enumerate(in_memlet.subset):
                 if tmap_rng == in_rng and j not in unavailable_ranges:
                     mapred_perm.append(i)
                     unavailable_ranges.add(j)
                     found = True
                     break
             if not found: break
 
         # Ensure all map variables matched with reduce variables
         assert len(tmem_perm) == len(tmem.subset)
-        assert len(mapred_perm) == len(in_memlet.subset)
+        assert len(mapred_perm) == len(in_memlet.subset) - len(unrelated_axes)
 
         # Prepare result from the two permutations and the reduction axes
         result = []
         for i in range(len(mapred_perm)):
             if reduce_node.axes is None or i in reduce_node.axes:
                 continue
             result.append(mapred_perm[tmem_perm[i]])
@@ -346,39 +369,38 @@
             tmap_in_edges = list(graph.in_edges(tmap_entry))
             for e in tmap_in_edges:
                 nxutil.change_edge_dest(graph, tmap_entry, omap_entry)
             for e in tmap_in_edges:
                 graph.add_edge(omap_entry, e.src_conn, tmap_entry, e.dst_conn,
                                copy.copy(e.data))
         elif expr_index == 2:  # Reduce node
-            # Find correspondence between map indices and array outputs
-            tmap = tmap_exit.map
-            perm = MapReduceFusion.find_permutation_reduce(
-                tmap, rmap_cr, graph, memlet_edge.data)
-
-            output_subset = [tmap.params[d] for d in perm]
-            if len(output_subset) == 0:  # Output is a scalar
-                output_subset = [0]
-
+            # Find which indices should be removed from new memlet
+            input_edge = graph.in_edges(rmap_cr)[0]
+            axes = rmap_cr.axes or list(range(input_edge.data.subset))
             array_edge = graph.out_edges(rmap_cr)[0]
 
             # Delete relevant edges and nodes
-            graph.remove_edge(memlet_edge)
             graph.remove_nodes_from(nodes_to_remove)
 
-            # Add new edges and nodes
-            #   From tasklet to map exit
-            graph.add_edge(
-                memlet_edge.src, memlet_edge.src_conn, memlet_edge.dst,
-                memlet_edge.dst_conn,
-                Memlet(out_array.data, memlet_edge.data.num_accesses,
-                       subsets.Indices(output_subset), memlet_edge.data.veclen,
-                       rmap_cr.wcr, rmap_cr.identity))
+            # Filter out reduced dimensions from subset
+            filtered_subset = [
+                dim for i, dim in enumerate(memlet_edge.data.subset)
+                if i not in axes
+            ]
+            if len(filtered_subset) == 0:  # Output is a scalar
+                filtered_subset = [0]
+
+            # Modify edge from tasklet to map exit
+            memlet_edge.data.data = out_array.data
+            memlet_edge.data.wcr = rmap_cr.wcr
+            memlet_edge.data.wcr_identity = rmap_cr.identity
+            memlet_edge.data.subset = type(
+                memlet_edge.data.subset)(filtered_subset)
 
-            #   From map exit to output array
+            # Add edge from map exit to output array
             graph.add_edge(
                 memlet_edge.dst, 'OUT_' + memlet_edge.dst_conn[3:],
                 array_edge.dst, array_edge.dst_conn,
                 Memlet(array_edge.data.data, array_edge.data.num_accesses,
                        array_edge.data.subset, array_edge.data.veclen,
                        rmap_cr.wcr, rmap_cr.identity))
 
@@ -390,15 +412,16 @@
         nodes_to_remove = nodes_to_remove[1:]
 
         # Create tasklet -> tmp -> tasklet connection
         tmp = graph.add_array(
             'tmp',
             memlet_edge.data.subset.bounding_box_size(),
             sdfg.arrays[memlet_edge.data.data].dtype,
-            transient=True)
+            transient=True,
+            find_new_name=True)
         tasklet_tmp_memlet = copy.deepcopy(memlet_edge.data)
         tasklet_tmp_memlet.data = tmp.data
         tasklet_tmp_memlet.subset = ShapeProperty.to_string(tmp.shape)
 
         # Modify memlet to point to output array
         memlet_edge.data.data = out_array.data
```

### Comparing `dace-0.9.0/dace/transformation/dataflow/mpi.py` & `dace-0.9.5/dace/transformation/dataflow/mpi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Contains the MPITransformMap transformation. """
 
-from dace import dtypes, symbolic
+from dace import dtypes
+from dace.sdfg import has_dynamic_map_inputs
 from dace.graph import nodes, nxutil
 from dace.transformation import pattern_matching
 from dace.properties import make_properties
 
 
 @make_properties
 class MPITransformMap(pattern_matching.Transformation):
@@ -77,34 +78,39 @@
         sdict = graph.scope_dict()
         parent = sdict[map_entry]
         while parent is not None:
             if parent.map.schedule not in schedule_whitelist:
                 return False
             parent = sdict[parent]
 
+        # Dynamic map ranges not supported (will allocate dynamic memory)
+        if has_dynamic_map_inputs(graph, map_entry):
+            return False
+
+        # MPI schedules currently do not support WCR
+        map_exit = graph.exit_nodes(map_entry)[0]
+        if any(e.data.wcr for e in graph.out_edges(map_exit)):
+            return False
+
         return True
 
     @staticmethod
     def match_to_str(graph, candidate):
         map_entry = graph.nodes()[candidate[MPITransformMap._map_entry]]
 
         return map_entry.map.label
 
     def apply(self, sdfg):
         graph = sdfg.nodes()[self.state_id]
 
         map_entry = graph.nodes()[self.subgraph[MPITransformMap._map_entry]]
 
         # Avoiding import loops
-        from dace.transformation.dataflow import StripMining
-        from dace.transformation.dataflow.stream_transient import (
-            InLocalStorage)
-        from dace.transformation.dataflow.stream_transient import (
-            OutLocalStorage)
-        from dace.graph import labeling
+        from dace.transformation.dataflow.strip_mining import StripMining
+        from dace.transformation.dataflow.local_storage import LocalStorage
 
         rangeexpr = str(map_entry.map.range.num_elements())
 
         stripmine_subgraph = {
             StripMining._map_entry: self.subgraph[MPITransformMap._map_entry]
         }
         sdfg_id = sdfg.sdfg_list.index(sdfg)
@@ -121,58 +127,44 @@
         edges = [
             e for e in graph.in_edges(map_entry)
             if isinstance(e.src, nodes.EntryNode)
         ]
 
         outer_map = edges[0].src
 
-        # We need a tasklet for InLocalStorage
-        tasklet = None
-        for e in graph.out_edges(map_entry):
-            if isinstance(e.dst, nodes.CodeNode):
-                tasklet = e.dst
-                break
-
-        if tasklet is None:
-            raise ValueError("Tasklet not found")
-
         # Add MPI schedule attribute to outer map
         outer_map.map._schedule = dtypes.ScheduleType.MPI
 
         # Now create a transient for each array
         for e in edges:
             in_local_storage_subgraph = {
-                InLocalStorage._outer_map_entry:
-                graph.node_id(outer_map),
-                InLocalStorage._inner_map_entry:
-                self.subgraph[MPITransformMap._map_entry]
+                LocalStorage._node_a: graph.node_id(outer_map),
+                LocalStorage._node_b: self.subgraph[MPITransformMap._map_entry]
             }
             sdfg_id = sdfg.sdfg_list.index(sdfg)
-            in_local_storage = InLocalStorage(sdfg_id, self.state_id,
-                                              in_local_storage_subgraph,
-                                              self.expr_index)
+            in_local_storage = LocalStorage(sdfg_id, self.state_id,
+                                            in_local_storage_subgraph,
+                                            self.expr_index)
             in_local_storage.array = e.data.data
             in_local_storage.apply(sdfg)
 
         # Transform OutLocalStorage for each output of the MPI map
         in_map_exits = graph.exit_nodes(map_entry)
         out_map_exits = graph.exit_nodes(outer_map)
         in_map_exit = in_map_exits[0]
         out_map_exit = out_map_exits[0]
 
         for e in graph.out_edges(out_map_exit):
             name = e.data.data
             outlocalstorage_subgraph = {
-                OutLocalStorage._inner_map_exit: graph.node_id(in_map_exit),
-                OutLocalStorage._outer_map_exit: graph.node_id(out_map_exit)
+                LocalStorage._node_a: graph.node_id(in_map_exit),
+                LocalStorage._node_b: graph.node_id(out_map_exit)
             }
             sdfg_id = sdfg.sdfg_list.index(sdfg)
-            outlocalstorage = OutLocalStorage(sdfg_id, self.state_id,
-                                              outlocalstorage_subgraph,
-                                              self.expr_index)
+            outlocalstorage = LocalStorage(sdfg_id, self.state_id,
+                                           outlocalstorage_subgraph,
+                                           self.expr_index)
             outlocalstorage.array = name
             outlocalstorage.apply(sdfg)
 
-        return
-
 
 pattern_matching.Transformation.register_pattern(MPITransformMap)
```

### Comparing `dace-0.9.0/dace/transformation/dataflow/reduce_expansion.py` & `dace-0.9.5/dace/transformation/dataflow/reduce_expansion.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/dace/transformation/dataflow/redundant_array.py` & `dace-0.9.5/dace/transformation/dataflow/redundant_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         graph.remove_node(in_array)
         if Config.get_bool("debugprint"):
             RedundantArray._arrays_removed += 1
 
     @staticmethod
     def print_debuginfo():
         print(
-            "Automatically removed {} redundant arrays using RedundantArray transform.".
-            format(RedundantArray._arrays_removed))
+            "Automatically removed {} redundant arrays using RedundantArray transform."
+            .format(RedundantArray._arrays_removed))
 
     def modifies_graph(self):
         return True
 
 
 pm.Transformation.register_pattern(RedundantArray)
```

### Comparing `dace-0.9.0/dace/transformation/dataflow/redundant_array_copying.py` & `dace-0.9.5/dace/transformation/dataflow/redundant_array_copying.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,16 +115,16 @@
 
     def modifies_graph(self):
         return True
 
     @staticmethod
     def print_debuginfo():
         print(
-            "Automatically removed {} redundant arrays using RedundantArrayCopying transform.".
-            format(RedundantArrayCopying._arrays_removed))
+            "Automatically removed {} redundant arrays using RedundantArrayCopying transform."
+            .format(RedundantArrayCopying._arrays_removed))
 
 
 pm.Transformation.register_pattern(RedundantArrayCopying)
 
 
 class RedundantArrayCopying2(pm.Transformation):
     """ Implements the redundant array removal transformation. Removes 
@@ -184,16 +184,16 @@
 
     def modifies_graph(self):
         return True
 
     @staticmethod
     def print_debuginfo():
         print(
-            "Automatically removed {} redundant arrays using RedundantArrayCopying2 transform.".
-            format(RedundantArrayCopying2._arrays_removed))
+            "Automatically removed {} redundant arrays using RedundantArrayCopying2 transform."
+            .format(RedundantArrayCopying2._arrays_removed))
 
 
 pm.Transformation.register_pattern(RedundantArrayCopying2)
 
 
 class RedundantArrayCopying3(pm.Transformation):
     """ Implements the redundant array removal transformation. Removes multiples
@@ -254,12 +254,12 @@
 
     def modifies_graph(self):
         return True
 
     @staticmethod
     def print_debuginfo():
         print(
-            "Automatically removed {} redundant arrays using RedundantArrayCopying3 transform.".
-            format(RedundantArrayCopying3._arrays_removed))
+            "Automatically removed {} redundant arrays using RedundantArrayCopying3 transform."
+            .format(RedundantArrayCopying3._arrays_removed))
 
 
 pm.Transformation.register_pattern(RedundantArrayCopying3)
```

### Comparing `dace-0.9.0/dace/transformation/dataflow/strip_mining.py` & `dace-0.9.5/dace/transformation/dataflow/strip_mining.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ This module contains classes and functions that implement the strip-mining
     transformation."""
 
 import dace
 from copy import deepcopy as dcpy
 from dace import dtypes, subsets, symbolic
+from dace.sdfg import SDFG, SDFGState
 from dace.properties import make_properties, Property
 from dace.graph import nodes, nxutil
 from dace.transformation import pattern_matching
 from math import ceil
 import sympy
 import networkx as nx
 
@@ -31,14 +32,15 @@
     for a_range in array_range:
         new_range = a_range
         for m_idx, m_range in zip(map_idx, map_set):
             symbol = symbolic.pystr_to_symbolic(m_idx)
             new_range = [
                 new_range[i].subs(symbol,
                                   dace.symbolic.overapproximate(m_range[i]))
+                if dace.symbolic.issymbolic(new_range[i]) else new_range[i]
                 for i in range(0, 3)
             ]
         image.append(new_range)
     return subsets.Range(image)
 
 
 def calc_set_image(map_idx, map_set, array_set):
@@ -83,14 +85,19 @@
     # Properties
     dim_idx = Property(
         dtype=int, default=-1, desc="Index of dimension to be strip-mined")
     new_dim_prefix = Property(
         dtype=str, default="tile", desc="Prefix for new dimension name")
     tile_size = Property(
         dtype=str, default="64", desc="Tile size of strip-mined dimension")
+    tile_stride = Property(
+        dtype=str,
+        default="",
+        desc="Stride between two tiles of the "
+        "strip-mined dimension")
     divides_evenly = Property(
         dtype=bool,
         default=False,
         desc="Tile size divides dimension range evenly?")
     strided = Property(
         dtype=bool,
         default=False,
@@ -115,18 +122,15 @@
     def match_to_str(graph, candidate):
         map_entry = graph.nodes()[candidate[StripMining._map_entry]]
         return map_entry.map.label + ': ' + str(map_entry.map.params)
 
     def apply(self, sdfg):
         graph = sdfg.nodes()[self.state_id]
         # Strip-mine selected dimension.
-        target_dim, new_dim, new_map = self.__stripmine(
-            sdfg, graph, self.subgraph)
-        # Modify edges to match strip-mined dimension.
-        # StripMining.__modify_edges(sdfg, graph, self.subgraph, target_dim, new_dim)
+        _, _, new_map = self._stripmine(sdfg, graph, self.subgraph)
         return new_map
 
     # def __init__(self, tag=True):
     def __init__(self, *args, **kwargs):
         self._entry = nodes.EntryNode()
         self._tasklet = nodes.Tasklet('_')
         self._exit = nodes.ExitNode()
@@ -148,212 +152,181 @@
     def print_match_pattern(self, candidate):
         gentry = candidate[self.entry]
         return str(gentry.map.params[-1])
 
     def modifies_graph(self):
         return True
 
-    def __stripmine(self, sdfg, graph, candidate):
+    def _find_new_dim(self, sdfg: SDFG, state: SDFGState,
+                      entry: nodes.MapEntry, prefix: str, target_dim: str):
+        """ Finds a variable that is not already defined in scope. """
+        stree = state.scope_tree()
+        candidate = '%s_%s' % (prefix, target_dim)
+        index = 1
+        while candidate in map(str, stree[entry].defined_vars):
+            candidate = '%s%d_%s' % (prefix, index, target_dim)
+            index += 1
+        return candidate
+
+    def _stripmine(self, sdfg, graph, candidate):
 
         # Retrieve map entry and exit nodes.
         map_entry = graph.nodes()[candidate[StripMining._map_entry]]
-        map_exits = graph.exit_nodes(map_entry)
+        map_exit = graph.exit_nodes(map_entry)[0]
 
         # Retrieve transformation properties.
         dim_idx = self.dim_idx
         new_dim_prefix = self.new_dim_prefix
         tile_size = self.tile_size
         divides_evenly = self.divides_evenly
         strided = self.strided
 
+        tile_stride = self.tile_stride
+        if tile_stride is None or len(tile_stride) == 0:
+            tile_stride = tile_size
+
         # Retrieve parameter and range of dimension to be strip-mined.
         target_dim = map_entry.map.params[dim_idx]
         td_from, td_to, td_step = map_entry.map.range[dim_idx]
 
         # Create new map. Replace by cloning???
-        new_dim = new_dim_prefix + '_' + target_dim
+        new_dim = self._find_new_dim(sdfg, graph, map_entry, new_dim_prefix,
+                                     target_dim)
         nd_from = 0
         nd_to = symbolic.pystr_to_symbolic(
             'int_ceil(%s + 1 - %s, %s) - 1' %
-            (symbolic.symstr(td_to), symbolic.symstr(td_from), tile_size))
+            (symbolic.symstr(td_to), symbolic.symstr(td_from), tile_stride))
         nd_step = 1
         new_dim_range = (nd_from, nd_to, nd_step)
         new_map = nodes.Map(new_dim + '_' + map_entry.map.label, [new_dim],
                             subsets.Range([new_dim_range]))
         new_map_entry = nodes.MapEntry(new_map)
+        new_map_exit = nodes.MapExit(new_map)
 
         # Change the range of the selected dimension to iterate over a single
         # tile
         if strided:
             td_from_new = symbolic.pystr_to_symbolic(new_dim)
             td_to_new_approx = td_to
             td_step = symbolic.pystr_to_symbolic(tile_size)
         else:
             td_from_new = symbolic.pystr_to_symbolic(
                 '%s + %s * %s' % (symbolic.symstr(td_from), str(new_dim),
-                                  tile_size))
+                                  tile_stride))
             td_to_new_exact = symbolic.pystr_to_symbolic(
                 'min(%s + 1, %s + %s * %s + %s) - 1' %
-                (symbolic.symstr(td_to), symbolic.symstr(td_from), tile_size,
+                (symbolic.symstr(td_to), symbolic.symstr(td_from), tile_stride,
                  str(new_dim), tile_size))
             td_to_new_approx = symbolic.pystr_to_symbolic(
-                '%s + %s * %s + %s - 1' % (symbolic.symstr(td_from), tile_size,
-                                           str(new_dim), tile_size))
+                '%s + %s * %s + %s - 1' % (symbolic.symstr(td_from),
+                                           tile_stride, str(new_dim),
+                                           tile_size))
         if divides_evenly or strided:
             td_to_new = td_to_new_approx
         else:
             td_to_new = dace.symbolic.SymExpr(td_to_new_exact,
                                               td_to_new_approx)
         map_entry.map.range[dim_idx] = (td_from_new, td_to_new, td_step)
 
         # Make internal map's schedule to "not parallel"
-        map_entry.map._schedule = dtypes.ScheduleType.Default
+        new_map.schedule = map_entry.map.schedule
+        map_entry.map.schedule = dtypes.ScheduleType.Sequential
+
+        # Redirect edges
+        new_map_entry.in_connectors = dcpy(map_entry.in_connectors)
+        nxutil.change_edge_dest(graph, map_entry, new_map_entry)
+        new_map_exit.out_connectors = dcpy(map_exit.out_connectors)
+        nxutil.change_edge_src(graph, map_exit, new_map_exit)
 
-        # Redirect/create edges.
-        new_in_edges = {}
-        for _src, conn, _dest, _, memlet in graph.out_edges(map_entry):
-            if not isinstance(sdfg.arrays[memlet.data], dace.data.Scalar):
+        # Create new entry edges
+        new_in_edges = dict()
+        entry_in_conn = set()
+        entry_out_conn = set()
+        for _src, src_conn, _dst, _, memlet in graph.out_edges(map_entry):
+            if (src_conn is not None
+                    and src_conn[:4] == 'OUT_' and not isinstance(
+                        sdfg.arrays[memlet.data], dace.data.Scalar)):
                 new_subset = calc_set_image(
                     map_entry.map.params,
                     map_entry.map.range,
                     memlet.subset,
                 )
-                if memlet.data in new_in_edges:
-                    src, src_conn, dest, dest_conn, new_memlet, num = \
-                        new_in_edges[memlet.data]
-                    new_memlet.subset = calc_set_union(new_memlet.subset,
-                                                       new_subset)
+                conn = src_conn[4:]
+                key = (memlet.data, 'IN_' + conn, 'OUT_' + conn)
+                if key in new_in_edges.keys():
+                    old_subset = new_in_edges[key].subset
+                    new_in_edges[key].subset = calc_set_union(
+                        old_subset, new_subset)
+                else:
+                    entry_in_conn.add('IN_' + conn)
+                    entry_out_conn.add('OUT_' + conn)
+                    new_memlet = dcpy(memlet)
+                    new_memlet.subset = new_subset
                     new_memlet.num_accesses = new_memlet.num_elements()
-                    new_in_edges.update({
-                        memlet.data: (src, src_conn, dest, dest_conn,
-                                      new_memlet, min(num, int(conn[4:])))
-                    })
+                    new_in_edges[key] = new_memlet
+            else:
+                if src_conn is not None and src_conn[:4] == 'OUT_':
+                    conn = src_conn[4:]
+                    in_conn = 'IN_' + conn
+                    out_conn = 'OUT_' + conn
                 else:
+                    in_conn = src_conn
+                    out_conn = src_conn
+                if in_conn:
+                    entry_in_conn.add(in_conn)
+                if out_conn:
+                    entry_out_conn.add(out_conn)
+                new_in_edges[(memlet.data, in_conn, out_conn)] = dcpy(memlet)
+        new_map_entry.out_connectors = entry_out_conn
+        map_entry.in_connectors = entry_in_conn
+        for (_, in_conn, out_conn), memlet in new_in_edges.items():
+            graph.add_edge(new_map_entry, out_conn, map_entry, in_conn, memlet)
+
+        # Create new exit edges
+        new_out_edges = dict()
+        exit_in_conn = set()
+        exit_out_conn = set()
+        for _src, _, _dst, dst_conn, memlet in graph.in_edges(map_exit):
+            if (dst_conn is not None
+                    and dst_conn[:3] == 'IN_' and not isinstance(
+                        sdfg.arrays[memlet.data], dace.data.Scalar)):
+                new_subset = calc_set_image(
+                    map_entry.map.params,
+                    map_entry.map.range,
+                    memlet.subset,
+                )
+                conn = dst_conn[3:]
+                key = (memlet.data, 'IN_' + conn, 'OUT_' + conn)
+                if key in new_out_edges.keys():
+                    old_subset = new_out_edges[key].subset
+                    new_out_edges[key].subset = calc_set_union(
+                        old_subset, new_subset)
+                else:
+                    exit_in_conn.add('IN_' + conn)
+                    exit_out_conn.add('OUT_' + conn)
                     new_memlet = dcpy(memlet)
                     new_memlet.subset = new_subset
                     new_memlet.num_accesses = new_memlet.num_elements()
-                    new_in_edges.update({
-                        memlet.data: (new_map_entry, None, map_entry, None,
-                                      new_memlet, int(conn[4:]))
-                    })
-        nxutil.change_edge_dest(graph, map_entry, new_map_entry)
-
-        new_out_edges = {}
-        new_exits = []
-        for map_exit in map_exits:
-            if isinstance(map_exit, nodes.MapExit):
-                new_exit = nodes.MapExit(new_map)
-                new_exits.append(new_exit)
-            for _src, conn, _dest, _, memlet in graph.in_edges(map_exit):
-                if not isinstance(sdfg.arrays[memlet.data], dace.data.Scalar):
-                    new_subset = calc_set_image(
-                        map_entry.map.params,
-                        map_entry.map.range,
-                        memlet.subset,
-                    )
-                    if memlet.data in new_out_edges:
-                        src, src_conn, dest, dest_conn, new_memlet, num = \
-                            new_out_edges[memlet.data]
-                        new_memlet.subset = calc_set_union(
-                            new_memlet.subset, new_subset)
-                        new_memlet.num_accesses = new_memlet.num_elements()
-                        new_out_edges.update({
-                            memlet.data: (src, src_conn, dest, dest_conn,
-                                          new_memlet, min(num, conn[4:]))
-                        })
-                    else:
-                        new_memlet = dcpy(memlet)
-                        new_memlet.subset = new_subset
-                        new_memlet.num_accesses = new_memlet.num_elements()
-                        new_out_edges.update({
-                            memlet.data: (map_exit, None, new_exit, None,
-                                          new_memlet, conn[4:])
-                        })
-            nxutil.change_edge_src(graph, map_exit, new_exit)
-
-        in_conn_nums = []
-        for _, e in new_in_edges.items():
-            _, _, _, _, _, num = e
-            in_conn_nums.append(num)
-        in_conn = {}
-        for i, num in enumerate(in_conn_nums):
-            in_conn.update({num: i + 1})
-
-        entry_in_connectors = set()
-        entry_out_connectors = set()
-        for i in range(len(in_conn_nums)):
-            entry_in_connectors.add('IN_' + str(i + 1))
-            entry_out_connectors.add('OUT_' + str(i + 1))
-        new_map_entry.in_connectors = entry_in_connectors
-        new_map_entry.out_connectors = entry_out_connectors
-
-        for _, e in new_in_edges.items():
-            src, _, dst, _, memlet, num = e
-            graph.add_edge(src, 'OUT_' + str(in_conn[num]), dst,
-                           'IN_' + str(in_conn[num]), memlet)
-
-        for new_exit in new_exits:
-
-            out_conn_nums = []
-            for _, e in new_out_edges.items():
-                _, _, dst, _, _, num = e
-                if dst is not new_exit:
-                    continue
-                out_conn_nums.append(num)
-            out_conn = {}
-            for i, num in enumerate(out_conn_nums):
-                out_conn.update({num: i + 1})
-
-            exit_in_connectors = set()
-            exit_out_connectors = set()
-            for i in range(len(out_conn_nums)):
-                exit_in_connectors.add('IN_' + str(i + 1))
-                exit_out_connectors.add('OUT_' + str(i + 1))
-            new_exit.in_connectors = exit_in_connectors
-            new_exit.out_connectors = exit_out_connectors
-
-            for _, e in new_out_edges.items():
-                src, _, dst, _, memlet, num = e
-                graph.add_edge(src, 'OUT_' + str(out_conn[num]), dst,
-                               'IN_' + str(out_conn[num]), memlet)
+                    new_out_edges[key] = new_memlet
+            else:
+                if dst_conn is not None and dst_conn[:3] == 'IN_':
+                    conn = dst_conn[3:]
+                    in_conn = 'IN_' + conn
+                    out_conn = 'OUT_' + conn
+                else:
+                    in_conn = src_conn
+                    out_conn = src_conn
+                if in_conn:
+                    exit_in_conn.add(in_conn)
+                if out_conn:
+                    exit_out_conn.add(out_conn)
+                new_in_edges[(memlet.data, in_conn, out_conn)] = dcpy(memlet)
+        new_map_exit.in_connectors = exit_in_conn
+        map_exit.out_connectors = exit_out_conn
+        for (_, in_conn, out_conn), memlet in new_out_edges.items():
+            graph.add_edge(map_exit, out_conn, new_map_exit, in_conn, memlet)
 
         # Return strip-mined dimension.
         return target_dim, new_dim, new_map
 
-    @staticmethod
-    def __modify_edges(sdfg, graph, candidate, target_dim, new_dim):
-        map_entry = graph.nodes()[candidate[StripMining._map_entry]]
-
-        processed = []
-        for src, _dest, memlet, _scope in nxutil.traverse_sdfg_scope(
-                graph, map_entry, True):
-            if memlet in processed:
-                continue
-            processed.append(memlet)
-
-            # Corner cases
-            if isinstance(sdfg.arrays[memlet.data], dace.data.Stream):
-                continue
-            if memlet.wcr is not None:
-                memlet.num_accesses = 1
-                continue
-
-            for i, dim in enumerate(memlet.subset):
-                if isinstance(dim, tuple):
-                    dim = tuple(
-                        symbolic.pystr_to_symbolic(d).subs(
-                            symbolic.pystr_to_symbolic(target_dim),
-                            symbolic.pystr_to_symbolic(
-                                '%s + %s' % (str(new_dim), str(target_dim))))
-                        for d in dim)
-                else:
-                    dim = symbolic.pystr_to_symbolic(dim).subs(
-                        symbolic.pystr_to_symbolic(target_dim),
-                        symbolic.pystr_to_symbolic(
-                            '%s + %s' % (str(new_dim), str(target_dim))))
-
-                memlet.subset[i] = dim
-
-        return
-
 
 pattern_matching.Transformation.register_pattern(StripMining)
```

### Comparing `dace-0.9.0/dace/transformation/dataflow/tensorflow_redundant_array.py` & `dace-0.9.5/dace/transformation/dataflow/tensorflow_redundant_array.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,12 +97,12 @@
 
     def modifies_graph(self):
         return True
 
     @staticmethod
     def print_debuginfo():
         print(
-            "Automatically removed {} tensorflow redundant arrays using TensorflowRedundantArray transform.".
-            format(TensorflowRedundantArray._arrays_removed))
+            "Automatically removed {} tensorflow redundant arrays using TensorflowRedundantArray transform."
+            .format(TensorflowRedundantArray._arrays_removed))
 
 
 pm.Transformation.register_pattern(TensorflowRedundantArray)
```

### Comparing `dace-0.9.0/dace/transformation/interstate/fpga_transform_sdfg.py` & `dace-0.9.5/dace/transformation/interstate/fpga_transform_sdfg.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,14 +21,24 @@
     @staticmethod
     def expressions():
         # Match anything
         return [nx.DiGraph()]
 
     @staticmethod
     def can_be_applied(graph, candidate, expr_index, sdfg, strict=False):
+        # Avoid import loops
+        from dace.transformation.interstate import FPGATransformState
+
+        # Condition match depends on matching FPGATransformState for each state
+        for state_id, state in enumerate(sdfg.nodes()):
+            candidate = {FPGATransformState._state: state_id}
+            if not FPGATransformState.can_be_applied(sdfg, candidate,
+                                                     expr_index, sdfg):
+                return False
+
         return True
 
     @staticmethod
     def match_to_str(graph, candidate):
         return graph.label
 
     def apply(self, sdfg):
```

### Comparing `dace-0.9.0/dace/transformation/interstate/gpu_transform_sdfg.py` & `dace-0.9.5/dace/transformation/interstate/gpu_transform_sdfg.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,20 +29,23 @@
           7. Make data ready for interstate edges that use them
           8. Re-apply strict transformations to get rid of extra states and
              transients
     """
 
     toplevel_trans = Property(
         desc="Make all GPU transients top-level", dtype=bool, default=True)
+
     register_trans = Property(
         desc="Make all transients inside GPU maps registers",
         dtype=bool,
         default=True)
+
     sequential_innermaps = Property(
         desc="Make all internal maps Sequential", dtype=bool, default=True)
+
     strict_transform = Property(
         desc='Reapply strict transformations after modifying graph',
         dtype=bool,
         default=True)
 
     exclude_copyin = Property(
         desc="Exclude these arrays from being copied into the device"
@@ -64,14 +67,28 @@
     @staticmethod
     def expressions():
         # Matches anything
         return [sd.SDFG('_')]
 
     @staticmethod
     def can_be_applied(graph, candidate, expr_index, sdfg, strict=False):
+        for node, _ in sdfg.all_nodes_recursive():
+            # Consume scopes are currently unsupported
+            if isinstance(node, (nodes.ConsumeEntry, nodes.ConsumeExit)):
+                return False
+
+        for state in sdfg.nodes():
+            sdict = state.scope_dict(node_to_children=True)
+            for node in sdict[None]:
+                # If two top-level tasklets are connected with a code->code
+                # memlet, they will transform into an invalid SDFG
+                if (isinstance(node, nodes.CodeNode) and any(
+                        isinstance(e.dst, nodes.CodeNode)
+                        for e in state.out_edges(node))):
+                    return False
         return True
 
     @staticmethod
     def match_to_str(graph, candidate):
         return graph.label
 
     def modifies_graph(self):
@@ -90,15 +107,24 @@
         for i, state in enumerate(sdfg.nodes()):
             sdict = state.scope_dict()
             for node in state.nodes():
                 if (isinstance(node, nodes.AccessNode)
                         and node.desc(sdfg).transient == False):
                     if (state.out_degree(node) > 0
                             and node.data not in input_nodes):
-                        input_nodes.append((node.data, node.desc(sdfg)))
+                        # Special case: nodes that lead to dynamic map ranges
+                        # must stay on host
+                        for e in state.out_edges(node):
+                            last_edge = state.memlet_path(e)[-1]
+                            if (isinstance(last_edge.dst, nodes.EntryNode)
+                                    and last_edge.dst_conn and
+                                    not last_edge.dst_conn.startswith('IN_')):
+                                break
+                        else:
+                            input_nodes.append((node.data, node.desc(sdfg)))
                     if (state.in_degree(node) > 0
                             and node.data not in output_nodes):
                         output_nodes.append((node.data, node.desc(sdfg)))
                 elif isinstance(node, nodes.CodeNode) and sdict[node] is None:
                     if not isinstance(node, nodes.EmptyTasklet):
                         global_code_nodes[i].append(node)
 
@@ -114,28 +140,32 @@
         end_states = sdfg.sink_nodes()
 
         #######################################################
         # Step 1: Create cloned GPU arrays and replace originals
 
         cloned_arrays = {}
         for inodename, inode in set(input_nodes):
+            if isinstance(inode, data.Scalar):  # Scalars can remain on host
+                continue
             newdesc = inode.clone()
             newdesc.storage = dtypes.StorageType.GPU_Global
             newdesc.transient = True
-            sdfg.add_datadesc('gpu_' + inodename, newdesc)
-            cloned_arrays[inodename] = 'gpu_' + inodename
+            name = sdfg.add_datadesc(
+                'gpu_' + inodename, newdesc, find_new_name=True)
+            cloned_arrays[inodename] = name
 
         for onodename, onode in set(output_nodes):
             if onodename in cloned_arrays:
                 continue
             newdesc = onode.clone()
             newdesc.storage = dtypes.StorageType.GPU_Global
             newdesc.transient = True
-            sdfg.add_datadesc('gpu_' + onodename, newdesc)
-            cloned_arrays[onodename] = 'gpu_' + onodename
+            name = sdfg.add_datadesc(
+                'gpu_' + onodename, newdesc, find_new_name=True)
+            cloned_arrays[onodename] = name
 
         # Replace nodes
         for state in sdfg.nodes():
             for node in state.nodes():
                 if (isinstance(node, nodes.AccessNode)
                         and node.data in cloned_arrays):
                     node.data = cloned_arrays[node.data]
@@ -149,16 +179,16 @@
         #######################################################
         # Step 2: Create copy-in state
         excluded_copyin = self.exclude_copyin.split(',')
 
         copyin_state = sdfg.add_state(sdfg.label + '_copyin')
         sdfg.add_edge(copyin_state, start_state, ed.InterstateEdge())
 
-        for nname, desc in set(input_nodes):
-            if nname in excluded_copyin:
+        for nname, desc in dtypes.deduplicate(input_nodes):
+            if nname in excluded_copyin or nname not in cloned_arrays:
                 continue
             src_array = nodes.AccessNode(nname, debuginfo=desc.debuginfo)
             dst_array = nodes.AccessNode(
                 cloned_arrays[nname], debuginfo=desc.debuginfo)
             copyin_state.add_node(src_array)
             copyin_state.add_node(dst_array)
             copyin_state.add_nedge(
@@ -169,16 +199,16 @@
         # Step 3: Create copy-out state
         excluded_copyout = self.exclude_copyout.split(',')
 
         copyout_state = sdfg.add_state(sdfg.label + '_copyout')
         for state in end_states:
             sdfg.add_edge(state, copyout_state, ed.InterstateEdge())
 
-        for nname, desc in set(output_nodes):
-            if nname in excluded_copyout:
+        for nname, desc in dtypes.deduplicate(output_nodes):
+            if nname in excluded_copyout or nname not in cloned_arrays:
                 continue
             src_array = nodes.AccessNode(
                 cloned_arrays[nname], debuginfo=desc.debuginfo)
             dst_array = nodes.AccessNode(nname, debuginfo=desc.debuginfo)
             copyout_state.add_node(src_array)
             copyout_state.add_node(dst_array)
             copyout_state.add_nedge(
@@ -249,23 +279,24 @@
                     state.add_edge(mx, 'OUT_' + e.src_conn, e.dst, e.dst_conn,
                                    e.data)
 
                 # Map without inputs
                 if len(in_edges) == 0:
                     state.add_nedge(me, gcode, memlet.EmptyMemlet())
         #######################################################
-        # Step 6: Change all top-level maps to GPU maps
+        # Step 6: Change all top-level maps and Reduce nodes to GPU schedule
 
         for i, state in enumerate(sdfg.nodes()):
             sdict = state.scope_dict()
             for node in state.nodes():
-                if isinstance(node, nodes.EntryNode):
+                if isinstance(node, (nodes.EntryNode, nodes.Reduce)):
                     if sdict[node] is None:
                         node.schedule = dtypes.ScheduleType.GPU_Device
-                    elif self.sequential_innermaps:
+                    elif (isinstance(node, nodes.EntryNode)
+                          and self.sequential_innermaps):
                         node.schedule = dtypes.ScheduleType.Sequential
 
         #######################################################
         # Step 7: Introduce copy-out if data used in outgoing interstate edges
 
         for state in list(sdfg.nodes()):
             arrays_used = set()
@@ -301,34 +332,11 @@
 
         #######################################################
         # Step 8: Strict transformations
         if not self.strict_transform:
             return
 
         # Apply strict state fusions greedily.
-        opt = optimizer.SDFGOptimizer(sdfg, inplace=True)
-        fusions = 0
-        arrays = 0
-        options = [
-            match for match in opt.get_pattern_matches(strict=True)
-            if isinstance(match, (StateFusion, RedundantArray))
-        ]
-        while options:
-            ssdfg = sdfg.sdfg_list[options[0].sdfg_id]
-            options[0].apply(ssdfg)
-            ssdfg.validate()
-            if isinstance(options[0], StateFusion):
-                fusions += 1
-            if isinstance(options[0], RedundantArray):
-                arrays += 1
-
-            options = [
-                match for match in opt.get_pattern_matches(strict=True)
-                if isinstance(match, (StateFusion, RedundantArray))
-            ]
-
-        if Config.get_bool('debugprint') and (fusions > 0 or arrays > 0):
-            print('Automatically applied {} strict state fusions and removed'
-                  ' {} redundant arrays.'.format(fusions, arrays))
+        sdfg.apply_strict_transformations()
 
 
 pattern_matching.Transformation.register_stateflow_pattern(GPUTransformSDFG)
```

### Comparing `dace-0.9.0/dace/transformation/interstate/state_fusion.py` & `dace-0.9.5/dace/transformation/interstate/state_fusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         in_edges = graph.in_edges(first_state)
 
         # First state must have only one output edge (with dst the second
         # state).
         if len(out_edges) != 1:
             return False
         # The interstate edge must not have a condition.
-        if out_edges[0].data.condition.as_string != "":
+        if not out_edges[0].data.is_unconditional():
             return False
         # The interstate edge may have assignments, as long as there are input
         # edges to the first state, that can absorb them.
         if out_edges[0].data.assignments and not in_edges:
             return False
         # There can be no state that have output edges pointing to both the
         # first and the second state. Such a case will produce a multi-graph.
@@ -189,14 +189,19 @@
         first_input = [
             node for node in first_input
             if next((x for x in first_output
                      if x.label == node.label), None) is None
         ]
 
         # Merge second state to first state
+        # First keep a backup of the topological sorted order of the nodes
+        order = [
+            x for x in reversed(list(nx.topological_sort(first_state._nx)))
+            if isinstance(x, nodes.AccessNode)
+        ]
         for node in second_state.nodes():
             first_state.add_node(node)
         for src, src_conn, dst, dst_conn, data in second_state.edges():
             first_state.add_edge(src, src_conn, dst, dst_conn, data)
 
         # Merge common (data) nodes
         for node in first_input:
@@ -213,14 +218,22 @@
                 new_node = next(
                     x for x in second_input if x.label == node.label)
             except StopIteration:
                 continue
             nxutil.change_edge_dest(first_state, node, new_node)
             first_state.remove_node(node)
             second_input.remove(new_node)
+        # Check if any input nodes of the second state have to be merged with
+        # non-input/output nodes of the first state.
+        for node in second_input:
+            if first_state.in_degree(node) == 0:
+                n = next((x for x in order if x.label == node.label), None)
+                if n:
+                    nxutil.change_edge_src(first_state, node, n)
+                    first_state.remove_node(node)
 
         # Redirect edges and remove second state
         nxutil.change_edge_src(sdfg, second_state, first_state)
         sdfg.remove_node(second_state)
         if Config.get_bool("debugprint"):
             StateFusion._states_fused += 1
```

### Comparing `dace-0.9.0/dace/transformation/optimizer.py` & `dace-0.9.5/dace/transformation/optimizer.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,113 +5,221 @@
 import os
 import re
 import time
 
 import dace
 from dace.config import Config
 from dace.graph import labeling
+from dace.graph.graph import SubgraphView
 from dace.transformation import pattern_matching
 
 # This import is necessary since it registers all the patterns
 from dace.transformation import dataflow, interstate
 
 
-class SDFGOptimizer(object):
+class Optimizer(object):
     """ Implements methods for optimizing a DaCe program stateful dataflow
         graph representation, by matching patterns and applying 
         transformations on it.
     """
 
     def __init__(self, sdfg, inplace=False):
         """ Constructs an SDFG optimizer.
-            @param sdfg: The SDFG to transform.
-            @param inplace: If True, performs transformations on the given SDFG
+            :param sdfg: The SDFG to transform.
+            :param inplace: If True, performs transformations on the given SDFG
                             in-place. Uses a copy of the SDFG otherwise, and
                             stores it as `self.sdfg`.
         """
         if inplace == True:
             self.sdfg = sdfg
         else:
             self.sdfg = copy.deepcopy(sdfg)
 
         # Initialize patterns to search for
         self.patterns = pattern_matching.Transformation.patterns()
         self.stateflow_patterns = pattern_matching.Transformation.stateflow_patterns(
         )
         self.applied_patterns = set()
 
-    def get_pattern_matches(self, strict=False, states=None, patterns=None):
+    def optimize(self):
+        # Should be implemented by subclass
+        raise NotImplementedError
+
+    def get_pattern_matches(self,
+                            strict=False,
+                            states=None,
+                            patterns=None,
+                            sdfg=None):
         """ Returns all possible transformations for the current SDFG.
-            @param strict: Only consider strict transformations (i.e., ones
+            :param strict: Only consider strict transformations (i.e., ones
                            that surely increase performance or enhance
                            readability)
-            @param states: An iterable of SDFG states to consider when pattern
+            :param states: An iterable of SDFG states to consider when pattern
                            matching. If None, considers all.
-            @param patterns: An iterable of transformation classes to consider
+            :param patterns: An iterable of transformation classes to consider
                              when matching. If None, considers all registered
                              transformations in `Transformation`.
-            @return: List of matching `Transformation` objects.
+            :param sdfg: If not None, searches for patterns on given SDFG.
+            :return: List of matching `Transformation` objects.
             @see: Transformation
         """
-
-        matches = []
+        sdfg = sdfg or self.sdfg
 
         if states is None:
             if patterns is None:
                 _patterns = self.stateflow_patterns
             else:
                 _patterns = [
                     p for p in patterns if p in self.stateflow_patterns
                 ]
 
             for pattern in _patterns:
                 yield from pattern_matching.match_stateflow_pattern(
-                    self.sdfg, pattern, strict=strict)
+                    sdfg, pattern, strict=strict)
 
         state_enum = []
         if states is None:
-            for state_id, state in enumerate(self.sdfg.nodes()):
+            for state_id, state in enumerate(sdfg.nodes()):
                 state_enum.append((state_id, state))
         else:
             for state in states:
-                state_id = self.sdfg.nodes().index(state)
+                state_id = sdfg.nodes().index(state)
                 state_enum.append((state_id, state))
 
         if patterns is None:
             _patterns = self.patterns
         else:
             _patterns = [p for p in patterns if p in self.patterns]
         for state_id, state in state_enum:
             for pattern in _patterns:
                 yield from pattern_matching.match_pattern(
-                    state_id, state, pattern, self.sdfg, strict=strict)
+                    state, pattern, sdfg, strict=strict)
+
+    def optimization_space(self):
+        """ Returns the optimization space of the current SDFG """
+
+        def get_actions(actions, graph, match):
+            subgraph_node_ids = match.subgraph.values()
+            subgraph_nodes = [graph.nodes()[nid] for nid in subgraph_node_ids]
+            for node in subgraph_nodes:
+                version = 0
+                while (node, type(match).__name__, match.expr_index,
+                       version) in actions.keys():
+                    version += 1
+                actions[(node, type(match).__name__, match.expr_index,
+                         version)] = match
+            subgraph = SubgraphView(graph, subgraph_nodes)
+            for edge in subgraph.edges():
+                version = 0
+                while (edge, type(match).__name__, match.expr_index,
+                       version) in actions.keys():
+                    version += 1
+                actions[(edge, type(match).__name__, match.expr_index,
+                         version)] = match
+            return actions
+
+        def get_dataflow_actions(actions, sdfg, match):
+            graph = sdfg.sdfg_list[match.sdfg_id].nodes()[match.state_id]
+            return get_actions(actions, graph, match)
+
+        def get_stateflow_actions(actions, sdfg, match):
+            graph = sdfg.sdfg_list[match.sdfg_id]
+            return get_actions(actions, graph, match)
+
+        actions = dict()
+
+        for match in self.get_pattern_matches():
+            if match.state_id >= 0:
+                actions = get_dataflow_actions(actions, self.sdfg, match)
+            else:
+                actions = get_stateflow_actions(actions, self.sdfg, match)
+
+        return actions
+
+
+def _parse_cli_input(line):
+    """ Parses a command line input, which may include a transformation name
+        (optional), its occurrence ID, and its parameters (optional).
+        Syntax Examples:
+            * 5                  - Chooses the fifth transformation
+            * MapReduceFusion$0  - First occurrence of MapReduceFusion
+            * 4(array='A')       - Transformation number 4 with one parameter
+            * StripMining$1(param='i', tile_size=64) - Strip mining #2 with
+                                                       parameters
+        :param line: Input line string
+        :return: A tuple with (transformation name or None if not given,
+                                      occurrence or -1 if not given,
+                                      parameter dictionary or {} if not given)
+    """
+    # First try matching explicit all-inclusive string "A$num(values)"
+    match = re.findall(r'(.*)\$(\d+)\((.*)\)', line)
+    if len(match) == 1:
+        trans_name, occurrence, param_dict = match[0]
+    else:
+        # Then, try to match "num(values)"
+        match = re.findall(r'(\d+)\((.*)\)', line)
+        if len(match) == 1:
+            trans_name = None
+            occurrence, param_dict = match[0]
+        else:
+            # After that, try to match "A$num"
+            match = re.findall(r'(.*)\$(\d+)', line)
+            if len(match) == 1:
+                trans_name, occurrence = match[0]
+                param_dict = {}
+            else:
+                # Finally, try to match "num"
+                match = re.findall(r'(\d+)', line)
+                if len(match) == 1:
+                    trans_name = None
+                    occurrence = match[0]
+                    param_dict = {}
+                else:
+                    return (None, -1, {})
+
+    # Try to parse the results
+    try:
+        occurrence = int(occurrence)
+    except ValueError:
+        occurrence = -1
+    try:
+        if isinstance(param_dict, str):
+            param_dict = eval('dict(' + param_dict + ')')
+    except:  # Here we have to catch ANY exception since literally anything
+        # can happen
+        param_dict = {}
+
+    return trans_name, occurrence, param_dict
 
-    def optimize(self, debugprint=True):
+
+class SDFGOptimizer(Optimizer):
+    def optimize(self):
         """ A command-line UI for applying patterns on the SDFG.
-            @param debugprint: Whether to print verbose information to the 
-                               console.
-            @return: An optimized SDFG object
+            :return: An optimized SDFG object
         """
         sdfg_file = self.sdfg.name + '.sdfg'
         if os.path.isfile(sdfg_file):
             ui_input = input(
                 'An SDFG with the filename "%s" was found. '
                 'Would you like to use it instead? [Y/n] ' % sdfg_file)
             if len(ui_input) == 0 or ui_input[0] not in ['n', 'N']:
                 return dace.SDFG.from_file(sdfg_file)
 
         # Visualize SDFGs during optimization process
         VISUALIZE = Config.get_bool('optimizer', 'visualize')
+        VISUALIZE_SDFV = Config.get_bool('optimizer', 'visualize_sdfv')
         SAVE_DOTS = Config.get_bool('optimizer', 'savedots')
 
         if SAVE_DOTS:
-            with open('before.dot', 'w') as dot_file:
-                dot_file.write(self.sdfg.draw())
+            self.sdfg.draw_to_file('before.dot')
+            self.sdfg.save(os.path.join('_dotgraphs', 'before.sdfg'))
             if VISUALIZE:
-                os.system('xdot before.dot&')
+                os.system('xdot _dotgraphs/before.dot&')
+            if VISUALIZE_SDFV:
+                os.system('sdfv _dotgraphs/before.sdfg&')
 
         # Optimize until there is not pattern matching or user stops the process.
         pattern_counter = 0
         while True:
             # Print in the UI all the pattern matching options.
             ui_options = sorted(self.get_pattern_matches())
             ui_options_idx = 0
@@ -161,82 +269,36 @@
             for k, v in param_dict.items():
                 setattr(pattern_match, k, v)
 
             pattern_match.apply(sdfg)
             self.applied_patterns.add(type(pattern_match))
 
             if SAVE_DOTS:
-                self.sdfg.draw_to_file(
-                    'after_%d_%s_b4lprop.dot' % (pattern_counter + 1,
-                                                 type(pattern_match).__name__))
+                filename = 'after_%d_%s_b4lprop' % (
+                    pattern_counter + 1, type(pattern_match).__name__)
+                self.sdfg.save(os.path.join('_dotgraphs', filename + '.sdfg'))
+                self.sdfg.draw_to_file(filename + '.dot')
 
             if not pattern_match.annotates_memlets():
                 labeling.propagate_labels_sdfg(self.sdfg)
 
             if True:
                 pattern_counter += 1
                 if SAVE_DOTS:
-                    self.sdfg.draw_to_file(
-                        'after_%d_%s.dot' % (pattern_counter,
-                                             type(pattern_match).__name__))
+                    filename = 'after_%d_%s' % (pattern_counter,
+                                                type(pattern_match).__name__)
+                    self.sdfg.save(
+                        os.path.join('_dotgraphs', filename + '.sdfg'))
+                    self.sdfg.draw_to_file(filename + '.dot')
+
                     if VISUALIZE:
                         time.sleep(0.7)
                         os.system(
                             'xdot _dotgraphs/after_%d_%s.dot&' %
                             (pattern_counter, type(pattern_match).__name__))
 
-        return self.sdfg
-
-
-def _parse_cli_input(line):
-    """ Parses a command line input, which may include a transformation name
-        (optional), its occurrence ID, and its parameters (optional).
-        Syntax Examples:
-            * 5                  - Chooses the fifth transformation
-            * MapReduceFusion$0  - First occurrence of MapReduceFusion
-            * 4(array='A')       - Transformation number 4 with one parameter
-            * StripMining$1(param='i', tile_size=64) - Strip mining #2 with
-                                                       parameters
-        @param line: Input line string
-        @return: A tuple with (transformation name or None if not given,
-                                      occurrence or -1 if not given,
-                                      parameter dictionary or {} if not given)
-    """
-    # First try matching explicit all-inclusive string "A$num(values)"
-    match = re.findall(r'(.*)\$(\d+)\((.*)\)', line)
-    if len(match) == 1:
-        trans_name, occurrence, param_dict = match[0]
-    else:
-        # Then, try to match "num(values)"
-        match = re.findall(r'(\d+)\((.*)\)', line)
-        if len(match) == 1:
-            trans_name = None
-            occurrence, param_dict = match[0]
-        else:
-            # After that, try to match "A$num"
-            match = re.findall(r'(.*)\$(\d+)', line)
-            if len(match) == 1:
-                trans_name, occurrence = match[0]
-                param_dict = {}
-            else:
-                # Finally, try to match "num"
-                match = re.findall(r'(\d+)', line)
-                if len(match) == 1:
-                    trans_name = None
-                    occurrence = match[0]
-                    param_dict = {}
-                else:
-                    return (None, -1, {})
-
-    # Try to parse the results
-    try:
-        occurrence = int(occurrence)
-    except ValueError:
-        occurrence = -1
-    try:
-        if isinstance(param_dict, str):
-            param_dict = eval('dict(' + param_dict + ')')
-    except:  # Here we have to catch ANY exception since literally anything
-        # can happen
-        param_dict = {}
+                    if VISUALIZE_SDFV:
+                        os.system(
+                            'sdfv _dotgraphs/after_%d_%s.sdfg&' %
+                            (pattern_counter, type(pattern_match).__name__))
 
-    return trans_name, occurrence, param_dict
+        return self.sdfg
```

### Comparing `dace-0.9.0/dace/transformation/pattern_matching.py` & `dace-0.9.5/dace/transformation/pattern_matching.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Contains classes and functions related to patterns/transformations.
 """
 
 from __future__ import print_function
 import inspect
-from types import GeneratorType
 import dace
+from dace.sdfg import SDFG, SDFGState
 from dace.properties import make_properties, Property, SubgraphProperty
-from dace.graph import labeling, graph as gr
+from dace.graph import labeling, graph as gr, nodes as nd
 import networkx as nx
 from networkx.algorithms import isomorphism as iso
+from typing import Dict, List, Tuple, Type, Union
 
 
 @make_properties
 class Transformation(object):
-    """ Base class for transformations, as well as a static registry of 
-        transformations, where new transformations can be added in a 
+    """ Base class for transformations, as well as a static registry of
+        transformations, where new transformations can be added in a
         decentralized manner.
     """
 
     ####################################################################
     # Transformation registry
 
     # Class attributes
@@ -26,44 +27,44 @@
     _patterns = set()
     _stateflow_patterns = set()
 
     # Static methods
 
     @staticmethod
     def patterns():
-        """ Returns a list of single-state (dataflow) transformations 
+        """ Returns a list of single-state (dataflow) transformations
             currently in the registry. """
 
         pattern_list = sorted(
             Transformation._patterns, key=lambda cls: cls.__name__)
         return pattern_list
 
     @staticmethod
     def stateflow_patterns():
-        """ Returns a list of multiple-state (interstate) transformations 
+        """ Returns a list of multiple-state (interstate) transformations
             currently in the registry. """
 
         pattern_list = sorted(
             Transformation._stateflow_patterns, key=lambda cls: cls.__name__)
         return pattern_list
 
     @staticmethod
     def register_pattern(clazz):
         """ Registers a single-state (dataflow) transformation in the registry.
-            @param clazz: The Transformation class type.
+            :param clazz: The Transformation class type.
         """
 
         if not issubclass(clazz, Transformation):
             raise TypeError
         Transformation._patterns.add(clazz)
 
     @staticmethod
     def register_stateflow_pattern(clazz):
         """ Registers a multi-state transformation in the registry.
-            @param clazz: The Transformation class type.
+            :param clazz: The Transformation class type.
         """
 
         if not issubclass(clazz, Transformation):
             raise TypeError
         Transformation._stateflow_patterns.add(clazz)
 
     @staticmethod
@@ -76,15 +77,15 @@
         for member in pattern_members.values():
             if inspect.isclass(member) and issubclass(member, Transformation):
                 Transformation.register_pattern(member)
 
     @staticmethod
     def deregister_pattern(clazz):
         """ De-registers a transformation.
-            @param clazz: The Transformation class type.
+            :param clazz: The Transformation class type.
         """
 
         if not issubclass(clazz, Transformation):
             raise TypeError
         Transformation._patterns.remove(clazz)
 
     ####################################################################
@@ -103,60 +104,61 @@
             whether to apply memlet propagation after the transformation.
         """
 
         return False
 
     @staticmethod
     def expressions():
-        """ Returns a list of Graph objects that will be matched in the 
-            subgraph isomorphism phase. Used as a pre-pass before calling 
+        """ Returns a list of Graph objects that will be matched in the
+            subgraph isomorphism phase. Used as a pre-pass before calling
             `can_be_applied`.
             @see Transformation.can_be_applied
         """
 
         raise NotImplementedError
 
     @staticmethod
     def can_be_applied(graph, candidate, expr_index, sdfg, strict=False):
         """ Returns True if this transformation can be applied on the candidate
             matched subgraph.
-            @param graph: SDFGState object if this Transformation is 
+            :param graph: SDFGState object if this Transformation is
                           single-state, or SDFG object otherwise.
-            @param candidate: A mapping between node IDs returned from 
-                              `Transformation.expressions` and the nodes in 
+            :param candidate: A mapping between node IDs returned from
+                              `Transformation.expressions` and the nodes in
                               `graph`.
-            @param expr_index: The list index from `Transformation.expressions`
+            :param expr_index: The list index from `Transformation.expressions`
                                that was matched.
-            @param sdfg: If `graph` is an SDFGState, its parent SDFG. Otherwise
+            :param sdfg: If `graph` is an SDFGState, its parent SDFG. Otherwise
                          should be equal to `graph`.
-            @return: True if the transformation can be applied.
+            :param strict: Whether transformation should run in strict mode.
+            :return: True if the transformation can be applied.
         """
         raise NotImplementedError
 
     @staticmethod
     def match_to_str(graph, candidate):
-        """ Returns a string representation of the pattern match on the 
-            candidate subgraph. Used when identifying matches in the console 
+        """ Returns a string representation of the pattern match on the
+            candidate subgraph. Used when identifying matches in the console
             UI.
         """
         raise NotImplementedError
 
     def __init__(self, sdfg_id, state_id, subgraph, expr_index):
         """ Initializes an instance of Transformation.
-            @param sdfg_id: A unique ID of the SDFG.
-            @param state_id: The node ID of the SDFG state, if applicable.
-            @param subgraph: A mapping between node IDs returned from 
-                             `Transformation.expressions` and the nodes in 
+            :param sdfg_id: A unique ID of the SDFG.
+            :param state_id: The node ID of the SDFG state, if applicable.
+            :param subgraph: A mapping between node IDs returned from
+                             `Transformation.expressions` and the nodes in
                              `graph`.
-            @param expr_index: The list index from `Transformation.expressions`
+            :param expr_index: The list index from `Transformation.expressions`
                                that was matched.
-            @raise TypeError: When transformation is not subclass of
+            :raise TypeError: When transformation is not subclass of
                               Transformation.
-            @raise TypeError: When state_id is not instance of int.
-            @raise TypeError: When subgraph is not a dict of 
+            :raise TypeError: When state_id is not instance of int.
+            :raise TypeError: When subgraph is not a dict of
                               dace.graph.nodes.Node : int.
         """
 
         self.sdfg_id = sdfg_id
         self.state_id = state_id
         for value in subgraph.values():
             if not isinstance(value, int):
@@ -207,18 +209,18 @@
     def apply_pattern(self, sdfg):
         """ Applies this transformation on the given SDFG. """
         self.apply(sdfg)
         if not self.annotates_memlets():
             labeling.propagate_labels_sdfg(sdfg)
 
     def __str__(self):
-        raise NotImplementedError
+        return type(self).__name__
 
     def print_match(self, sdfg):
-        """ Returns a string representation of the pattern match on the 
+        """ Returns a string representation of the pattern match on the
             given SDFG. Used for printing matches in the console UI.
         """
         if not isinstance(sdfg, dace.SDFG):
             raise TypeError("Expected SDFG, got: {}".format(
                 type(sdfg).__name__))
         if self.state_id == -1:
             graph = sdfg
@@ -232,27 +234,29 @@
     def print_debuginfo():
         pass
 
 
 # Module functions ############################################################
 
 
-def collapse_multigraph_to_nx(graph: gr.MultiDiGraph) -> nx.DiGraph:
+def collapse_multigraph_to_nx(
+        graph: Union[gr.MultiDiGraph, gr.OrderedMultiDiGraph]) -> nx.DiGraph:
     """ Collapses a directed multigraph into a networkx directed graph.
 
-        In the output directed graph, each node is a number, which contains 
-        itself as node_data['node'], while each edge contains a list of the 
+        In the output directed graph, each node is a number, which contains
+        itself as node_data['node'], while each edge contains a list of the
         data from the original edges as its attribute (edge_data[0...N]).
 
-        @param graph: Directed multigraph object to be collapsed.
-        @return: Collapsed directed graph object.
+        :param graph: Directed multigraph object to be collapsed.
+        :return: Collapsed directed graph object.
   """
 
     # Create the digraph nodes.
-    digraph_nodes = [None] * graph.number_of_nodes()
+    digraph_nodes: List[Tuple[int, Dict[str, nd.Node]]] = (
+        [None] * graph.number_of_nodes())
     node_id = {}
     for i, node in enumerate(graph.nodes()):
         digraph_nodes[i] = (i, {'node': node})
         node_id[node] = i
 
     # Create the digraph edges.
     digraph_edges = {}
@@ -272,100 +276,41 @@
     result.add_edges_from(digraph_edges)
 
     return result
 
 
 def type_match(node_a, node_b):
     """ Checks whether the node types of the inputs match.
-        @param node_a: First node.
-        @param node_b: Second node.
-        @return: True if the object types of the nodes match, False otherwise.
-        @raise TypeError: When at least one of the inputs is not a dictionary 
+        :param node_a: First node.
+        :param node_b: Second node.
+        :return: True if the object types of the nodes match, False otherwise.
+        :raise TypeError: When at least one of the inputs is not a dictionary
                           or does not have a 'node' attribute.
-        @raise KeyError: When at least one of the inputs is a dictionary, 
+        :raise KeyError: When at least one of the inputs is a dictionary,
                          but does not have a 'node' key.
     """
     return isinstance(node_a['node'], type(node_b['node']))
 
 
-def match_expression(graph,
-                     expressions,
-                     node_match=type_match,
-                     edge_match=None,
-                     pattern_match=None,
-                     strict=False):
-    """ Returns a generator which yields a subgraph mapping from 
-        `expression_node` to `graph_node`.
-        @param graph: Directed multigraph object to be searched for subgraphs.
-        @param expressions: List of directed graphs, isomorphic to any 
-                            (sub)graph that potentially matches a 
-                            transformation.
-        @param node_match: Function for checking whether two nodes match.
-        @param edge_match: Function for checking whether two edges match.
-        @param pattern_match: Function for checking whether a subgraph matches
-                              a transformation.
-        @return: Generator of 2-tuples: (subgraph, expression index in 
-                 `expressions`).
-    """
-
-    # Collapse multigraph into directed graph
-    digraph = collapse_multigraph_to_nx(graph)
-
-    # If expression is a list, try to match each one of them
-    if not isinstance(expressions, list) and not isinstance(
-            expressions, GeneratorType):
-        expressions = [expressions]
-
-    for expr_index, expr in enumerate(expressions):
-        # Also collapse expression multigraph
-        cexpr = collapse_multigraph_to_nx(expr)
-
-        # Find candidate subgraphs (per-node / per-edge matching)
-        graph_matcher = iso.DiGraphMatcher(
-            digraph, cexpr, node_match=node_match, edge_match=edge_match)
-        for subgraph in graph_matcher.subgraph_isomorphisms_iter():
-            # Convert candidate to original graph node representation
-            # The type of subgraph is {graph_node_id: subgraph_node_id}
-            # We return the inverse mapping: {subgraph_node: graph_node} for
-            # ease of access
-            subgraph = {
-                cexpr.nodes[j]['node']: digraph.nodes[i]['node']
-                for (i, j) in subgraph.items()
-            }
-
-            # Match original (regular) expression on found candidate
-            if pattern_match is None:
-                # Yield mapping and index of expression found
-                yield subgraph, expr_index
-            else:
-                match_found = pattern_match(graph, subgraph)
-                if match_found:
-                    # Yield mapping and index of expression found
-                    # expr_index_list = list(range(match_num))
-                    yield subgraph, expr_index  # expr_index_list
-
-
-def match_pattern(state_id,
-                  state,
-                  pattern,
-                  sdfg,
+def match_pattern(state: SDFGState,
+                  pattern: Type[Transformation],
+                  sdfg: SDFG,
                   node_match=type_match,
                   edge_match=None,
                   strict=False):
     """ Returns a list of single-state Transformations of a certain class that
         match the input SDFG.
-        @param state_id: The node ID of the state in the given SDFG.
-        @param state: An SDFGState object to match.
-        @param pattern: Transformation object to match.
-        @param sdfg: The SDFG to match in.
-        @param node_match: Function for checking whether two nodes match.
-        @param edge_match: Function for checking whether two edges match.
-        @param strict: Only match transformation if strict (i.e., can only
+        :param state: An SDFGState object to match.
+        :param pattern: Transformation type to match.
+        :param sdfg: The SDFG to match in.
+        :param node_match: Function for checking whether two nodes match.
+        :param edge_match: Function for checking whether two edges match.
+        :param strict: Only match transformation if strict (i.e., can only
                        improve the performance/reduce complexity of the SDFG).
-        @return: A list of Transformation objects that match.
+        :return: A list of Transformation objects that match.
     """
 
     # Collapse multigraph into directed graph
     # Handling VF2 in networkx for now
     digraph = collapse_multigraph_to_nx(state)
 
     for idx, expression in enumerate(pattern.expressions()):
@@ -373,43 +318,50 @@
         graph_matcher = iso.DiGraphMatcher(
             digraph, cexpr, node_match=node_match, edge_match=edge_match)
         for subgraph in graph_matcher.subgraph_isomorphisms_iter():
             subgraph = {
                 cexpr.nodes[j]['node']: state.node_id(digraph.nodes[i]['node'])
                 for (i, j) in subgraph.items()
             }
-            match_found = pattern.can_be_applied(
-                state, subgraph, idx, sdfg, strict=strict)
+            try:
+                match_found = pattern.can_be_applied(
+                    state, subgraph, idx, sdfg, strict=strict)
+            except Exception as e:
+                print('WARNING: {p}::can_be_applied triggered a {c} exception:'
+                      ' {e}'.format(
+                          p=pattern.__name__, c=e.__class__.__name__, e=e))
+                match_found = False
             if match_found:
                 yield pattern(
-                    sdfg.sdfg_list.index(sdfg), state_id, subgraph, idx)
+                    sdfg.sdfg_list.index(sdfg), sdfg.node_id(state), subgraph,
+                    idx)
 
     # Recursive call for nested SDFGs
     for node in state.nodes():
-        if isinstance(node, dace.graph.nodes.NestedSDFG):
+        if isinstance(node, nd.NestedSDFG):
             sub_sdfg = node.sdfg
-            for i, sub_state in enumerate(sub_sdfg.nodes()):
+            for sub_state in sub_sdfg.nodes():
                 yield from match_pattern(
-                    i, sub_state, pattern, sub_sdfg, strict=strict)
+                    sub_state, pattern, sub_sdfg, strict=strict)
 
 
 def match_stateflow_pattern(sdfg,
                             pattern,
                             node_match=type_match,
                             edge_match=None,
                             strict=False):
     """ Returns a list of multi-state Transformations of a certain class that
         match the input SDFG.
-        @param sdfg: The SDFG to match in.
-        @param pattern: Transformation object to match.
-        @param node_match: Function for checking whether two nodes match.
-        @param edge_match: Function for checking whether two edges match.
-        @param strict: Only match transformation if strict (i.e., can only
+        :param sdfg: The SDFG to match in.
+        :param pattern: Transformation object to match.
+        :param node_match: Function for checking whether two nodes match.
+        :param edge_match: Function for checking whether two edges match.
+        :param strict: Only match transformation if strict (i.e., can only
                        improve the performance/reduce complexity of the SDFG).
-        @return: A list of Transformation objects that match.
+        :return: A list of Transformation objects that match.
     """
 
     # Collapse multigraph into directed graph
     # Handling VF2 in networkx for now
     digraph = collapse_multigraph_to_nx(sdfg)
 
     for idx, expression in enumerate(pattern.expressions()):
@@ -417,18 +369,24 @@
         graph_matcher = iso.DiGraphMatcher(
             digraph, cexpr, node_match=node_match, edge_match=edge_match)
         for subgraph in graph_matcher.subgraph_isomorphisms_iter():
             subgraph = {
                 cexpr.nodes[j]['node']: sdfg.node_id(digraph.nodes[i]['node'])
                 for (i, j) in subgraph.items()
             }
-            match_found = pattern.can_be_applied(sdfg, subgraph, idx, sdfg,
-                                                 strict)
+            try:
+                match_found = pattern.can_be_applied(sdfg, subgraph, idx, sdfg,
+                                                     strict)
+            except Exception as e:
+                print('WARNING: {p}::can_be_applied triggered a {c} exception:'
+                      ' {e}'.format(
+                          p=pattern.__name__, c=e.__class__.__name__, e=e))
+                match_found = False
             if match_found:
                 yield pattern(sdfg.sdfg_list.index(sdfg), -1, subgraph, idx)
 
     # Recursive call for nested SDFGs
     for state in sdfg.nodes():
         for node in state.nodes():
-            if isinstance(node, dace.graph.nodes.NestedSDFG):
+            if isinstance(node, nd.NestedSDFG):
                 yield from match_stateflow_pattern(
                     node.sdfg, pattern, strict=strict)
```

### Comparing `dace-0.9.0/dace.egg-info/PKG-INFO` & `dace-0.9.5/dace.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: dace
-Version: 0.9.0
+Version: 0.9.5
 Summary: Data-Centric Parallel Programming Framework
 Home-page: https://github.com/spcl/dace
 Author: SPCL @ ETH Zurich
 Author-email: talbn@inf.ethz.ch
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/spcl/dace.svg?branch=master)](https://travis-ci.org/spcl/dace)
+        [![Documentation Status](https://readthedocs.org/projects/spcldace/badge/?version=latest)](https://spcldace.readthedocs.io/en/latest/?badge=latest)
+        [![PyPI version](https://badge.fury.io/py/dace.svg)](https://badge.fury.io/py/dace)
         
         
         ![D](dace.svg)aCe - Data-Centric Parallel Programming
         =====================================================
         
         _Decoupling domain science from performance optimization._
         
@@ -20,15 +22,15 @@
         DaCe can be written inline in Python and transformed in the command-line/Jupyter Notebooks, or SDFGs can be interactively modified using the Data-centric Interactive Optimization Development Environment (DIODE, currently experimental).
         
         For more information, see our [paper](http://www.arxiv.org/abs/1902.10345).
         
         Tutorials
         ---------
         
-        * _Data-Centric Python Programs with NumPy (coming soon)_
+        * [Data-Centric Python Programs with NumPy](https://nbviewer.jupyter.org/github/spcl/dace/blob/master/tutorials/numpy_frontend.ipynb)
         * [Explicit Dataflow in Python](https://nbviewer.jupyter.org/github/spcl/dace/blob/master/tutorials/explicit.ipynb)
         * [SDFG API](https://nbviewer.jupyter.org/github/spcl/dace/blob/master/tutorials/sdfg_api.ipynb)
         * [Transformations](https://nbviewer.jupyter.org/github/spcl/dace/blob/master/tutorials/transformations.ipynb)
         
         Installation and Dependencies
         -----------------------------
         
@@ -40,21 +42,21 @@
          * CMake 2.8.12 or newer (for Windows, CMake 3.15 is recommended)
         
         Running
         -------
         
         **Python scripts:** Run DaCe programs (in implicit, explicit, or TensorFlow syntax) using Python directly.
         
-        **DIODE interactive development (experimental):**: Either run the installed script `diode`, or call `python3 -m diode.diode_rest` from the shell. Then, follow the printed instructions to enter the web interface.
+        **DIODE interactive development (experimental):**: Either run the installed script `diode`, or call `python3 -m diode.diode_server` from the shell. Then, follow the printed instructions to enter the web interface.
         
         **Octave scripts (experimental):** `.m` files can be run using the installed script `dacelab`, which will create the appropriate SDFG file.
         
         **Jupyter Notebooks:** DaCe is Jupyter-compatible. If a result is an SDFG or a state, it will show up directly in the notebook. See the [tutorials](tutorials) for examples.
         
-        **SDFV (standalone SDFG viewer):** To view SDFGs separately, run the `sdfv` installed script with the `.sdfg` file as an argument. Alternatively, you can open `diode/sdfv.html` directly and choose a file in the browser.
+        **[SDFV (standalone SDFG viewer)](https://spcl.github.io/dace/sdfv.html):** To view SDFGs separately, run the `sdfv` installed script with the `.sdfg` file as an argument. Alternatively, you can use the link or open `diode/sdfv.html` directly and choose a file in the browser.
         
         **Note for Windows/Visual C++ users:** If compilation fails in the linkage phase, try setting the following environment variable to force Visual C++ to use Multi-Threaded linkage:
         ```
         X:\path\to\dace> set _CL_=/MT
         ```
```

### Comparing `dace-0.9.0/dace.egg-info/SOURCES.txt` & `dace-0.9.5/dace.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 dace/config.py
 dace/data.py
 dace/dtypes.py
 dace/jupyter.py
 dace/memlet.py
 dace/properties.py
 dace/sdfg.py
+dace/serialize.py
 dace/subsets.py
 dace/symbolic.py
 dace.egg-info/PKG-INFO
 dace.egg-info/SOURCES.txt
 dace.egg-info/dependency_links.txt
 dace.egg-info/requires.txt
 dace.egg-info/top_level.txt
@@ -24,18 +25,21 @@
 dace/codegen/instrumentation/__init__.py
 dace/codegen/instrumentation/cuda_events.py
 dace/codegen/instrumentation/papi.py
 dace/codegen/instrumentation/perfdb.py
 dace/codegen/instrumentation/provider.py
 dace/codegen/instrumentation/timer.py
 dace/codegen/targets/__init__.py
+dace/codegen/targets/common.py
 dace/codegen/targets/cpu.py
 dace/codegen/targets/cuda.py
+dace/codegen/targets/fpga.py
 dace/codegen/targets/framecode.py
 dace/codegen/targets/immaterial.py
+dace/codegen/targets/intel_fpga.py
 dace/codegen/targets/mpi.py
 dace/codegen/targets/target.py
 dace/codegen/targets/xilinx.py
 dace/frontend/__init__.py
 dace/frontend/operations.py
 dace/frontend/common/__init__.py
 dace/frontend/common/op_impl.py
@@ -53,83 +57,73 @@
 dace/frontend/octave/ast_values.py
 dace/frontend/octave/lexer.py
 dace/frontend/octave/parse.py
 dace/frontend/python/__init__.py
 dace/frontend/python/astnodes.py
 dace/frontend/python/astutils.py
 dace/frontend/python/decorators.py
-dace/frontend/python/ndarray.py
 dace/frontend/python/ndloop.py
 dace/frontend/python/newast.py
 dace/frontend/python/parser.py
 dace/frontend/python/simulator.py
+dace/frontend/python/wrappers.py
 dace/frontend/tensorflow/__init__.py
 dace/frontend/tensorflow/tensorflow.py
 dace/frontend/tensorflow/winograd.py
 dace/graph/__init__.py
 dace/graph/dot.py
 dace/graph/edges.py
 dace/graph/graph.py
 dace/graph/labeling.py
 dace/graph/nodes.py
 dace/graph/nxutil.py
 dace/transformation/__init__.py
+dace/transformation/helpers.py
 dace/transformation/optimizer.py
 dace/transformation/pattern_matching.py
+dace/transformation/testing.py
 dace/transformation/dataflow/__init__.py
 dace/transformation/dataflow/copy_to_device.py
+dace/transformation/dataflow/double_buffering.py
 dace/transformation/dataflow/fpga_transform.py
 dace/transformation/dataflow/gpu_transform.py
 dace/transformation/dataflow/gpu_transform_local_storage.py
+dace/transformation/dataflow/local_storage.py
 dace/transformation/dataflow/map_collapse.py
 dace/transformation/dataflow/map_dim_interchange.py
 dace/transformation/dataflow/map_expansion.py
 dace/transformation/dataflow/map_for_loop.py
 dace/transformation/dataflow/map_fusion.py
 dace/transformation/dataflow/map_interchange.py
 dace/transformation/dataflow/mapreduce.py
+dace/transformation/dataflow/merge_arrays.py
 dace/transformation/dataflow/mpi.py
 dace/transformation/dataflow/reduce_expansion.py
 dace/transformation/dataflow/redundant_array.py
 dace/transformation/dataflow/redundant_array_copying.py
 dace/transformation/dataflow/stream_transient.py
 dace/transformation/dataflow/strip_mining.py
 dace/transformation/dataflow/tensorflow_redundant_array.py
 dace/transformation/dataflow/tiling.py
 dace/transformation/dataflow/vectorization.py
 dace/transformation/interstate/__init__.py
-dace/transformation/interstate/double_buffering.py
 dace/transformation/interstate/fpga_transform_sdfg.py
 dace/transformation/interstate/fpga_transform_state.py
 dace/transformation/interstate/gpu_transform_sdfg.py
 dace/transformation/interstate/sdfg_nesting.py
 dace/transformation/interstate/state_fusion.py
+diode/DaceState.py
 diode/__init__.py
 diode/abstract_sdfg.py
 diode/adjust_settings.py
 diode/config_ui.py
-diode/diode1.py
 diode/diode_client.py
-diode/diode_optscript_translator.py
-diode/diode_rest.py
-diode/images.py
-diode/pattern_editor.py
-diode/performance_plot.py
-diode/property_renderer.py
+diode/diode_server.py
 diode/remote_execution.py
-diode/rendered_graph.py
-diode/rendered_graph_html5.py
-diode/rendered_graphs.py
-diode/sdfg_editor.py
 diode/sdfv.py
 diode/db_scripts/__init__.py
-diode/db_scripts/db_insert.py
-diode/db_scripts/db_query.py
 diode/db_scripts/db_setup.py
 diode/db_scripts/sql_to_json.py
 diode/db_scripts/sql_to_json_test.py
-diode/optgraph/DaceState.py
-diode/optgraph/__init__.py
-diode/optgraph/optgraph.py
 scripts/dacelab
 scripts/diode
 scripts/sdfv
```

### Comparing `dace-0.9.0/diode/abstract_sdfg.py` & `dace-0.9.5/diode/abstract_sdfg.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/diode/config_ui.py` & `dace-0.9.5/diode/config_ui.py`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/diode/db_scripts/db_setup.py` & `dace-0.9.5/diode/db_scripts/db_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,8 +93,9 @@
     ''')
 
     conn.commit()
 
     conn.close()
 
 
-db_setup()
+if __name__ == '__main__':
+    db_setup()
```

### Comparing `dace-0.9.0/diode/db_scripts/sql_to_json.py` & `dace-0.9.5/diode/db_scripts/sql_to_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1317,16 +1317,16 @@
             if modestr == "default":
                 continue
             PAPISettings.merging_print("Generating table for " + modestr)
             table_str = "{s}_sel".format(s=modestr)
             c.execute("CREATE TEMPORARY TABLE `{tablename}` AS ".format(
                 tablename=table_str) + query.format(mode=modestr))
             c.execute(
-                "CREATE INDEX `{t}_ind` ON `default_sel`(SuperSectionID, entryID, threadID, iteration);".
-                format(t=table_str))
+                "CREATE INDEX `{t}_ind` ON `default_sel`(SuperSectionID, entryID, threadID, iteration);"
+                .format(t=table_str))
             # Cool, now we just match by rowid
             PAPISettings.merging_print("Creating temporary table...")
             esel_query = """
 SELECT
     DISTINCT ds.entryID as entryid, ms.entryID as oldentryid
 FROM `default_sel` AS ds INNER JOIN `{t}` AS ms ON ds.rowid = ms.rowid
 ;
@@ -2316,20 +2316,27 @@
             shared_input_db=cache_conn,
             critical_path_analysis=get_cpa,
             perfdata_path=db_path)
         memory_op_analysis = MemoryOpAnalysis(shared_input_db=cache_conn)
         cache_op_analysis = CacheOpAnalysis(shared_input_db=cache_conn)
 
         analyses = [
-            ("ThreadAnalysis", thread_analysis, lambda unified_id, ssid, sid: [unified_id, ssid]),
-            ("CriticalPathAnalysis", critical_path_analysis, lambda unified_id, ssid, sid: [int(unified_id) & 0xFFFF, (int(unified_id) >> 16) & 0xFFFF]),
-            ("MemoryAnalysis", memory_analysis, lambda unified_id, ssid, sid: [unified_id, ssid]),
-            ("VectorizationAnalysis", vectorization_analysis, lambda unified_id, ssid, sid: [unified_id, ssid]),
-            ("MemoryOpAnalysis", memory_op_analysis, lambda unified_id, ssid, sid: [unified_id, ssid]),
-            ("CacheOpAnalysis", cache_op_analysis, lambda unified_id, ssid, sid: [unified_id, ssid])
+            ("ThreadAnalysis", thread_analysis,
+             lambda unified_id, ssid, sid: [unified_id, ssid]),
+            ("CriticalPathAnalysis", critical_path_analysis,
+             lambda unified_id, ssid, sid:
+             [int(unified_id) & 0xFFFF, (int(unified_id) >> 16) & 0xFFFF]),
+            ("MemoryAnalysis", memory_analysis,
+             lambda unified_id, ssid, sid: [unified_id, ssid]),
+            ("VectorizationAnalysis", vectorization_analysis,
+             lambda unified_id, ssid, sid: [unified_id, ssid]),
+            ("MemoryOpAnalysis", memory_op_analysis,
+             lambda unified_id, ssid, sid: [unified_id, ssid]),
+            ("CacheOpAnalysis", cache_op_analysis,
+             lambda unified_id, ssid, sid: [unified_id, ssid])
         ]
 
         PAPISettings.canning_print("unified_ids: " + str(unified_ids))
 
         # Generate all analyses for this
         for x in unified_ids:
             unified_id, = x
```

### Comparing `dace-0.9.0/diode/diode_client.py` & `dace-0.9.5/diode/diode_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,326 +1,339 @@
 #!/usr/bin/python3
 # DIODE client using a command line interface
 
 # Usage example: cat ../samples/simple/gemm.py | ./diode_client.py --code --compile
 import argparse, requests, json, sys
 
-parser = argparse.ArgumentParser()
-parser.add_argument(
-    "-c",
-    "--connect",
-    default="localhost",
-    metavar="IP",
-    help="Connect to Server IP. Default is localhost.")
-
-parser.add_argument(
-    "-p", "--port", default="5000", help="Set server port. Default is 5000")
-
-parser.add_argument(
-    "-compile",
-    "--compile",
-    action="store_true",
-    help="Compiles the SDFG and returns resulting structures.")
-
-parser.add_argument(
-    "-tf",
-    "--transform",
-    default="",
-    help=
-    "Sets the name of the transform to apply. If the transformation name is ambiguous, the first transformation with that name is chosen."
-)
-
-parser.add_argument(
-    "-r",
-    "--run",
-    action="store_true",
-    help=
-    "Executes the SDFG on the target machine specified in Config and prints the execution output (blocking)"
-)
-
-parser.add_argument(
-    "-code",
-    "--code",
-    action="store_true",
-    help=
-    "Setting this indicates that the input is dace code. Default is false (compile JSON serialization of SDFG)"
-)
-
-parser.add_argument(
-    "-u",
-    "--user",
-    default="default",
-    help=
-    "Setting this indicates that the input is dace code. Default is false (compile JSON serialization of SDFG)"
-)
-
-parser.add_argument(
-    "-e",
-    "--extract",
-    nargs="+",
-    choices=[
-        "txform", "sdfg", "structure", "struct_noprop", "outcode",
-        "txform_detail", "runnercode"
-    ])
-
-parser.add_argument(
-    "-ver",
-    "--version",
-    default="1.0",
-    help="Sets the REST API Version to use.")
-args = parser.parse_args()
-
-if args.compile or args.run:
-    url = 'http://' + str(args.connect) + ":" + str(args.port)
-    data = {}
-    stdin_input = sys.stdin.read()
-    if args.code:
-        # Compile from code
-        data['code'] = stdin_input
-    else:
-        # Compile from serialized data
-        try:
-            data['sdfg'] = json.loads(stdin_input)['sdfg']
-        except:
-            sys.stderr.write(
-                "Failed to parse serialized SDFG input, is it in a correct json format?"
-            )
-            sys.stdout.write("Invalid data: " + str(stdin_input))
-            sys.exit(-3)
-
-        # Append runnercode if available
-        try:
-            data['code'] = json.loads(stdin_input)['runnercode'][0]
-        except:
-            pass
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "-c",
+        "--connect",
+        default="localhost",
+        metavar="IP",
+        help="Connect to Server IP. Default is localhost.")
+
+    parser.add_argument(
+        "-p",
+        "--port",
+        default="5000",
+        help="Set server port. Default is 5000")
+
+    parser.add_argument(
+        "-compile",
+        "--compile",
+        action="store_true",
+        help="Compiles the SDFG and returns resulting structures.")
+
+    parser.add_argument(
+        "-tf",
+        "--transform",
+        default="",
+        help=
+        "Sets the name of the transform to apply. If the transformation name is ambiguous, the first transformation with that name is chosen."
+    )
+
+    parser.add_argument(
+        "-r",
+        "--run",
+        action="store_true",
+        help=
+        "Executes the SDFG on the target machine specified in Config and prints the execution output (blocking)"
+    )
+
+    parser.add_argument(
+        "-code",
+        "--code",
+        action="store_true",
+        help=
+        "Setting this indicates that the input is dace code. Default is false (compile JSON serialization of SDFG)"
+    )
+
+    parser.add_argument(
+        "-u",
+        "--user",
+        default="default",
+        help=
+        "Setting this indicates that the input is dace code. Default is false (compile JSON serialization of SDFG)"
+    )
+
+    parser.add_argument(
+        "-e",
+        "--extract",
+        nargs="+",
+        choices=[
+            "txform", "sdfg", "structure", "struct_noprop", "outcode",
+            "txform_detail", "runnercode"
+        ])
+
+    parser.add_argument(
+        "-ver",
+        "--version",
+        default="1.0",
+        help="Sets the REST API Version to use.")
+    args = parser.parse_args()
+
+    if args.compile or args.run:
+        url = 'http://' + str(args.connect) + ":" + str(args.port)
+        data = {}
+        stdin_input = sys.stdin.read()
+        if args.code:
+            # Compile from code
+            data['code'] = stdin_input
+        else:
+            # Compile from serialized data
+            try:
+                data['sdfg'] = json.loads(stdin_input)['sdfg']
+            except:
+                sys.stderr.write("Failed to parse serialized SDFG input, "
+                                 "is it in a correct json format?")
+                sys.stdout.write("Invalid data: " + str(stdin_input))
+                sys.exit(-3)
 
-    data['client_id'] = args.user
+            # Append runnercode if available
+            try:
+                data['code'] = json.loads(stdin_input)['runnercode'][0]
+            except:
+                pass
 
-    #data = json.dumps(data)
-    cmdstr = "run/" if args.run else "compile/dace"
+        data['client_id'] = args.user
 
-    if args.transform:
-        if args.code:
-            sys.stderr.write(
-                "Cannot combine --code and --transform. Compile using '--code --extract sdfg txform_detail' first, then pipe the output into a command with --transform"
-            )
-            sys.exit(-4)
-
-        try:
-            transforms = json.loads(stdin_input)['advanced_transform']
-        except:
-            sys.stderr.write(
-                "Commands executed with --transform need an input file generated previously that includes --extract txform_detail. (Not passing --extract is not valid)"
-            )
-            sys.exit(-4)
-
-        # Apply default transform (no property change)
-        txf_found = False
-        txform_sdfg = ""
-        for k, v in transforms.items():
-            # Compound level (key = target sdfg name, value = Object of transforms)
+        #data = json.dumps(data)
+        cmdstr = "run/" if args.run else "compile/dace"
+
+        if args.transform:
+            if args.code:
+                sys.stderr.write(
+                    "Cannot combine --code and --transform. Compile using '--code --extract sdfg txform_detail' first, then pipe the output into a command with --transform"
+                )
+                sys.exit(-4)
 
             try:
-                txform = v[args.transform]
-                txf_found = True
-                txform_sdfg = k
-                break
+                transforms = json.loads(stdin_input)['advanced_transform']
             except:
-                # Key not found
-                continue
-        if not txf_found:
-            sys.stderr.write("Could not find a transformation named " +
-                             args.transform)
-            sys.exit(-5)
-        # Else we have a transform to apply
-
-        # Build the format for the transformation manually
-        data['optpath'] = {
-            txform_sdfg: [{
-                'name': args.transform,
-                'params': {
-                    'props': txform
-                }
-            }]
-        }
-
-    nofail = False
-    for i in range(0, 5):
-        uri = url + "/dace/api/v" + args.version + "/" + cmdstr
-        try:
-            response = requests.post(uri, json=data)
-        except Exception as e:
-            print("Failed to request url '" + uri + "' with error " + str(e))
-            import time
-            time.sleep(2)
-            continue
-
-        # Break if there was no exception
-        nofail = True
-        break
-    if not nofail:
-        # Cannot continue
-        sys.exit(-2)
-
-    if args.run:
-        first_out = response.text
-        output_ok = False
-        # Output is a json asking to use a different URL to read the output
+                sys.stderr.write(
+                    "Commands executed with --transform need an input file generated previously that includes --extract txform_detail. (Not passing --extract is not valid)"
+                )
+                sys.exit(-4)
+
+            # Apply default transform (no property change)
+            txf_found = False
+            txform_sdfg = ""
+            for k, v in transforms.items():
+                # Compound level (key = target sdfg name, value = Object of transforms)
+
+                try:
+                    txform = v[args.transform]
+                    txf_found = True
+                    txform_sdfg = k
+                    break
+                except:
+                    # Key not found
+                    continue
+            if not txf_found:
+                sys.stderr.write("Could not find a transformation named " +
+                                 args.transform)
+                sys.exit(-5)
+            # Else we have a transform to apply
+
+            # Build the format for the transformation manually
+            data['optpath'] = {
+                txform_sdfg: [{
+                    'name': args.transform,
+                    'params': {
+                        'props': txform
+                    }
+                }]
+            }
+
+        nofail = False
         for i in range(0, 5):
-            import time
-            time.sleep(1)
-            response = requests.post(
-                url + "/dace/api/v" + args.version + "/run/status/",
-                json={'client_id': args.user})
+            uri = url + "/dace/api/v" + args.version + "/" + cmdstr
             try:
-                tmp = json.loads(response.text)
-            except:
-                # Got valid data
-                output_ok = True
-                break
-        if not output_ok:
-            sys.stderr.write("Failed to get run reference\n")
-            sys.exit(-1)
-        sys.stdout.write(response.text)
-        sys.exit(0)
-
-    resp_json = response.json()
-
-    def dict_scanner(d, nometa=False):
-        if not isinstance(d, dict):
-            return None
-        else:
-            for x in list(d.keys()):
-                if nometa:
-                    if x.startswith("_meta_"):
-                        del d[x]
-                        continue
-                d[x] = dict_scanner(d[x], nometa=nometa)
-        return d
-
-    def get_transformations(resp_json, cb):
-        clist = resp_json['compounds'].keys()
-        for x in clist:
-            sys.stdout.write('"' + x + '"' + ":\n{")
-            l = resp_json['compounds'][x]['matching_opts']
-            encountered = {}
-            for c in l:
-                if c['opt_name'] not in encountered:
-                    encountered[c['opt_name']] = 0
-                else:
-                    encountered[c['opt_name']] += 1
-                name_str = "" if encountered[c['opt_name']] == 0 else (
-                    "$" + str(encountered[c['opt_name']]))
-                #sys.stdout.write(c['opt_name'] + name_str + '\n')
-                cb(x, c['opt_name'] + name_str, c)
-                if c != l[-1]: sys.stdout.write(',')
-
-            sys.stdout.write("}")
-            if x != list(clist)[-1]: sys.stdout.write(',')
-
-    extract_list = list(args.extract)
-    # Extract if requested
-    if args.extract:
-        if len(args.extract) == 1 and "outcode" in args.extract:
-            pass
-        else:
-            sys.stdout.write("{")
-        for elem in extract_list:
+                response = requests.post(uri, json=data)
+            except Exception as e:
+                print("Failed to request url '" + uri + "' with error " +
+                      str(e))
+                import time
+                time.sleep(2)
+                continue
+
+            # Break if there was no exception
+            nofail = True
+            break
+        if not nofail:
+            # Cannot continue
+            sys.exit(-2)
+
+        if args.run:
+            first_out = response.text
+            output_ok = False
+            # Output is a json asking to use a different URL to read the output
+            for i in range(0, 5):
+                import time
+                time.sleep(1)
+                response = requests.post(
+                    url + "/dace/api/v" + args.version + "/run/status/",
+                    json={'client_id': args.user})
+                try:
+                    tmp = json.loads(response.text)
+                except:
+                    # Got valid data
+                    output_ok = True
+                    break
+            if not output_ok:
+                sys.stderr.write("Failed to get run reference\n")
+                sys.exit(-1)
+            sys.stdout.write(response.text)
+            sys.exit(0)
+
+        resp_json = response.json()
+        if "error" in resp_json:
+            s = ""
+            if "traceback" in resp_json:
+                s += resp_json["traceback"]
+            raise ValueError(s + resp_json["error"])
+
+        def dict_scanner(d, nometa=False):
+            if not isinstance(d, dict):
+                return None
+            else:
+                for x in list(d.keys()):
+                    if nometa:
+                        if x.startswith("_meta_"):
+                            del d[x]
+                            continue
+                    d[x] = dict_scanner(d[x], nometa=nometa)
+            return d
+
+        def get_transformations(resp_json, cb):
+            clist = resp_json['compounds'].keys()
+            for x in clist:
+                sys.stdout.write('"' + x + '"' + ":\n{")
+                l = resp_json['compounds'][x]['matching_opts']
+                encountered = {}
+                for c in l:
+                    if c['opt_name'] not in encountered:
+                        encountered[c['opt_name']] = 0
+                    else:
+                        encountered[c['opt_name']] += 1
+                    name_str = "" if encountered[c['opt_name']] == 0 else (
+                        "$" + str(encountered[c['opt_name']]))
+                    #sys.stdout.write(c['opt_name'] + name_str + '\n')
+                    cb(x, c['opt_name'] + name_str, c)
+                    if c != l[-1]: sys.stdout.write(',')
 
-            if "sdfg" == elem:
-                # Output SDFG
-                comps = resp_json['compounds']
-                ret = {}
-                for k, v in comps.items():
-                    ret[k] = v['sdfg']
-                sys.stdout.write('"sdfg":')
-                sys.stdout.write(json.dumps(ret, indent=2))
-                if "sdfg" != args.extract[-1]: sys.stdout.write(',')
-            if "txform" == elem:
-                # Output available transformations
-                sys.stdout.write('"simple_transform":')
-                sys.stdout.write("{")
-                get_transformations(resp_json,
-                                    lambda a, b, c: sys.stdout.write(b + '\n'))
                 sys.stdout.write("}")
-                if "txform" != args.extract[-1]: sys.stdout.write(',')
-            if "txform_detail" == elem:
-                # Output available transformations in json-format (necessary to apply)
-                sys.stdout.write('"advanced_transform":')
+                if x != list(clist)[-1]: sys.stdout.write(',')
+
+        extract_list = list(args.extract)
+        # Extract if requested
+        if args.extract:
+            if len(args.extract) == 1 and "outcode" in args.extract:
+                pass
+            else:
                 sys.stdout.write("{")
-                get_transformations(resp_json, lambda a, b, c: sys.stdout.write('"' + b + '":\n' + json.dumps(c, indent=2) + '\n\n'))
-                sys.stdout.write("}")
-                if "txform_detail" != args.extract[-1]: sys.stdout.write(',')
-            if "structure" == elem:
-                # Remove values; only output skeleton structure (i.e. only true tree nodes, no leafs)
-                sys.stdout.write('"structure":')
-                new_d = dict_scanner(resp_json)
-                sys.stdout.write(json.dumps(new_d, indent=2))
-            if "struct_noprop" == elem:
-                sys.stdout.write('"struct_noprop":')
-                new_d = dict_scanner(resp_json, nometa=True)
-                sys.stdout.write(json.dumps(new_d, indent=2))
-            if "outcode" == elem:
-                # Don't add objects if this is the only requested output
-                as_json = False
-                if len(args.extract) > 1:
-                    sys.stdout.write('"outcode": ')
-                    as_json = True
-                if as_json:
-                    sys.stdout.write(
-                        json.dumps({
-                            k: v['generated_code']
-                            for k, v in resp_json['compounds'].items()
-                        }))
+            for elem in extract_list:
 
-                else:
-                    try:
-                        for x in resp_json['compounds'].keys():
-                            sys.stdout.write("//" + x + ":\n")
-                            l = resp_json['compounds'][x]['generated_code']
-                            for c in l:
-                                sys.stdout.write("// #### Next ####\n")
-                                sys.stdout.write(c)
-                    except:
-                        if 'error' in resp_json:
-                            print('ERROR:', resp_json['error'])
-                            if 'traceback' in resp_json:
-                                print(resp_json['traceback'])
-                        else:
-                            print('Received erroneous JSON:', resp_json)
-                        raise
-                if len(args.extract) > 1:
-                    if "outcode" != extract_list[-1]:
+                if "sdfg" == elem:
+                    # Output SDFG
+                    comps = resp_json['compounds']
+                    ret = {}
+                    for k, v in comps.items():
+                        ret[k] = v['sdfg']
+                    sys.stdout.write('"sdfg":')
+                    sys.stdout.write(json.dumps(ret, indent=2))
+                    if "sdfg" != args.extract[-1]: sys.stdout.write(',')
+                if "txform" == elem:
+                    # Output available transformations
+                    sys.stdout.write('"simple_transform":')
+                    sys.stdout.write("{")
+                    get_transformations(
+                        resp_json, lambda a, b, c: sys.stdout.write(b + '\n'))
+                    sys.stdout.write("}")
+                    if "txform" != args.extract[-1]: sys.stdout.write(',')
+                if "txform_detail" == elem:
+                    # Output available transformations in json-format (necessary to apply)
+                    sys.stdout.write('"advanced_transform":')
+                    sys.stdout.write("{")
+                    get_transformations(
+                        resp_json, lambda a, b, c: sys.
+                        stdout.write('"' + b + '":\n' + json.dumps(
+                            c, indent=2) + '\n\n'))
+                    sys.stdout.write("}")
+                    if "txform_detail" != args.extract[-1]:
                         sys.stdout.write(',')
-            if "runnercode" == elem:
+                if "structure" == elem:
+                    # Remove values; only output skeleton structure (i.e. only true tree nodes, no leafs)
+                    sys.stdout.write('"structure":')
+                    new_d = dict_scanner(resp_json)
+                    sys.stdout.write(json.dumps(new_d, indent=2))
+                if "struct_noprop" == elem:
+                    sys.stdout.write('"struct_noprop":')
+                    new_d = dict_scanner(resp_json, nometa=True)
+                    sys.stdout.write(json.dumps(new_d, indent=2))
+                if "outcode" == elem:
+                    # Don't add objects if this is the only requested output
+                    as_json = False
+                    if len(args.extract) > 1:
+                        sys.stdout.write('"outcode": ')
+                        as_json = True
+                    if as_json:
+                        sys.stdout.write(
+                            json.dumps({
+                                k: v['generated_code']
+                                for k, v in resp_json['compounds'].items()
+                            }))
+
+                    else:
+                        try:
+                            for x in resp_json['compounds'].keys():
+                                sys.stdout.write("//" + x + ":\n")
+                                l = resp_json['compounds'][x]['generated_code']
+                                for c in l:
+                                    sys.stdout.write("// #### Next ####\n")
+                                    sys.stdout.write(c)
+                        except:
+                            if 'error' in resp_json:
+                                print('ERROR:', resp_json['error'])
+                                if 'traceback' in resp_json:
+                                    print(resp_json['traceback'])
+                            else:
+                                print('Received erroneous JSON:', resp_json)
+                            raise
+                    if len(args.extract) > 1:
+                        if "outcode" != extract_list[-1]:
+                            sys.stdout.write(',')
+                if "runnercode" == elem:
 
-                sys.stdout.write('"runnercode": ')
-                # Pass the input code through
+                    sys.stdout.write('"runnercode": ')
+                    # Pass the input code through
 
-                # Check if the code was in already passed-through data input (read json)
-                runnercode = ""
-                try:
-                    d = json.loads(stdin_input)
-                    runnercode = d['runnercode'][0]
-                except:
-                    pass
-                if not args.code and runnercode == "":
-                    sys.stderr.write(
-                        "Error: Cannot extract runnercode as it was not in input."
-                    )
-                    sys.exit(-4)
-                elif args.code:
-                    # Take stdin_input
-                    runnercode = stdin_input
+                    # Check if the code was in already passed-through data input (read json)
+                    runnercode = ""
+                    try:
+                        d = json.loads(stdin_input)
+                        runnercode = d['runnercode'][0]
+                    except:
+                        pass
+                    if not args.code and runnercode == "":
+                        sys.stderr.write(
+                            "Error: Cannot extract runnercode as it was not in input."
+                        )
+                        sys.exit(-4)
+                    elif args.code:
+                        # Take stdin_input
+                        runnercode = stdin_input
 
-                sys.stdout.write(json.dumps([runnercode]))
+                    sys.stdout.write(json.dumps([runnercode]))
 
-                if "runnercode" != extract_list[-1]:
-                    sys.stdout.write(',')
+                    if "runnercode" != extract_list[-1]:
+                        sys.stdout.write(',')
 
-        if len(args.extract) == 1 and "outcode" in args.extract:
-            pass
-        else:
-            sys.stdout.write("}")
+            if len(args.extract) == 1 and "outcode" in args.extract:
+                pass
+            else:
+                sys.stdout.write("}")
 
-    else:
-        sys.stdout.write(response.text)
+        else:
+            sys.stdout.write(response.text)
```

### Comparing `dace-0.9.0/diode/diode_rest.py` & `dace-0.9.5/diode/diode_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 #!flask/bin/python
 
 import dace
+import dace.serialize
 import dace.frontend.octave.parse as octave_frontend
-import dace.frontend.python.parser as python_frontend
-from diode.optgraph.DaceState import DaceState
+from diode.DaceState import DaceState
 from dace.transformation.optimizer import SDFGOptimizer
 import inspect
-from flask import Flask, Response, request, redirect, url_for, abort, make_response, jsonify, send_from_directory, send_file
-import json, copy
+from flask import Flask, Response, request, redirect, url_for, abort, jsonify, send_from_directory, send_file
+import json
+import copy
+import multiprocessing
 import re
-from diode.remote_execution import Executor, AsyncExecutor
+from diode.remote_execution import AsyncExecutor
 
-import traceback, os, threading, queue, time
-
-# Enum imports
-from dace.dtypes import AccessType
-from dace import ScheduleType, Language, StorageType
+import traceback
+import os
+import threading
+import queue
+import time
 
 app = Flask(__name__)
 
 # Prepare a whitelist of DaCe enumeration types
 enum_list = [
     typename
     for typename, dtype in inspect.getmembers(dace.dtypes, inspect.isclass)
     if issubclass(dtype, dace.dtypes.AutoNumber)
 ]
 
 es_ref = []
+remote_execution = False
 
 config_lock = threading.Lock()
 
 RUNNING_TIMEOUT = 3
 
 
 class ConfigCopy:
@@ -68,15 +71,15 @@
         with open(path, 'w') as f:
             import yaml
             yaml.dump(self._config, f, default_flow_style=False)
 
 
 class ExecutorServer:
     """
-       Implements a server scheduling execution of dace programs 
+       Implements a server scheduling execution of dace programs
     """
 
     def __init__(self):
 
         self._command_queue = queue.Queue(
         )  # Fast command queue. Must be polled often (< 30 ms response time)
         self._executor_queue = queue.Queue(
@@ -132,29 +135,26 @@
                     del self._command_results[ticket]
             except:
                 time.sleep(2)
                 continue
             return ret
 
     def addCommand(self, cmd):
-        import random
         with self._oplock:
             cmd['ticket'] = self._ticket_counter
             self._ticket_counter += 1
             self._command_queue.put(cmd)
             print("Added command to queue")
             return cmd['ticket']
 
     def consume_programs(self):
 
         try:
             cmd = self._executor_queue.get(timeout=3)
 
-            #print("cmd: " + str(cmd))
-
             if cmd['cmd'] == "run":
                 while True:
                     with self._run_cv:
                         if self._slot_available:
                             break
                     import time
                     time.sleep(0.5)
@@ -218,15 +218,15 @@
                     # Clean database and create tables
                     db_setup(perf_tmp_dir)
 
                 elif cmd['operation'] == 'remove_group':
                     perfdir = ExecutorServer.getPerfdataDir(cmd['cid'])
                     perfdata_path = os.path.join(perfdir, "perfdata.db")
                     os.remove(perfdata_path)
-                    os.rmdir(perf_tmp_dir)
+                    os.rmdir(perfdir)
 
                 elif cmd['operation'] == 'endgroup':
                     print("Ending group")
                     from diode.db_scripts.sql_to_json import MergeRuns, Conserver
                     from dace.config import Config
 
                     config_path = cmd['config_path']
@@ -342,15 +342,15 @@
                 except:
                     err_count += 1
                     if err_count < 20:  # Give 20 seconds of space for compilation and distribution
                         time.sleep(1)
                         continue
 
                     def egen():
-                        yield "{'error': 'Failed to get run reference'}"
+                        yield "ERROR: Failed to get run reference"
 
                     return egen
                 return ret
 
     def stop(self):
         self._running = False
 
@@ -358,15 +358,14 @@
         self._oplock.acquire()
 
     def unlock(self):
         self._oplock.release()
 
     @staticmethod
     def getPerfdataDir(client_id):
-        import tempfile
 
         if not os.path.isdir("perfdata-dir/"):
             os.mkdir("perfdata-dir")
 
         tpath = "perfdata-dir/" + client_id
 
         try:
@@ -424,15 +423,15 @@
                 'config_path': config_path,
                 'cmd': 'run',
                 'cot': compilation_output_tuple,
                 'opt': more_options,
                 'state': 'pending',
                 'reset-perfdata': False
             }
-            self._executor_queue.put(item=val)
+            self._executor_queue.put(val)
 
             self._task_dict[self._run_num] = val
             self._run_num += 1
 
         def error_gen():
             yield '{ "error": "Run was scheduled. Please poll until ready or longpoll." }'
 
@@ -446,33 +445,19 @@
         compilation_output_tuple = cot
         runindex = options['index']
         config_path = options['config_path']
         client_id = options['client_id']
         perfopts = options['perfopts']
         sdfgs, code_tuples, dace_state = compilation_output_tuple
 
-        terminal_queue = queue.Queue()
-
-        # Generator used to pass the serial output through (using HTTP1.1. streaming)
-        def output_feeder(output):
-            if isinstance(output, str):
-                # It's already in a usable format
-                pass
-            else:
-                try:
-                    output = output.decode('utf-8')
-                except UnicodeDecodeError:
-                    # Try again escaping
-                    output = output.decode('unicode_escape')
-            terminal_queue.put(output)
-
+        # Passes output through HTTP1.1 streaming (using yield)
         def runner():
             print("Trying to get lock")
             with self._run_cv:
-                print("Run starting")
+                yield "Run starting\n"
 
                 perfmode = perfopts['mode']
                 perfcores = perfopts['core_counts']
 
                 with config_lock:
                     from dace.config import Config
                     Config.load(config_path)
@@ -507,52 +492,62 @@
 
                     # Copy the config - this allows releasing the config lock without suffering from potential side effects
                     copied_config = ConfigCopy(Config._config)
 
                 self._slot_available = False
                 dace_state.set_is_compiled(False)
 
-                async_executor = AsyncExecutor(None, True, None, None)
+                terminal_queue = multiprocessing.Queue()
+                async_executor = AsyncExecutor(remote=remote_execution)
                 async_executor.autoquit = True
-                async_executor.executor.output_generator = output_feeder
-                async_executor.executor.setConfig(copied_config)
+                async_executor.executor.output_queue = terminal_queue
+                async_executor.executor.set_config(copied_config)
                 async_executor.run_async(dace_state)
-                async_executor.to_thread_message_queue.put("forcequit")
+                async_executor.to_proc_message_queue.put("forcequit")
 
-                while async_executor.running_thread.is_alive():
+                while async_executor.running_proc.is_alive():
                     try:
-                        new = terminal_queue.get(block=True, timeout=1)
+                        new = terminal_queue.get(timeout=1)
                         yield new
                     except:
-                        # Check if the thread is still running
+                        # Check if the sub-process is still running
                         continue
 
+                # Flush remaining outputs
+                while not terminal_queue.empty():
+                    new = terminal_queue.get(timeout=1)
+                    yield new
+
                 with self._oplock:
                     # Delete from the tasklist
                     del self._task_dict[runindex]
 
-                    print("Run done, notifying")
+                    yield ('Run finished with exit code %d' %
+                           async_executor.running_proc.exitcode)
+
                     self._slot_available = True
 
         return runner
 
 
 @app.route('/')
 def redirect_base():
     return redirect(url_for("index", path="index.html"), code=301)
 
 
-@app.route('/client/<path:path>', methods=['GET'])
+@app.route('/webclient/<path:path>', methods=['GET'])
 def index(path):
     """
         This is an http server (on the same port as the REST API).
-        It serves the files from the 'client'-directory to user agents.
+        It serves the files from the 'webclient'-directory to user agents.
         Note: This is NOT intended for production environments and security is disregarded!
     """
-    return send_from_directory("client", path)
+    return send_from_directory(
+        os.path.join(os.path.dirname(os.path.abspath(__file__)), "webclient"),
+        path)
 
 
 @app.route('/dace/api/v1.0/getPubSSH/', methods=['GET'])
 def getPubSSH():
     try:
         with open(os.path.expanduser("~/.ssh/id_rsa.pub")) as f:
             key = f.read()
@@ -562,15 +557,15 @@
         print("Failed to open keyfile")
         traceback.print_exc()
         return jsonify({"pubkey": "0"})
 
 
 @app.route('/dace/api/v1.0/getEnum/<string:name>', methods=['GET'])
 def getEnum(name):
-    """   
+    """
         Helper function to enumerate available values for `ScheduleType`.
 
         Returns:
             enum: List of string-representations of the values in the enum
     """
 
     valid_params = enum_list
@@ -652,31 +647,14 @@
             "type": typestr,
             "default": str(x.default),
             "value": str(val)
         })
     return ret
 
 
-def set_properties_from_json(obj, prop, sdfg=None):
-    if prop['default'] == "None" and sdfg is None:
-        # This dropout is only valid for transformations
-        # Properties without a default are transformation-generic and should not be settable.
-        pass
-    else:
-        # Catching some transcription errors
-        val = prop['value'] == 'True' if prop['type'] == 'bool' else prop[
-            'value']
-        if any(map(lambda x: x in prop['type'], enum_list)):
-            # This is an enum. If the value was fully qualified, it needs to be trimmed
-            if '.' in val:
-                val = val.split('.')[-1]
-        dace.properties.set_property_from_string(
-            prop['name'], obj, json.dumps(val), sdfg, from_json=True)
-
-
 def applySDFGProperty(sdfg, property_element, step=None):
 
     try:
         prop_step = int(property_element['step'])
     except:
         print("[Warning] Prop step was not provided")
         prop_step = 0
@@ -687,15 +665,15 @@
         return sdfg
 
     sid = int(property_element['state_id'])
     nid = int(property_element['node_id'])
     node = sdfg.find_node(sid, nid)
 
     for prop in property_element['params']:
-        set_properties_from_json(node, prop, sdfg)
+        dace.serialize.set_properties_from_json(node, prop, context=sdfg)
 
     return sdfg
 
 
 def applySDFGProperties(sdfg, properties, step=None):
 
     for x in properties:
@@ -730,30 +708,30 @@
                     name += "$" + str(tmp)
 
             if name == x['name']:
                 #for prop in x['params']['props']:
                 #if prop['name'] == 'subgraph': continue
                 #set_properties_from_json(pattern, prop, sdfg)
 
-                dace.properties.Property.set_properties_from_json(
-                    pattern, x['params']['props'], context={'sdfg': sdfg})
+                dace.serialize.set_properties_from_json(
+                    pattern, x['params']['props'], context=sdfg)
                 pattern.apply_pattern(sdfg)
 
                 if not useGlobalSuffix:
                     break
 
         step += 1
     sdfg = applySDFGProperties(sdfg, sdfg_props, step)
     return sdfg
 
 
 def create_DaceState(code, sdfg_dict, errors):
     dace_state = None
     try:
-        dace_state = DaceState(code, "fake.py", headless=True)
+        dace_state = DaceState(code, "fake.py", remote=remote_execution)
         for x in dace_state.sdfgs:
             name, sdfg = x
             sdfg_dict[name] = sdfg
 
         return dace_state
 
     except SyntaxError as se:
@@ -848,52 +826,52 @@
 
         dace_state = None
         in_sdfg = None
         if "sdfg" in request.json:
             in_sdfg = request.json['sdfg']
             if isinstance(in_sdfg, list):
                 if len(in_sdfg) > 1:
-                    print("More than 1 sdfg provided!")
-                    raise Exception("#TODO: Allow multiple sdfg inputs")
+                    # TODO: Allow multiple sdfg inputs
+                    raise NotImplementedError("More than 1 SDFG provided")
 
                 in_sdfg = in_sdfg[0]
 
             if isinstance(in_sdfg, str):
                 in_sdfg = json.loads(in_sdfg)
 
             if isinstance(in_sdfg, dict):
                 # Generate callbacks (needed for elements referencing others)
                 def loader_callback(name: str):
                     # Check if already available and if yes, return it
                     if name in sdfg_dict:
                         return sdfg_dict[name]
 
                     # Else: This function has to recreate the given sdfg
-                    sdfg_dict[name] = dace.SDFG.fromJSON_object(
+                    sdfg_dict[name] = dace.SDFG.from_json(
                         in_sdfg[name], {
                             'sdfg': None,
                             'callback': loader_callback
                         })
                     sdfg_eval_order.append(name)
                     return sdfg_dict[name]
 
                 for k, v in in_sdfg.items():
                     # Leave it be if the sdfg was already created
                     # (this might happen with SDFG references)
                     if k in sdfg_dict: continue
                     if isinstance(v, str):
                         v = json.loads(v)
-                    sdfg_dict[k] = dace.SDFG.fromJSON_object(
+                    sdfg_dict[k] = dace.SDFG.from_json(
                         v, {
                             'sdfg': None,
                             'callback': loader_callback
                         })
                     sdfg_eval_order.append(k)
             else:
-                in_sdfg = dace.SDFG.fromJSON_object(in_sdfg)
+                in_sdfg = dace.SDFG.from_json(in_sdfg)
                 sdfg_dict[in_sdfg.name] = in_sdfg
         else:
             print("Using code to compile")
             code = request.json['code']
             if (isinstance(code, list)):
                 if len(code) > 1:
                     print("More than 1 code file provided!")
@@ -943,15 +921,15 @@
                     code_tuple_dict[n] = codegen.generate_code(s)
 
         if dace_state is None:
             if "code" in request.json:
                 in_code = request.json['code']
             else:
                 in_code = ""
-            dace_state = DaceState(in_code, "tmp.py", headless=True)
+            dace_state = DaceState(in_code, "tmp.py", remote=remote_execution)
             dace_state.set_sdfg(
                 list(codegen_sdfgs_dace_state.values())[0],
                 list(codegen_sdfgs_dace_state.keys())[0])
             if len(dace_state.errors) > 0:
                 print("ERRORS: " + str(dace_state.errors))
                 errors.extend(dace_state.errors)
 
@@ -982,16 +960,15 @@
             properties = []
             if p is not None:
                 sid = p.state_id
                 nodes = list(p.subgraph.values())
                 for n in nodes:
                     nodeids.append([sid, n])
 
-                properties = json.loads(
-                    dace.properties.Property.all_properties_to_json(p))
+                properties = dace.serialize.all_properties_to_json(p)
             optimizations.append({
                 'opt_name': label,
                 'opt_params': properties,
                 'affects': nodeids,
                 'children': []
             })
 
@@ -1193,15 +1170,15 @@
     """
         This function is equivalent to the old DIODE "Run"-Button.
 
         POST-Parameters:
             (Same as for compile(), language defaults to 'dace')
             perfmodes: list including every queried mode
             corecounts: list of core counts (one run for every number of cores)
-            
+
     """
 
     try:
         perfmodes = request.json['perfmodes']
     except:
         perfmodes = ["noperf"]
 
@@ -1254,25 +1231,23 @@
 def optimize():
     """
         Returns a list of possible optimizations (transformations) and their properties.
 
 
         POST-Parameters:
             input_code: list. Contains all necessary input code files
-            [opt] optpath:  list of dicts, as { name: <str>, params: <dict> }. Contains the current optimization path/tree.
+            optpath:  list of dicts, as { name: <str>, params: <dict> }. Contains the current optimization path/tree.
                             This optpath is applied to the provided code before evaluating possible pattern matches.
+            client_id: For identification. May be unique across all runs,
+                       must be unique across clients
 
-            client_id: <string>:    For later identification. May be unique across all runs, 
-                                    must be unique across clients
-
-        Returns:
-            matching_opts:  list of dicts, as { opt_name: <str>, opt_params: <dict>, affects: <list>, children: <recurse> }.
+        :return: matching_opts:  list of dicts, as { opt_name: <str>, opt_params: <dict>, affects: <list>, children: <recurse> }.
                             Contains the matching transformations.
                             `affects` is a list of affected node ids, which must be unique in the current program.
-    
+
     """
     tmp = compileProgram(request, 'dace')
     if len(tmp) > 1:
         sdfgs, code_tuples, dace_state = tmp
     else:
         # Error
         return jsonify({'error': tmp})
@@ -1296,100 +1271,53 @@
                                 The step element of the dicts is optional. If it is provided, it specifies the number
                                 of optpath elements that preceed it. E.g. a step value of 0 means that the property is applied before the first optimization.
                                 If it is omitted, the property is applied after all optimization steps, i.e. to the resulting SDFG
 
             [opt] perf_mode:    string. Providing "null" has the same effect as omission. If specified, enables performance instrumentation with the counter set
                                 provided in the DaCe settings. If null (or omitted), no instrumentation is enabled.
 
-            client_id: <string>:    For later identification. May be unique across all runs, 
+            client_id: <string>:    For later identification. May be unique across all runs,
                                     must be unique across clients
 
         Returns:
             sdfg: object. Contains a serialization of the resulting SDFGs.
             generated_code: string.     Contains the output code
             sdfg_props: object. Contains a dict of all properties for
                                 every existing node of the sdfgs returned
                                 in the sdfg field
     """
 
     tmp = None
     try:
         tmp = compileProgram(request, language)
-    except Exception as e:
-        return jsonify({'error': str(e), 'traceback': traceback.format_exc()})
-
-    if len(tmp) > 1:
-        sdfgs, code_tuples, dace_state = tmp
-    else:
-        # Error
-        return jsonify({'error': tmp})
-
-    opts = get_transformations(sdfgs)
-    compounds = {}
-    for n, s in sdfgs.items():
-        compounds[n] = {
-            "sdfg": json.loads(s.toJSON()),
-            "matching_opts": opts[n]['matching_opts'],
-            "generated_code": [*map(lambda x: x.code, code_tuples[n])]
-        }
-    return jsonify({"compounds": compounds})
-
-
-@app.route('/dace/api/v1.0/decompile/<string:obj>/', methods=['POST'])
-def decompile(obj):
-    """
-        De-compiles (pickles) an SDFG in python binary format.
-
-        POST-Parameters:
-            binary: base64 string. The object to pickle (the URL encodes the expected type).
-    """
-
-    import base64, pickle
-
-    try:
-        b64_data = request.json['binary']
-        decoded = base64.decodebytes(b64_data.encode())
-    except:
-        abort(Response("Invalid input", 400))
-    if obj == "SDFG":
-        loaded_sdfg = ""
-        from dace.sdfg import SDFG
 
-        try:
-            loaded_sdfg = SDFG.from_bytes(decoded)
-        except:
-            abort(Response("The provided file is not a valid SDFG", 400))
+        if len(tmp) > 1:
+            sdfgs, code_tuples, dace_state = tmp
+        else:
+            # Error
+            return jsonify({'error': tmp})
 
-        # With the SDFG decoded, we must adhere to the output format of compile() for the best interoperability
-        sdfg_name = loaded_sdfg.name
-        opts = get_transformations({sdfg_name: loaded_sdfg})
-
-        from dace.codegen import codegen
-        gen_code = codegen.generate_code(loaded_sdfg)
-
-        return jsonify({
-            "compounds": {
-                sdfg_name: {
-                    'input_code': loaded_sdfg.sourcecode,
-                    'sdfg': loaded_sdfg.toJSON(),
-                    'matching_opts': opts[sdfg_name]['matching_opts'],
-                    'generated_code': [*map(lambda x: x.code, gen_code)]
-                }
+        opts = get_transformations(sdfgs)
+        compounds = {}
+        for n, s in sdfgs.items():
+            compounds[n] = {
+                "sdfg": s.to_json(),
+                "matching_opts": opts[n]['matching_opts'],
+                "generated_code": [*map(lambda x: x.code, code_tuples[n])]
             }
-        })
+        return jsonify({"compounds": compounds})
 
-    else:
-        print("Invalid object type '" + obj + "' specified for decompilation")
-        abort(400)
+    except Exception as e:
+        return jsonify({'error': str(e), 'traceback': traceback.format_exc()})
 
 
 @app.route('/dace/api/v1.0/diode/themes', methods=['GET'])
 def get_available_ace_editor_themes():
     import glob, os.path
-    path = "./client/external_lib/ace/"
+    path = "./webclient/external_lib/ace/"
 
     files = [f for f in glob.glob(path + "theme-*.js")]
 
     filenames = map(os.path.basename, files)
 
     return jsonify([*filenames])
 
@@ -1440,14 +1368,15 @@
         Config.load()
 
     for path, val in settings_array.items():
         path = path.split("/")
         Config.set(*path, value=val)
 
     Config.save(clientpath)
+    return Config.get()
 
 
 @app.route('/dace/api/v1.0/preferences/<string:operation>', methods=['POST'])
 def diode_settings(operation):
     if operation == "get":
         client_id = request.json['client_id']
         return jsonify(get_settings(client_id))
@@ -1475,74 +1404,57 @@
     parser.add_argument(
         "-l",
         "--localhost",
         action="store_true",
         help="Bind to localhost only")
 
     parser.add_argument(
-        "-ld",
-        "--localdace",
+        "-r",
+        "--remotedace",
         action="store_true",
-        help="Use local commands instead of ssh")
+        help="Use ssh commands instead of locally running dace")
 
     parser.add_argument(
         "-rd",
         "--restoredace",
         action="store_true",
         help="Restore the backup file")
 
+    parser.add_argument(
+        "-e",
+        "--executor",
+        action="store_true",
+        help="Run as an executor server instead of DIODE server")
+
     parser.add_argument("-p", "--port", type=int, help="Port to listen on")
 
     args = parser.parse_args()
 
     if args.restoredace:
         from dace.config import Config
         Config.load("./dace.conf.bak")
         Config.save()
 
-    if args.localdace:
-        from dace.config import Config
-        Config.load()
-        Config.save("./dace.conf.bak")
-        Config.load()
-        Config.set(
-            "execution",
-            "general",
-            "execcmd",
-            value='${command}',
-            autosave=True)
-        Config.set(
-            "execution",
-            "general",
-            "copycmd_r2l",
-            value='cp ${srcfile} ${dstfile}',
-            autosave=True)
-        Config.set(
-            "execution",
-            "general",
-            "copycmd_l2r",
-            value='cp ${srcfile} ${dstfile}',
-            autosave=True)
-        if not os.path.isdir("./client_configs"):
-            os.mkdir("./client_configs")
-        Config.save("./client_configs/default.conf")
+    remote_execution = args.remotedace
 
     es = ExecutorServer()
     es_ref.append(es)
-    app.run(
-        host='localhost' if args.localhost else "0.0.0.0",
-        debug=True,
-        port=args.port,
-        use_reloader=False)
-
-    es.stop()
-else:
-    # Start the executor server
-    es = ExecutorServer()
-    es_ref.append(es)
 
-    import atexit
+    if not args.executor:
+        app.run(
+            host='localhost' if args.localhost else "0.0.0.0",
+            debug=True,
+            port=args.port,
+            use_reloader=False)
 
-    def tmp():
         es.stop()
+    else:
+        import atexit
+
+        def tmp():
+            es.stop()
+
+        atexit.register(tmp)
 
-    atexit.register(tmp)
+        # Wait for an event that will never arrive (passive wait)
+        event = threading.Event()
+        event.wait()
```

### Comparing `dace-0.9.0/diode/optgraph/DaceState.py` & `dace-0.9.5/diode/DaceState.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,79 +12,58 @@
 from dace.transformation import optimizer
 from dace.sdfg import SDFG
 from dace.frontend.python import parser
 from dace.frontend.python.parser import DaceProgram
 
 
 class DaceState:
-    """ This class abstracts away the DaCe implementation from the GUI, the 
-        idea is that you pass in a string of DaCe code and this class will 
-        compile the code, give you access to the SDFG and the generated code, 
-        as well as the matching optimization patterns. 
+    """ This class abstracts the DaCe implementation from the GUI.
+        It accepts a string of DaCe code and compiles it, giving access to
+        the SDFG and the generated code, as well as the matching
+        transformations.
     
         DaCe requires the code to be in a file (for code inspection), but 
         while the user types in the GUI we do not have the data available in a 
-        file. Thus we create a temp directory and save it there. However, the 
-        user might check for the filename in the code, thus we provide the 
+        file. Thus we create a temporary directory and save it there. However,
+        the user might check for the filename in the code, thus we provide the
         original file name in argv[0].
     """
 
     # TODO: rewrite this class to use in-memory code.
 
     def __init__(self,
                  dace_code,
                  fake_fname,
                  source_code=None,
                  sdfg=None,
-                 headless=False):
+                 remote=False):
 
         # TODO: Due to symbols, only one state per process is supported
         dace.symbolic.symbol.erase_all()
 
         self.compiled = False
         self.dace_tmpfile = None
         self.dace_filename = os.path.basename(fake_fname)
         self.sdfg = sdfg  # This is the toplevel one
         self.sdfgs = []  # This is a collection of all the SDFGs
         self.generated_code = []
         self.generated_code_files = None
         self.matching_patterns = []
-        self.headless = headless
         self.dace_code = dace_code
         self.source_code = source_code
+        self.remote = remote
         self.repetitions = None
         self.errors = [
         ]  # Any errors that arise from compilation are placed here to show
         # them once the sdfg is rendered
 
         self.has_multiple_eligible_sdfgs = False
 
         if self.sdfg is not None:
             self.compiled = True
-
-            # Generate python stub to initialize inputs and load the SDFG
-            self.dace_code = """
-# THIS IS AN AUTOGENERATED LOADER FOR A SAVED SDFG
-
-import dace
-import numpy
-
-{initializers}
-
-sdfg = dace.SDFG.from_file("sdfg.out")
-func = sdfg.compile()
-func({args})
-
-{prints}    """.format(
-                initializers=self.get_arg_initializers(),
-                args=", ".join([x + "=" + x for x in self.get_call_args()]),
-                prints='\n'.join([
-                    'print("{x} =", numpy.array2string({x}))'.format(x=x)
-                    for x in self.get_call_args()
-                ]))
             self.sdfgs = [('deserialized', self.sdfg)]
 
         tempdir = tempfile.mkdtemp()
         self.dace_tmpfile = os.path.join(tempdir, self.dace_filename)
         fh = open(self.dace_tmpfile, "wb")
         fh.write(self.dace_code.encode('utf-8'))
         fh.close()
@@ -105,14 +84,16 @@
                           for name, obj in gen_module.items()
                           if isinstance(obj, DaceProgram)]
             self.sdfgs += [(name, obj) for name, obj in gen_module.items()
                            if isinstance(obj, SDFG)]
             try:
                 self.sdfg = self.sdfgs[0][1]
             except IndexError:
+                if len(self.errors) > 0:
+                    raise self.errors[-1]
                 if len(self.sdfgs) == 0:
                     raise ValueError('No SDFGs found in file. SDFGs are only '
                                      'recognized when @dace.programs or SDFG '
                                      'objects are found in the global scope')
                 raise
             if len(self.sdfg) > 1:
                 self.has_multiple_eligible_sdfgs = True
@@ -167,17 +148,16 @@
         #except dace.sdfg.InvalidSDFGError:
         except:
             exstr = StringIO()
             formatted_lines = traceback.format_exc().splitlines()
             exstr.write("Compilation failed:\n%s\n\n" % formatted_lines[-1])
             traceback.print_exc(file=exstr)
             self.generated_code = exstr.getvalue()
-            if self.headless == True:
-                print("Codegen failed!\n" + str(self.generated_code))
-                sys.exit(-1)
+            print("Codegen failed!\n" + str(self.generated_code))
+            sys.exit(-1)
 
     def get_dace_generated_files(self):
         """ Writes the generated code to a temporary file and returns the file
             name. Compiles the code if not already compiled. """
         tempdir = tempfile.mkdtemp()
         self.generated_code_files = []
```

### Comparing `dace-0.9.0/diode/remote_execution.py` & `dace-0.9.5/diode/remote_execution.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,122 +1,185 @@
+import multiprocessing
 import os
 import sys
 import stat
 import tempfile
 import traceback
 import subprocess
-import dace.dtypes
+import runpy
+from typing import List, Callable, Any, AnyStr
 from string import Template
-from dace.codegen.compiler import generate_program_folder
+from dace.sdfg import SDFG
+from dace.codegen.compiler import generate_program_folder, configure_and_compile
+from dace.codegen.codegen import CodeObject
 from dace.config import Config
 from dace.codegen.instrumentation.papi import PAPISettings, PAPIUtils
 
 
-class Executor:
-    """ Remote DaCe program execution management class for DIODE. """
+def _task(obj):
+    obj.run()
 
-    def __init__(self, perfplot, headless, sdfg_renderer, async_host=None):
+
+class FunctionStreamWrapper(object):
+    """ Class that wraps around a function with a stream-like API (write). """
+
+    def __init__(self, *funcs: Callable[[AnyStr], Any]):
+        self.funcs = funcs
+
+    def write(self, *args, **kwargs):
+        for func in self.funcs:
+            func(' '.join(args), **kwargs)
+
+    def flush(self):
+        pass
+
+
+def _output_feeder(terminal: multiprocessing.Queue, output: AnyStr):
+    if isinstance(output, str):
+        # It's already in a usable format
+        pass
+    else:
+        try:
+            output = output.decode('utf-8')
+        except UnicodeDecodeError:
+            # Try again escaping
+            output = output.decode('unicode_escape')
+    terminal.put(output)
+
+
+class Executor(object):
+    """ DaCe program execution management class for DIODE. """
+
+    def __init__(self, remote, async_host=None):
         self.counter = 0
-        self.perfplot = perfplot
-        self.headless = headless
-        self.exit_on_error = self.headless
-        self.rendered_graphs = sdfg_renderer
+        self.remote = remote
+        self.exit_on_error = True
 
         self.running_async = async_host is not None
         self.async_host = async_host
 
         self._config = None
 
-        self.output_generator = None
+        self.output_queue = None
 
-    def setExitOnError(self, do_exit):
+    def set_exit_on_error(self, do_exit):
         self.exit_on_error = do_exit
 
-    def setConfig(self, config):
+    def set_config(self, config):
         self._config = config
 
     def config_get(self, *key_hierarchy):
         if self._config is None:
             return Config.get(*key_hierarchy)
         else:
             return self._config.get(*key_hierarchy)
 
-    def run(self, dace_state, fail_on_nonzero=False):
-        dace_progname = dace_state.get_sdfg().name
-        code_objects = dace_state.get_generated_code()
-
+    @staticmethod
+    def _use_mpi(code_objects: List[CodeObject]):
         # Figure out whether we should use MPI for launching
-        use_mpi = False
         for code_object in code_objects:
             if code_object.target.target_name == 'mpi':
-                use_mpi = True
-                break
+                return True
+        return False
+
+    def run(self, dace_state, fail_on_nonzero=False):
+        sdfg = dace_state.get_sdfg()
 
         # Check counter validity
         PAPIUtils.check_performance_counters(self)
 
+        if self.remote:
+            self.show_output("Executing DaCe program " + sdfg.name + " on " +
+                             self.config_get("execution", "general", "host") +
+                             "\n")
+            self.run_remote(sdfg, dace_state, fail_on_nonzero)
+        else:
+            self.show_output("Executing DaCe program " + sdfg.name +
+                             " locally\n")
+            self.run_local(sdfg, dace_state.get_dace_tmpfile())
+
+    def run_local(self, sdfg: SDFG, driver_file: str):
+        workdir = os.path.join('.dacecache', sdfg.name)
+        code_objects = sdfg.generate_code()
+        use_mpi = Executor._use_mpi(code_objects)
+        # TODO: Implement (instead of pyrun, use mpirun/mpiexec)
+        if use_mpi:
+            raise NotImplementedError('Running MPI locally unimplemented')
+
+        # Pipe stdout/stderr back to client output
+        stdout = sys.stdout
+        stderr = sys.stderr
+        sys.stdout = FunctionStreamWrapper(self.show_output, stdout.write)
+        sys.stderr = FunctionStreamWrapper(self.show_output, stderr.write)
+
+        # Compile SDFG
+        generate_program_folder(sdfg, code_objects, workdir, self._config)
+        configure_and_compile(workdir)
+
+        self.show_output("Running script\n")
+
+        # Run driver script with the compiled SDFG(s) as the default
+        old_usecache = Config.get_bool('compiler', 'use_cache')
+        Config.set('compiler', 'use_cache', value=True)
+        try:
+            runpy.run_path(driver_file, run_name='__main__')
+        # Catching all exceptions, including SystemExit
+        except (Exception, SystemExit) as ex:
+            # Corner case: If exited with error code 0, it is a success
+            if isinstance(ex, SystemExit):
+                # If the exit code is nonzero, "raise" will not trigger a
+                # printout on the server
+                if ex.code != 0:
+                    traceback.print_exc()
+                    raise
+            else:
+                raise
+
+        self.show_output("Execution Terminated\n")
+
+        # Revert configuration and output redirection
+        Config.set('compiler', 'use_cache', value=old_usecache)
+        sys.stdout = stdout
+        sys.stderr = stderr
+
+    def run_remote(self, sdfg: SDFG, dace_state, fail_on_nonzero: bool):
+        dace_progname = sdfg.name
+        code_objects = sdfg.generate_code()
+        use_mpi = Executor._use_mpi(code_objects)
         remote_workdir = self.config_get("execution", "general", "workdir")
-        remote_dace_dir = remote_workdir + "/.dacecache/%s/" % dace_progname
-        self.show_output("Executing DaCe program " + dace_progname + " on " + \
-                self.config_get("execution", "general", "host") + "\n")
+        remote_dace_dir = os.path.join(remote_workdir, ".dacecache",
+                                       dace_progname)
 
         try:
-            if self.running_async:
-                # Add information about what is being run
-                self.async_host.notify("Generating remote workspace")
             tmpfolder = tempfile.mkdtemp()
             generate_program_folder(
-                dace_state.get_sdfg(),
-                code_objects,
-                tmpfolder,
-                config=self._config)
+                sdfg, code_objects, tmpfolder, config=self._config)
             self.create_remote_directory(remote_dace_dir)
             self.copy_folder_to_remote(tmpfolder, remote_dace_dir)
 
-            if self.running_async:
-                # Add information about what is being run
-                self.async_host.notify("Compiling...")
             # call compile.py on the remote node in the copied folder
             self.remote_compile(remote_dace_dir, dace_progname)
 
-            if self.running_async:
-                # Add information about what is being run
-                self.async_host.notify("Done compiling")
-
             # copy the input file and the .so file (with the right name)
             # to remote_dace_dir
             so_name = "lib" + dace_progname + "." + self.config_get(
                 'compiler', 'library_extension')
             self.copy_file_from_remote(remote_dace_dir + "/build/" + so_name,
                                        tmpfolder + "/" + so_name)
             self.copy_file_to_remote(tmpfolder + "/" + so_name,
                                      remote_dace_dir)
 
             dace_file = dace_state.get_dace_tmpfile()
             if dace_file is None:
                 raise ValueError("Dace file is None!")
 
-            # copy the SDFG
-            try:
-                local_sdfg = tmpfolder + "/sdfg.out"
-                sdfg = dace_state.get_sdfg()
-                sdfg.save(local_sdfg)
-                remote_sdfg = remote_workdir + "/sdfg.out"
-                self.copy_file_to_remote(local_sdfg, remote_sdfg)
-            except:
-                print("Could NOT save the SDFG")
-
             remote_dace_file = remote_workdir + "/" + os.path.basename(
                 dace_file)
             self.copy_file_to_remote(dace_file, remote_dace_file)
 
-            if self.running_async:
-                # Add information about what is being run
-                self.async_host.notify("All files copied to remote")
-
             papi = PAPIUtils.is_papi_used(sdfg)
 
             # We got the file there, now we can run with different
             # configurations.
             if papi:
                 multirun_num = PAPISettings.perf_multirun_num(
                     config=self._config)
@@ -128,123 +191,59 @@
                         remote_workdir,
                         remote_dace_file,
                         use_mpi,
                         fail_on_nonzero,
                         omp_num_threads=omp_thread_num,
                         repetitions=dace_state.repetitions,
                         additional_options_dict=optdict)
-
-                    if self.running_async:
-                        # Add information about what is being run
-                        self.async_host.notify("Done option threads=" +
-                                               str(omp_thread_num))
             else:
                 self.remote_exec_dace(
                     remote_workdir,
                     remote_dace_file,
                     use_mpi,
                     fail_on_nonzero,
                     repetitions=dace_state.repetitions)
 
             self.show_output("Execution Terminated\n")
 
             try:
                 self.copy_file_from_remote(remote_workdir + "/results.log",
                                            ".")
-            except:
+            except RuntimeError:
                 pass
 
             if papi:
                 # Copy back the vectorization results
                 PAPIUtils.retrieve_vectorization_report(
                     self, code_objects, remote_dace_dir)
 
                 # Copy back the instrumentation results
                 PAPIUtils.retrieve_instrumentation_results(
                     self, remote_workdir)
 
-            if self.running_async:
-                # Add information about what is being run
-                self.async_host.notify("Cleaning up")
-
             try:
                 self.remote_delete_file(remote_workdir + "/results.log")
-            except:
-                print(
-                    "WARNING: results.log could not be transmitted (probably not created)"
-                )
+            except RuntimeError:
+                pass
 
             self.remote_delete_file(remote_dace_file)
             self.remote_delete_dir(remote_dace_dir)
+        except:  # Running a custom script (the driver file), which can raise
+            # any exception
+            self.show_output(traceback.format_exc())
+            raise
 
-            def deferred():
-                try:
-                    res = self.update_performance_plot("results.log",
-                                                       str(self.counter))
-                    os.remove("results.log")
-                except FileNotFoundError:
-                    print("WARNING: results.log could not be read")
-
-            if not self.headless or self.perfplot is None:
-                if self.running_async and not self.headless:
-                    self.async_host.run_sync(deferred)
-                else:
-                    deferred()
-
-            if self.running_async:
-                # Add information about what is being run
-                self.async_host.notify("Done cleaning")
-
-            # Update the performance data.
-            if self.rendered_graphs is not None:
-                self.rendered_graphs.set_memspeed_target()
-                self.rendered_graphs.render_performance_data(
-                    self.config_get("instrumentation", "papi_mode"))
-        except Exception as e:
-            print("\n\n\n")
-            print("!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!")
-            print("Running the program failed:")
-            traceback.print_exc()
-            print(
-                "Inspect above output for more information about executed command sequence."
-            )
-            print("!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!")
-            if self.headless:
-                sys.exit(1)
-
-        if self.running_async:
-            self.async_host.notify("All done")
         self.counter += 1
 
-    def update_performance_plot(self, resfile, name):
-        # Each result.log will give us many runs of one size and optimization.
-        # We ignore everything in the result log except the timing
-
-        # If no perfplot is set, write it to the output as text with a prefix
-        if self.perfplot is None:
-            import re
-            with open(resfile) as f:
-                data = f.read()
-            p = re.compile('\s(\d+\.\d+)$', re.MULTILINE)
-            times = p.findall(data)
-            self.show_output("\n~#~#" + str(times))
-        else:
-            times = self.perfplot.parse_result_log(resfile)
-            self.perfplot.add_run(name, times)
-            self.perfplot.render()
-        t = sorted([float(s) for s in times])
-        print(t)
-        return t[int(len(t) / 2)]
-
     def show_output(self, outstr):
         """ Displays output of any ongoing compilation or computation. """
 
-        if self.output_generator is not None:
+        if self.output_queue is not None:
             # Pipe the output
-            self.output_generator(outstr)
+            _output_feeder(self.output_queue, outstr)
             return
 
         if isinstance(outstr, str):
             print(outstr, end="", flush=True)
             return
         sys.stdout.buffer.write(outstr)
 
@@ -404,122 +403,97 @@
             if out != '' and out != b'':
                 self.show_output(out)
         stdout, _ = p.communicate(timeout=60)
         self.show_output(stdout)
         if p.returncode != 0 and fail_on_nonzero:
             print("The command " + cmd + " failed (retcode " +\
                     str(p.returncode) + ")!\n")
-            if self.headless and self.exit_on_error:
+            if self.exit_on_error:
                 os._exit(p.returncode)
             else:
-                raise ValueError("The command " + cmd + " failed (retcode " + \
+                raise RuntimeError("The command " + cmd + " failed (retcode " + \
                          str(p.returncode) + ")!")
 
 
-import threading, queue
-
-
 class AsyncExecutor:
     """ Asynchronous remote execution. """
 
-    def __init__(self, perfplot, headless, sdfg_renderer, diode):
+    def __init__(self, remote):
+        self.executor = Executor(remote)
+        self.executor.set_exit_on_error(False)
+        self.to_proc_message_queue = multiprocessing.Queue(128)
+        self.running_proc = None
 
-        self.executor = Executor(perfplot, headless, sdfg_renderer, self)
-        self.executor.setExitOnError(False)
-        self.to_thread_message_queue = queue.Queue(128)
-        self.from_thread_message_queue = queue.Queue(128)
-        self.diode = diode
-        self.running_thread = None
-        self.autoquit = True  # This determines if a "quit"-message stops the thread
+        # This determines if a "quit"-message stops the subprocess
+        self.autoquit = True
 
-        self.sync_run_lock = threading.Lock()
-
-    def counter_issue(self):
-        self.diode.onCounterIssue()
+        self.sync_run_lock = multiprocessing.Lock()
 
     def run_sync(self, func):
 
         # Synchronize using a lock
         def deferred():
             with self.sync_run_lock:
                 func()
             return False
 
-        from gi.repository import GObject
-        GObject.idle_add(deferred)
-
-    def notify(self, message):
-
-        if self.diode is None:
-            return
-
-        import time
-
-        print("Got message " + str(message))
-
-        def deferred():
-
-            status_text = self.diode.builder.get_object("run_status_text")
-            status_progress_bar = self.diode.builder.get_object("run_status")
-            status_text.set_text(message)
-            return False
-
-        from gi.repository import GObject
-        GObject.idle_add(deferred)
-
-        if (message == "All done"):
-            self.to_thread_message_queue.put("quit")
-
-        time.sleep(0.001)  # Equivalent of `sched_yield()` for Python
+        deferred()
 
     def run_async(self, dace_state, fail_on_nonzero=False):
-        if self.running_thread is not None and self.running_thread.is_alive():
-            print("Cannot start another thread!")
+        if self.running_proc is not None and self.running_proc.is_alive():
+            print("Cannot start another sub-process!")
             return
 
-        def task():
-            self.run()
-
-        self.running_thread = threading.Thread(target=task)
-        self.running_thread.start()
+        # Use multiple processes to handle crashing processes
+        self.running_proc = multiprocessing.Process(
+            target=_task, args=(self, ))
+        self.running_proc.start()
 
         self.append_run_async(dace_state, fail_on_nonzero=False)
 
     def append_run_async(self, dace_state, fail_on_nonzero=False):
-        self.to_thread_message_queue.put(("run", dace_state, fail_on_nonzero))
+        self.to_proc_message_queue.put(
+            ("run", (dace_state.dace_code,
+                     dace_state.dace_filename, dace_state.source_code,
+                     dace_state.sdfg.to_json(), dace_state.remote),
+             fail_on_nonzero))
 
     def add_async_task(self, task):
-        self.to_thread_message_queue.put(("execute_task", self, task))
+        self.to_proc_message_queue.put(("execute_task", self, task))
 
     def execute_task(self, task):
         return task()
 
     def callMethod(self, obj, name, *args):
         # Shortcut for executing a simple task
         if name == "execute_task":
             _, subargs = args
 
             return self.execute_task(subargs)
+        elif name == "run":
+            # Convert arguments back to dace_state, deserializing the SDFG
+            from diode.DaceState import DaceState
+            dace_state = DaceState(args[0][0], args[0][1], args[0][2],
+                                   SDFG.from_json(args[0][3]), args[0][4])
+            args = (dace_state, *args[1:])
+
         return getattr(obj, name)(*args)
 
     def run(self):
         while True:
             # Read a message (blocking)
-            msg = self.to_thread_message_queue.get()
+            msg = self.to_proc_message_queue.get()
             if msg == "quit":
-                if self.to_thread_message_queue.empty() and self.autoquit:
+                if self.to_proc_message_queue.empty() and self.autoquit:
                     print("Quitting async execution")
                     break
                 else:
                     # There still is some queued work.
                     continue
             if msg == "forcequit":
                 break
 
             # Unwrap and call
-            ret = self.callMethod(self.executor, *msg)
-
-            # Put the return value (including the complete command)
-            self.from_thread_message_queue.put(("retval", ret, *msg))
+            self.callMethod(self.executor, *msg)
 
     def join(self, timeout=None):
         pass
```

### Comparing `dace-0.9.0/diode/sdfv.py` & `dace-0.9.5/diode/sdfv.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 """ SDFG visualizer that uses Flask, HTML5, and Javascript. """
 
 import json
 import sys
 import os
+import platform
 
 import dace
-
-# Create Flask (Web interface) application
-from flask import Flask, render_template, jsonify, request
-app = Flask(__name__, static_url_path='', static_folder='client')
-
-sdfg_json = None
-
-
-@app.route('/', methods=['GET'])
-def main():
-    return render_template('sdfv.html', sdfg=json.dumps(sdfg_json))
-
+import tempfile
+import jinja2
 
 if __name__ == '__main__':
     if len(sys.argv) != 2:
         print('USAGE: sdfv <PATH TO SDFG FILE>')
         exit(1)
     if os.path.isdir(sys.argv[1]):
         filename = os.path.join(sys.argv[1], 'program.sdfg')
     else:
         filename = sys.argv[1]
 
     if not os.path.isfile(filename):
         print('SDFG file', filename, 'not found')
         exit(2)
 
+    sdfg_json = None
+
     # Open JSON file directly
     with open(filename, 'rb') as fp:
         firstbyte = fp.read(1)
         fp.seek(0)
         if firstbyte == b'{':
             sdfg_json = fp.read().decode('utf-8')
 
     # Load SDFG
     if sdfg_json is None:
         sdfg = dace.SDFG.from_file(filename)
-        sdfg_json = sdfg.toJSON()
+        sdfg_json = sdfg.to_json()
 
-    app.run(port=5799)
+    basepath = os.path.dirname(os.path.realpath(__file__))
+    template_loader = jinja2.FileSystemLoader(
+        searchpath=os.path.join(basepath, 'templates'))
+    template_env = jinja2.Environment(loader=template_loader)
+    template = template_env.get_template('sdfv.html')
+
+    html = template.render(sdfg=json.dumps(sdfg_json), dir=basepath + '/')
+
+    html_filename = filename + ".html"
+
+    with open(html_filename, "w") as fp:
+        fp.write(html)
+    print("File saved at %s" % html_filename)
+
+    system = platform.system()
+
+    if system == 'Windows':
+        os.system(html_filename)
+    elif system == 'Darwin':
+        os.system('open %s' % html_filename)
+    else:
+        os.system('xdg-open %s' % html_filename)
```

### Comparing `dace-0.9.0/scripts/dacelab` & `dace-0.9.5/scripts/dacelab`

 * *Files identical despite different names*

### Comparing `dace-0.9.0/setup.py` & `dace-0.9.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,20 +8,16 @@
 diode_path = os.path.dirname(os.path.abspath(__file__)) + '/diode/'
 runtime_files = [
     f[len(dace_path):]
     for f in glob.glob(dace_path + 'runtime/include/**/*', recursive=True)
 ]
 diode_files = [
     f[len(diode_path):]
-    for f in (glob.glob(diode_path + '**/*.js', recursive=True) +
-              glob.glob(diode_path + '**/*.css', recursive=True) +
-              glob.glob(diode_path + '**/*.html', recursive=True) +
-              glob.glob(diode_path + '**/LICENSE', recursive=True) +
-              glob.glob(diode_path + 'client/external_lib/material/*') +
-              glob.glob(diode_path + 'db_scripts/*', recursive=True))
+    for f in (glob.glob(diode_path + 'webclient/**/*', recursive=True) +
+              glob.glob(diode_path + '**/LICENSE', recursive=True))
 ]
 cub_files = [
     f[len(dace_path):]
     for f in glob.glob(dace_path + 'external/cub/cub/**/*', recursive=True)
 ] + [dace_path + 'external/cub/LICENSE.TXT']
 hlslib_files = [
     f[len(dace_path):] for f in glob.glob(
@@ -32,34 +28,36 @@
 ] + [dace_path + 'external/hlslib/LICENSE.md']
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setup(
     name='dace',
-    version='0.9.0',
+    version='0.9.5',
     url='https://github.com/spcl/dace',
     author='SPCL @ ETH Zurich',
     author_email='talbn@inf.ethz.ch',
     description='Data-Centric Parallel Programming Framework',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
+    packages=find_packages(
+        exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     package_data={
         '': [
             '*.yml', 'codegen/CMakeLists.txt', 'codegen/tools/*.cpp',
-            '../diode/main.glade', 'external/moodycamel/*.h',
-            'external/moodycamel/LICENSE.md', 'codegen/Xilinx_HLS.tcl.in'
+            'external/moodycamel/*.h', 'external/moodycamel/LICENSE.md',
+            'codegen/Xilinx_HLS.tcl.in'
         ] + runtime_files + cub_files + diode_files + hlslib_files
     },
     include_package_data=True,
     install_requires=[
         'numpy', 'networkx >= 2.2', 'astunparse', 'sympy', 'scipy', 'pyyaml',
-        'absl-py', 'ply', 'websockets', 'graphviz', 'requests', 'flask'
+        'absl-py', 'ply', 'websockets', 'graphviz', 'requests', 'flask',
+        'scikit-build', 'cmake'
     ],
     scripts=['scripts/diode', 'scripts/dacelab', 'scripts/sdfv'])
```

