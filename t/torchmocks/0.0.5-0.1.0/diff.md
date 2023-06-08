# Comparing `tmp/torchmocks-0.0.5.tar.gz` & `tmp/torchmocks-0.1.0.tar.gz`

## Comparing `torchmocks-0.0.5.tar` & `torchmocks-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,19 @@
--rw-r--r--   0        0        0   277581 2020-02-02 00:00:00.000000 torchmocks-0.0.5/scratch.ipynb
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 torchmocks-0.0.5/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 torchmocks-0.0.5/.vscode/settings.json
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 torchmocks-0.0.5/tests/conv.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 torchmocks-0.0.5/tests/fx_trace.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 torchmocks-0.0.5/tests/lightning_train.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 torchmocks-0.0.5/tests/mock.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 torchmocks-0.0.5/tests/pooling.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 torchmocks-0.0.5/torchmocks/__init__.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 torchmocks-0.0.5/torchmocks/torchmocks.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 torchmocks-0.0.5/torchmocks/nn/activation.py
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 torchmocks-0.0.5/torchmocks/nn/conv.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 torchmocks-0.0.5/torchmocks/nn/dropout.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 torchmocks-0.0.5/torchmocks/nn/embedding.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 torchmocks-0.0.5/torchmocks/nn/linear.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 torchmocks-0.0.5/torchmocks/nn/normalization.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 torchmocks-0.0.5/torchmocks/nn/pooling.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 torchmocks-0.0.5/LICENSE
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 torchmocks-0.0.5/README.md
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 torchmocks-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 torchmocks-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 torchmocks-0.1.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 torchmocks-0.1.0/tests/conv.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 torchmocks-0.1.0/tests/fx_trace.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 torchmocks-0.1.0/tests/lightning_train.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 torchmocks-0.1.0/tests/mock.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 torchmocks-0.1.0/tests/pooling.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 torchmocks-0.1.0/torchmocks/__init__.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 torchmocks-0.1.0/torchmocks/torchmocks.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 torchmocks-0.1.0/torchmocks/nn/activation.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 torchmocks-0.1.0/torchmocks/nn/conv.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 torchmocks-0.1.0/torchmocks/nn/dropout.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 torchmocks-0.1.0/torchmocks/nn/embedding.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 torchmocks-0.1.0/torchmocks/nn/linear.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 torchmocks-0.1.0/torchmocks/nn/normalization.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 torchmocks-0.1.0/torchmocks/nn/pooling.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 torchmocks-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 torchmocks-0.1.0/README.md
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 torchmocks-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 torchmocks-0.1.0/PKG-INFO
```

### Comparing `torchmocks-0.0.5/.github/workflows/python-package.yml` & `torchmocks-0.1.0/.github/workflows/python-package.yml`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install flake8 pytest torch torchvision pytorch-lightning vit-pytorch
+        python -m pip install flake8 pytest torch torchvision lightning vit-pytorch
         python -m pip install -e .
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
```

### Comparing `torchmocks-0.0.5/tests/conv.py` & `torchmocks-0.1.0/tests/conv.py`

 * *Files identical despite different names*

### Comparing `torchmocks-0.0.5/tests/fx_trace.py` & `torchmocks-0.1.0/tests/fx_trace.py`

 * *Files identical despite different names*

### Comparing `torchmocks-0.0.5/tests/lightning_train.py` & `torchmocks-0.1.0/tests/lightning_train.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pytorch_lightning
+from lightning import pytorch as pytorch_lightning
 import torch
 import torchvision
 from torchmocks import mock
 from torchvision.datasets import FakeData
 from torchvision.models import feature_extraction, resnet152
```

### Comparing `torchmocks-0.0.5/tests/mock.py` & `torchmocks-0.1.0/tests/mock.py`

 * *Files identical despite different names*

### Comparing `torchmocks-0.0.5/tests/pooling.py` & `torchmocks-0.1.0/tests/pooling.py`

 * *Files identical despite different names*

### Comparing `torchmocks-0.0.5/torchmocks/torchmocks.py` & `torchmocks-0.1.0/torchmocks/torchmocks.py`

 * *Files identical despite different names*

### Comparing `torchmocks-0.0.5/torchmocks/nn/activation.py` & `torchmocks-0.1.0/torchmocks/nn/activation.py`

 * *Files identical despite different names*

### Comparing `torchmocks-0.0.5/torchmocks/nn/conv.py` & `torchmocks-0.1.0/torchmocks/nn/conv.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,30 +38,30 @@
                         - 1
                         + stride[i]
                     )
                     // stride[i]
                     for i in range(spacial_dim)
                 ]
                 new_shape = tuple([batch_size, out_channels] + new_spacial_shape)
-            return torch.zeros(new_shape)
+            return torch.zeros(new_shape, device=x.device)
 
         @staticmethod
         def backward(ctx, grad_output):
             x_shape, weight_shape, bias_shape = ctx.saved_tensors
             x_shape = tuple(x_shape.tolist())
             weight_shape = tuple(weight_shape.tolist())
             bias_shape = tuple(bias_shape.tolist()) if bias_shape is not None else None
 
             grad_input = grad_weight = grad_bias = None
             if ctx.needs_input_grad[0]:
