# Comparing `tmp/onnx2kerastl-0.0.96.tar.gz` & `tmp/onnx2kerastl-0.0.97.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.96.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.97.dev1.tar", max compression
```

## Comparing `onnx2kerastl-0.0.96.tar` & `onnx2kerastl-0.0.97.dev1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1067 2023-05-17 10:05:24.840017 onnx2kerastl-0.0.96/LICENSE
--rw-r--r--   0        0        0       66 2023-05-17 10:05:24.840536 onnx2kerastl-0.0.96/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-05-17 10:05:24.840790 onnx2kerastl-0.0.96/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2023-05-17 10:05:24.840968 onnx2kerastl-0.0.96/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2023-06-07 15:57:44.568650 onnx2kerastl-0.0.96/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    14415 2023-06-07 16:25:57.562217 onnx2kerastl-0.0.96/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    11968 2023-05-17 10:05:24.841507 onnx2kerastl-0.0.96/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      584 2023-05-23 13:09:48.518074 onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2023-05-17 10:05:24.841906 onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2023-05-17 10:05:24.842046 onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0      606 2023-05-17 10:05:24.842190 onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0     1730 2023-05-17 10:05:24.842337 onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxlstm.py
--rw-r--r--   0        0        0      605 2023-05-17 10:05:24.842473 onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2023-05-17 10:05:24.842602 onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9380 2023-06-07 16:25:57.562862 onnx2kerastl-0.0.96/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2023-05-17 10:05:24.842900 onnx2kerastl-0.0.96/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3947 2023-05-30 11:43:46.982250 onnx2kerastl-0.0.96/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-05-30 11:55:17.207286 onnx2kerastl-0.0.96/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3791 2023-05-17 10:05:24.843376 onnx2kerastl-0.0.96/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2023-05-17 10:05:24.843508 onnx2kerastl-0.0.96/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5551 2023-05-17 10:05:24.843673 onnx2kerastl-0.0.96/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    16027 2023-06-07 15:57:44.569123 onnx2kerastl-0.0.96/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     3015 2023-05-17 10:05:24.844012 onnx2kerastl-0.0.96/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-05-17 10:05:24.844205 onnx2kerastl-0.0.96/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    17750 2023-06-07 16:25:57.564211 onnx2kerastl-0.0.96/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     5006 2023-06-07 10:11:23.748652 onnx2kerastl-0.0.96/onnx2kerastl/sampling_layers.py
--rw-r--r--   0        0        0     1655 2023-05-17 10:05:24.844792 onnx2kerastl-0.0.96/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     5822 2023-06-07 16:25:57.564995 onnx2kerastl-0.0.96/onnx2kerastl/utils.py
--rw-r--r--   0        0        0     1030 2023-06-07 16:25:57.566693 onnx2kerastl-0.0.96/pyproject.toml
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.96/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-17 10:05:24.840017 onnx2kerastl-0.0.97.dev1/LICENSE
+-rw-r--r--   0        0        0       66 2023-05-17 10:05:24.840536 onnx2kerastl-0.0.97.dev1/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-05-17 10:05:24.840790 onnx2kerastl-0.0.97.dev1/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2023-05-17 10:05:24.840968 onnx2kerastl-0.0.97.dev1/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2023-06-07 15:57:44.568650 onnx2kerastl-0.0.97.dev1/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    14415 2023-06-07 16:25:57.562217 onnx2kerastl-0.0.97.dev1/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    11968 2023-05-17 10:05:24.841507 onnx2kerastl-0.0.97.dev1/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      584 2023-05-23 13:09:48.518074 onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2023-05-17 10:05:24.841906 onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2023-05-17 10:05:24.842046 onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0      606 2023-05-17 10:05:24.842190 onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0     1730 2023-05-17 10:05:24.842337 onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxlstm.py
+-rw-r--r--   0        0        0      605 2023-05-17 10:05:24.842473 onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2023-05-17 10:05:24.842602 onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9380 2023-06-07 16:25:57.562862 onnx2kerastl-0.0.97.dev1/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2023-05-17 10:05:24.842900 onnx2kerastl-0.0.97.dev1/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3947 2023-05-30 11:43:46.982250 onnx2kerastl-0.0.97.dev1/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-05-30 11:55:17.207286 onnx2kerastl-0.0.97.dev1/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3791 2023-05-17 10:05:24.843376 onnx2kerastl-0.0.97.dev1/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2023-05-17 10:05:24.843508 onnx2kerastl-0.0.97.dev1/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5551 2023-05-17 10:05:24.843673 onnx2kerastl-0.0.97.dev1/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    16027 2023-06-07 15:57:44.569123 onnx2kerastl-0.0.97.dev1/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     3015 2023-05-17 10:05:24.844012 onnx2kerastl-0.0.97.dev1/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-05-17 10:05:24.844205 onnx2kerastl-0.0.97.dev1/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    18236 2023-06-08 08:23:24.978235 onnx2kerastl-0.0.97.dev1/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     5006 2023-06-07 10:11:23.748652 onnx2kerastl-0.0.97.dev1/onnx2kerastl/sampling_layers.py
+-rw-r--r--   0        0        0     1655 2023-05-17 10:05:24.844792 onnx2kerastl-0.0.97.dev1/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     5822 2023-06-07 16:25:57.564995 onnx2kerastl-0.0.97.dev1/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1035 2023-06-08 08:23:24.978933 onnx2kerastl-0.0.97.dev1/pyproject.toml
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.97.dev1/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.96/LICENSE` & `onnx2kerastl-0.0.97.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/converter.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/convolution_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/__init__.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxlstm.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxlstm.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/elementwise_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/ltsm_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/normalization_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/operation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/padding_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/reshape_layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,19 +217,26 @@
                     tf_shape = tf.shape(input_0)
                     layers[node_name] = tf.reshape(input_0, [*tf_shape[:first_mismatch], -1, *tf_shape[end_idx_match:]])
                 else:
                     logger.debug('The first argument is Keras/tf layer. Apply keras.Reshape.')
                     logger.debug('Target shape :')
                     logger.debug(np.int32(input_1[1:]))
 
