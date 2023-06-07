# Comparing `tmp/tensorizer-1.1.0.tar.gz` & `tmp/tensorizer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorizer-1.1.0.tar", last modified: Fri May  5 20:46:36 2023, max compression
+gzip compressed data, was "tensorizer-2.0.0.tar", last modified: Wed Jun  7 23:35:05 2023, max compression
```

## Comparing `tensorizer-1.1.0.tar` & `tensorizer-2.0.0.tar`

### file list

```diff
@@ -1,41 +1,39 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-05 20:46:36.964947 tensorizer-1.1.0/
--rw-rw-r--   0 root         (0) root         (0)     7407 2023-03-07 19:10:06.000000 tensorizer-1.1.0/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)     1049 2023-03-16 20:33:00.000000 tensorizer-1.1.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       48 2023-03-20 20:37:06.000000 tensorizer-1.1.0/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)    21912 2023-05-05 20:46:36.964947 tensorizer-1.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    21111 2023-05-02 19:45:36.000000 tensorizer-1.1.0/README.md
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-05 20:46:36.936947 tensorizer-1.1.0/proto/
--rw-rw-r--   0 root         (0) root         (0)       52 2023-03-07 19:10:06.000000 tensorizer-1.1.0/proto/requirements.txt
--rw-rw-r--   0 root         (0) root         (0)      921 2023-03-07 19:10:06.000000 tensorizer-1.1.0/proto/tensors.proto
--rw-rw-r--   0 root         (0) root         (0)     1530 2023-05-02 20:22:23.000000 tensorizer-1.1.0/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-05-05 20:46:36.964947 tensorizer-1.1.0/setup.cfg
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-05 20:46:36.944947 tensorizer-1.1.0/tensorizer/
--rw-rw-r--   0 root         (0) root         (0)      183 2023-05-02 18:44:59.000000 tensorizer-1.1.0/tensorizer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6709 2023-05-02 19:17:39.000000 tensorizer-1.1.0/tensorizer/_wide_pipes.py
--rw-rw-r--   0 root         (0) root         (0)     5415 2023-05-02 19:22:34.000000 tensorizer-1.1.0/tensorizer/protobuf.py
--rw-rw-r--   0 root         (0) root         (0)    46239 2023-05-02 19:18:50.000000 tensorizer-1.1.0/tensorizer/serialization.py
--rw-rw-r--   0 root         (0) root         (0)    26472 2023-05-02 19:18:13.000000 tensorizer-1.1.0/tensorizer/stream_io.py
--rw-rw-r--   0 root         (0) root         (0)      921 2023-03-07 19:10:06.000000 tensorizer-1.1.0/tensorizer/tensors.proto
--rw-rw-r--   0 root         (0) root         (0)     4121 2023-05-02 20:14:59.000000 tensorizer-1.1.0/tensorizer/tensors_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    12109 2023-05-05 20:43:52.000000 tensorizer-1.1.0/tensorizer/utils.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-05 20:46:36.948947 tensorizer-1.1.0/tensorizer.egg-info/
--rw-rw-r--   0 root         (0) root         (0)    21912 2023-05-05 20:46:36.000000 tensorizer-1.1.0/tensorizer.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      768 2023-05-05 20:46:36.000000 tensorizer-1.1.0/tensorizer.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-05-05 20:46:36.000000 tensorizer-1.1.0/tensorizer.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       72 2023-05-05 20:46:36.000000 tensorizer-1.1.0/tensorizer.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       11 2023-05-05 20:46:36.000000 tensorizer-1.1.0/tensorizer.egg-info/top_level.txt
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-05 20:46:36.956947 tensorizer-1.1.0/tensors/
--rw-rw-r--   0 root         (0) root         (0)     1049 2023-03-16 20:33:00.000000 tensorizer-1.1.0/tensors/LICENSE
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-07 19:10:06.000000 tensorizer-1.1.0/tensors/__init__.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-05 20:46:36.960947 tensorizer-1.1.0/tensors/__pycache__/
--rw-rw-r--   0 root         (0) root         (0)      145 2023-03-16 22:38:55.000000 tensorizer-1.1.0/tensors/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 root         (0) root         (0)     2631 2023-03-16 22:39:04.000000 tensorizer-1.1.0/tensors/__pycache__/tensors_pb2.cpython-310.pyc
--rw-rw-r--   0 root         (0) root         (0)      100 2023-03-07 19:10:06.000000 tensorizer-1.1.0/tensors/go.mod
--rw-rw-r--   0 root         (0) root         (0)      739 2023-03-07 19:10:06.000000 tensorizer-1.1.0/tensors/go.sum
--rw-rw-r--   0 root         (0) root         (0)    18826 2023-03-07 19:10:06.000000 tensorizer-1.1.0/tensors/tensors.pb.go
--rw-rw-r--   0 root         (0) root         (0)     4846 2023-03-07 19:10:06.000000 tensorizer-1.1.0/tensors/tensors_pb.d.ts
--rw-rw-r--   0 root         (0) root         (0)    29992 2023-03-07 19:10:06.000000 tensorizer-1.1.0/tensors/tensors_pb.js
--rw-rw-r--   0 root         (0) root         (0)     4121 2023-05-02 20:14:59.000000 tensorizer-1.1.0/tensors/tensors_pb2.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-05 20:46:36.960947 tensorizer-1.1.0/tests/
--rw-rw-r--   0 root         (0) root         (0)    10621 2023-05-02 19:38:57.000000 tensorizer-1.1.0/tests/test_serialization.py
--rw-rw-r--   0 root         (0) root         (0)     5871 2023-05-02 19:40:40.000000 tensorizer-1.1.0/tests/test_stream_io.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-06-07 23:35:05.296369 tensorizer-2.0.0/
+-rw-rw-r--   0 root         (0) root         (0)     7407 2023-03-07 19:10:06.000000 tensorizer-2.0.0/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     1049 2023-03-16 20:33:00.000000 tensorizer-2.0.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       48 2023-03-20 20:37:06.000000 tensorizer-2.0.0/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)    24587 2023-06-07 23:35:05.296369 tensorizer-2.0.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    23786 2023-06-06 21:04:46.000000 tensorizer-2.0.0/README.md
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-06-07 23:35:05.268369 tensorizer-2.0.0/proto/
+-rw-rw-r--   0 root         (0) root         (0)       52 2023-03-07 19:10:06.000000 tensorizer-2.0.0/proto/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)      921 2023-03-07 19:10:06.000000 tensorizer-2.0.0/proto/tensors.proto
+-rw-rw-r--   0 root         (0) root         (0)     1530 2023-05-30 17:54:12.000000 tensorizer-2.0.0/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-06-07 23:35:05.296369 tensorizer-2.0.0/setup.cfg
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-06-07 23:35:05.276369 tensorizer-2.0.0/tensorizer/
+-rw-rw-r--   0 root         (0) root         (0)    10231 2023-06-07 18:49:33.000000 tensorizer-2.0.0/tensorizer/_NumpyTensor.py
+-rw-rw-r--   0 root         (0) root         (0)      183 2023-05-02 18:44:59.000000 tensorizer-2.0.0/tensorizer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6709 2023-05-02 19:17:39.000000 tensorizer-2.0.0/tensorizer/_wide_pipes.py
+-rw-rw-r--   0 root         (0) root         (0)     5415 2023-05-02 19:22:34.000000 tensorizer-2.0.0/tensorizer/protobuf.py
+-rw-rw-r--   0 root         (0) root         (0)    52789 2023-06-07 23:30:42.000000 tensorizer-2.0.0/tensorizer/serialization.py
+-rw-rw-r--   0 root         (0) root         (0)    26478 2023-06-07 18:49:47.000000 tensorizer-2.0.0/tensorizer/stream_io.py
+-rw-rw-r--   0 root         (0) root         (0)      921 2023-03-07 19:10:06.000000 tensorizer-2.0.0/tensorizer/tensors.proto
+-rw-rw-r--   0 root         (0) root         (0)     4121 2023-05-02 20:14:59.000000 tensorizer-2.0.0/tensorizer/tensors_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    12109 2023-05-05 20:43:52.000000 tensorizer-2.0.0/tensorizer/utils.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-06-07 23:35:05.284369 tensorizer-2.0.0/tensorizer.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)    24587 2023-06-07 23:35:05.000000 tensorizer-2.0.0/tensorizer.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      702 2023-06-07 23:35:05.000000 tensorizer-2.0.0/tensorizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-06-07 23:35:05.000000 tensorizer-2.0.0/tensorizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       72 2023-06-07 23:35:05.000000 tensorizer-2.0.0/tensorizer.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       11 2023-06-07 23:35:05.000000 tensorizer-2.0.0/tensorizer.egg-info/top_level.txt
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-06-07 23:35:05.292369 tensorizer-2.0.0/tensors/
+-rw-rw-r--   0 root         (0) root         (0)     1049 2023-03-16 20:33:00.000000 tensorizer-2.0.0/tensors/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-03-07 19:10:06.000000 tensorizer-2.0.0/tensors/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      100 2023-03-07 19:10:06.000000 tensorizer-2.0.0/tensors/go.mod
+-rw-rw-r--   0 root         (0) root         (0)      739 2023-03-07 19:10:06.000000 tensorizer-2.0.0/tensors/go.sum
+-rw-rw-r--   0 root         (0) root         (0)    18826 2023-03-07 19:10:06.000000 tensorizer-2.0.0/tensors/tensors.pb.go
+-rw-rw-r--   0 root         (0) root         (0)     4846 2023-03-07 19:10:06.000000 tensorizer-2.0.0/tensors/tensors_pb.d.ts
+-rw-rw-r--   0 root         (0) root         (0)    29992 2023-03-07 19:10:06.000000 tensorizer-2.0.0/tensors/tensors_pb.js
+-rw-rw-r--   0 root         (0) root         (0)     4121 2023-05-02 20:14:59.000000 tensorizer-2.0.0/tensors/tensors_pb2.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-06-07 23:35:05.292369 tensorizer-2.0.0/tests/
+-rw-rw-r--   0 root         (0) root         (0)    11758 2023-06-06 21:28:24.000000 tensorizer-2.0.0/tests/test_serialization.py
+-rw-rw-r--   0 root         (0) root         (0)     5871 2023-05-02 19:40:40.000000 tensorizer-2.0.0/tests/test_stream_io.py
```

### Comparing `tensorizer-1.1.0/CMakeLists.txt` & `tensorizer-2.0.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tensorizer-1.1.0/LICENSE` & `tensorizer-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorizer-1.1.0/PKG-INFO` & `tensorizer-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: tensorizer
-Version: 1.1.0
-Summary: A tool for fast PyTorch module, model, and tensor serialization + deserialization.
-Author: CoreWeave
-License: MIT License
-Project-URL: Homepage, https://github.com/coreweave/tensorizer
-Keywords: tensorizer,machine learning,serialization,tensor,pytorch
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: System :: Distributed Computing
-Classifier: Topic :: Internet
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # tensorizer
 Module, Model, and Tensor Serialization/Deserialization
 
 ## TLDR
 Extremely fast model loads from HTTP/HTTPS and S3 endpoints. GPT-J
 (`20GB`) loads at wire-speed (`~5GB/s`) on a 40GbE network, and is
 only bottlenecked by the Linux kernel TCP stack.
