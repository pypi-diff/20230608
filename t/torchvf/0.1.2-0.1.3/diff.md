# Comparing `tmp/torchvf-0.1.2.tar.gz` & `tmp/torchvf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchvf-0.1.2.tar", max compression
+gzip compressed data, was "torchvf-0.1.3.tar", max compression
```

## Comparing `torchvf-0.1.2.tar` & `torchvf-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    10762 2022-08-28 01:18:25.336023 torchvf-0.1.2/LICENSE
--rw-r--r--   0        0        0     6989 2022-09-05 22:57:48.436642 torchvf-0.1.2/README.md
--rw-r--r--   0        0        0      932 2023-03-30 22:09:36.090039 torchvf-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      604 2022-09-01 22:49:28.718439 torchvf-0.1.2/torchvf/__init__.py
--rw-r--r--   0        0        0      746 2022-09-01 22:44:33.723212 torchvf-0.1.2/torchvf/dataloaders/__init__.py
--rw-r--r--   0        0        0     4387 2022-08-28 19:51:36.958577 torchvf-0.1.2/torchvf/dataloaders/bpcis.py
--rw-r--r--   0        0        0     1301 2022-08-28 19:51:35.302585 torchvf-0.1.2/torchvf/dataloaders/dataloader.py
--rw-r--r--   0        0        0     4188 2022-08-28 19:51:33.734593 torchvf-0.1.2/torchvf/dataloaders/sartorius.py
--rw-r--r--   0        0        0      711 2022-09-01 21:58:08.031975 torchvf-0.1.2/torchvf/losses/__init__.py
--rw-r--r--   0        0        0     2929 2022-08-28 19:50:48.626833 torchvf-0.1.2/torchvf/losses/dice.py
--rw-r--r--   0        0        0     3138 2022-09-01 21:59:00.796330 torchvf-0.1.2/torchvf/losses/ivp_loss.py
--rw-r--r--   0        0        0     2690 2022-09-01 21:59:25.188494 torchvf-0.1.2/torchvf/losses/tversky.py
--rw-r--r--   0        0        0      693 2022-09-01 21:56:50.659452 torchvf-0.1.2/torchvf/metrics/__init__.py
--rw-r--r--   0        0        0      962 2022-08-28 19:33:43.969269 torchvf-0.1.2/torchvf/metrics/f1.py
--rw-r--r--   0        0        0      955 2022-08-28 19:33:44.753274 torchvf-0.1.2/torchvf/metrics/iou.py
--rw-r--r--   0        0        0     3430 2022-08-28 19:33:45.401277 torchvf-0.1.2/torchvf/metrics/map_iou.py
--rw-r--r--   0        0        0      646 2022-09-01 21:45:11.446507 torchvf-0.1.2/torchvf/models/__init__.py
--rw-r--r--   0        0        0     1588 2022-09-01 21:54:07.962341 torchvf-0.1.2/torchvf/models/decoder.py
--rw-r--r--   0        0        0     2566 2022-09-01 21:54:17.490407 torchvf-0.1.2/torchvf/models/encoder.py
--rw-r--r--   0        0        0     2700 2022-09-01 21:55:52.435056 torchvf-0.1.2/torchvf/models/models.py
--rw-r--r--   0        0        0     1394 2022-08-28 19:33:42.633262 torchvf-0.1.2/torchvf/models/modules.py
--rw-r--r--   0        0        0      795 2022-09-01 22:54:10.861461 torchvf-0.1.2/torchvf/numerics/__init__.py
--rw-r--r--   0        0        0     3685 2022-09-01 14:53:48.930004 torchvf-0.1.2/torchvf/numerics/affinity.py
--rw-r--r--   0        0        0      717 2022-09-01 22:20:57.779094 torchvf-0.1.2/torchvf/numerics/differentiation/__init__.py
--rw-r--r--   0        0        0     1275 2022-09-01 22:20:20.210265 torchvf-0.1.2/torchvf/numerics/differentiation/finite_differences.py
--rw-r--r--   0        0        0     2296 2022-08-28 19:33:30.913196 torchvf-0.1.2/torchvf/numerics/differentiation/kernels.py
--rw-r--r--   0        0        0      847 2022-09-01 22:51:59.308058 torchvf-0.1.2/torchvf/numerics/integration/__init__.py
--rw-r--r--   0        0        0     2207 2022-09-01 22:18:50.388144 torchvf-0.1.2/torchvf/numerics/integration/ivp_int.py
--rw-r--r--   0        0        0     1810 2022-08-28 19:33:27.861179 torchvf-0.1.2/torchvf/numerics/integration/solvers.py
--rw-r--r--   0        0        0     1261 2022-08-28 19:33:28.713183 torchvf-0.1.2/torchvf/numerics/integration/utils.py
--rw-r--r--   0        0        0      647 2022-09-01 21:21:05.484887 torchvf-0.1.2/torchvf/numerics/interpolation/__init__.py
--rw-r--r--   0        0        0     5508 2022-08-28 19:33:25.113163 torchvf-0.1.2/torchvf/numerics/interpolation/functional.py
--rw-r--r--   0        0        0     1392 2022-09-01 21:16:24.790987 torchvf-0.1.2/torchvf/numerics/interpolation/interp_vf.py
--rw-r--r--   0        0        0     3302 2022-09-05 22:59:48.665364 torchvf-0.1.2/torchvf/numerics/vector_fields.py
--rw-r--r--   0        0        0      985 2022-09-01 22:56:56.723220 torchvf-0.1.2/torchvf/transforms/__init__.py
--rw-r--r--   0        0        0     1401 2022-08-28 19:33:15.329109 torchvf-0.1.2/torchvf/transforms/functional.py
--rw-r--r--   0        0        0     3616 2022-09-01 22:43:16.306347 torchvf-0.1.2/torchvf/transforms/transforms.py
--rw-r--r--   0        0        0      750 2022-09-01 22:25:32.876345 torchvf-0.1.2/torchvf/utils/__init__.py
--rw-r--r--   0        0        0     2650 2022-09-01 14:18:13.722015 torchvf-0.1.2/torchvf/utils/clustering.py
--rw-r--r--   0        0        0     2419 2022-08-28 19:33:04.985051 torchvf-0.1.2/torchvf/utils/logger.py
--rw-r--r--   0        0        0     1050 2022-09-01 22:26:47.097571 torchvf-0.1.2/torchvf/utils/tiling/__init__.py
--rw-r--r--   0        0        0     5411 2022-09-01 22:34:26.132066 torchvf-0.1.2/torchvf/utils/tiling/base.py
--rw-r--r--   0        0        0     3356 2022-09-03 17:05:16.632024 torchvf-0.1.2/torchvf/utils/tiling/dynamic_overlap.py
--rw-r--r--   0        0        0     1821 2022-09-01 22:27:14.946015 torchvf-0.1.2/torchvf/utils/tiling/padding.py
--rw-r--r--   0        0        0     1187 2022-09-01 22:27:13.549992 torchvf-0.1.2/torchvf/utils/tiling/reshape.py
--rw-r--r--   0        0        0     4201 2022-09-01 14:19:39.174514 torchvf-0.1.2/torchvf/utils/utils.py
--rw-r--r--   0        0        0     8267 2023-03-30 22:09:57.001495 torchvf-0.1.2/setup.py
--rw-r--r--   0        0        0     8069 2023-03-30 22:09:57.002636 torchvf-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    10762 2022-08-28 01:18:25.336023 torchvf-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6989 2022-09-05 22:57:48.436642 torchvf-0.1.3/README.md
+-rw-r--r--   0        0        0      941 2023-06-08 02:41:59.992050 torchvf-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      604 2022-09-01 22:49:28.718439 torchvf-0.1.3/torchvf/__init__.py
+-rw-r--r--   0        0        0      746 2022-09-01 22:44:33.723212 torchvf-0.1.3/torchvf/dataloaders/__init__.py
+-rw-r--r--   0        0        0     4387 2022-08-28 19:51:36.958577 torchvf-0.1.3/torchvf/dataloaders/bpcis.py
+-rw-r--r--   0        0        0     1301 2022-08-28 19:51:35.302585 torchvf-0.1.3/torchvf/dataloaders/dataloader.py
+-rw-r--r--   0        0        0     4188 2022-08-28 19:51:33.734593 torchvf-0.1.3/torchvf/dataloaders/sartorius.py
+-rw-r--r--   0        0        0      711 2022-09-01 21:58:08.031975 torchvf-0.1.3/torchvf/losses/__init__.py
+-rw-r--r--   0        0        0     2929 2022-08-28 19:50:48.626833 torchvf-0.1.3/torchvf/losses/dice.py
+-rw-r--r--   0        0        0     3403 2023-06-08 02:34:56.463406 torchvf-0.1.3/torchvf/losses/ivp_loss.py
+-rw-r--r--   0        0        0     2690 2022-09-01 21:59:25.188494 torchvf-0.1.3/torchvf/losses/tversky.py
+-rw-r--r--   0        0        0      693 2022-09-01 21:56:50.659452 torchvf-0.1.3/torchvf/metrics/__init__.py
+-rw-r--r--   0        0        0      962 2022-08-28 19:33:43.969269 torchvf-0.1.3/torchvf/metrics/f1.py
+-rw-r--r--   0        0        0      955 2022-08-28 19:33:44.753274 torchvf-0.1.3/torchvf/metrics/iou.py
+-rw-r--r--   0        0        0     3430 2022-08-28 19:33:45.401277 torchvf-0.1.3/torchvf/metrics/map_iou.py
+-rw-r--r--   0        0        0      646 2022-09-01 21:45:11.446507 torchvf-0.1.3/torchvf/models/__init__.py
+-rw-r--r--   0        0        0     1588 2022-09-01 21:54:07.962341 torchvf-0.1.3/torchvf/models/decoder.py
+-rw-r--r--   0        0        0     2566 2022-09-01 21:54:17.490407 torchvf-0.1.3/torchvf/models/encoder.py
+-rw-r--r--   0        0        0     2700 2022-09-01 21:55:52.435056 torchvf-0.1.3/torchvf/models/models.py
+-rw-r--r--   0        0        0     1394 2022-08-28 19:33:42.633262 torchvf-0.1.3/torchvf/models/modules.py
+-rw-r--r--   0        0        0      795 2022-09-01 22:54:10.861461 torchvf-0.1.3/torchvf/numerics/__init__.py
+-rw-r--r--   0        0        0     3685 2022-09-01 14:53:48.930004 torchvf-0.1.3/torchvf/numerics/affinity.py
+-rw-r--r--   0        0        0      717 2022-09-01 22:20:57.779094 torchvf-0.1.3/torchvf/numerics/differentiation/__init__.py
+-rw-r--r--   0        0        0     1275 2022-09-01 22:20:20.210265 torchvf-0.1.3/torchvf/numerics/differentiation/finite_differences.py
+-rw-r--r--   0        0        0     2296 2022-08-28 19:33:30.913196 torchvf-0.1.3/torchvf/numerics/differentiation/kernels.py
+-rw-r--r--   0        0        0      847 2022-09-01 22:51:59.308058 torchvf-0.1.3/torchvf/numerics/integration/__init__.py
+-rw-r--r--   0        0        0     2207 2022-09-01 22:18:50.388144 torchvf-0.1.3/torchvf/numerics/integration/ivp_int.py
+-rw-r--r--   0        0        0     1810 2022-08-28 19:33:27.861179 torchvf-0.1.3/torchvf/numerics/integration/solvers.py
+-rw-r--r--   0        0        0     1261 2022-08-28 19:33:28.713183 torchvf-0.1.3/torchvf/numerics/integration/utils.py
+-rw-r--r--   0        0        0      647 2022-09-01 21:21:05.484887 torchvf-0.1.3/torchvf/numerics/interpolation/__init__.py
+-rw-r--r--   0        0        0     6705 2023-06-08 02:24:24.120520 torchvf-0.1.3/torchvf/numerics/interpolation/functional.py
+-rw-r--r--   0        0        0     1623 2023-06-08 02:10:21.900015 torchvf-0.1.3/torchvf/numerics/interpolation/interp_vf.py
+-rw-r--r--   0        0        0     3302 2022-09-05 22:59:48.665364 torchvf-0.1.3/torchvf/numerics/vector_fields.py
+-rw-r--r--   0        0        0      985 2022-09-01 22:56:56.723220 torchvf-0.1.3/torchvf/transforms/__init__.py
+-rw-r--r--   0        0        0     1401 2022-08-28 19:33:15.329109 torchvf-0.1.3/torchvf/transforms/functional.py
+-rw-r--r--   0        0        0     3616 2022-09-01 22:43:16.306347 torchvf-0.1.3/torchvf/transforms/transforms.py
+-rw-r--r--   0        0        0      750 2022-09-01 22:25:32.876345 torchvf-0.1.3/torchvf/utils/__init__.py
+-rw-r--r--   0        0        0     2650 2022-09-01 14:18:13.722015 torchvf-0.1.3/torchvf/utils/clustering.py
+-rw-r--r--   0        0        0     2419 2022-08-28 19:33:04.985051 torchvf-0.1.3/torchvf/utils/logger.py
+-rw-r--r--   0        0        0     1050 2022-09-01 22:26:47.097571 torchvf-0.1.3/torchvf/utils/tiling/__init__.py
+-rw-r--r--   0        0        0     5411 2022-09-01 22:34:26.132066 torchvf-0.1.3/torchvf/utils/tiling/base.py
+-rw-r--r--   0        0        0     3356 2022-09-03 17:05:16.632024 torchvf-0.1.3/torchvf/utils/tiling/dynamic_overlap.py
+-rw-r--r--   0        0        0     1821 2022-09-01 22:27:14.946015 torchvf-0.1.3/torchvf/utils/tiling/padding.py
+-rw-r--r--   0        0        0     1187 2022-09-01 22:27:13.549992 torchvf-0.1.3/torchvf/utils/tiling/reshape.py
+-rw-r--r--   0        0        0     4201 2022-09-01 14:19:39.174514 torchvf-0.1.3/torchvf/utils/utils.py
+-rw-r--r--   0        0        0     8276 2023-06-08 02:47:29.679083 torchvf-0.1.3/setup.py
+-rw-r--r--   0        0        0     8078 2023-06-08 02:47:29.679941 torchvf-0.1.3/PKG-INFO
```

### Comparing `torchvf-0.1.2/LICENSE` & `torchvf-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/README.md` & `torchvf-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/pyproject.toml` & `torchvf-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torchvf"
-version = "0.1.2"
+version = "0.1.3"
 description = "Vector fields for instance segmentation in PyTorch."
 authors = ["Ryan Peters <RyanIRL@icloud.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/ryanirl/torchvf"
 repository = "https://github.com/ryanirl/torchvf"
 classifiers = [  
@@ -21,15 +21,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 torch = ">=1.6.0,<2.1.0"
 scikit-learn = "*"
 matplotlib = "*"
-opencv-python = "*"
+opencv-python-headless = "*"
 numpy = "*"
 pandas = "*"
 torchvision = "*"
 pyyaml = "*"
 edt = "*"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `torchvf-0.1.2/torchvf/__init__.py` & `torchvf-0.1.3/torchvf/__init__.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/dataloaders/__init__.py` & `torchvf-0.1.3/torchvf/dataloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/dataloaders/bpcis.py` & `torchvf-0.1.3/torchvf/dataloaders/bpcis.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/dataloaders/dataloader.py` & `torchvf-0.1.3/torchvf/dataloaders/dataloader.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/dataloaders/sartorius.py` & `torchvf-0.1.3/torchvf/dataloaders/sartorius.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/losses/__init__.py` & `torchvf-0.1.3/torchvf/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/losses/dice.py` & `torchvf-0.1.3/torchvf/losses/dice.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/losses/ivp_loss.py` & `torchvf-0.1.3/torchvf/losses/ivp_loss.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,50 +29,61 @@
     Known issues:
         - Under interpolation we clip values that go beyond our image domain,
         therefore backpropogated gradients at the image borders might not be as
         expected. This isn't necessarily a problem with this loss function
         iteself as it is with the interpolation.
 
     """
-    def __init__(self, dx = 0.5, n_steps = 8, solver = "euler", device = "cpu"):
+    def __init__(self, 
+        dx = 0.5, 
+        n_steps = 8, 
+        solver = "euler", 
+        mode = "bilinear_batched",
+        device = "cpu"
+    ):
         """
         Args:
             dx (float): Numeric integration step size.
             n_steps (int): Number of numeric integration steps.
             solver (str): Numeric integration solver. One of:
                 - "euler"
                 - "midpoint"
                 - "runge_kutta"
+            mode (str): The type of interpolation to do. One of:
+                - "bilinear_batched"
+                - "nearest_batched"
 
         """
         super(IVPLoss, self).__init__()
 
         self.dx = dx
         self.n_steps = n_steps
         self.solver = solver
+        self.mode = mode
         self.device = device
 
-    def _compute_init_values(self, B, H, W):
-        y, x = torch.meshgrid(
-            torch.arange(0, H, device = self.device), 
-            torch.arange(0, W, device = self.device),
-            indexing = "ij"
-        )
+    def _compute_init_values(self, shape):
+        B, C, *dims = shape
 
-        init_values = torch.stack([x, y], dim = 0)
-        init_values = init_values.repeat(B, 1, 1, 1)
+        coords = [
+            torch.arange(0, l, device = self.device) 
+            for l in dims
+        ]
+        mesh = torch.meshgrid(coords, indexing = "ij")
+
+        init_shape = [B, 1] + ([1] * len(dims))
+        init_values = torch.stack(mesh[::-1], dim = 0)
+        init_values = init_values.repeat(init_shape)
 
         return init_values
 
     def _compute_batched_trajectories(self, vf):
-        B, C, H, W = vf.shape
+        init_values = self._compute_init_values(vf.shape)
 
-        vf = interp_vf(vf, mode = "bilinear_batched")
-
-        init_values = self._compute_init_values(B, H, W)
+        vf = interp_vf(vf, mode = self.mode)
 
         trajectories = ivp_solver(
             vf, 
             init_values, 
             dx = self.dx, 
             n_steps = self.n_steps, 
             solver = self.solver
```

### Comparing `torchvf-0.1.2/torchvf/losses/tversky.py` & `torchvf-0.1.3/torchvf/losses/tversky.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/metrics/__init__.py` & `torchvf-0.1.3/torchvf/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/metrics/f1.py` & `torchvf-0.1.3/torchvf/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/metrics/iou.py` & `torchvf-0.1.3/torchvf/metrics/iou.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/metrics/map_iou.py` & `torchvf-0.1.3/torchvf/metrics/map_iou.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/models/__init__.py` & `torchvf-0.1.3/torchvf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/models/decoder.py` & `torchvf-0.1.3/torchvf/models/decoder.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/models/encoder.py` & `torchvf-0.1.3/torchvf/models/encoder.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/models/models.py` & `torchvf-0.1.3/torchvf/models/models.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/models/modules.py` & `torchvf-0.1.3/torchvf/models/modules.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/numerics/__init__.py` & `torchvf-0.1.3/torchvf/numerics/__init__.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/numerics/affinity.py` & `torchvf-0.1.3/torchvf/numerics/affinity.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/numerics/differentiation/__init__.py` & `torchvf-0.1.3/torchvf/numerics/differentiation/__init__.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/numerics/differentiation/finite_differences.py` & `torchvf-0.1.3/torchvf/numerics/differentiation/finite_differences.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/numerics/differentiation/kernels.py` & `torchvf-0.1.3/torchvf/numerics/differentiation/kernels.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/numerics/integration/__init__.py` & `torchvf-0.1.3/torchvf/numerics/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/numerics/integration/ivp_int.py` & `torchvf-0.1.3/torchvf/numerics/integration/ivp_int.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/numerics/integration/solvers.py` & `torchvf-0.1.3/torchvf/numerics/integration/solvers.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/numerics/integration/utils.py` & `torchvf-0.1.3/torchvf/numerics/integration/utils.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/numerics/interpolation/__init__.py` & `torchvf-0.1.3/torchvf/numerics/interpolation/__init__.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/numerics/interpolation/functional.py` & `torchvf-0.1.3/torchvf/numerics/interpolation/functional.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     Returns:
         torch.float32: The interpolated values of shape (D, N).
 
     """
     _, H, W = vf.shape
 
     clipped = torch.empty_like(points)
-    clipped[0] = torch.clip(points[0], 0, W - 1)
-    clipped[1] = torch.clip(points[1], 0, H - 1)
+    clipped[0] = torch.clamp(points[0], 0, W - 1)
+    clipped[1] = torch.clamp(points[1], 0, H - 1)
 
     x, y = torch.round(clipped).long()
 
     return vf[:, y, x]
 
 
 def bilinear_interpolation(vf, points):
@@ -188,10 +188,47 @@
         lerp_x1,
         delta_y
     )
 
     return lerp_y
 
 
+def nearest_interpolation_batched(vf, points):
+    """ 
+    Computes a batched nearest-neighbor interpolation on the vector 
+    field `vf` given `points`. Because it's batched, all points
+    on `vf` need to be considered and therefore the `points` shape 
+    will be (B, D, *TYX) where `len(TXW) == D`. Assumes `points` 
+    index `vf`, and that `vf` is defined on a regular rectangular 
+    grid of equidistant points.
+
+    Modified code from Kevin Cutler: 
+        - https://github.com/kevinjohncutler
+
+    Args:
+        vf (torch.float32): Vector field of shape (B, D, *TYX). Must
+            be of type float. For example:
+                - (B, 2, H, W)
+                - (B, 3, H, W, D)
+                - (B, 4, H, W, D, ...)
+        pt (torch.float32): The points of dimension D to be 
+            interpolated. Of shape (B, D, TYX). Must be of type float.
+
+    Returns:
+        torch.float32: The interpolated values of shape (B, D, TYX).
+
+    """
+    B, D, *dims = vf.shape
+
+    points = torch.stack([
+        torch.clamp(points[:, i], 0, d - 1)
+        for i, d in enumerate(dims)
+    ], axis = 1)
+
+    points = points.round_().long().contiguous()
+
+    return vf.gather(-1, points)
+
+
```

### Comparing `torchvf-0.1.2/torchvf/numerics/interpolation/interp_vf.py` & `torchvf-0.1.3/torchvf/numerics/interpolation/interp_vf.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,26 +10,34 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from torchvf.numerics.interpolation.functional import (
     bilinear_interpolation_batched,
+    nearest_interpolation_batched,
     bilinear_interpolation,
     nearest_interpolation
 )
 
 
 def _vf_bilinear_batched(vector_field):
     def _vf(p):
         out = bilinear_interpolation_batched(vector_field, p)
         return out
     return _vf
 
 
+def _vf_nearest_batched(vector_field):
+    def _vf(p):
+        out = nearest_interpolation_batched(vector_field, p)
+        return out
+    return _vf
+
+
 def _vf_bilinear(vector_field):
     def _vf(p):
         out = bilinear_interpolation(vector_field[0], p)
         return out
     return _vf
 
 
@@ -38,14 +46,15 @@
         out = nearest_interpolation(vector_field[0], p)
         return out
     return _vf
 
 
 vf_interpolators = {
     "bilinear_batched": _vf_bilinear_batched,
+    "nearest_batched": _vf_nearest_batched,
     "bilinear": _vf_bilinear,
     "nearest": _vf_nearest
 }
 
 
 def interp_vf(vector_field, mode = "bilinear"):
     return vf_interpolators[mode](vector_field)
```

### Comparing `torchvf-0.1.2/torchvf/numerics/vector_fields.py` & `torchvf-0.1.3/torchvf/numerics/vector_fields.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/transforms/__init__.py` & `torchvf-0.1.3/torchvf/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/transforms/functional.py` & `torchvf-0.1.3/torchvf/transforms/functional.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/transforms/transforms.py` & `torchvf-0.1.3/torchvf/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/utils/__init__.py` & `torchvf-0.1.3/torchvf/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/utils/clustering.py` & `torchvf-0.1.3/torchvf/utils/clustering.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/utils/logger.py` & `torchvf-0.1.3/torchvf/utils/logger.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/utils/tiling/__init__.py` & `torchvf-0.1.3/torchvf/utils/tiling/__init__.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/utils/tiling/base.py` & `torchvf-0.1.3/torchvf/utils/tiling/base.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/utils/tiling/dynamic_overlap.py` & `torchvf-0.1.3/torchvf/utils/tiling/dynamic_overlap.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/utils/tiling/padding.py` & `torchvf-0.1.3/torchvf/utils/tiling/padding.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/utils/tiling/reshape.py` & `torchvf-0.1.3/torchvf/utils/tiling/reshape.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/torchvf/utils/utils.py` & `torchvf-0.1.3/torchvf/utils/utils.py`

 * *Files identical despite different names*

### Comparing `torchvf-0.1.2/setup.py` & `torchvf-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['edt',
  'matplotlib',
  'numpy',
- 'opencv-python',
+ 'opencv-python-headless',
  'pandas',
  'pyyaml',
  'scikit-learn',
  'torch>=1.6.0,<2.1.0',
  'torchvision']
 
 setup_kwargs = {
     'name': 'torchvf',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Vector fields for instance segmentation in PyTorch.',
     'long_description': '# TorchVF\n\nTorchVF is a unifying Python library for using vector fields for efficient\nproposal-free instance segmentation. Vector field based methods are\nlightweight, fast to train, and can accurately segment objects with arbitrary\nmorphology and population density. Read more about vector field based methods\nfor instance segmentation in my \n[article](https://github.com/ryanirl/torchvf/blob/main/article/first_draft.pdf).\nTorchVF provides a vector field agnostic API for ground truth vector field\ncomputation, interpolation of discretely sampled vector fields, numeric\nintegration solvers, clustering functions, and various other utilities. \n\nThis repository also provides all configs, code, and tools necessary to\nreproduce the results presented in my\n[article](https://github.com/ryanirl/torchvf/blob/main/article/first_draft.pdf)\non vector field based methods.\n\n## Installation \n\nTorchVF can be install via pip:\n\n```\npip install torchvf\n```\n\nFor the most up-to-date version, you could install directly from GitHub (this\nis not recommended):\n\n```\npip install git+https://github.com/ryanirl/torchvf.git\n```\n\n## Quick Start\n\nFor deriving the instance segmentation from the semantic segmentation and\nvector field, the TorchVF API is centered around 4 functions:\n - `interp_vf()`\n - `init_values_semantic()`\n - `ivp_solver()`\n - `cluster()`\n\nTo demonstrate how these functions work, consider we are given a semantic\nsegmentation `semantic` and vector field `vf`. TorchVF can be used to compute\nthe instance segmentation of an image via the following code: \n\n```Python\nfrom torchvf.numerics import interp_vf, ivp_solver, init_values_semantic\nfrom torchvf.utils import cluster\n\n# Step 1: Convert our discretely sampled vector field into continuous vector\n# field through bilinear interpolation. \nvf = interp_vf(vf, mode = "bilinear")\n\n# Step 2. Convert our semantic segmentation `semantic` into a set of\n# initial-values to be integrated through our vector field `vf`.\ninit_values = init_values_semantic(semantic, device = "cuda:0")\n\n# Step 3. Integrate our initial-values `init_values` through our vector field\n# `vf` for 25 steps with a step size of 0.1 using Euler\'s method for numeric \n# integration. \nsolutions = ivp_solver(\n    vf, \n    init_values, \n    dx = 0.1,\n    n_steps = 25,\n    solver = "euler"\n)[-1] # Get the final solution. \n\n# Clustering can only be done on the CPU. \nsolutions = solutions.cpu()\nsemantic = semantic.cpu()\n\n# Step 4. Cluster the integrated semantic points `solutions` to obtain the\n# instance segmentation. \ninstance_segmentation = cluster(\n    solutions, \n    semantic[0], \n    eps = 2.25,\n    min_samples = 15,\n    snap_noise = False\n)\n\n```\n\n## Supported Features\n\n<details>\n   <summary>Interpolators:</summary>\n\n</br>\n\n| Interpolator             | Implemented          |\n| ------------------------ | -------------------- |\n| Nearest Neighbor         | :white_check_mark:   |\n| Nearest Neighbor Batched | :white_large_square: |\n| Bilinear                 | :white_check_mark:   |\n| Bilinear Batched         | :white_check_mark:   |\n\n</details>\n\n<details>\n   <summary>Numeric Integration Solvers:</summary>\n\n</br>\n\n| Interpolator            | Implemented          |\n| ----------------------- | -------------------- |\n| Euler\'s Method          | :white_check_mark:   |\n| Midpoint Method         | :white_check_mark:   |\n| Runge Kutta (4th Order) | :white_check_mark:   |\n| Adaptive Dormand Prince | :white_large_square: |\n\n</details>\n\n<details>\n   <summary>Clustering Schemes:</summary>\n\n</br>\n\n| Interpolator            | Implemented          |\n| ----------------------- | -------------------- |\n| DBSCAN (Scikit-learn)   | :white_check_mark:   |\n| DCSCAN (PyTorch)        | :white_large_square: |\n| ...?                    | :white_large_square: | \n\n</details>\n\n<details>\n   <summary>Vector Field Computation:</summary>\n\n</br>\n\n| Interpolator           | Implemented          |\n| ---------------------- | -------------------- |\n| Truncated SDF + Kernel | :white_check_mark:   |\n| Affinity Derived       | :white_check_mark:   |\n| Omnipose               | :white_large_square: |\n| Centroid Based         | :white_large_square: | \n\n</details>\n\n<details>\n   <summary>Other Utilities:</summary>\n\n</br>\n\n - Tiler wrapper for models. \n - Semantic -> euclidean conversion.\n - The IVP vector field loss function. \n - Tversky and Dice semantic loss functions. \n - Training and evalution scripts. \n - Various pretrained models on the BPCIS dataset.  \n - Modeling for the presented H1 and H2 models. \n - mAP IoU, F1, IoU metrics. \n\n</details>\n\n## Dependencies\n\nThe ultimate goal of TorchVF is to be solely dependent on PyTorch. Although at\nthe moment, the signed distance function computation relies on Seung Lab\'s\neuclidean distance transform [library](https://github.com/seung-lab/euclidean-distance-transform-3d)\nand the DBSCAN clustering implementation relies on Scikit-learn.  Furthermore,\nNumPy appears in various places (mAP IoU metric, clustering, ...).\n\n## Reproducability\n\nThis is a reproducability guide for people who want to reproduce the results\npresented in my [article](https://github.com/ryanirl/torchvf/blob/main/article/first_draft.pdf)\non vector field based methods. First, install the torchvf library and clone the\nrepository to get access to the scripts:\n\n```\npip install torchvf \n\ngit clone https://github.com/ryanirl/torchvf.git\n```\n\n### Installing the Weights\n\nI provide weights for the H1 and H2 models trained on each subset of the BPCIS dataset. These weights,\nalong with configs and logging information for both training and evaluation, can be downloaded \n[here](https://drive.google.com/drive/folders/14fvNNZkr4ewuy0-Q2mwjCX-fbMVS7X90?usp=sharing)\n(157.5 MB zipped | 185.5 MB unzipped). \n\nOnce you download the weights:\n - Unzip the file.\n - Replace the `torchvf/weights` file with the downloaded and unzipped `torchvf_weights` file. \n - Rename `torchvf/torchvf_weights` to `torchvf/weights`.\n\n### Installing the BPCIS Dataset\n\nDownload the BPCIS dataset [here](http://www.cellpose.org/dataset_omnipose).\nThen setup the file system this way:\n\n```bash\n├── torchvf/\n├── data/\n│   └── bpcis/\n│       ├── bact_fluor_train/\n│       ├── bact_fluor_test/\n│       ├── bact_phase_train/\n│       ├── bact_phase_test/\n│       ├── worm_train/\n│       └── worm_test/\n├── weights/\n└── ***\n```\n\nIf you have cloned the library, downloaded the weights, and downloaded the\nBPCIS dataset you *should* be able to do \n`python3 scripts/eval.py --config_dir ./weights/bact_fluor/h1/eval_config.py`.\nThis will run evaluation on the bacterial fluorescence subset using the evaluation \nconfig file provided with the downloaded weights. \n\n\n## Citation\n\n```\n@article{TorchVF,\n   author = {Ryan Peters},\n   title = {TorchVF: Vector Fields for Instance Segmentation},\n   year = 2022\n}\n```\n\n## License\n\nDistributed under the Apache-2.0 license. See `LICENSE` for more information.\n\n\n\n\n\n',
     'author': 'Ryan Peters',
     'author_email': 'RyanIRL@icloud.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ryanirl/torchvf',
```

### Comparing `torchvf-0.1.2/PKG-INFO` & `torchvf-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchvf
-Version: 0.1.2
+Version: 0.1.3
 Summary: Vector fields for instance segmentation in PyTorch.
 Home-page: https://github.com/ryanirl/torchvf
 License: Apache-2.0
 Author: Ryan Peters
 Author-email: RyanIRL@icloud.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: edt
 Requires-Dist: matplotlib
 Requires-Dist: numpy
-Requires-Dist: opencv-python
+Requires-Dist: opencv-python-headless
 Requires-Dist: pandas
 Requires-Dist: pyyaml
 Requires-Dist: scikit-learn
 Requires-Dist: torch (>=1.6.0,<2.1.0)
 Requires-Dist: torchvision
 Project-URL: Repository, https://github.com/ryanirl/torchvf
 Description-Content-Type: text/markdown
```