-                    if input_0.shape[0] != input_1[0]:  # keras reshape don't work
-                        layers[node_name] = tf.reshape(input_0, input_1, name=keras_name)
+                    if len(np.int32(input_1[1:])) == 1 and np.int32(input_1[1:])[0] == -1:
+                        if input_0.shape.rank == 1:
+                            input_0 = tf.expand_dims(input_0, 0)
+                        logger.debug('The first argument is Keras/tf layer. Apply keras.Flatten.')
+                        flatten = keras.layers.Flatten(name=keras_name)
+                        layers[node_name] = flatten(input_0)
                     else:
-                        reshape = keras.layers.Reshape(np.int32(input_1[1:]), name=keras_name)
-                        layers[node_name] = reshape(input_0)
+                        if input_0.shape[0] != input_1[0]:  # keras reshape don't work
+                            layers[node_name] = tf.reshape(input_0, input_1, name=keras_name)
+                        else:
+                            reshape = keras.layers.Reshape(np.int32(input_1[1:]), name=keras_name)
+                            layers[node_name] = reshape(input_0)
     else:
         raise AttributeError('Can\'t reshape dynamic size.')
 
 
 def convert_unsqueeze(node, params, layers, lambda_func, node_name, keras_name):
     """
     Convert unsqueeze.
```

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/sampling_layers.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/sampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/onnx2kerastl/utils.py` & `onnx2kerastl-0.0.97.dev1/onnx2kerastl/utils.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.96/pyproject.toml` & `onnx2kerastl-0.0.97.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.96"
+version = "0.0.97.dev1"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.96/PKG-INFO` & `onnx2kerastl-0.0.97.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.96
+Version: 0.0.97.dev1
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

