# Comparing `tmp/concept-erasure-0.0.1.tar.gz` & `tmp/concept-erasure-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concept-erasure-0.0.1.tar", last modified: Wed Jun  7 08:07:58 2023, max compression
+gzip compressed data, was "concept-erasure-0.0.2.tar", last modified: Thu Jun  8 01:29:11 2023, max compression
```

## Comparing `concept-erasure-0.0.1.tar` & `concept-erasure-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-06-07 08:07:58.523967 concept-erasure-0.0.1/
--rw-rw-r--   0 nora      (1000) nora      (1000)     1067 2023-05-06 06:37:09.000000 concept-erasure-0.0.1/LICENSE
--rw-rw-r--   0 nora      (1000) nora      (1000)     3451 2023-06-07 08:07:58.523967 concept-erasure-0.0.1/PKG-INFO
--rw-rw-r--   0 nora      (1000) nora      (1000)     3134 2023-06-07 06:34:32.000000 concept-erasure-0.0.1/README.md
-drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-06-07 08:07:58.507967 concept-erasure-0.0.1/concept_erasure/
--rw-rw-r--   0 nora      (1000) nora      (1000)      280 2023-06-06 08:24:40.000000 concept-erasure-0.0.1/concept_erasure/__init__.py
--rw-rw-r--   0 nora      (1000) nora      (1000)     9565 2023-06-06 08:24:40.000000 concept-erasure-0.0.1/concept_erasure/concept_eraser.py
--rw-rw-r--   0 nora      (1000) nora      (1000)     4455 2023-06-07 03:57:21.000000 concept-erasure-0.0.1/concept_erasure/concept_scrubber.py
--rw-rw-r--   0 nora      (1000) nora      (1000)     5134 2023-05-15 22:58:42.000000 concept-erasure-0.0.1/concept_erasure/data.py
-drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-06-07 08:07:58.519967 concept-erasure-0.0.1/concept_erasure/scrubbing/
--rw-rw-r--   0 nora      (1000) nora      (1000)       83 2023-06-07 06:41:41.000000 concept-erasure-0.0.1/concept_erasure/scrubbing/__init__.py
--rw-rw-r--   0 nora      (1000) nora      (1000)     1376 2023-06-07 06:36:03.000000 concept-erasure-0.0.1/concept_erasure/scrubbing/auto.py
--rw-rw-r--   0 nora      (1000) nora      (1000)     7356 2023-06-07 06:38:39.000000 concept-erasure-0.0.1/concept_erasure/scrubbing/llama.py
--rw-rw-r--   0 nora      (1000) nora      (1000)     5239 2023-06-07 06:38:48.000000 concept-erasure-0.0.1/concept_erasure/scrubbing/neox.py
--rw-rw-r--   0 nora      (1000) nora      (1000)     1746 2023-06-06 08:24:40.000000 concept-erasure-0.0.1/concept_erasure/utils.py
-drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-06-07 08:07:58.511967 concept-erasure-0.0.1/concept_erasure.egg-info/
--rw-rw-r--   0 nora      (1000) nora      (1000)     3451 2023-06-07 08:07:58.000000 concept-erasure-0.0.1/concept_erasure.egg-info/PKG-INFO
--rw-rw-r--   0 nora      (1000) nora      (1000)      609 2023-06-07 08:07:58.000000 concept-erasure-0.0.1/concept_erasure.egg-info/SOURCES.txt
--rw-rw-r--   0 nora      (1000) nora      (1000)        1 2023-06-07 08:07:58.000000 concept-erasure-0.0.1/concept_erasure.egg-info/dependency_links.txt
--rw-rw-r--   0 nora      (1000) nora      (1000)       41 2023-06-07 08:07:58.000000 concept-erasure-0.0.1/concept_erasure.egg-info/entry_points.txt
--rw-rw-r--   0 nora      (1000) nora      (1000)       94 2023-06-07 08:07:58.000000 concept-erasure-0.0.1/concept_erasure.egg-info/requires.txt
--rw-rw-r--   0 nora      (1000) nora      (1000)       16 2023-06-07 08:07:58.000000 concept-erasure-0.0.1/concept_erasure.egg-info/top_level.txt
--rw-rw-r--   0 nora      (1000) nora      (1000)     1394 2023-06-07 07:08:05.000000 concept-erasure-0.0.1/pyproject.toml
--rw-rw-r--   0 nora      (1000) nora      (1000)       38 2023-06-07 08:07:58.523967 concept-erasure-0.0.1/setup.cfg
-drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-06-07 08:07:58.523967 concept-erasure-0.0.1/tests/
--rw-rw-r--   0 nora      (1000) nora      (1000)     5432 2023-06-07 06:25:12.000000 concept-erasure-0.0.1/tests/test_concept_eraser.py
--rw-rw-r--   0 nora      (1000) nora      (1000)     1748 2023-06-07 07:53:07.000000 concept-erasure-0.0.1/tests/test_scrubbing.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-06-08 01:29:11.243680 concept-erasure-0.0.2/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1067 2023-05-06 06:37:09.000000 concept-erasure-0.0.2/LICENSE
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3538 2023-06-08 01:29:11.243680 concept-erasure-0.0.2/PKG-INFO
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3221 2023-06-08 01:12:37.000000 concept-erasure-0.0.2/README.md
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-06-08 01:29:11.223680 concept-erasure-0.0.2/concept_erasure/
+-rw-rw-r--   0 nora      (1000) nora      (1000)      316 2023-06-07 20:01:09.000000 concept-erasure-0.0.2/concept_erasure/__init__.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)    10680 2023-06-07 20:04:25.000000 concept-erasure-0.0.2/concept_erasure/concept_eraser.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4019 2023-06-07 20:04:25.000000 concept-erasure-0.0.2/concept_erasure/concept_scrubber.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5134 2023-05-15 22:58:42.000000 concept-erasure-0.0.2/concept_erasure/data.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-06-08 01:29:11.231680 concept-erasure-0.0.2/concept_erasure/scrubbing/
+-rw-rw-r--   0 nora      (1000) nora      (1000)       83 2023-06-07 06:41:41.000000 concept-erasure-0.0.2/concept_erasure/scrubbing/__init__.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1665 2023-06-07 20:04:25.000000 concept-erasure-0.0.2/concept_erasure/scrubbing/auto.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7308 2023-06-07 19:40:03.000000 concept-erasure-0.0.2/concept_erasure/scrubbing/llama.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5191 2023-06-07 19:39:44.000000 concept-erasure-0.0.2/concept_erasure/scrubbing/neox.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1746 2023-06-06 08:24:40.000000 concept-erasure-0.0.2/concept_erasure/utils.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-06-08 01:29:11.227680 concept-erasure-0.0.2/concept_erasure.egg-info/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3538 2023-06-08 01:29:11.000000 concept-erasure-0.0.2/concept_erasure.egg-info/PKG-INFO
+-rw-rw-r--   0 nora      (1000) nora      (1000)      609 2023-06-08 01:29:11.000000 concept-erasure-0.0.2/concept_erasure.egg-info/SOURCES.txt
+-rw-rw-r--   0 nora      (1000) nora      (1000)        1 2023-06-08 01:29:11.000000 concept-erasure-0.0.2/concept_erasure.egg-info/dependency_links.txt
+-rw-rw-r--   0 nora      (1000) nora      (1000)       41 2023-06-08 01:29:11.000000 concept-erasure-0.0.2/concept_erasure.egg-info/entry_points.txt
+-rw-rw-r--   0 nora      (1000) nora      (1000)       87 2023-06-08 01:29:11.000000 concept-erasure-0.0.2/concept_erasure.egg-info/requires.txt
+-rw-rw-r--   0 nora      (1000) nora      (1000)       16 2023-06-08 01:29:11.000000 concept-erasure-0.0.2/concept_erasure.egg-info/top_level.txt
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1312 2023-06-07 19:52:23.000000 concept-erasure-0.0.2/pyproject.toml
+-rw-rw-r--   0 nora      (1000) nora      (1000)       38 2023-06-08 01:29:11.243680 concept-erasure-0.0.2/setup.cfg
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-06-08 01:29:11.239680 concept-erasure-0.0.2/tests/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5417 2023-06-07 19:38:40.000000 concept-erasure-0.0.2/tests/test_concept_eraser.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1748 2023-06-07 07:53:07.000000 concept-erasure-0.0.2/tests/test_scrubbing.py
```

### Comparing `concept-erasure-0.0.1/LICENSE` & `concept-erasure-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `concept-erasure-0.0.1/PKG-INFO` & `concept-erasure-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: concept-erasure
-Version: 0.0.1
+Version: 0.0.2
 Summary: Erasing concepts from neural representations with provable guarantees
 License: MIT License
 Keywords: fairness,interpretability,explainable-ai
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Least-Squares Concept Erasure (LEACE)
 Concept erasure aims to remove specified features from a representation. It can be used to improve fairness (e.g. preventing a classifier from using gender or race) and interpretability (e.g. removing a concept to observe changes in model behavior). This is the repo for **LEAst-squares Concept Erasure (LEACE)**, a closed-form method which provably prevents all linear classifiers from detecting a concept while inflicting the least possible damage to the representation. You can check out the paper [here](https://arxiv.org/abs/2306.03819).
 
+# Installation
+
+```bash
+pip install concept-erasure
+```
+
 # Usage
 
 `ConceptEraser` is the central class in this repo. It keeps track of the covariance and cross-covariance statistics needed to erase a concept, and lazily computes the LEACE parameters when needed.
 
 ## Batch usage
 
 In most cases, you probably have a batch of feature vectors `X` and concept labels `Z` and want to erase the concept from `X`. The easiest way to do this is using `ConceptEraser.fit()` followed by `ConceptEraser.forward()`:
@@ -79,12 +85,12 @@
 
 # Erase the concept from the data
 x_ = eraser(X_t[0])
 ```
 
 # Paper replication
 