-                grad_input = torch.zeros(x_shape)
+                grad_input = torch.zeros(x_shape, device=grad_output.device)
             if ctx.needs_input_grad[1]:
-                grad_weight = torch.zeros(weight_shape)
+                grad_weight = torch.zeros(weight_shape, device=grad_output.device)
             if bias_shape is not None and ctx.needs_input_grad[2]:
-                grad_bias = torch.zeros(bias_shape)
+                grad_bias = torch.zeros(bias_shape, device=grad_output.device)
             return grad_input, grad_weight, grad_bias, None, None, None, None
 
     class MockConvModule:
         def __init__(self, obj):
             super().__init__()
             self.__class__ = type(
                 obj.__class__.__name__, (self.__class__, obj.__class__), {}
```

### Comparing `torchmocks-0.0.5/torchmocks/nn/embedding.py` & `torchmocks-0.1.0/torchmocks/nn/embedding.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,14 @@
         )
         self.__dict__ = obj.__dict__
         self.embedding_dim = obj.embedding_dim
         self.mock_gradient_sink = torch.ones(1, requires_grad=True)
 
     def forward(self, x):
         new_shape = tuple(list(x.shape) + [self.embedding_dim])
-        return self.mock_gradient_sink * torch.zeros(new_shape)
+        return self.mock_gradient_sink * torch.zeros(new_shape, device=x.device)
 
 
 mock_dict = {
     torch.nn.modules.sparse.Embedding: EmbeddingMock,
     torch.nn.modules.sparse.EmbeddingBag: None,
 }
```

### Comparing `torchmocks-0.0.5/torchmocks/nn/linear.py` & `torchmocks-0.1.0/torchmocks/nn/linear.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,31 +8,31 @@
             torch.IntTensor(tuple(x.shape)),
             torch.IntTensor(tuple(weight.shape)),
             torch.IntTensor(tuple(bias.shape)) if bias is not None else None,
         )
         out_features, in_features = weight.shape
         assert x.shape[-1] == in_features
         output_shape = (*x.shape[:-1], out_features)
-        output = torch.zeros(output_shape)
+        output = torch.zeros(output_shape, device=x.device)
         return output
 
     @staticmethod
     def backward(ctx, grad_output):
         x_shape, weight_shape, bias_shape = ctx.saved_tensors
         x_shape = tuple(x_shape.tolist())
         weight_shape = tuple(weight_shape.tolist())
         bias_shape = tuple(bias_shape.tolist()) if bias_shape is not None else None
 
         grad_input = grad_weight = grad_bias = None
         if ctx.needs_input_grad[0]:
-            grad_input = torch.zeros(x_shape)
+            grad_input = torch.zeros(x_shape, device=grad_output.device)
         if ctx.needs_input_grad[1]:
-            grad_weight = torch.zeros(weight_shape)
+            grad_weight = torch.zeros(weight_shape, device=grad_output.device)
         if bias_shape is not None and ctx.needs_input_grad[2]:
-            grad_bias = torch.zeros(bias_shape)
+            grad_bias = torch.zeros(bias_shape, device=grad_output.device)
         return grad_input, grad_weight, grad_bias
 
 
 class LinearModuleMock:
     def __init__(self, obj):
         super().__init__()
         self.__class__ = type(
```

### Comparing `torchmocks-0.0.5/torchmocks/nn/normalization.py` & `torchmocks-0.1.0/torchmocks/nn/normalization.py`

 * *Files identical despite different names*

### Comparing `torchmocks-0.0.5/torchmocks/nn/pooling.py` & `torchmocks-0.1.0/torchmocks/nn/pooling.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
                 - 1
                 + stride[i]
             )
             // stride[i]
             for i in range(spacial_dim)
         ]
         new_shape = tuple([batch_size, out_channels] + new_spacial_shape)
-        return torch.zeros(new_shape)
+        return torch.zeros(new_shape, device=x.device)
 
     @staticmethod
     def backward(ctx, grad_output):
         x_shape = tuple(ctx.saved_tensors[0])
-        return torch.zeros(x_shape), None, None, None, None
+        return torch.zeros(x_shape, device=grad_output.device), None, None, None, None
 
 
 def tupleize(d, dim=2):
     if isinstance(d, int):
         return tuple([d] * dim)
     elif isinstance(d, tuple):
         if len(d) == 1:
```

### Comparing `torchmocks-0.0.5/LICENSE` & `torchmocks-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmocks-0.0.5/README.md` & `torchmocks-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `torchmocks-0.0.5/pyproject.toml` & `torchmocks-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling>=1.10.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "torchmocks"
-version = "0.0.5"
+version = "0.1.0"
 description = "Mocks pytorch modules so that test run faster"
 readme = "README.md"
 requires-python = ">=3.7"
 
 keywords = [
     'deep learning',
     'neural networks',
```

### Comparing `torchmocks-0.0.5/PKG-INFO` & `torchmocks-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchmocks
-Version: 0.0.5
+Version: 0.1.0
 Summary: Mocks pytorch modules so that test run faster
 Project-URL: Homepage, https://github.com/nathanbreitsch/torchmocks
 Author: Nathan Breitsch
 License: MIT
 License-File: LICENSE
 Keywords: deep learning,machine learning,neural networks,scientific computations,torchmocks
 Classifier: Intended Audience :: Science/Research
```