@@ -367,14 +347,71 @@
 Keep in mind that `load_state_dict` is not a fast operation, and will
 likely be much slower than `load_into_module`.
 
 The `state_dict` can also be used to initialize a HuggingFace Transformers
 AutoModel. But HuggingFace Transformers performs three or more copies of
 the data, so memory use will explode.
 
+### `bfloat16` Support
+
+Tensorizer supports models using the `bfloat16` data type. However, tensorizer
+uses numpy to save the tensors as binary and numpy doesn't support `bfloat16`.
+This means that special conversions need to be applied.
+
+To be saved, the torch tensor is cast to `int16` before being converted to
+numpy, which doesn't change any of the underlying data. When serialized, the
+original `bfloat16` datatype string is also saved so that it will be cast back
+to `bfloat16` during the deserialization process.
+
+The `complex32` datatype is supported in a similar way, by casting to `int32`.
+The quantized datatypes (`qint8`, `qint32`, etc.) are not currently supported
+by tensorizer as they would require supplemental quantization parameters to be
+deserialized correctly.
+
+**NOTE:** The exact choice of intermediate types as `int16` and `int32` is
+considered an implementation detail, and is subject to change,
+so they should not be relied upon.
+
+**NOTE2:** This does not interfere with storing actual `int` datatypes
+used in tensors in tensorized files.
+
+### Numpy Support
+
+Tensorizer can be used with `numpy` directly to read and write
+`numpy.ndarray`s.
+
+The serializer's `write_tensor` function handles supplying both
+`torch.Tensor`s and `numpy.ndarray`s.
+
+The deserializer has a separate function `read_numpy_arrays` that will return
+the data as `numpy.ndarray`s.
+
+As explained above in [bfloat16 support](#bfloat16-support), tensorizer uses
+special conversions to write "opaque" datatypes, those not supported by numpy.
+Therefore, special considerations need to be taken when loading such data as
+`numpy.ndarray`s.
+
+By default, the `TensorDeserializer.read_numpy_arrays` function sets its
+`allow_raw_data` parameter to `False`. This means that if a file contains
+opaque datatypes, a `ValueError` will be raised during deserialization.
+
+If you want to return the raw data regardless, set `allow_raw_data` to `True`.
+Otherwise, the file may be read with `TensorDeserializer.read_tensors`
+instead, which yields `torch.Tensor` objects of the correct datatype.
+
+A fifth and sixth variable are also returned by the `read_numpy_arrays`
+generator. The fifth is a `bool` that indicates whether the returned array
+has an opaque datatype and requires special handling (only legal when
+`allow_raw_data=True`). The sixth is a string describing the true, non-numpy
+datatype that the raw data should be interpreted as in such cases.
+For all other datatypes that require no special handling, these are returned as
+`False` and `None`, respectively.
+The exact numpy datatypes used by the returned opaque `numpy.ndarray` objects
+is not guaranteed, and should not be relied upon.
+
 ## Running Tests
 `tensorizer` uses `unittest` for testing.
 The tests have their own set of dependencies, which can be installed with
 `pip install -r tests/requirements.txt`.
 
 Some tests require a GPU, and will be skipped if no GPU is available.
 To run the tests, run the following in the root of the repository:
```

### Comparing `tensorizer-1.1.0/README.md` & `tensorizer-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: tensorizer
+Version: 2.0.0
+Summary: A tool for fast PyTorch module, model, and tensor serialization + deserialization.
+Author: CoreWeave
+License: MIT License
+Project-URL: Homepage, https://github.com/coreweave/tensorizer
+Keywords: tensorizer,machine learning,serialization,tensor,pytorch
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: System :: Distributed Computing
+Classifier: Topic :: Internet
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # tensorizer
 Module, Model, and Tensor Serialization/Deserialization
 
 ## TLDR
 Extremely fast model loads from HTTP/HTTPS and S3 endpoints. GPT-J
 (`20GB`) loads at wire-speed (`~5GB/s`) on a 40GbE network, and is
 only bottlenecked by the Linux kernel TCP stack.
@@ -347,14 +367,71 @@
 Keep in mind that `load_state_dict` is not a fast operation, and will
 likely be much slower than `load_into_module`.
 
 The `state_dict` can also be used to initialize a HuggingFace Transformers
 AutoModel. But HuggingFace Transformers performs three or more copies of
 the data, so memory use will explode.
 
+### `bfloat16` Support
+
+Tensorizer supports models using the `bfloat16` data type. However, tensorizer
+uses numpy to save the tensors as binary and numpy doesn't support `bfloat16`.
+This means that special conversions need to be applied.
+
+To be saved, the torch tensor is cast to `int16` before being converted to
+numpy, which doesn't change any of the underlying data. When serialized, the
+original `bfloat16` datatype string is also saved so that it will be cast back
+to `bfloat16` during the deserialization process.
+
+The `complex32` datatype is supported in a similar way, by casting to `int32`.
+The quantized datatypes (`qint8`, `qint32`, etc.) are not currently supported
+by tensorizer as they would require supplemental quantization parameters to be
+deserialized correctly.
+
+**NOTE:** The exact choice of intermediate types as `int16` and `int32` is
+considered an implementation detail, and is subject to change,
+so they should not be relied upon.
+
+**NOTE2:** This does not interfere with storing actual `int` datatypes
+used in tensors in tensorized files.
+
+### Numpy Support
+
+Tensorizer can be used with `numpy` directly to read and write
+`numpy.ndarray`s.
+
+The serializer's `write_tensor` function handles supplying both
+`torch.Tensor`s and `numpy.ndarray`s.
+
+The deserializer has a separate function `read_numpy_arrays` that will return
+the data as `numpy.ndarray`s.
+
+As explained above in [bfloat16 support](#bfloat16-support), tensorizer uses
+special conversions to write "opaque" datatypes, those not supported by numpy.
+Therefore, special considerations need to be taken when loading such data as
+`numpy.ndarray`s.
+
+By default, the `TensorDeserializer.read_numpy_arrays` function sets its
+`allow_raw_data` parameter to `False`. This means that if a file contains
+opaque datatypes, a `ValueError` will be raised during deserialization.
+
+If you want to return the raw data regardless, set `allow_raw_data` to `True`.
+Otherwise, the file may be read with `TensorDeserializer.read_tensors`
+instead, which yields `torch.Tensor` objects of the correct datatype.
+
+A fifth and sixth variable are also returned by the `read_numpy_arrays`
+generator. The fifth is a `bool` that indicates whether the returned array
+has an opaque datatype and requires special handling (only legal when
+`allow_raw_data=True`). The sixth is a string describing the true, non-numpy
+datatype that the raw data should be interpreted as in such cases.
+For all other datatypes that require no special handling, these are returned as
+`False` and `None`, respectively.
+The exact numpy datatypes used by the returned opaque `numpy.ndarray` objects
+is not guaranteed, and should not be relied upon.
+
 ## Running Tests
 `tensorizer` uses `unittest` for testing.
 The tests have their own set of dependencies, which can be installed with
 `pip install -r tests/requirements.txt`.
 
 Some tests require a GPU, and will be skipped if no GPU is available.
 To run the tests, run the following in the root of the repository:
```

### Comparing `tensorizer-1.1.0/proto/tensors.proto` & `tensorizer-2.0.0/proto/tensors.proto`

 * *Files identical despite different names*

### Comparing `tensorizer-1.1.0/pyproject.toml` & `tensorizer-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tensorizer"
-version = "1.1.0"
+version = "2.0.0"
 license = { text = "MIT License" }
 keywords = ["tensorizer", "machine learning", "serialization", "tensor", "pytorch"]
 authors = [
   { name="CoreWeave" }
 ]
 description = "A tool for fast PyTorch module, model, and tensor serialization + deserialization."
 readme = "README.md"
```

### Comparing `tensorizer-1.1.0/tensorizer/_wide_pipes.py` & `tensorizer-2.0.0/tensorizer/_wide_pipes.py`

 * *Files identical despite different names*

### Comparing `tensorizer-1.1.0/tensorizer/protobuf.py` & `tensorizer-2.0.0/tensorizer/protobuf.py`

 * *Files identical despite different names*

### Comparing `tensorizer-1.1.0/tensorizer/serialization.py` & `tensorizer-2.0.0/tensorizer/serialization.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from enum import Enum
 
 import numpy
 import torch
 
 import tensorizer.stream_io as stream_io
 import tensorizer.utils as utils
+from tensorizer._NumpyTensor import _NumpyTensor
 
 if torch.cuda.is_available():
     cudart = torch.cuda.cudart()
 else:
     cudart = None
 
 from collections import OrderedDict
@@ -50,17 +51,24 @@
 # Whether the tensor is a parameter or a buffer on the model.
 class TensorType(Enum):
     PARAM = 0
     BUFFER = 1
     STATE_DICT = 2
 
 
-TENSORIZER_VERSION = 1
+# If tensors with "opaque" dtypes (those that are not supported by numpy) are
+# saved, then a tensorizer data version of 2 is required to (de)serialize the
+# file. Otherwise, the file is compatible with tensorizer data version 1
+TENSORIZER_VERSION = 2
+NON_OPAQUE_TENSORIZER_VERSION = 1
+
 TENSORIZER_MAGIC = b"|TZR|"
 
+OPAQUE_DTYPE_SEP = "\0"
+
 
 class TensorEntry(typing.TypedDict):
     name: str
     type: TensorType
     offset: int
     data_offset: int
     data_length: int
@@ -74,48 +82,14 @@
 
 
 class TensorHash(typing.TypedDict):
     type: HashType
     hash: bytes
 
 
-def _convert_dtype_to_numpy(dtype: Union[numpy.dtype, str, torch.dtype]):
-    if isinstance(dtype, numpy.dtype):
-        return dtype
-    elif isinstance(dtype, str):
-        return numpy.dtype(dtype)
-    elif isinstance(dtype, torch.dtype):
-        # Converted from PyTorch's own mapping used in their testing:
-        # https://github.com/pytorch/pytorch/blob/v2.0.0/torch/testing/_internal/common_utils.py#L1009
-        numpy_dtype = {
-            torch.bool: numpy.bool_,
-            torch.uint8: numpy.uint8,
-            torch.int8: numpy.int8,
-            torch.int16: numpy.int16,
-            torch.int32: numpy.int32,
-            torch.int64: numpy.int64,
-            torch.float16: numpy.float16,
-            torch.float32: numpy.float32,
-            torch.float64: numpy.float64,
-            torch.complex64: numpy.complex64,
-            torch.complex128: numpy.complex128,
-        }.get(dtype)
-
-        if numpy_dtype is None:
-            raise TypeError(
-                "The provided torch.dtype class could not be converted to a"
-                " numpy.dtype"
-            )
-        else:
-            # Convert it from a dtype class to a dtype object instance
-            return numpy.dtype(numpy_dtype)
-    else:
-        raise TypeError("Could not interpret provided dtype as a numpy.dtype")
-
-
 class TensorDeserializer(collections.abc.Mapping):
     """
     Given a file-like object for read, deserialize tensors to a state_dict or
     a torch.nn.Module.
 
     See the docs_ for a usage walkthrough.
 
@@ -124,16 +98,16 @@
     Args:
         file_obj: A file-like object to read from. It can also be a string
             representing a path to a file or an HTTP/HTTPS/S3 URI.
         device: The device to load the tensors to.
         filter_func: A function (tensor_name: str) -> bool that returns True
             if a tensor should be loaded, or False if it should be skipped.
             If None, all tensors are loaded.
-        dtype: The dtype to load the tensors as. If None, the dtype will be
-            inferred from the file.
+        dtype: The dtype to cast the tensors as when loading them into a torch
+            module. If None, the dtype will be inferred from the file.
         lazy_load: If True, tensors will be loaded and cached when keys are
             accessed. If False, all tensors will be loaded into memory up
             front.
         plaid_mode: If True, tensors will be loaded extremely fast into the
             target device. This is only supported on CUDA devices, and the
             buffers are going to be inconsistent due to the extreme
             naughtiness of reusing a backing buffer. This is only recommended
@@ -186,15 +160,15 @@
             str,
             bytes,
             os.PathLike,
             int,
         ],
         device: Union[torch.device, str, None] = None,
         filter_func: Optional[Callable[[str], Union[bool, Any]]] = None,
-        dtype: Union[numpy.dtype, str, None] = None,
+        dtype: Optional[torch.dtype] = None,
         *,
         lazy_load: bool = False,
         plaid_mode: bool = False,
     ):
         if isinstance(file_obj, (str, bytes, os.PathLike, int)):
             self._file = stream_io.open_stream(file_obj, "rb")
         else:
@@ -202,32 +176,30 @@
             self._file = file_obj
         self.total_compressed_tensor_bytes = 0
         self.read_bytes = 0
 
         # If device is None, use the current device, otherwise use the given
         # device.
         device = utils.get_device() if device is None else torch.device(device)
-        self._device = device
+        self._device: torch.device = device
 
-        # If dtype is not None, convert all tensors to this dtype if possible.
-        if dtype is None:
-            self._dtype = None
-        else:
-            self._dtype = _convert_dtype_to_numpy(dtype)
+        self._dtype: Optional[torch.dtype] = dtype
+
+        self._plaid_mode: bool = plaid_mode
+
+        # plaid_mode implies lazy_load
+        self._lazy_load: bool = lazy_load or plaid_mode
 
         self._metadata: Dict[str, TensorEntry] = {}
 
-        if plaid_mode and (
+        if self._plaid_mode and (
             not torch.cuda.is_available() or self._device.type == "cpu"
         ):
             raise ValueError("Plaid mode requires CUDA")
 
-        # plaid_mode implies lazy_load
-        self._lazy_load = lazy_load or plaid_mode
-
         # Read the magic
         magic = self._file.read(5)
         if magic != TENSORIZER_MAGIC:
             raise ValueError("Not a tensorizer file")
 
         # Read the version
         version = struct.unpack("<I", self._file.read(4))[0]
@@ -253,15 +225,14 @@
 
         # Read the metadata index of tensors. This is a list of offsets into the
         # file where the per-tensor data is stored. filter_func is a test that
         # determines the tensor names to read. If filter_func is None,
         # all tensors are read.
         self._load_metadatas(filter_func)
 
-        self._plaid_mode: bool = plaid_mode
         self._prior_key: Optional[str] = None
 
         # We calculate the total tensor bytes here so that we can use mmap,
         # based on the total size of the tensors that we're going to read,
         # filtered by the filter_func.
         self.total_tensor_bytes = 0
         self._largest_tensor_bytes = 0
@@ -271,15 +242,15 @@
                 self._largest_tensor_bytes = metadata["data_length"]
 
         # Allocate the buffer for the tensors. If we're not in lazy_load mode,
         # we'll allocate a single buffer for all the tensors. Otherwise, we'll
         # allocate a buffer for the largest tensor.
         self._buffer_addr = None
         self._is_memory_pinned = False
-        if not lazy_load and not plaid_mode:
+        if not self._lazy_load and not self._plaid_mode:
             start_allocate = time.time()
 
             # Check if our platform supports mmap.MAP_ANONYMOUS and
             # mmap.MAP_PRIVATE
             mmap_flags = 0
             mmap_flags |= getattr(mmap, "MAP_PRIVATE", 0)
             mmap_flags |= getattr(mmap, "MAP_ANONYMOUS", 0)
@@ -320,15 +291,15 @@
         # Our cache of tensors. This is a dict of name -> tensor. If lazy_load
         # is True, then the tensors are not loaded until they are accessed.
         self._cache: typing.OrderedDict[str, Union[torch.Tensor, None, bool]]
 
         # The offset in the file where the tensor data begins.
         self._tensors_begin = self._file.tell()
 
-        if not lazy_load:
+        if not self._lazy_load:
             # If we're not in lazy_load mode, we populate the cache with all
             # the tensors.
             self._cache = self._generate_state_dict()
         else:
             # We populate the cache with None values so that we can
             # differentiate between tensors that have not been loaded yet
             # and tensors that are not present in the file.
@@ -551,23 +522,22 @@
                 hash=hash_bytes,
             )
             hash_idx = hash_end
             hashes.append(hash_entry)
 
         return hashes
 
-    def read_tensors(
+    def _read_numpytensors(
         self,
         filter_func: Optional[Callable[[str], Union[bool, Any]]] = None,
         num_tensors: int = -1,
-    ) -> Iterator[Tuple[int, int, str, numpy.ndarray]]:
+    ) -> Iterator[Tuple[int, int, str, _NumpyTensor]]:
         """
         A generator that deserializes tensors and returns the `module_idx`,
-        `tensor_type`, parameter/buffer `name`, and the numpy `arr` that
-        represents the tensor.
+        `tensor_type`, parameter/buffer `name`, and a _NumpyTensor `tensor`.
 
         Note that this function does not seek to the beginning of the tensor
         data. It assumes that the file pointer is already at the beginning
         of the tensor data that it should read.
 
         It will read `num_tensors` tensors from the file, or all tensors
         if `num_tensors` is -1.
@@ -605,15 +575,28 @@
                 idx = name_sz + 5
                 name_bytes = headers[5:idx]
                 name: str = name_bytes.decode("utf-8")
 
                 # Read the dtype of the tensor.
                 dtype_len = struct.unpack("<B", headers[idx : idx + 1])[0]
                 dtype_end = idx + dtype_len + 1
-                dtype = headers[idx + 1 : dtype_end]
+                dtype = headers[idx + 1 : dtype_end].decode("utf-8")
+
+                numpy_dtype, *torch_dtype = dtype.split(OPAQUE_DTYPE_SEP)
+                if len(torch_dtype) == 0:
+                    torch_dtype = None
+                elif len(torch_dtype) == 1:
+                    torch_dtype = torch_dtype[0]
+                else:
+                    raise ValueError(
+                        "Can't deserialize a tensor with "
+                        "multiple opaque dtype separators "
+                        f"({OPAQUE_DTYPE_SEP!r}) in its dtype: "
+                        f"{dtype!r}"
+                    )
 
                 # Read the shape amount, according to the serialized format.
                 # The shape length is 1 byte after the dtype end.
                 shape_len = struct.unpack(
                     "<B", headers[dtype_end : dtype_end + 1]
                 )[0]
                 # The shape elements are <I, so we read 4 bytes. _read_shapes
@@ -681,52 +664,192 @@
                     # In lazy_load mode, we allocate a new buffer for each
                     # tensor. This is a bit slower, but it's the only way
                     # to support lazy loading.
                     buffer = bytearray(data_length)
                     mv = memoryview(buffer)
                     self._file.readinto(mv)
 
-                # Convert the memoryview to a numpy array. We use the
-                # memmap class to avoid copying the data.
-                arr = numpy.ndarray.__new__(
-                    numpy.memmap,
+                tensor = _NumpyTensor.from_buffer(
+                    numpy_dtype,
+                    torch_dtype,
                     shape_list,
-                    dtype=dtype,
-                    buffer=mv,
-                    offset=0,
+                    mv,
                 )
+
                 tensors_read += 1
-                yield module_idx, tensor_type, name, arr
+
+                yield module_idx, tensor_type, name, tensor
         except EOFError:
             return
 
+    def read_tensors(
+        self,
+        filter_func: Optional[Callable[[str], Union[bool, Any]]] = None,
+        num_tensors: int = -1,
+    ) -> Iterator[Tuple[int, int, str, torch.Tensor]]:
+        """
+        A generator that deserializes tensors and returns the `module_idx`,
+        `tensor_type`, parameter/buffer `name`, and torch `tensor`.
+
+        Note that this function does not seek to the beginning of the tensor
+        data. It assumes that the file pointer is already at the beginning
+        of the tensor data that it should read.
+
+        It will read `num_tensors` tensors from the file, or all tensors
+        if `num_tensors` is -1.
+
+        The generator yields tuples of the form:
+            (module_idx, tensor_type, name, tensor)
+
+        Args:
+            filter_func: A function that takes a tensor name and returns
+                True if the tensor should be returned, False otherwise.
+            num_tensors: The number of tensors to read. If -1, all tensors
+                will be read. If the zero-byte header is encountered before
+                `num_tensors` tensors are read, the generator will stop
+                yielding values.
+
+        Yields:
+            Tuples of the form (module_idx, tensor_type, name, tensor).
+        """
+
+        data = self._read_numpytensors(
+            filter_func=filter_func, num_tensors=num_tensors
+        )
+        for module_idx, tensor_type, name, tensor in data:
+            yield module_idx, tensor_type, name, tensor.to_tensor()
+
+    def read_numpy_arrays(
+        self,
+        filter_func: Optional[Callable[[str], Union[bool, Any]]] = None,
+        num_tensors: int = -1,
+        allow_raw_data: bool = False,
+    ) -> Iterator[Tuple[int, int, str, numpy.ndarray, bool, Optional[str]]]:
+        """
+        A generator that deserializes tensors and returns the `module_idx`,
+        `tensor_type`, parameter/buffer `name`, the numpy `arr` that
+        represents the tensor, a boolean representing if the returned datatype
+        is opaque, and the name of the true datatype represented by the opaque
+        data, if applicable.
+
+
+        "Opaque data" refers to numpy arrays holding accurate raw binary data
+        but an invalid dtype attribute, occurring when there is no numpy dtype
+        corresponding to the original type that was serialized.
+        These are only returned if `allow_raw_data` is set to `True`,
+        otherwise, encountering such a datatype is an error,
+        and the file should instead be deserialized with
+        `TensorDeserializer.read_tensors()`.
+
+        For example, if a ``torch.Tensor`` with the dtype ``torch.bfloat16``
+        is serialized, then it can be accurately deserialized using
+        `TensorDeserializer.read_tensors()`. Since there is no numpy type
+        corresponding to ``torch.bfloat16``, attempting to deserialize the same
+        file via `TensorDeserializer.read_numpy_arrays()` will raise a
+        ``ValueError``.
+        However, if `allow_raw_data` is set to ``True``, then
+        `TensorDeserializer.read_numpy_arrays()` will return these
+        arrays regardless, and the final two values of the yielded tuple,
+        `is_opaque` and `torch_dtype`, will be ``True`` and a string
+        representing the true non-numpy datatype represented by the data,
+        respectively. Special handling is then required to use the returned
+        data accurately.
+
+
+
+        Note that this function does not seek to the beginning of the tensor
+        data. It assumes that the file pointer is already at the beginning
+        of the tensor data that it should read.
+
+        It will read `num_tensors` tensors from the file, or all tensors
+        if `num_tensors` is -1.
+
+        The generator yields tuples of the form:
+            (module_idx, tensor_type, name, arr, is_opaque, torch_dtype)
+
+        See also: `TensorDeserializer.read_tensors`
+
+        Args:
+            filter_func: A function that takes a tensor name and returns
+                True if the tensor should be returned, False otherwise.
+            num_tensors: The number of tensors to read. If -1, all tensors
+                will be read. If the zero-byte header is encountered before
+                `num_tensors` tensors are read, the generator will stop
+                yielding values.
+            allow_raw_data: Whether to return numpy arrays containing
+                uninterpretable opaque datatypes. If False and opaque
+                datatypes are encountered, then a `ValueError` is raised.
+                Defaults to False.
+
+        Yields:
+            Tuples of the form:
+            (
+                module_idx,
+                tensor_type,
+                name,
+                arr,
+                is_opaque,
+                torch_dtype
+            )
+            If the `allow_raw_data` parameter is ``False`` (the default),
+            the final two elements are always ``False`` and ``None``,
+            respectively. Otherwise, ``is_opaque`` may be ``True``, and
+            ``torch_dtype`` will then be a string representing the actual
+            non-numpy datatype represented by the data in `arr`.
+
+        Raises:
+            ValueError: If an opaque datatype is encountered in the file
+                and ``allow_raw_data=False``.
+        """
+
+        data = self._read_numpytensors(
+            filter_func=filter_func, num_tensors=num_tensors
+        )
+        for module_idx, tensor_type, name, tensor in data:
+            is_opaque = tensor.is_opaque
+            arr = tensor.data
+            torch_dtype = tensor.torch_dtype if is_opaque else None
+
+            if is_opaque and not allow_raw_data:
+                np_dtype = arr.dtype.str
+                raise ValueError(
+                    f"{name} has an opaque datatype: "
+                    f"(Torch: {tensor.torch_dtype}, Numpy: {np_dtype}). "
+                    "Set `allow_raw_data=True` to return as a numpy array "
+                    f"with a datatype of {np_dtype}"
+                )
+
+            yield module_idx, tensor_type, name, arr, is_opaque, torch_dtype
+
     def _to_torch_parameter(
-        self, arr: Union[numpy.ndarray, torch.nn.Parameter]
+        self, tensor: Union[torch.Tensor, torch.nn.Parameter]
     ) -> torch.nn.Parameter:
         """
-        Convert a numpy array to a torch.nn.Parameter on a device, forcing
+        Convert a tensor to a torch.nn.Parameter on a device, forcing
         gradient when appropriate. We also handle torch.nn.Parameter objects in
         a passthrough manner.
         """
-        if isinstance(arr, torch.nn.Parameter):
-            arr.data = arr.data.to(self._device)
-            if arr.grad is not None:
-                arr.grad = arr.grad.to(self._device)
-            return arr
+        if isinstance(tensor, torch.nn.Parameter):
+            tensor.data = tensor.data.to(self._device)
+            if tensor.grad is not None:
+                tensor.grad = tensor.grad.to(self._device)
+            return tensor
 
+        # Cast the tensor if a global dtype was given to the TensorDeserializer
         if (
             self._dtype is not None
-            and arr.dtype != "bool"
-            and arr.dtype != self._dtype
+            and tensor.dtype != torch.bool
+            and torch.dtype != self._dtype
         ):
-            arr = arr.astype(self._dtype)
-        gradient = arr.dtype.kind in ("f", "c")
+            tensor = tensor.to(self._dtype)
+
+        gradient = tensor.dtype.is_complex or tensor.dtype.is_floating_point
 
         return torch.nn.Parameter(
-            torch.from_numpy(arr).to(self._device), requires_grad=gradient
+            tensor.to(self._device), requires_grad=gradient
         )
 
     def _generate_state_dict(self) -> OrderedDict:
         """
         Load the tensors in this Tensorizer object into a state_dict. This
         is used to populate the cache in non-lazy_load cases.
         """
@@ -864,15 +987,17 @@
         else:
             self.lz4_frame = None
 
         # Write our magic bytes.
         self._file.write(TENSORIZER_MAGIC)
 
         # Write the version number.
-        self._file.write(struct.pack("<I", TENSORIZER_VERSION))
+        self._version_loc = self._file.tell()
+        self._version = NON_OPAQUE_TENSORIZER_VERSION
+        self._file.write(struct.pack("<I", self._version))
 
         # Reserve 32 bytes for the hash. (Unused for now)
         self._hash_loc = self._file.tell()
         self._file.write(struct.pack("<Q", 0) * 4)
 
         # Reserve 8 bytes for the total size of the file.
         self._size_loc = self._file.tell()
@@ -940,24 +1065,33 @@
             compression_ratio = (
                 self.total_tensor_bytes / self.total_compressed_tensor_bytes
             )
             logger.info(f"Uncomp'd bytes: {self.total_tensor_bytes}")
             logger.info(f"Comp'd bytes: {self.total_compressed_tensor_bytes}")
             logger.info(f"Ratio: {compression_ratio:.2f}")
 
-    def _sync_prologue_state(self):
+    def _sync_prologue_state(self, update_version: bool = False):
         """
         This is called after the tensor has been written to the file, and
         ensures that the file is in a consistent state.
+
+        Args:
+            update_version: If true, the file's version will be updated to
+                `self._version`.
         """
         curr = self._file.tell()
 
         # Write our zero-length field, that indicates that this is the last
         # tensor. This will be overwritten if another tensor is written.
         self._file.write(struct.pack("<Q", 0))
+
+        if update_version:
+            self._file.seek(self._version_loc)
+            self._file.write(struct.pack("<I", self._version))
+
         # Write the total number of tensors.
         self._file.seek(self._tensor_ct_loc)
         self._file.write(struct.pack("<Q", self._tensors))
         # Write our total file size.
         self._file.seek(self._size_loc)
         self._file.write(struct.pack("<Q", curr))
         # Write the total bytes of tensor data written.
@@ -1006,18 +1140,31 @@
               []char                        hash_str,
              }                              hashes,
            uint64                           tensor_sz,
            []byte                           tensor }
         """
 
         if isinstance(tensor, torch.Tensor):
-            tensor = tensor.cpu().detach().numpy()
+            numpy_tensor = _NumpyTensor.from_tensor(tensor)
+        else:
+            numpy_tensor = _NumpyTensor.from_array(tensor)
 
-        if len(str(tensor.dtype)) >= 256:
-            raise ValueError("dtype length should be less than 256")
+        dtype_name = numpy_tensor.numpy_dtype
+        update_version = False
+        if numpy_tensor.is_opaque:
+            # The datatype name needs to contain both the numpy dtype that the
+            # data is serialized as and the original torch dtype.
+            dtype_name += OPAQUE_DTYPE_SEP + numpy_tensor.torch_dtype
+
+            if self._version != TENSORIZER_VERSION:
+                self._version = TENSORIZER_VERSION
+                update_version = True
+
+        if len(dtype_name) >= 256:
+            raise ValueError("dtype name length should be less than 256")
 
         # Reserve room for our tensor header size.
         ds_header_begin = self._file.tell()
         self._file.write(struct.pack("<Q", 0))
 
         # Module index.
         self._file.write(struct.pack("<H", idx))
@@ -1027,21 +1174,21 @@
 
         # Parameter/buffer name
         name_bytes = bytes(name, "utf-8")
         self._file.write(struct.pack("<H", len(name_bytes)))
         self._file.write(name_bytes)
 
         # Write out our tensor dtype
-        dtype_bytes = bytes(tensor.dtype.str, "utf-8")
+        dtype_bytes = bytes(dtype_name, "utf-8")
         dtype_len = len(dtype_bytes)
         self._file.write(struct.pack("<B", dtype_len))
         self._file.write(dtype_bytes)
 
         # ... and shape
-        shape_bytes = self._dump_shape(tensor.shape)
+        shape_bytes = self._dump_shape(numpy_tensor.data.shape)
         self._file.write(shape_bytes)
 
         # Reserve room for our tensor hashes.
         hash_loc = self._file.tell()
         # Reserve the length of the hash data structures.
         self._file.write(struct.pack("<H", 0))
         # Write the number of hashes we're going to write.
@@ -1080,28 +1227,28 @@
         if self.compress_tensors:
             # NOTE: This compression feature is not complete, as we do not
             #       yet decompress. This was judged to *not* be worthwhile.
             #       This is left here as an example for future adventurers that
             #       may want to do model compression.
             # Create a write buffer to compress our tensor serialization.
             tensor_buffer = tempfile.TemporaryFile()
-            tensor.tofile(tensor_buffer)
+            numpy_tensor.data.tofile(tensor_buffer)
             tensor_raw_sz = tensor_buffer.tell()
             self.total_tensor_bytes += tensor_raw_sz
             tensor_buffer.seek(0)
             tensor_compressed = self.lz4_frame.compress(tensor_buffer.read())
             tensor_compressed_sz = len(tensor_compressed)
             compression_ratio = (tensor_raw_sz * 1.0) / tensor_compressed_sz
             if compression_ratio > 2:
                 self.total_compressed_tensor_bytes += tensor_compressed_sz
             else:
                 self.total_compressed_tensor_bytes += tensor_raw_sz
 
         # Serialize our tensors
-        tensor.tofile(self._file)
+        numpy_tensor.data.tofile(self._file)
         tensor_endpos = self._file.tell()
 
         # Go back and write our tensor length out
         self._file.seek(tensor_size_loc, io.SEEK_SET)
         # We write this signed, so that we can use the signedness as an
         # indicator of possible tensor compression in the future.
         tensor_size = tensor_endpos - tensor_startpos
@@ -1145,15 +1292,15 @@
         self._file.write(sha256)
 
         # Move to the end of our serialized tensor to prepare for the next one.
         self._file.seek(tensor_endpos)
         self._tensors += 1
 
         # Update our prolog and epilog.
-        self._sync_prologue_state()
+        self._sync_prologue_state(update_version=update_version)
 
         ds_size = self._file.tell() - ds_header_begin
         ds_bytes = f"{ds_size:,} bytes"
 
         typ = {
             TensorType.PARAM: "p",
             TensorType.BUFFER: "b",
```

### Comparing `tensorizer-1.1.0/tensorizer/stream_io.py` & `tensorizer-2.0.0/tensorizer/stream_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         end: Optional[int] = None,
         headers: Dict[str, Any] = None,
     ) -> None:
         self._uri = uri
         self._error_context = []
 
         if curl_path is None:
-            RuntimeError(
+            raise RuntimeError(
                 "cURL is a required dependency for streaming downloads"
                 " and could not be found."
             )
 
         # NOTE: `256mb` buffer on the python IO object.
         cmd = [
             curl_path,
```

### Comparing `tensorizer-1.1.0/tensorizer/tensors.proto` & `tensorizer-2.0.0/tensorizer/tensors.proto`

 * *Files identical despite different names*

### Comparing `tensorizer-1.1.0/tensorizer/tensors_pb2.py` & `tensorizer-2.0.0/tensorizer/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorizer-1.1.0/tensorizer/utils.py` & `tensorizer-2.0.0/tensorizer/utils.py`

 * *Files identical despite different names*

### Comparing `tensorizer-1.1.0/tensorizer.egg-info/PKG-INFO` & `tensorizer-2.0.0/tensorizer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorizer
-Version: 1.1.0
+Version: 2.0.0
 Summary: A tool for fast PyTorch module, model, and tensor serialization + deserialization.
 Author: CoreWeave
 License: MIT License
 Project-URL: Homepage, https://github.com/coreweave/tensorizer
 Keywords: tensorizer,machine learning,serialization,tensor,pytorch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -367,14 +367,71 @@
 Keep in mind that `load_state_dict` is not a fast operation, and will
 likely be much slower than `load_into_module`.
 
 The `state_dict` can also be used to initialize a HuggingFace Transformers
 AutoModel. But HuggingFace Transformers performs three or more copies of
 the data, so memory use will explode.
 
+### `bfloat16` Support
+
+Tensorizer supports models using the `bfloat16` data type. However, tensorizer
+uses numpy to save the tensors as binary and numpy doesn't support `bfloat16`.
+This means that special conversions need to be applied.
+
+To be saved, the torch tensor is cast to `int16` before being converted to
+numpy, which doesn't change any of the underlying data. When serialized, the
+original `bfloat16` datatype string is also saved so that it will be cast back
+to `bfloat16` during the deserialization process.
+
+The `complex32` datatype is supported in a similar way, by casting to `int32`.
+The quantized datatypes (`qint8`, `qint32`, etc.) are not currently supported
+by tensorizer as they would require supplemental quantization parameters to be
+deserialized correctly.
+
+**NOTE:** The exact choice of intermediate types as `int16` and `int32` is
+considered an implementation detail, and is subject to change,
+so they should not be relied upon.
+
+**NOTE2:** This does not interfere with storing actual `int` datatypes
+used in tensors in tensorized files.
+
+### Numpy Support
+
+Tensorizer can be used with `numpy` directly to read and write
+`numpy.ndarray`s.
+
+The serializer's `write_tensor` function handles supplying both
+`torch.Tensor`s and `numpy.ndarray`s.
+
+The deserializer has a separate function `read_numpy_arrays` that will return
+the data as `numpy.ndarray`s.
+
+As explained above in [bfloat16 support](#bfloat16-support), tensorizer uses
+special conversions to write "opaque" datatypes, those not supported by numpy.
+Therefore, special considerations need to be taken when loading such data as
+`numpy.ndarray`s.
+
+By default, the `TensorDeserializer.read_numpy_arrays` function sets its
+`allow_raw_data` parameter to `False`. This means that if a file contains
+opaque datatypes, a `ValueError` will be raised during deserialization.
+
+If you want to return the raw data regardless, set `allow_raw_data` to `True`.
+Otherwise, the file may be read with `TensorDeserializer.read_tensors`
+instead, which yields `torch.Tensor` objects of the correct datatype.
+
+A fifth and sixth variable are also returned by the `read_numpy_arrays`
+generator. The fifth is a `bool` that indicates whether the returned array
+has an opaque datatype and requires special handling (only legal when
+`allow_raw_data=True`). The sixth is a string describing the true, non-numpy
+datatype that the raw data should be interpreted as in such cases.
+For all other datatypes that require no special handling, these are returned as
+`False` and `None`, respectively.
+The exact numpy datatypes used by the returned opaque `numpy.ndarray` objects
+is not guaranteed, and should not be relied upon.
+
 ## Running Tests
 `tensorizer` uses `unittest` for testing.
 The tests have their own set of dependencies, which can be installed with
 `pip install -r tests/requirements.txt`.
 
 Some tests require a GPU, and will be skipped if no GPU is available.
 To run the tests, run the following in the root of the repository:
```

### Comparing `tensorizer-1.1.0/tensorizer.egg-info/SOURCES.txt` & `tensorizer-2.0.0/tensorizer.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CMakeLists.txt
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 proto/requirements.txt
 proto/tensors.proto
+tensorizer/_NumpyTensor.py
 tensorizer/__init__.py
 tensorizer/_wide_pipes.py
 tensorizer/protobuf.py
 tensorizer/serialization.py
 tensorizer/stream_io.py
 tensorizer/tensors.proto
 tensorizer/tensors_pb2.py
@@ -22,11 +23,9 @@
 tensors/__init__.py
 tensors/go.mod
 tensors/go.sum
 tensors/tensors.pb.go
 tensors/tensors_pb.d.ts
 tensors/tensors_pb.js
 tensors/tensors_pb2.py
-tensors/__pycache__/__init__.cpython-310.pyc
-tensors/__pycache__/tensors_pb2.cpython-310.pyc
 tests/test_serialization.py
 tests/test_stream_io.py
```

### Comparing `tensorizer-1.1.0/tensors/LICENSE` & `tensorizer-2.0.0/tensors/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorizer-1.1.0/tensors/go.sum` & `tensorizer-2.0.0/tensors/go.sum`

 * *Files identical despite different names*

### Comparing `tensorizer-1.1.0/tensors/tensors.pb.go` & `tensorizer-2.0.0/tensors/tensors.pb.go`

 * *Files identical despite different names*

### Comparing `tensorizer-1.1.0/tensors/tensors_pb.d.ts` & `tensorizer-2.0.0/tensors/tensors_pb.d.ts`

 * *Files identical despite different names*

### Comparing `tensorizer-1.1.0/tensors/tensors_pb.js` & `tensorizer-2.0.0/tensors/tensors_pb.js`

 * *Files identical despite different names*

### Comparing `tensorizer-1.1.0/tensors/tensors_pb2.py` & `tensorizer-2.0.0/tensors/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorizer-1.1.0/tests/test_serialization.py` & `tensorizer-2.0.0/tests/test_serialization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import contextlib
 import gc
 import os
 import re
 import tempfile
 import unittest
 from typing import Tuple
+from unittest.mock import patch
 
 import torch
 
 os.environ["TOKENIZERS_PARALLELISM"] = (
     "false"  # avoids excessive warnings about forking after using a tokenizer
 )
 
 from transformers import AutoConfig, AutoModelForCausalLM, AutoTokenizer
 
-from tensorizer import TensorDeserializer, TensorSerializer, utils
+from tensorizer import TensorDeserializer, TensorSerializer, stream_io, utils
+from tensorizer.serialization import TensorType
 
 model_name = "EleutherAI/gpt-neo-125M"
 num_hellos = 400
 is_cuda_available = torch.cuda.is_available()
 default_device = "cuda" if is_cuda_available else "cpu"
 
 
@@ -111,14 +113,37 @@
                         deserialized = TensorDeserializer(in_file, device="cpu")
                         check_deserialized(deserialized, model_name)
                         deserialized.close()
                         del deserialized
                 finally:
                     os.unlink(serialized_model)
 
+    def test_bfloat16(self):
+        shape = (50, 50)
+        tensor = torch.normal(0, 0.5, shape, dtype=torch.bfloat16)
+        tensorized_file = tempfile.NamedTemporaryFile("wb+", delete=False)
+
+        try:
+            serializer = TensorSerializer(tensorized_file)
+            serializer.write_tensor(0, "test_tensor", TensorType.PARAM, tensor)
+            serializer.close()
+
+            with open(tensorized_file.name, "rb") as in_file:
+                deserializer = TensorDeserializer(
+                    in_file, device="cpu", lazy_load=True
+                )
+                deserialized_tensor = [
+                    t for t in deserializer.read_tensors(num_tensors=1)
+                ][0][-1]
+                deserializer.close()
+        finally:
+            os.unlink(tensorized_file.name)
+
+        assert torch.equal(tensor, deserialized_tensor)
+
 
 class TestDeserialization(unittest.TestCase):
     _serialized_model_path: str
 
     @classmethod
     def setUpClass(cls):
         serialized_model_path, sd = serialize_model(model_name, "cpu")
@@ -198,33 +223,36 @@
         _ = deserialized[keys[1]]
 
         with self.assertRaises(RuntimeError):
             _ = deserialized[keys[0]]
 
         deserialized.close()
 
+    @patch.object(stream_io, "_s3_default_config_paths", ())
     def test_s3(self):
         deserialized = TensorDeserializer(
             f"s3://tensorized/{model_name}/model.tensors", device=default_device
         )
         check_deserialized(deserialized, model_name)
         check_inference(deserialized, model_name, default_device)
         deserialized.close()
 
+    @patch.object(stream_io, "_s3_default_config_paths", ())
     def test_s3_fp16(self):
         deserialized = TensorDeserializer(
             f"s3://tensorized/{model_name}/fp16/model.tensors",
             device=default_device,
         )
         assert deserialized.total_tensor_bytes > 0
         if is_cuda_available and default_device != "cpu":
             # FP16 tensors don't work correctly on CPU in PyTorch
             check_inference(deserialized, model_name, default_device)
         deserialized.close()
 
+    @patch.object(stream_io, "_s3_default_config_paths", ())
     def test_s3_lazy_load(self):
         deserialized = TensorDeserializer(
             f"s3://tensorized/{model_name}/model.tensors",
             device=default_device,
             lazy_load=True,
         )
         check_deserialized(deserialized, model_name)
```

### Comparing `tensorizer-1.1.0/tests/test_stream_io.py` & `tensorizer-2.0.0/tests/test_stream_io.py`

 * *Files identical despite different names*