-Scripts used to generate the part-of-speech tags for the concept scrubbing experiments can be found in the `experiments` folder. We plan to upload the tagged datasets to the HuggingFace Hub shortly.
+Scripts used to generate the part-of-speech tags for the concept scrubbing experiments can be found in [this repo](https://github.com/EleutherAI/tagged-pile). We plan to upload the tagged datasets to the HuggingFace Hub shortly.
 
 ## Concept scrubbing
 
 The concept scrubbing code is a bit messy right now, and will probably be refactored soon. We found it necessary to write bespoke implementations for different HuggingFace model families. So far we've implemented LLaMA and GPT-NeoX. These can be found in the `concept_erasure.scrubbing` submodule.
```

### Comparing `concept-erasure-0.0.1/README.md` & `concept-erasure-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # Least-Squares Concept Erasure (LEACE)
 Concept erasure aims to remove specified features from a representation. It can be used to improve fairness (e.g. preventing a classifier from using gender or race) and interpretability (e.g. removing a concept to observe changes in model behavior). This is the repo for **LEAst-squares Concept Erasure (LEACE)**, a closed-form method which provably prevents all linear classifiers from detecting a concept while inflicting the least possible damage to the representation. You can check out the paper [here](https://arxiv.org/abs/2306.03819).
 
+# Installation
+
+```bash
+pip install concept-erasure
+```
+
 # Usage
 
 `ConceptEraser` is the central class in this repo. It keeps track of the covariance and cross-covariance statistics needed to erase a concept, and lazily computes the LEACE parameters when needed.
 
 ## Batch usage
 
 In most cases, you probably have a batch of feature vectors `X` and concept labels `Z` and want to erase the concept from `X`. The easiest way to do this is using `ConceptEraser.fit()` followed by `ConceptEraser.forward()`:
@@ -68,12 +74,12 @@
 
 # Erase the concept from the data
 x_ = eraser(X_t[0])
 ```
 
 # Paper replication
 
-Scripts used to generate the part-of-speech tags for the concept scrubbing experiments can be found in the `experiments` folder. We plan to upload the tagged datasets to the HuggingFace Hub shortly.
+Scripts used to generate the part-of-speech tags for the concept scrubbing experiments can be found in [this repo](https://github.com/EleutherAI/tagged-pile). We plan to upload the tagged datasets to the HuggingFace Hub shortly.
 
 ## Concept scrubbing
 
 The concept scrubbing code is a bit messy right now, and will probably be refactored soon. We found it necessary to write bespoke implementations for different HuggingFace model families. So far we've implemented LLaMA and GPT-NeoX. These can be found in the `concept_erasure.scrubbing` submodule.
```

### Comparing `concept-erasure-0.0.1/concept_erasure/concept_eraser.py` & `concept-erasure-0.0.2/concept_erasure/concept_eraser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 from typing import Literal
 
 import torch
 from torch import Tensor, nn
 
+ErasureMethod = Literal["leace", "orth", "relaxed"]
+
 
 class ConceptEraser(nn.Module):
-    """Minimally edit features to make specified concepts linearly undetectable."""
+    """Minimally edit features to make specified concepts linearly undetectable.
+
+    There are three erasure methods currently supported:
+    - `"leace"`: Least-squares Concept Erasure from https://arxiv.org/abs/2306.03819.
+    - `"orth"`: Orthogonal projection onto colsp(Sigma_xz)^perp.
+    - `"relaxed"`: Applies a PSD map with spectral norm <= 1 that ensures the resulting
+    cross-covariance matrix Cov(PX, Z) has spectral norm no greater than `svd_tol`.
+    Importantly, this method **does not** ensure linear guardedness, but may be useful
+    for concept scrubbing purposes. It has the benefit of being less sensitive to noise
+    and the choice of `svd_tol` than other methods.
+    """
 
     mean_x: Tensor
     """Running mean of X."""
 
     mean_z: Tensor
     """Running mean of Z."""
 
@@ -24,56 +36,63 @@
 
     n_z: Tensor
     """Number of Z samples seen so far."""
 
     _P: Tensor | None
 
     @classmethod
-    def fit(cls, x: Tensor, y: Tensor, **kwargs) -> "ConceptEraser":
+    def fit(cls, x: Tensor, z: Tensor, **kwargs) -> "ConceptEraser":
         """Convenience method to fit a ConceptEraser on data and return it."""
         n, d = x.shape
-        _, k = y.reshape(n, -1).shape
+        _, k = z.reshape(n, -1).shape
 
-        return cls(d, k, device=x.device, dtype=x.dtype, **kwargs).update(x, y)
+        return cls(d, k, device=x.device, dtype=x.dtype, **kwargs).update(x, z)
 
     def __init__(
         self,
         x_dim: int,
         z_dim: int,
-        proj_type: Literal["leace", "orth", "relaxed"] = "leace",
+        method: ErasureMethod = "leace",
         *,
         affine: bool = True,
+        constrain_cov_trace: bool = True,
         device: str | torch.device | None = None,
         dtype: torch.dtype | None = None,
         svd_tol: float = 0.01,
     ):
         """Initialize a ConceptEraser.
 
         Args:
             x_dim: Dimensionality of the input.
             z_dim: Dimensionality of the labels.
-            proj_type: Type of projection matrix to use.
+            method: Type of projection matrix to use.
             affine: Whether to use a bias term to ensure the unconditional mean of the
                 features remains the same after erasure.
+            constrain_cov_trace: Whether to constrain the trace of the covariance of X
+                after erasure to be no greater than before erasure. This is especially
+                useful when injecting the scrubbed features back into a model. Without
+                this constraint, the norm of the model's hidden states may diverge in
+                some cases.
             device: Device to put the statistics on.
             dtype: Data type to use for the statistics.
             svd_tol: Singular values under this threshold are truncated, both during
                 the phase where we do SVD on the cross-covariance matrix, and at the
                 phase where we compute the pseudoinverse of the projected covariance
                 matrix. Higher values are more numerically stable and result in less
                 damage to the representation, but may leave trace correlations intact.
         """
         super().__init__()
 
         self.z_dim = z_dim
         self.x_dim = x_dim
 
         self.affine = affine
+        self.constrain_cov_trace = constrain_cov_trace
         self.proj_rank = z_dim
-        self.proj_type = proj_type
+        self.method = method
         self.z_dim = z_dim
 
         assert svd_tol > 0.0, "`svd_tol` must be positive for numerical stability."
         self.svd_tol = svd_tol
 
         self.register_buffer("mean_x", torch.zeros(x_dim, device=device, dtype=dtype))
         self.register_buffer("mean_z", self.mean_x.new_zeros(z_dim))
@@ -81,20 +100,20 @@
             "sigma_xz_M2",
             self.mean_x.new_zeros(x_dim, z_dim),
         )
         self.register_buffer("n_x", torch.tensor(0, device=device, dtype=dtype))
         self.register_buffer("n_z", torch.tensor(0, device=device, dtype=dtype))
         self.register_buffer("_P", None)
 
-        if self.proj_type == "leace":
+        if self.method == "leace":
             M2 = self.mean_x.new_zeros(x_dim, x_dim)
-        elif self.proj_type in ("orth", "relaxed"):
+        elif self.method in ("orth", "relaxed"):
             M2 = None
         else:
-            raise ValueError(f"Unknown projection type {self.proj_type}")
+            raise ValueError(f"Unknown projection type {self.method}")
 
         self.register_buffer("x_M2", M2)
 
     def forward(self, x: Tensor) -> Tensor:
         """Minimally edit `x` to remove correlations with the target concepts.
 
         Args:
@@ -135,15 +154,15 @@
 
         # Welford's online algorithm
         delta_x = x - self.mean_x
         self.mean_x += delta_x.sum(dim=0) / self.n_x
         delta_x2 = x - self.mean_x
 
         # Update the covariance matrix of X if needed (for LEACE)
-        if self.proj_type == "leace":
+        if self.method == "leace":
             assert self.x_M2 is not None
             self.x_M2.addmm_(delta_x.mT, delta_x2)
 
         # Invalidate the cached projection matrix
         self._P = None
 
         # We do have labels, so we can update the Z statistics
@@ -168,15 +187,15 @@
         """Projection matrix for removing the subspace."""
         if self._P is not None:
             return self._P
 
         eye = torch.eye(self.x_dim, device=self.mean_x.device, dtype=self.mean_x.dtype)
         u, s, _ = torch.linalg.svd(self.sigma_xz, full_matrices=False)
 
-        if self.proj_type == "relaxed":
+        if self.method == "relaxed":
             # Treat `svd_tol` as a constraint on the spectral norm of sigma_xz after
             # erasure. In this case Q is not actually a projection matrix, it's a
             # PSD non-expansive map (spectral norm <= 1).
             Q = eye - u * torch.clamp(1 - self.svd_tol / s, 0, 1) @ u.T
         else:
             # Throw away singular values that are too small
             mask = s > self.svd_tol
@@ -185,15 +204,15 @@
 
             u = u[:, mask]
             Q = eye - u @ u.T if mask.any() else eye
 
             # Save this for debugging
             self.proj_rank = mask.sum().item()
 
-        if self.proj_type != "leace":
+        if self.method != "leace":
             self._P = Q
             return self._P
 
         self._P = self.proj_for_subspace(u)
         return self._P
 
     def proj_for_subspace(self, u: Tensor) -> Tensor:
@@ -221,15 +240,15 @@
         # Prevent the covariance trace from increasing
         old_trace = torch.trace(sigma)
         new_trace = torch.trace(P @ sigma @ P.mT)
 
         # If applying the projection matrix increases the variance, this might
         # cause instability, especially when erasure is applied multiple times.
         # We regularize toward the orthogonal projection matrix to avoid this.
-        if new_trace > old_trace:
+        if self.constrain_cov_trace and new_trace > old_trace:
             # Set up the variables for the quadratic equation
             x = new_trace
             y = 2 * torch.trace(P @ sigma @ Q.mT)
             z = torch.trace(Q @ sigma @ Q.mT)
             w = old_trace
 
             # Solve for the mixture of P and Q that makes the trace equal to the
```

### Comparing `concept-erasure-0.0.1/concept_erasure/concept_scrubber.py` & `concept-erasure-0.0.2/concept_erasure/concept_scrubber.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 from contextlib import contextmanager
 from functools import partial
-from typing import Callable, Literal
+from typing import Callable
 
 import torch
 from torch import Tensor, nn
 from transformers import PreTrainedModel
 
-from .concept_eraser import ConceptEraser
+from .concept_eraser import ConceptEraser, ErasureMethod
 from .utils import assert_type, is_norm_layer, mangle_module_path
 
 
 class ConceptScrubber(nn.Module):
+    """Wrapper for a dictionary mapping module paths to `ConceptEraser` objects."""
+
     @classmethod
     def from_model(
         cls,
         model: PreTrainedModel,
         z_dim: int = 1,
         affine: bool = True,
         module_suffix: str = "",
-        proj_type: Literal["leace", "orth"] = "leace",
+        method: ErasureMethod = "leace",
         pre_hook: bool = False,
     ):
+        """Create a scrubber with a `ConceptEraser` for each norm layer in `model`."""
         d_model = model.config.hidden_size
 
         scrubber = cls(pre_hook=pre_hook)
         scrubber.erasers.update(
             {
                 mangle_module_path(name): ConceptEraser(
                     d_model,
                     z_dim,
                     affine=affine,
                     device=model.device,
-                    proj_type=proj_type,
+                    method=method,
                 )
                 # Note that we are unwrapping the base model here
                 for name, mod in model.base_model.named_modules()
                 if is_norm_layer(mod) and name.endswith(module_suffix)
             }
         )
         return scrubber
@@ -43,37 +46,19 @@
     def __init__(self, pre_hook: bool = False):
         super().__init__()
 
         self.erasers = nn.ModuleDict()
         self.pre_hook = pre_hook
 
     @contextmanager
-    def record(
-        self,
-        model: PreTrainedModel,
-        label: Tensor | None = None,
-    ):
-        """Update erasers with the activations of the model, using the given label.
-
-        This method adds a forward pre-hook to each layer of the model, which
-        records its input activations. These are used to update the erasers.
-        """
-
-        def record_hook(eraser: ConceptEraser, x: Tensor):
-            eraser.update(x, label)
-
-        with self.apply_hook(model, record_hook):
-            yield self
-
-    @contextmanager
-    def scrub(self, model, dry_run: bool = False):
+    def scrub(self, model):
         """Add hooks to the model which apply the erasers during a forward pass."""
 
         def scrub_hook(eraser: ConceptEraser, x: Tensor):
-            return eraser(x).type_as(x) if not dry_run else x
+            return eraser(x).type_as(x)
 
         with self.apply_hook(model, scrub_hook):
             yield self
 
     @contextmanager
     def random_scrub(self, model):
         eraser = assert_type(ConceptEraser, next(iter(self.erasers.values())))
```

### Comparing `concept-erasure-0.0.1/concept_erasure/data.py` & `concept-erasure-0.0.2/concept_erasure/data.py`

 * *Files identical despite different names*

### Comparing `concept-erasure-0.0.1/concept_erasure/scrubbing/auto.py` & `concept-erasure-0.0.2/concept_erasure/scrubbing/auto.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-from typing import Literal
+from warnings import warn
 
+import torch.nn.functional as F
 from datasets import Dataset
 from transformers import GPTNeoXForCausalLM, LlamaForCausalLM, PreTrainedModel
 
+from ..concept_eraser import ErasureMethod
 from ..concept_scrubber import ConceptScrubber
 from .llama import patch_attention_llama_, scrub_llama
 from .neox import patch_attention_neox_, scrub_neox
 
 
 def patch_attention_(model: PreTrainedModel):
     """Patch the attention layers of a model to use fast attention kernels."""
     ty = model.config.model_type
+    if not hasattr(F, "scaled_dot_product_attention"):
+        warn(
+            "Fast, memory-efficient attention requires PyTorch >= 2.0.0. "
+            "For best performance, please upgrade your version of PyTorch."
+        )
+        return
 
     if ty == "gpt_neox":
         patch_attention_neox_(model)
     elif ty == "llama":
         patch_attention_llama_(model)
     else:
         raise NotImplementedError(f"Unsupported model type: {type(model)}")
@@ -22,19 +30,19 @@
 
 def scrub(
     model: PreTrainedModel,
     train: Dataset,
     z_column: str | None,
     affine: bool = True,
     batch_size: int = 1,
-    proj_type: Literal["leace", "loracs", "orth"] = "leace",
+    method: ErasureMethod = "leace",
     sublayers: bool = True,
 ) -> tuple[ConceptScrubber | None, float]:
     """Scrub a model to remove the fast attention kernels."""
     if isinstance(model, GPTNeoXForCausalLM):
-        return scrub_neox(model, train, z_column, batch_size, proj_type, affine)
+        return scrub_neox(model, train, z_column, batch_size, method, affine)
     elif isinstance(model, LlamaForCausalLM):
         return scrub_llama(
-            model, train, z_column, batch_size, proj_type, sublayers, affine
+            model, train, z_column, batch_size, method, sublayers, affine
         )
     else:
         raise NotImplementedError(f"Unsupported model type: {type(model).__name__}")
```

### Comparing `concept-erasure-0.0.1/concept_erasure/scrubbing/llama.py` & `concept-erasure-0.0.2/concept_erasure/scrubbing/llama.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from types import MethodType
-from typing import Literal
 
 import torch
 import torch.nn.functional as F
 from datasets import Dataset
 from tqdm.auto import tqdm
 from transformers import (
     LlamaForCausalLM,
@@ -11,15 +10,15 @@
 )
 from transformers.models.llama.modeling_llama import (
     LlamaAttention,
     LlamaDecoderLayer,
     apply_rotary_pos_emb,
 )
 
-from concept_erasure import ConceptEraser, ConceptScrubber
+from concept_erasure import ConceptEraser, ConceptScrubber, ErasureMethod
 from concept_erasure.utils import assert_type
 
 
 def _fast_attn(
     self,
     hidden_states: torch.Tensor,
     attention_mask: torch.Tensor | None = None,
@@ -79,15 +78,15 @@
 
 @torch.no_grad()
 def scrub_llama(
     model: LlamaForCausalLM,
     train: Dataset,
     z_column: str | None,
     batch_size: int = 1,
-    proj_type: Literal["leace", "loracs", "orth"] = "leace",
+    method: ErasureMethod = "leace",
     sublayers: bool = True,
     affine: bool = True,
 ) -> tuple[ConceptScrubber | None, float]:
     base = assert_type(LlamaModel, model.base_model)
     d = assert_type(int, base.config.hidden_size)
 
     if z_column is None:
@@ -120,15 +119,15 @@
     # Enumerate the layers
     for j, layer in enumerate(tqdm(base.layers, unit="layer")):
         assert isinstance(layer, LlamaDecoderLayer)
 
         attn_eraser = None
         if scrubber is not None:
             attn_eraser = ConceptEraser(
-                d, k, affine=affine, device=model.device, proj_type=proj_type
+                d, k, affine=affine, device=model.device, method=method
             )
             scrubber.erasers[f"layers-{j}-input_layernorm"] = attn_eraser
 
             # Fit the next eraser on the previous hidden states
             for x, z in tqdm(zip(xs, zs), desc="Fitting (attn)", total=N):
                 assert scrubber is not None
 
@@ -163,15 +162,15 @@
         # Skip the part where we scrub the MLP if we're not doing that
         if not sublayers:
             continue
 
         mlp_eraser = None
         if scrubber is not None:
             mlp_eraser = ConceptEraser(
-                d, k, affine=affine, device=model.device, proj_type=proj_type
+                d, k, affine=affine, device=model.device, method=method
             )
             scrubber.erasers[f"layers-{j}-post_attention_layernorm"] = mlp_eraser
 
             # Fit the next eraser on the previous hidden states
             for x, z in tqdm(zip(xs, zs), desc="Fitting (MLP)", total=N):
                 assert scrubber is not None
```

### Comparing `concept-erasure-0.0.1/concept_erasure/scrubbing/neox.py` & `concept-erasure-0.0.2/concept_erasure/scrubbing/neox.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from types import MethodType
-from typing import Literal
 
 import torch
 import torch.nn.functional as F
 from datasets import Dataset
 from tqdm.auto import tqdm
 from transformers import (
     GPTNeoXForCausalLM,
     GPTNeoXLayer,
     GPTNeoXModel,
 )
 from transformers.models.gpt_neox.modeling_gpt_neox import GPTNeoXAttention
 
-from concept_erasure import ConceptEraser, ConceptScrubber
+from concept_erasure import ConceptEraser, ConceptScrubber, ErasureMethod
 from concept_erasure.utils import assert_type
 
 
 def patch_attention_neox_(model: torch.nn.Module):
     """Patch the attention layers of a GPTNeoX model to use fast attention kernels."""
 
     def fast_attn(self, q, k, v, attention_mask=None, head_mask=None):
@@ -34,15 +33,15 @@
 
 @torch.no_grad()
 def scrub_neox(
     model: GPTNeoXForCausalLM,
     train: Dataset,
     z_column: str | None,
     batch_size: int = 32,
-    proj_type: Literal["leace", "loracs", "orth"] = "leace",
+    method: ErasureMethod = "leace",
     affine: bool = True,
 ) -> tuple[ConceptScrubber | None, float]:
     base = assert_type(GPTNeoXModel, model.base_model)
     d = assert_type(int, base.config.hidden_size)
 
     # Put model in eval mode
     model.eval()
@@ -78,20 +77,20 @@
     for j, layer in enumerate(tqdm(base.layers, unit="layer")):
         assert isinstance(layer, GPTNeoXLayer)
         assert layer.use_parallel_residual, "Only parallel residual is supported"
 
         attn_eraser, mlp_eraser = None, None
         if scrubber is not None:
             attn_eraser = ConceptEraser(
-                d, k, affine=affine, device=model.device, proj_type=proj_type
+                d, k, affine=affine, device=model.device, method=method
             )
             scrubber.erasers[f"layers-{j}-input_layernorm"] = attn_eraser
 
             mlp_eraser = ConceptEraser(
-                d, k, affine=affine, device=model.device, proj_type=proj_type
+                d, k, affine=affine, device=model.device, method=method
             )
             scrubber.erasers[f"layers-{j}-post_attention_layernorm"] = mlp_eraser
 
             # Fit the next eraser on the previous hidden states
             for i, (x, z) in tqdm(enumerate(zip(xs, zs)), desc="Fitting", total=N):
                 x = x.to(model.device)
```

### Comparing `concept-erasure-0.0.1/concept_erasure/utils.py` & `concept-erasure-0.0.2/concept_erasure/utils.py`

 * *Files identical despite different names*

### Comparing `concept-erasure-0.0.1/concept_erasure.egg-info/PKG-INFO` & `concept-erasure-0.0.2/concept_erasure.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: concept-erasure
-Version: 0.0.1
+Version: 0.0.2
 Summary: Erasing concepts from neural representations with provable guarantees
 License: MIT License
 Keywords: fairness,interpretability,explainable-ai
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Least-Squares Concept Erasure (LEACE)
 Concept erasure aims to remove specified features from a representation. It can be used to improve fairness (e.g. preventing a classifier from using gender or race) and interpretability (e.g. removing a concept to observe changes in model behavior). This is the repo for **LEAst-squares Concept Erasure (LEACE)**, a closed-form method which provably prevents all linear classifiers from detecting a concept while inflicting the least possible damage to the representation. You can check out the paper [here](https://arxiv.org/abs/2306.03819).
 
+# Installation
+
+```bash
+pip install concept-erasure
+```
+
 # Usage
 
 `ConceptEraser` is the central class in this repo. It keeps track of the covariance and cross-covariance statistics needed to erase a concept, and lazily computes the LEACE parameters when needed.
 
 ## Batch usage
 
 In most cases, you probably have a batch of feature vectors `X` and concept labels `Z` and want to erase the concept from `X`. The easiest way to do this is using `ConceptEraser.fit()` followed by `ConceptEraser.forward()`:
@@ -79,12 +85,12 @@
 
 # Erase the concept from the data
 x_ = eraser(X_t[0])
 ```
 
 # Paper replication
 
-Scripts used to generate the part-of-speech tags for the concept scrubbing experiments can be found in the `experiments` folder. We plan to upload the tagged datasets to the HuggingFace Hub shortly.
+Scripts used to generate the part-of-speech tags for the concept scrubbing experiments can be found in [this repo](https://github.com/EleutherAI/tagged-pile). We plan to upload the tagged datasets to the HuggingFace Hub shortly.
 
 ## Concept scrubbing
 
 The concept scrubbing code is a bit messy right now, and will probably be refactored soon. We found it necessary to write bespoke implementations for different HuggingFace model families. So far we've implemented LLaMA and GPT-NeoX. These can be found in the `concept_erasure.scrubbing` submodule.
```

### Comparing `concept-erasure-0.0.1/concept_erasure.egg-info/SOURCES.txt` & `concept-erasure-0.0.2/concept_erasure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `concept-erasure-0.0.1/pyproject.toml` & `concept-erasure-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 description = "Erasing concepts from neural representations with provable guarantees"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["fairness", "interpretability", "explainable-ai"]
 license = {text = "MIT License"}
 dependencies = [
     "datasets",
-    # We use F.scaled_dot_product_attention, which was introduced in 2.0.0
-    "torch>=2.0.0",
+    "torch",
     # 4.0 introduced the breaking change of using return_dict=True by default
     "transformers>=4.0.0",
 ]
-version = "0.0.1"
+version = "0.0.2"
 
 [project.optional-dependencies]
 dev = [
     "numpy",
     "pre-commit",
     "pytest",
     "pyright",
```

### Comparing `concept-erasure-0.0.1/tests/test_concept_eraser.py` & `concept-erasure-0.0.2/tests/test_concept_eraser.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,28 +71,28 @@
         Y_1h = torch.nn.functional.one_hot(Y_t, num_classes)
     else:
         Y_1h = Y_t
 
     eps = 2e-9
     mse_dict: dict[tuple[bool, str], float] = {}
 
-    for affine, proj_type in product([False, True], ["leace", "orth"]):
-        eraser = ConceptEraser.fit(X_t, Y_1h, affine=affine, proj_type=proj_type)
+    for affine, method in product([False, True], ["leace", "orth"]):
+        eraser = ConceptEraser.fit(X_t, Y_1h, affine=affine, method=method)
         X_ = eraser(X_t)
 
         # Check idempotence
         torch.testing.assert_close(eraser(X_), X_)
 
         # Check that the rank of the update <= num_classes
         rank = torch.linalg.svdvals(X_t - X_).gt(eps).sum()
         assert rank <= num_classes
 
         # Record the mean squared error for comparison
         X_np = X_.numpy()
-        mse_dict[(affine, proj_type)] = np.square(X_np - X).mean()
+        mse_dict[(affine, method)] = np.square(X_np - X).mean()
 
         # Check that the unconditional mean is unchanged
         if affine:
             torch.testing.assert_close(X_t.mean(dim=0), X_.mean(dim=0))
 
         # Compute class means and check that they are equal after the projection
         class_means_ = torch.stack(
@@ -137,10 +137,10 @@
         ).fit(X_np, Y)
         assert abs(null_svm.coef_).max() < eps
 
         # But it should learn something before the projection
         real_svm = LinearSVC(dual=False, intercept_scaling=1e6, tol=eps).fit(X, Y)
         assert abs(real_svm.coef_).max() > 0.1
 
-    # Check that using proj_type="leace" strictly better than "orth"
+    # Check that using method="leace" strictly better than "orth"
     assert mse_dict[(True, "leace")] < mse_dict[(True, "orth")]
     assert mse_dict[(False, "leace")] < mse_dict[(False, "orth")]
```

### Comparing `concept-erasure-0.0.1/tests/test_scrubbing.py` & `concept-erasure-0.0.2/tests/test_scrubbing.py`

 * *Files identical despite different names*

