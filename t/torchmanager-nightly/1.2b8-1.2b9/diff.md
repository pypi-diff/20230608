# Comparing `tmp/torchmanager_nightly-1.2b8.tar.gz` & `tmp/torchmanager_nightly-1.2b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager_nightly-1.2b8.tar", max compression
+gzip compressed data, was "torchmanager_nightly-1.2b9.tar", max compression
```

## Comparing `torchmanager_nightly-1.2b8.tar` & `torchmanager_nightly-1.2b9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1318 2023-04-21 19:45:23.217167 torchmanager_nightly-1.2b8/LICENSE
--rw-r--r--   0        0        0      659 2023-05-26 15:09:49.947121 torchmanager_nightly-1.2b8/pyproject.toml
--rw-r--r--   0        0        0      290 2023-05-26 15:07:26.272267 torchmanager_nightly-1.2b8/torchmanager/__init__.py
--rw-r--r--   0        0        0    10862 2023-05-26 15:07:26.273598 torchmanager_nightly-1.2b8/torchmanager/basic.py
--rw-r--r--   0        0        0      638 2023-05-26 15:07:26.275089 torchmanager_nightly-1.2b8/torchmanager/callbacks/__init__.py
--rw-r--r--   0        0        0     4444 2023-05-26 15:07:26.276587 torchmanager_nightly-1.2b8/torchmanager/callbacks/callback.py
--rw-r--r--   0        0        0     4628 2023-05-26 14:55:58.693727 torchmanager_nightly-1.2b8/torchmanager/callbacks/ckpt.py
--rw-r--r--   0        0        0     3523 2023-05-26 14:55:58.693887 torchmanager_nightly-1.2b8/torchmanager/callbacks/dynamic.py
--rw-r--r--   0        0        0     1608 2023-05-26 14:55:58.694033 torchmanager_nightly-1.2b8/torchmanager/callbacks/early_stop.py
--rw-r--r--   0        0        0     4642 2023-05-26 15:07:26.277845 torchmanager_nightly-1.2b8/torchmanager/callbacks/experiment.py
--rw-r--r--   0        0        0     2224 2023-05-26 14:55:58.694400 torchmanager_nightly-1.2b8/torchmanager/callbacks/lr.py
--rw-r--r--   0        0        0     2599 2023-05-26 15:07:26.278448 torchmanager_nightly-1.2b8/torchmanager/callbacks/tensorboard.py
--rw-r--r--   0        0        0      964 2023-05-26 15:07:26.279144 torchmanager_nightly-1.2b8/torchmanager/compatibility.py
--rw-r--r--   0        0        0       26 2023-05-26 15:07:26.279332 torchmanager_nightly-1.2b8/torchmanager/configs/__init__.py
--rw-r--r--   0        0        0     3013 2023-05-26 15:07:26.280129 torchmanager_nightly-1.2b8/torchmanager/configs/basic.py
--rw-r--r--   0        0        0       85 2023-05-26 14:55:58.695089 torchmanager_nightly-1.2b8/torchmanager/data/__init__.py
--rw-r--r--   0        0        0     6968 2023-05-26 15:07:26.280966 torchmanager_nightly-1.2b8/torchmanager/data/dataset.py
--rw-r--r--   0        0        0     2238 2023-05-26 15:07:26.281606 torchmanager_nightly-1.2b8/torchmanager/data/sliding.py
--rw-r--r--   0        0        0      156 2023-05-26 15:07:26.282249 torchmanager_nightly-1.2b8/torchmanager/losses/__init__.py
--rw-r--r--   0        0        0     5386 2023-05-26 14:55:58.695855 torchmanager_nightly-1.2b8/torchmanager/losses/cross_entropy.py
--rw-r--r--   0        0        0     1047 2023-05-26 15:07:26.282728 torchmanager_nightly-1.2b8/torchmanager/losses/dice.py
--rw-r--r--   0        0        0     5757 2023-05-26 15:07:26.283917 torchmanager_nightly-1.2b8/torchmanager/losses/loss.py
--rw-r--r--   0        0        0     3117 2023-05-26 15:07:26.284752 torchmanager_nightly-1.2b8/torchmanager/losses/mse.py
--rw-r--r--   0        0        0      362 2023-05-26 15:07:26.285400 torchmanager_nightly-1.2b8/torchmanager/metrics/__init__.py
--rw-r--r--   0        0        0     4033 2023-05-26 15:07:26.286652 torchmanager_nightly-1.2b8/torchmanager/metrics/accuracy.py
--rw-r--r--   0        0        0     3678 2023-05-26 15:07:26.287441 torchmanager_nightly-1.2b8/torchmanager/metrics/conf_met.py
--rw-r--r--   0        0        0     5139 2023-05-26 15:07:26.287876 torchmanager_nightly-1.2b8/torchmanager/metrics/extractor.py
--rw-r--r--   0        0        0     2070 2023-05-26 15:07:26.288465 torchmanager_nightly-1.2b8/torchmanager/metrics/iou.py
--rw-r--r--   0        0        0     4003 2023-05-26 15:07:26.289542 torchmanager_nightly-1.2b8/torchmanager/metrics/metric.py
--rw-r--r--   0        0        0     2307 2023-05-26 15:09:49.947536 torchmanager_nightly-1.2b8/torchmanager/metrics/similarity.py
--rw-r--r--   0        0        0     9558 2023-05-26 15:07:26.290610 torchmanager_nightly-1.2b8/torchmanager/testing.py
--rw-r--r--   0        0        0       96 2023-05-26 15:07:26.291264 torchmanager_nightly-1.2b8/torchmanager/train/__init__.py
--rw-r--r--   0        0        0     4964 2023-05-26 14:55:58.698577 torchmanager_nightly-1.2b8/torchmanager/train/checkpoint.py
--rw-r--r--   0        0        0      694 2023-05-26 15:07:26.291528 torchmanager_nightly-1.2b8/torchmanager/train/learning_rate.py
--rw-r--r--   0        0        0    13808 2023-05-26 15:07:26.292056 torchmanager_nightly-1.2b8/torchmanager/training.py
--rw-r--r--   0        0        0      459 2023-05-26 15:07:26.292957 torchmanager_nightly-1.2b8/torchmanager_core/__init__.py
--rw-r--r--   0        0        0      109 2023-05-26 15:07:26.293236 torchmanager_nightly-1.2b8/torchmanager_core/devices/__init__.py
--rw-r--r--   0        0        0     4879 2023-05-26 15:07:26.293903 torchmanager_nightly-1.2b8/torchmanager_core/devices/device.py
--rw-r--r--   0        0        0      264 2023-05-26 14:55:58.701197 torchmanager_nightly-1.2b8/torchmanager_core/devices/protocols.py
--rw-r--r--   0        0        0      153 2023-05-26 14:55:58.701398 torchmanager_nightly-1.2b8/torchmanager_core/errors/__init__.py
--rw-r--r--   0        0        0      350 2023-05-26 14:55:58.701746 torchmanager_nightly-1.2b8/torchmanager_core/errors/runtime.py
--rw-r--r--   0        0        0      669 2023-05-26 14:55:58.701938 torchmanager_nightly-1.2b8/torchmanager_core/errors/train.py
--rw-r--r--   0        0        0     2772 2023-05-26 15:07:26.294864 torchmanager_nightly-1.2b8/torchmanager_core/protocols.py
--rw-r--r--   0        0        0       44 2023-05-26 15:07:26.295205 torchmanager_nightly-1.2b8/torchmanager_core/random/__init__.py
--rw-r--r--   0        0        0     1029 2023-05-26 15:07:26.295759 torchmanager_nightly-1.2b8/torchmanager_core/random/seed.py
--rw-r--r--   0        0        0      204 2023-05-26 14:55:58.702551 torchmanager_nightly-1.2b8/torchmanager_core/typing.py
--rw-r--r--   0        0        0     5260 2023-05-26 15:09:49.948122 torchmanager_nightly-1.2b8/torchmanager_core/version.py
--rw-r--r--   0        0        0      439 2023-05-26 15:07:26.296612 torchmanager_nightly-1.2b8/torchmanager_core/view/__init__.py
--rw-r--r--   0        0        0      313 2023-05-26 14:55:58.703314 torchmanager_nightly-1.2b8/torchmanager_core/view/protocols.py
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 torchmanager_nightly-1.2b8/PKG-INFO
+-rw-r--r--   0        0        0     1318 2023-03-14 14:54:20.813363 torchmanager_nightly-1.2b9/LICENSE
+-rw-r--r--   0        0        0      672 2023-06-08 15:47:06.822835 torchmanager_nightly-1.2b9/pyproject.toml
+-rw-r--r--   0        0        0      290 2023-06-08 13:42:56.795253 torchmanager_nightly-1.2b9/torchmanager/__init__.py
+-rw-r--r--   0        0        0    11928 2023-06-08 15:47:06.823206 torchmanager_nightly-1.2b9/torchmanager/basic.py
+-rw-r--r--   0        0        0      638 2023-06-08 13:42:56.796148 torchmanager_nightly-1.2b9/torchmanager/callbacks/__init__.py
+-rw-r--r--   0        0        0     4444 2023-06-08 13:42:56.796532 torchmanager_nightly-1.2b9/torchmanager/callbacks/callback.py
+-rw-r--r--   0        0        0     4628 2023-06-01 19:00:58.329930 torchmanager_nightly-1.2b9/torchmanager/callbacks/ckpt.py
+-rw-r--r--   0        0        0     3523 2023-06-01 19:00:58.330042 torchmanager_nightly-1.2b9/torchmanager/callbacks/dynamic.py
+-rw-r--r--   0        0        0     1608 2023-06-01 19:00:58.330150 torchmanager_nightly-1.2b9/torchmanager/callbacks/early_stop.py
+-rw-r--r--   0        0        0     4642 2023-06-08 13:42:56.797025 torchmanager_nightly-1.2b9/torchmanager/callbacks/experiment.py
+-rw-r--r--   0        0        0     2224 2023-06-01 19:00:58.330768 torchmanager_nightly-1.2b9/torchmanager/callbacks/lr.py
+-rw-r--r--   0        0        0     2599 2023-06-08 13:42:56.797496 torchmanager_nightly-1.2b9/torchmanager/callbacks/tensorboard.py
+-rw-r--r--   0        0        0      586 2023-06-08 15:47:06.823480 torchmanager_nightly-1.2b9/torchmanager/compatibility.py
+-rw-r--r--   0        0        0       26 2023-06-08 13:42:56.798472 torchmanager_nightly-1.2b9/torchmanager/configs/__init__.py
+-rw-r--r--   0        0        0     2980 2023-06-08 15:47:06.823739 torchmanager_nightly-1.2b9/torchmanager/configs/basic.py
+-rw-r--r--   0        0        0       85 2023-06-01 19:00:58.331061 torchmanager_nightly-1.2b9/torchmanager/data/__init__.py
+-rw-r--r--   0        0        0     6968 2023-06-08 13:42:56.799616 torchmanager_nightly-1.2b9/torchmanager/data/dataset.py
+-rw-r--r--   0        0        0     2238 2023-06-08 13:42:56.799838 torchmanager_nightly-1.2b9/torchmanager/data/sliding.py
+-rw-r--r--   0        0        0      156 2023-06-08 13:42:56.800621 torchmanager_nightly-1.2b9/torchmanager/losses/__init__.py
+-rw-r--r--   0        0        0     5557 2023-06-08 15:47:06.823928 torchmanager_nightly-1.2b9/torchmanager/losses/cross_entropy.py
+-rw-r--r--   0        0        0     1047 2023-06-08 13:42:56.801183 torchmanager_nightly-1.2b9/torchmanager/losses/dice.py
+-rw-r--r--   0        0        0     5740 2023-06-08 15:47:06.824071 torchmanager_nightly-1.2b9/torchmanager/losses/loss.py
+-rw-r--r--   0        0        0     3156 2023-06-08 15:47:06.824201 torchmanager_nightly-1.2b9/torchmanager/losses/mse.py
+-rw-r--r--   0        0        0      351 2023-06-08 15:47:06.824339 torchmanager_nightly-1.2b9/torchmanager/metrics/__init__.py
+-rw-r--r--   0        0        0     4098 2023-06-08 15:47:06.824464 torchmanager_nightly-1.2b9/torchmanager/metrics/accuracy.py
+-rw-r--r--   0        0        0     3651 2023-06-08 15:47:06.824750 torchmanager_nightly-1.2b9/torchmanager/metrics/conf_met.py
+-rw-r--r--   0        0        0     5139 2023-06-08 13:42:56.804542 torchmanager_nightly-1.2b9/torchmanager/metrics/extractor.py
+-rw-r--r--   0        0        0     2070 2023-06-08 13:42:56.804802 torchmanager_nightly-1.2b9/torchmanager/metrics/iou.py
+-rw-r--r--   0        0        0     3937 2023-06-08 15:47:06.824930 torchmanager_nightly-1.2b9/torchmanager/metrics/metric.py
+-rw-r--r--   0        0        0     2307 2023-06-08 13:42:56.805688 torchmanager_nightly-1.2b9/torchmanager/metrics/similarity.py
+-rw-r--r--   0        0        0     8702 2023-06-08 15:47:06.825235 torchmanager_nightly-1.2b9/torchmanager/testing.py
+-rw-r--r--   0        0        0       96 2023-06-08 13:42:56.806384 torchmanager_nightly-1.2b9/torchmanager/train/__init__.py
+-rw-r--r--   0        0        0     4964 2023-06-01 19:00:58.336017 torchmanager_nightly-1.2b9/torchmanager/train/checkpoint.py
+-rw-r--r--   0        0        0      694 2023-06-08 13:42:56.806863 torchmanager_nightly-1.2b9/torchmanager/train/learning_rate.py
+-rw-r--r--   0        0        0    13483 2023-06-08 15:47:06.825551 torchmanager_nightly-1.2b9/torchmanager/training.py
+-rw-r--r--   0        0        0      459 2023-06-08 13:42:56.807626 torchmanager_nightly-1.2b9/torchmanager_core/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-08 13:42:56.808055 torchmanager_nightly-1.2b9/torchmanager_core/devices/__init__.py
+-rw-r--r--   0        0        0     4879 2023-06-08 13:42:56.808230 torchmanager_nightly-1.2b9/torchmanager_core/devices/device.py
+-rw-r--r--   0        0        0      264 2023-06-01 19:00:58.337503 torchmanager_nightly-1.2b9/torchmanager_core/devices/protocols.py
+-rw-r--r--   0        0        0      153 2023-06-01 19:00:58.337794 torchmanager_nightly-1.2b9/torchmanager_core/errors/__init__.py
+-rw-r--r--   0        0        0      350 2023-06-01 19:00:58.338065 torchmanager_nightly-1.2b9/torchmanager_core/errors/runtime.py
+-rw-r--r--   0        0        0      669 2023-06-01 19:00:58.338329 torchmanager_nightly-1.2b9/torchmanager_core/errors/train.py
+-rw-r--r--   0        0        0     3076 2023-06-08 15:47:06.825701 torchmanager_nightly-1.2b9/torchmanager_core/protocols.py
+-rw-r--r--   0        0        0       44 2023-06-08 13:42:56.808831 torchmanager_nightly-1.2b9/torchmanager_core/random/__init__.py
+-rw-r--r--   0        0        0     1029 2023-06-08 13:42:56.809065 torchmanager_nightly-1.2b9/torchmanager_core/random/seed.py
+-rw-r--r--   0        0        0      204 2023-06-01 19:00:58.338499 torchmanager_nightly-1.2b9/torchmanager_core/typing.py
+-rw-r--r--   0        0        0     5256 2023-06-08 15:47:06.825892 torchmanager_nightly-1.2b9/torchmanager_core/version.py
+-rw-r--r--   0        0        0      439 2023-06-08 13:42:56.809755 torchmanager_nightly-1.2b9/torchmanager_core/view/__init__.py
+-rw-r--r--   0        0        0      313 2023-06-01 19:00:58.338878 torchmanager_nightly-1.2b9/torchmanager_core/view/protocols.py
+-rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 torchmanager_nightly-1.2b9/PKG-INFO
```

### Comparing `torchmanager_nightly-1.2b8/LICENSE` & `torchmanager_nightly-1.2b9/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/pyproject.toml` & `torchmanager_nightly-1.2b9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "torchmanager-nightly"
-version = "1.2b8"
-description = "PyTorch Training Manager v1.2 (Beta 8)"
+version = "1.2b9"
+description = "PyTorch Training Manager v1.2 (Beta 9)"
 authors = ["Qisheng He <Qisheng.He@wayne.edu>"]
 repository = "https://github.com/kisonho/torchmanager.git"
 packages = [
     { include = "torchmanager" },
     { include = "torchmanager_core" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
+shutil = "*"
 torch = "*"
 tqdm = "*"
 
 [tool.poetry.optional-dependencies]
 scipy = { version = "*" }
 tensorboard = { version = "*" }
```

### Comparing `torchmanager_nightly-1.2b8/torchmanager/basic.py` & `torchmanager_nightly-1.2b9/torchmanager/basic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from torchmanager_core import torch, Version, deprecated, _raise, API_VERSION, VERSION as CURRENT_VERSION
-from torchmanager_core.typing import Any, Collection, Dict, Generic, Module, Optional, OrderedDict, Self, Tuple, Union
+from torchmanager_core import devices, torch, Version, deprecated, _raise, API_VERSION, VERSION as CURRENT_VERSION
+from torchmanager_core.protocols import VersionConvertible
+from torchmanager_core.typing import Any, Collection, Dict, Generic, List, Module, Optional, OrderedDict, Self, Tuple, Union
 
-from .compatibility import convert
 from .losses import Loss, MultiLosses, ParallelLoss
 from .metrics import Metric
 from .train import Checkpoint
 
 
 class BaseManager(Generic[Module]):
     """
@@ -41,15 +41,15 @@
         - optimizer: A `torch.optim.Optimizer` to train the model
         - raw_loss_fn: An optional `Loss` of the non-paralleled loss function
         - raw_model: A non-paralleled target `torch.nn.Module` model
     """
     # properties
     loss_fn: Optional[Union[Loss, ParallelLoss]]
     metric_fns: Dict[str, Metric]
-    model: Module
+    model: Union[Module, torch.nn.DataParallel]
     optimizer: Optional[torch.optim.Optimizer]
     version: Version
 
     @property
     def compiled(self) -> bool:
         return True if self.loss_fn is not None and self.optimizer is not None else False
 
@@ -63,15 +63,15 @@
             self.loss_fn._metric_fn = self.loss_fn._metric_fn.module
             return self.loss_fn
         else:
             return self.loss_fn
 
     @property
     def raw_model(self) -> Module:
-        return self.model.module if isinstance(self.model, torch.nn.parallel.DataParallel) else self.model
+        return self.model.module if isinstance(self.model, torch.nn.parallel.DataParallel) else self.model  # type: ignore
 
     def __init__(self, model: Module, optimizer: Optional[torch.optim.Optimizer] = None, loss_fn: Optional[Union[Loss, Dict[str, Loss]]] = None, metrics: Dict[str, Metric] = {}) -> None:
         """
         Constructor
 
         - Parameters:
             - loss_fn: An optional `Loss` object to calculate the loss for single loss or a `dict` of losses in `Loss` with their names in `str` to calculate multiple losses
@@ -118,14 +118,26 @@
         - Parameters:
             - loss_fn: A `Loss` object to calculate the loss for single loss or a `dict` of losses in `Loss` with their names in `str` to calculate multiple losses
             - metrics: A `dict` of metrics with a name in `str` and a `Metric` object to calculate the metric
             - optimizer: A `torch.optim.Optimizer` to train the model
         """
         self._compile(optimizer, loss_fn, metrics)
 
+    def data_parallel(self, target_devices: List[torch.device]) -> bool:
+        """
+        Data parallel all available models
+
+        - Parameters:
+            - target_devices: The target multiple devices for data parallel
+        - Returns: A `bool` flag of if use multi GPUs
+        """
+        # multi gpus support for model
+        self.model, use_multi_gpus = devices.data_parallel(self.model, devices=target_devices)
+        return use_multi_gpus
+
     @classmethod
     def from_checkpoint(cls, ckpt: Union[Checkpoint[Any], str], map_location: Optional[torch.device] = None):
         """
         Method to load a manager from a saved `Checkpoint`. The manager will not be compiled with a loss function and its metrics.
 
         - Parameters:
             - ckpt: Either a `Checkpoint` of `Any` object or a `str` of checkpoint path
@@ -148,23 +160,30 @@
                     assert isinstance(manager.loss_fn._metric_fn.module, Loss), _raise(TypeError("Loss function is not a valid `Loss`."))
                     manager.loss_fn = manager.loss_fn._metric_fn.module
             else:
                 manager.loss_fn = None
         else:
             raise TypeError(f"The saved checkpoint contains a model with type of {type(ckpt.model)} that cannot be recoverred to a `Manager`.")
         
-        # convert manager version
+        # initialize manager version
         if not hasattr(manager, "version"):
-            manager.loss_fn = convert(manager.loss_fn)
-            for k in manager.metric_fns:
-                manager.metric_fns[k] = convert(manager.metric_fns[k])
-        elif manager.version < API_VERSION:
-            manager.loss_fn = convert(manager.loss_fn, from_version=manager.version)
-            for k in manager.metric_fns:
-                manager.metric_fns[k] = convert(manager.metric_fns[k], from_version=manager.version)
+            manager.version = Version("v1.0")
+
+        # check manager version
+        if manager.version < API_VERSION:
+            if isinstance(manager.raw_loss_fn, VersionConvertible):
+                manager.raw_loss_fn.convert(manager.version)
+        
+            # convert metrics version
+            for m in manager.metric_fns.items():
+                if isinstance(m, VersionConvertible):
+                    m.convert(manager.version)
+
+        # set to current version
+        manager.version = CURRENT_VERSION
         return manager
 
     def load_state_dict(self, state_dict: OrderedDict[str, Any], strict: bool = True) -> None:
         # load state dict elements
         assert "model" in state_dict, _raise(KeyError("The given dictionary does not have 'model' element."))
         assert "optimizer" in state_dict, _raise(KeyError("The given dictionary does not have 'optimizer' element."))
         assert "loss_fn" in state_dict, _raise(KeyError("The given dictionary does not have 'loss_fn' element."))
@@ -183,14 +202,25 @@
             assert self.loss_fn is not None, _raise(ValueError("The manager has not been compiled with 'loss_fn' given."))
             self.loss_fn.load_state_dict(loss_fn)
         assert metrics is not None, _raise(ValueError("The given dictionary must have 'metrics' element not to be None."))
         for k, m in metrics.items():
             assert k in self.metric_fns, _raise(KeyError(f"The manager does not have a metric named '{k}'."))
             self.metric_fns[k].load_state_dict(m)
 
+    def reset(self, cpu: torch.device = devices.CPU) -> None:
+        """
+        Reset model and loss functions, move all to CPU and empty device cache
+
+        - Parameters:
+            - cpu: The CPU in `torch.device`
+        """
+        self.model = self.raw_model.to(cpu)
+        self.loss_fn = self.raw_loss_fn.to(cpu) if self.raw_loss_fn is not None else self.raw_loss_fn
+        devices.empty_cache()
+
     def state_dict(self, prefix: str = '', keep_vars: bool = False) -> OrderedDict[str, Any]:
         return OrderedDict({
             "model": self.model.state_dict(prefix=prefix, keep_vars=keep_vars),
             "optimizer": self.optimizer.state_dict() if self.optimizer is not None else None,
             "loss_fn": self.loss_fn.state_dict(keep_vars=keep_vars) if self.loss_fn is not None else None,
             "metrics": {k: m.state_dict(keep_vars=keep_vars) for k, m in self.metric_fns.items()}
         })
@@ -198,14 +228,15 @@
     def to(self, device: torch.device) -> None:
         """
         Move the elements in the manager to a target device
 
         - Parameters:
             - device: A target `torch.device`
         """
+        # Move to device
         self.model = self.model.to(device)
         if self.loss_fn is not None:
             self.loss_fn = self.loss_fn.to(device)
         for k, m in self.metric_fns.items():
             self.metric_fns[k] = m.to(device)
 
     def to_checkpoint(self) -> Checkpoint[Self]:
```

### Comparing `torchmanager_nightly-1.2b8/torchmanager/callbacks/__init__.py` & `torchmanager_nightly-1.2b9/torchmanager/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/callbacks/callback.py` & `torchmanager_nightly-1.2b9/torchmanager/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/callbacks/ckpt.py` & `torchmanager_nightly-1.2b9/torchmanager/callbacks/ckpt.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/callbacks/dynamic.py` & `torchmanager_nightly-1.2b9/torchmanager/callbacks/dynamic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/callbacks/early_stop.py` & `torchmanager_nightly-1.2b9/torchmanager/callbacks/early_stop.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/callbacks/experiment.py` & `torchmanager_nightly-1.2b9/torchmanager/callbacks/experiment.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/callbacks/lr.py` & `torchmanager_nightly-1.2b9/torchmanager/callbacks/lr.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/callbacks/tensorboard.py` & `torchmanager_nightly-1.2b9/torchmanager/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/configs/basic.py` & `torchmanager_nightly-1.2b9/torchmanager/configs/basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from torchmanager_core import argparse, abc, os, shutil, torch, view
 from torchmanager_core.typing import Any, Union
-from torchmanager_core import VERSION, DESCRIPTION
+from torchmanager_core import DESCRIPTION
 
 
 class Configs(argparse.Namespace, abc.ABC):
     """
     Basic Configurations
     
     * extends: `argparse.Namespace`
@@ -60,12 +60,12 @@
     def get_arguments(parser: Union[argparse.ArgumentParser, argparse._ArgumentGroup] = argparse.ArgumentParser()) -> Union[argparse.ArgumentParser, argparse._ArgumentGroup]:
         parser.add_argument("-exp", "--experiment", type=str, default="test.exp", help="The name of experiment")
         parser.add_argument("--replace_experiment", action="store_true", default=False, help="The flag to replace given experiment if exists.")
         return parser
 
     def show_environments(self, description: str = DESCRIPTION) -> None:
         view.logger.info(description)
-        view.logger.info(f"torch={torch.__version__}, torchmanager={VERSION}")
+        view.logger.info(f"torch={torch.__version__}")
 
     @abc.abstractmethod
     def show_settings(self) -> None:
         pass
```

### Comparing `torchmanager_nightly-1.2b8/torchmanager/data/dataset.py` & `torchmanager_nightly-1.2b9/torchmanager/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/data/sliding.py` & `torchmanager_nightly-1.2b9/torchmanager/data/sliding.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/losses/cross_entropy.py` & `torchmanager_nightly-1.2b9/torchmanager/losses/cross_entropy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from torchmanager_core import functional as F, torch, _raise
+from torchmanager_core import functional as F, torch, Version, _raise
 from torchmanager_core.typing import Any, Optional
 
 from .dice import Dice
 from .loss import Loss
 
 
 class CrossEntropy(Loss):
@@ -111,14 +111,19 @@
         loss_fn = torch.nn.KLDivLoss(*args, **kwargs)
         super().__init__(loss_fn, target=target, weight=weight)
         self._t = softmax_temperature
         if self._t is not None:
             assert self._t > 0, _raise(ValueError(f"Temperature must be a positive number, got {self._t}."))
         self.replace_nan = replace_nan
 
+    def convert(self, from_version: Version) -> None:
+        if from_version < Version("v1.1"):
+            self.replace_nan = False
+            self._t = None
+
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         # softmax input and target
         if self._t is not None:
             temperatured_input = input / self._t
             temperatured_target = target / self._t
             temperatured_input = temperatured_input.softmax(dim=1).log()
             temperatured_target = temperatured_target if self.log_target else target.softmax(dim=1)
```

### Comparing `torchmanager_nightly-1.2b8/torchmanager/losses/dice.py` & `torchmanager_nightly-1.2b9/torchmanager/losses/dice.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/losses/loss.py` & `torchmanager_nightly-1.2b9/torchmanager/losses/loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from torchmanager_core import torch, _raise
 from torchmanager_core.typing import Any, Callable, List, Optional
 
-from ..metrics import Metric, Reduction
+from ..metrics import Metric
 
 
 class Loss(Metric):
     """
     The main loss function
 
     * extends: `..metrics.Metric`
@@ -36,15 +36,15 @@
         return self.__weight
 
     @weight.setter
     def weight(self, w: float) -> None:
         assert w >= 0, f"Weight must be a non-negative number, got {w}."
         self.__weight = w
 
-    def __init__(self, loss_fn: Optional[Callable[[Any, Any], torch.Tensor]] = None, *, target: Optional[str] = None, weight: float = 1) -> None:
+    def __init__(self, loss_fn: Optional[Callable[[Any, Any], torch.Tensor]] = None, target: Optional[str] = None, weight: float = 1) -> None:
         """
         Constructor
 
         - Parameters:
             - loss_fn: An optional `Callable` function that accepts input or `y_pred` in `Any` kind and target or `y_true` in `Any` kind as inputs and gives a loss in `torch.Tensor`
             - target: An optional `str` of target name in `input` and `target` during direct calling
             - weight: A `float` of the loss weight
@@ -80,15 +80,15 @@
 
     __losses: torch.nn.ModuleList
 
     @property
     def losses(self) -> torch.nn.ModuleList:
         return self.__losses
 
-    def __init__(self, losses: List[Loss], *, target: Optional[str] = None, weight: float = 1) -> None:
+    def __init__(self, losses: List[Loss], target: Optional[str] = None, weight: float = 1) -> None:
         """
         Constructor
 
         - Parameters:
             - losses: A `list` of `Loss` function
             - target: An optional `str` of target name in `input` and `target` during direct calling
             - weight: A `float` of the loss weight
```

### Comparing `torchmanager_nightly-1.2b8/torchmanager/losses/mse.py` & `torchmanager_nightly-1.2b9/torchmanager/losses/mse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from torchmanager_core import torch
+from torchmanager_core.protocols import Reduction
 from torchmanager_core.typing import Any, Callable, Optional
 
-from .loss import Loss, Reduction
+from .loss import Loss
 
 
 class _ReductableLoss(Loss):
     """
     The MSE loss
 
     - Properties:
```

### Comparing `torchmanager_nightly-1.2b8/torchmanager/metrics/accuracy.py` & `torchmanager_nightly-1.2b9/torchmanager/metrics/metric.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,141 +1,107 @@
-from torchmanager_core import torch
-from torchmanager_core.typing import Optional, Tuple
+from torchmanager_core import torch, _raise
+from torchmanager_core.typing import Any, Callable, Enum, List, Optional
 
-from .conf_met import BinaryConfusionMetric
-from .metric import Metric, Reduction
 
-
-class Accuracy(Metric):
-    """
-    The traditional accuracy metric to compare two `torch.Tensor`
-
-    * extends: `.metric.Metric`
-    """
-    reduction: Reduction
-
-    def __init__(self, *, reduction: Reduction = Reduction.MEAN, target: Optional[str] = None) -> None:
-        super().__init__(target=target)
-        self.reduction = reduction
-
-    def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
-        if self.reduction == Reduction.MEAN:
-            return input.eq(target).to(torch.float32).mean()
-        elif self.reduction == Reduction.SUM:
-            return input.eq(target).to(torch.float32).sum()
-        else:
-            return input.eq(target)
-
-
-class SparseCategoricalAccuracy(Accuracy):
+class Metric(torch.nn.Module):
     """
-    The accuracy metric for normal integer labels
+    The basic metric class
 
-    * extends: `Accuracy`
+    * extends: `torch.nn.Module`
+    * implements: `torchmanager_core.protocols.Resulting`
+    * Metric tensor is released from memory as soon as the result returned
 
     - Properties:
-        - dim: An `int` of the probability dim index for the input
+        - result: The `torch.Tensor` of average metric results
+        - results: An optional `torch.Tensor` of all metric results
     """
+    _metric_fn: Optional[Callable[[Any, Any], torch.Tensor]]
+    _results: List[torch.Tensor]
+    _target: Optional[str]
+
+    @property
+    def result(self) -> torch.Tensor:
+        if len(self._results) > 0:
+            return torch.concat(self._results).mean()
+        else:
+            return torch.tensor(torch.nan)
 
-    _dim: int
+    @property
+    def results(self) -> Optional[torch.Tensor]:
+        if len(self._results) > 0:
+            return torch.concat(self._results)
+        else:
+            return None
 
-    def __init__(self, dim: int = -1, *, target: Optional[str] = None) -> None:
+    def __init__(self, metric_fn: Optional[Callable[[Any, Any], torch.Tensor]] = None, target: Optional[str] = None) -> None:
         """
         Constructor
 
         - Parameters:
-            - dim: An `int` of the classification dimension
+            - metric_fn: An optional `Callable` metrics function that accepts `Any` kind of prediction input and target and returns a metric `torch.Tensor`. A `call` method must be overriden if this parameter is set as `None`.
             - target: A `str` of target name in `input` and `target` during direct calling
         """
-        super().__init__(target=target)
-        self._dim = dim
-
-    def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
-        input = input.argmax(dim=self._dim)
-        return super().forward(input, target)
-
-
-class CategoricalAccuracy(SparseCategoricalAccuracy):
-    """
-    The accuracy metric for categorical labels
+        super().__init__()
+        self._metric_fn = metric_fn
+        self._results = []
+        self._target = target
+
+    def __call__(self, input: Any, target: Any) -> torch.Tensor:
+        # unpack input and target
+        if self._target is not None:
+            assert isinstance(input, dict) and isinstance(target, dict), _raise(TypeError(f"Given input or target must be dictionaries, got {type(input)} and {type(target)}."))
+            assert self._target in input and self._target in target, _raise(TypeError(f"Target ‘{self._target}’ cannot be found not in input or target"))
+            input, target = input[self._target], target[self._target]
+
+        # call
+        m: torch.Tensor = super().__call__(input, target)
+        self._results.append(m.unsqueeze(0).cpu().detach())
+        return m
 
-    * extends: `SparseCategoricalAccuracy`
-    """
-
-    def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
-        target = target.argmax(dim=self._dim)
-        return super().forward(input, target)
-
-
-class F1(BinaryConfusionMetric):
-    """
-    The F1 metrics
-    """
-
-    def forward(self, input: Tuple[torch.Tensor, torch.Tensor, torch.Tensor], target: torch.Tensor) -> torch.Tensor:
-        # extract input
-        tp, fp, fn = input
-
-        # calculate precision and recall
-        precision = tp / (tp + fp + self._eps)
-        recall = tp / (tp + fn + self._eps)
-
-        # calculate F1
-        f1 = 2 * precision * recall / (precision + recall + self._eps)
-        f1 = torch.mean(f1)
-        return f1
-
-
-class MAE(Metric):
-    """
-    The Mean Absolute Error metric
-
-    * extends: `.metrics.Metric`
-
-    - Properties:
-        - reduction: A `.loss.Reduction` of reduction method
-    """
-    reduction: Reduction
-
-    def __init__(self, *, reduction: Reduction = Reduction.MEAN, target: Optional[str] = None) -> None:
+    def forward(self, input: Any, target: Any) -> torch.Tensor:
         """
-        Constructor
+        Forward the current result method
 
         - Parameters:
-            - reduction: A `.loss.Reduction` of reduction method
-            - target: An optional `str` of target name in `input` and `target` during direct calling
+            - input: The prediction, or `y_pred`, in `Any` kind
+            - target: The label, or `y_true`, in `Any` kind
+        - Returns: The metric in `torch.Tensor`
         """
-        super().__init__(target=target)
-        self.reduction = reduction
-
-    def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
-        # calculate MAE
-        error = input - target
-        error = error.abs()
-
-        # error reduction
-        if self.reduction == Reduction.MEAN:
-            return error.mean()
-        elif self.reduction == Reduction.SUM:
-            return error.sum()
+        # main method
+        if self._metric_fn is not None:
+            return self._metric_fn(input, target)
         else:
-            return error
+            raise NotImplementedError("metric_fn is not given.")
 
+    def reset(self) -> None:
+        """Reset the current results list"""
+        self._results.clear()
 
-class Precision(BinaryConfusionMetric):
-    """
-    The Precision metrics
+
+def metric(fn: Callable[[Any, Any], torch.Tensor]) -> Metric:
     """
+    The metric wrapping function that wrap a function into a metric
 
-    def forward(self, input: Tuple[torch.Tensor, torch.Tensor, torch.Tensor], target: torch.Tensor) -> torch.Tensor:
-        tp, fp, _ = input
-        return tp / (tp + fp + self._eps)
+    Use as a decorator:
+    >>> import torch
+    >>> @metric
+    >>> def some_metric_fn(input: Any, target: Any) -> torch.Tensor:
+    ...    return ...
+    >>> manager = (..., metric_fns={'out': some_metric_fn})
+    """
+    return Metric(fn)
 
 
-class Recall(BinaryConfusionMetric):
-    """
-    The Recall metrics
+def metric_fn(target: Optional[str] = None) -> Callable[[Callable[[Any, Any], torch.Tensor]], Metric]:
     """
+    The loss wrapping function that wrap a function with target and weight given into a loss
 
-    def forward(self, input: Tuple[torch.Tensor, torch.Tensor, torch.Tensor], target: torch.Tensor) -> torch.Tensor:
-        tp, _, fn = input
-        return tp / (tp + fn + self._eps)
+    Use as a decorator:
+    >>> import torch
+    >>> @metric_fn(target='out')
+    >>> def some_metric_fn(input: Any, target: Any) -> torch.Tensor:
+    ...    return ...
+    >>> manager = (..., metric_fns={'out': some_metric_fn})
+    """
+    def wrapped_fn(fn_to_wrap: Callable[[Any, Any], torch.Tensor]) -> Metric:
+        return Metric(fn_to_wrap, target=target)
+    return wrapped_fn
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torchmanager_nightly-1.2b8/torchmanager/metrics/conf_met.py` & `torchmanager_nightly-1.2b9/torchmanager/metrics/conf_met.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from torchmanager_core import abc, torch, deprecated, _raise
-from torchmanager_core.typing import Any, Optional, Tuple
+from torchmanager_core.typing import Any, Optional
 
 from .metric import Metric
 
 
 class BinaryConfusionMetric(Metric, abc.ABC):
     """
-    The binary confusion metrics that forwards input as a `tuple` of TP, FP, and FN
+    The binary confusion metrics that calculates TP, FP, and FN and forward further to calculate the final metric
 
     * extends: `.metric.Metric`
     * Abstract class
 
     - Methods to implement:
-        - forward: The main `forward` method that accepts input as a `tuple` of TP, FP, and FN as `torch.Tensor` and returns the final metric as `torch.Tensor`
+        - forward_metric: The main method that accepts TP, FP, and FN as `torch.Tensor` and returns the final metric as `torch.Tensor`
     """
     _dim: int
     _eps: float
 
     def __init__(self, dim: int = -1, *, eps: float=1e-7):
         super().__init__()
         self._dim = dim
         self._eps = eps
 
-    def __call__(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
+    def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         # argmax input
         input = input.argmax(dim=self._dim)
 
         # calculate TP, FP, and FN
         tp = torch.sum(target * input, dim=0)
         fp = torch.sum((1 - target) * input, dim=0)
         fn = torch.sum(target * (1 - input), dim=0)
-        return super().__call__((tp, fp, fn), target)
+        return self.forward_metric(tp, fp, fn)
 
     @abc.abstractmethod
-    def forward(self, input: Tuple[torch.Tensor, torch.Tensor, torch.Tensor], target: torch.Tensor) -> torch.Tensor:
+    def forward_metric(self, tp: torch.Tensor, fp: torch.Tensor, fn: torch.Tensor) -> torch.Tensor:
         return NotImplemented
 
 
 class ConfusionMetrics(Metric, abc.ABC):
     """
     The metric that forward confusion metrics calculated by given `input` and `target` as final `input` in `forward` method
```

### Comparing `torchmanager_nightly-1.2b8/torchmanager/metrics/extractor.py` & `torchmanager_nightly-1.2b9/torchmanager/metrics/extractor.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/metrics/iou.py` & `torchmanager_nightly-1.2b9/torchmanager/metrics/iou.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/metrics/similarity.py` & `torchmanager_nightly-1.2b9/torchmanager/metrics/similarity.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/testing.py` & `torchmanager_nightly-1.2b9/torchmanager/testing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from torch.utils.data import DataLoader
-from torchmanager_core import devices, errors, torch, view, _raise
+from torchmanager_core import devices, errors, torch, view
 from torchmanager_core.protocols import Resulting
-from torchmanager_core.typing import Any, Collection, Dict, List, Module, Optional, Union
+from torchmanager_core.typing import Any, Collection, Dict, List, Module, Optional, Tuple, Union
 
 from .basic import BaseManager
 from .data import Dataset
-from .losses import Loss, ParallelLoss
 
 
 class Manager(BaseManager[Module]):
     """
     A testing manager, only used for testing
 
     * extends: `.basic.BaseManager`
@@ -36,33 +35,46 @@
 
         # summarize loss
         if self.loss_fn is not None:
             summary["loss"] = float(self.loss_fn.result.detach())
 
         # summarize metrics
         for name, fn in self.metric_fns.items():
-            if name.startswith("val_"):
+            if name.startswith("val_") and self.model.training:
+                continue
+            elif name.startswith("val_"):
                 name = name.replace("val_", "")
             try:
                 summary[name] = float(fn.result.detach())
             except Exception as metric_error:
                 runtime_error = errors.MetricError(name)
                 raise runtime_error from metric_error
         return summary
 
-
-    def forward(self, x_train: Any) -> Any:
+    def forward(self, x_train: Any, y_test: Optional[Any] = None) -> Tuple[Any, Optional[torch.Tensor]]:
         """
         Forward pass function
 
         - Parameters:
             - x_train: The training data
         - Returns: `Any` kind of model output
         """
-        return self.model(x_train)
+        # forward model
+        y = self.model(x_train)
+
+        # forward loss
+        if self.loss_fn is not None and y_test is not None:
+            try:
+                loss = self.loss_fn(y, y_test)
+            except Exception as loss_error:
+                runtime_error = errors.LossError()
+                raise loss_error from runtime_error
+        else:
+            loss = None
+        return y, loss
 
     @torch.no_grad()
     def predict(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection[Any]], /, *, device: Optional[Union[torch.device, List[torch.device]]] = None, use_multi_gpus: bool = False, show_verbose: bool = False) -> List[Any]:
         '''
         Predict the whole dataset
 
         - Parameters:
@@ -85,28 +97,28 @@
             dataset_len = dataset.batched_len
         else:
             dataset_len = len(dataset)
         progress_bar = view.tqdm(total=dataset_len) if show_verbose else None
 
         # move model
         try:
-            if use_multi_gpus and not isinstance(self.model, torch.nn.parallel.DataParallel):
-                self.model, use_multi_gpus = devices.data_parallel(self.model, devices=target_devices)
+            # multi gpus support
+            use_multi_gpus = self.data_parallel(target_devices)
 
             # initialize predictions
             self.model.eval()
             predictions: List[Any] = []
             self.to(device)
 
             # loop the dataset
             for data in dataset:
                 x, _ = self.unpack_data(data)
                 if use_multi_gpus is not True:
                     x = devices.move_to_device(x, device)
-                y = self.forward(x)
+                y, _ = self.forward(x, None)
                 predictions.append(y)
                 if progress_bar is not None:
                     progress_bar.update()
 
             # reset model and loss
             return predictions
         except KeyboardInterrupt:
@@ -118,31 +130,30 @@
             raise runtime_error from error
         finally:
             # end epoch training
             if progress_bar is not None:
                 progress_bar.close()
 
             # empty cache
-            self.model = self.raw_model.to(cpu)
-            devices.empty_cache()
+            self.reset(cpu)
 
     @torch.no_grad()
     def test(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection[Any]],  /, *,device: Optional[Union[torch.device, List[torch.device]]] = None, empty_cache: bool = True, use_multi_gpus: bool = False, show_verbose: bool = False) -> Dict[str, float]:
         """
         Test target model
 
         - Parameters:
             - dataset: A `torch.utils.data.DataLoader` or `.data.Dataset` dataset
             - device: An optional `torch.device` to test on if not using multi-GPUs or an optional default `torch.device` for testing otherwise
             - empyt_cache: A `bool` flag to empty cache after testing
             - use_multi_gpus: A `bool` flag to use multi gpus during testing
             - show_verbose: A `bool` flag to show the progress bar during testing
         - Returns: A `dict` of validation summary
         """
-        # initialize device
+        # find available device
         cpu, device, target_devices = devices.search(device)
         if device == cpu and len(target_devices) < 2:
             use_multi_gpus = False
         devices.set_default(target_devices[0])
 
         # initialize progress bar
         if len(dataset) == 0:
@@ -156,27 +167,18 @@
         # reset loss function and metrics
         if self.loss_fn is not None:
             self.loss_fn.eval().reset()
         for _, m in self.metric_fns.items():
             m.eval().reset()
 
         try:
-            # multi-gpus support for model
-            if use_multi_gpus and not isinstance(self.model, torch.nn.parallel.DataParallel):
-                self.model, use_multi_gpus = devices.data_parallel(self.model, devices=target_devices)
-
-            # multi-gpus support for loss function
-            if use_multi_gpus and self.loss_fn is not None and not isinstance(self.loss_fn, torch.nn.parallel.DataParallel):
-                paralleled_loss_fn, use_multi_gpus = devices.data_parallel(self.loss_fn, devices=target_devices, parallel_type=ParallelLoss)
-                assert isinstance(paralleled_loss_fn, ParallelLoss) or isinstance(paralleled_loss_fn, Loss), _raise(TypeError("Paralleled function is not a valid `ParallelLoss` or `Loss` after parallel."))
-                self.loss_fn = paralleled_loss_fn
-
-            # set module status and move to device
-            self.model.eval()
+            # move to device
+            use_multi_gpus = self.data_parallel(target_devices)
             self.to(device)
+            self.model.eval()
 
             # batch loop
             for data in dataset:
                 # move x_test, y_test to device
                 x_test, y_test = self.unpack_data(data)
                 if use_multi_gpus is not True:
                     x_test = devices.move_to_device(x_test, device)
@@ -202,43 +204,33 @@
         finally:
             # end epoch training
             if progress_bar is not None:
                 progress_bar.close()
 
             # empty cache
             if empty_cache:
-                self.model = self.raw_model.to(cpu)
-                self.loss_fn = self.raw_loss_fn.to(cpu) if self.raw_loss_fn is not None else self.raw_loss_fn
-                devices.empty_cache()
+                self.reset(cpu)
 
     def test_step(self, x_test: Any, y_test: Any) -> Dict[str, float]:
         """
         A single testing step
 
         - Parameters:
             - x_train: The testing data in `torch.Tensor`
             - y_train: The testing label in `torch.Tensor`
         - Returns: A `dict` of validation summary
         """
         # forward pass
-        y = self.forward(x_test)
+        y, _ = self.forward(x_test)
 
         # forward metrics
         for name, fn in self.compiled_metrics.items():
             if name.startswith("val_"):
                 name = name.replace("val_", "")
             elif "loss" in name:
                 continue
             try:
                 fn(y, y_test)
             except Exception as metric_error:
                 runtime_error = errors.MetricError(name)
                 raise runtime_error from metric_error
-
-        # forward loss
-        if self.loss_fn is not None:
-            try:
-                self.loss_fn(y, y_test)
-            except Exception as loss_error:
-                runtime_error = errors.LossError()
-                raise loss_error from runtime_error
         return self.summary
```

### Comparing `torchmanager_nightly-1.2b8/torchmanager/train/checkpoint.py` & `torchmanager_nightly-1.2b9/torchmanager/train/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/train/learning_rate.py` & `torchmanager_nightly-1.2b9/torchmanager/train/learning_rate.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager/training.py` & `torchmanager_nightly-1.2b9/torchmanager/training.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from torch.utils.data import DataLoader
-from torchmanager_core import devices, errors, math, torch, view
+from torchmanager_core import devices, errors, math, torch, view, _raise
 from torchmanager_core.protocols import Resulting
 from torchmanager_core.typing import Any, Collection, Dict, List, Module, Optional, Self, Union
 
 from .callbacks import Callback
 from .data import Dataset
 from .losses import Loss, ParallelLoss
 from .metrics import Metric
@@ -137,14 +137,22 @@
         - Parameters:
             - loss: A `torch.Tensor` of loss value
         """
         self.compiled_optimizer.zero_grad()
         loss.backward()
         self.compiled_optimizer.step()
 
+    def data_parallel(self, target_devices: List[torch.device]) -> bool:
+        # multi gpus support for loss
+        assert isinstance(self.compiled_losses, Loss), errors._raise(TypeError("The compiled loss function is not a valid `Loss` object."))
+        paralleled_loss_fn, use_multi_gpus = devices.data_parallel(self.compiled_losses, devices=target_devices, parallel_type=ParallelLoss)
+        assert isinstance(paralleled_loss_fn, ParallelLoss) or isinstance(paralleled_loss_fn, Loss), errors._raise(TypeError("Paralleled function is not a valid `ParallelLoss` or `Loss` after parallel."))
+        self.loss_fn = paralleled_loss_fn
+        return super().data_parallel(target_devices) and use_multi_gpus
+
     def fit(self, training_dataset: Union[DataLoader[Any], Dataset[Any], Collection], /, epochs: Optional[int] = None, val_dataset: Optional[Union[DataLoader[Any], Dataset[Any], Collection]] = None, callbacks_list: List[Callback] = [], *, iterations: Optional[int] = None, initial_epoch: Optional[int] = None, device: Optional[Union[torch.device, List[torch.device]]] = None, use_multi_gpus: bool = False, **kwargs) -> Module:
         """
         Training algorithm
 
         - Parameters:
             - training_dataset: Any kind of training dataset in `torch.utils.data.DataLoader` or `.data.Dataset`
             - epochs: An optional `int` number of training epochs (`iterations` must be not given)
@@ -174,38 +182,27 @@
             assert initial_epoch < epochs, errors._raise(ValueError(f"The initial_epoch must be smaller than total epochs, got epochs={epochs} but initial_epoch={initial_epoch}."))
             self.current_epoch = initial_epoch
         elif self.current_epoch > 0:
             initial_epoch = self.current_epoch + 1  # skip the latest current epoch when resuming training
         else:
             initial_epoch = self.current_epoch
 
-        # initialize training
+        # find available device
         cpu, device, target_devices = devices.search(device)
         if device == cpu and len(target_devices) < 2:
             use_multi_gpus = False
         devices.set_default(target_devices[0])
+
+        # initialize training
         for c in callbacks_list:
             c.on_train_start(initial_epoch)
 
         try:
-            # multi gpus support for model
-            if use_multi_gpus and not isinstance(self.model, torch.nn.parallel.DataParallel):
-                model, use_multi_gpus = devices.data_parallel(self.model, devices=target_devices)
-            else:
-                model = self.model
-            self.model = model
-
-            # multi gpus support for loss
-            if use_multi_gpus and not isinstance(self.compiled_losses, torch.nn.parallel.DataParallel):
-                assert isinstance(self.compiled_losses, Loss), errors._raise(TypeError("The compiled loss function is not a valid `Loss` object."))
-                paralleled_loss_fn, use_multi_gpus = devices.data_parallel(self.compiled_losses, devices=target_devices, parallel_type=ParallelLoss)
-                assert isinstance(paralleled_loss_fn, ParallelLoss) or isinstance(paralleled_loss_fn, Loss), errors._raise(TypeError("Paralleled function is not a valid `ParallelLoss` or `Loss` after parallel."))
-                self.loss_fn = paralleled_loss_fn
-
             # move to device
+            use_multi_gpus = self.data_parallel(target_devices)
             self.to(device)
 
             # epoch loop
             for self.current_epoch in range(initial_epoch, epochs):
                 # initialize epoch
                 view.logger.info(f"Training epoch {self.current_epoch + 1}/{epochs}")
                 for c in callbacks_list:
@@ -249,38 +246,36 @@
             view.logger.info("Training interrupted.")
             pass
         except Exception as error:
             view.logger.error(error)
             runtime_error = errors.StopTraining(self.current_epoch, "Training failed.")
             raise runtime_error from error
         finally:
-            self.model = self.raw_model.to(cpu)
-            self.loss_fn = self.raw_loss_fn.to(cpu) if self.raw_loss_fn is not None else self.raw_loss_fn
-            devices.empty_cache()
+            self.reset(cpu)
         return self.raw_model
 
     def train_step(self, x_train: Any, y_train: Any) -> Dict[str, float]:
         """
         A single training step
 
         - Parameters:
             - x_train: The training data
             - y_train: The training label
         - Returns: A summary of `dict` with keys as `str` and values as `float`
         """
         # forward pass
-        y = self.forward(x_train)
-        loss = self.compiled_losses(y, y_train)
-
-        # backward pass
-        self.backward(loss)
+        y, loss = self.forward(x_train, y_train)
+        assert loss is not None, _raise(TypeError("Loss cannot be fetched."))
 
         # forward metrics
         for name, fn in self.compiled_metrics.items():
             if not name.startswith("val_") and "loss" not in name:
                 fn(y, y_train)
+
+        # backward pass
+        self.backward(loss)
         return self.summary
 
     def to_checkpoint(self) -> Checkpoint[Self]:
         ckpt = super().to_checkpoint()
         ckpt.last_epoch = self.current_epoch
         return ckpt
```

### Comparing `torchmanager_nightly-1.2b8/torchmanager_core/devices/device.py` & `torchmanager_nightly-1.2b9/torchmanager_core/devices/device.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager_core/errors/train.py` & `torchmanager_nightly-1.2b9/torchmanager_core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager_core/protocols.py` & `torchmanager_nightly-1.2b9/torchmanager_core/protocols.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import abc, torch, sys
 from enum import Enum
 from typing import Any, Dict, List, Optional, OrderedDict, Protocol, runtime_checkable
 from typing_extensions import Self
 
 from .devices.protocols import DeviceMovable
+from .version import Version
 from .view.protocols import VerboseControllable
 
 
 class Frequency(Enum):
     """
     The frequency enum for learning rate
     """
@@ -69,14 +70,21 @@
     def eval(self) -> Self:
         return NotImplemented
 
     @abc.abstractmethod
     def train(self, mode: bool = True) -> Self:
         return NotImplemented
 
+
+class Reduction(Enum):
+    NONE = 0
+    MEAN = 1
+    SUM = 2
+
+
 class Resulting(StateDictLoadable, Trainable, Protocol):
     """An object that have result available with reset method"""
     @property
     @abc.abstractmethod
     def _target(self) -> Optional[str]:
         return NotImplemented
 
@@ -103,11 +111,20 @@
     """The SummaryWriter protocol"""
 
     @abc.abstractmethod
     def add_scalars(self, main_tag: str, tag_scalar_dict: Any, global_step: Optional[int] = None) -> None:
         pass
 
 
+@runtime_checkable
+class VersionConvertible(Protocol):
+    """The protocol that can convert from previous version"""
+
+    @abc.abstractmethod
+    def convert(self, from_version: Version) -> None:
+        pass
+
+
 class Weighted(Protocol):
     """A weigthted protocol that contains `weight` as its property"""
 
     weight: Any
```

### Comparing `torchmanager_nightly-1.2b8/torchmanager_core/random/seed.py` & `torchmanager_nightly-1.2b9/torchmanager_core/random/seed.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b8/torchmanager_core/version.py` & `torchmanager_nightly-1.2b9/torchmanager_core/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,16 @@
         return self == other or self < other
 
     def __ge__(self, other: Any) -> bool:
         return self == other or self > other
 
 
 API = Version("v1.2")
-CURRENT = Version("v1.2b8")
-DESCRIPTION: str = "PyTorch Training Manager v1.2 (Beta 8)"
+CURRENT = Version("v1.2b9")
+DESCRIPTION: str = "PyTorch Training Manager {CURRENT}"
 
 
 class VersionError(SystemError):
     def __init__(self, method_name: str, maximum_supported_version: str) -> None:
         super().__init__(f"`{method_name}` has been deprecated and removed from version {maximum_supported_version}. Current version: {CURRENT}.")
```

### Comparing `torchmanager_nightly-1.2b8/PKG-INFO` & `torchmanager_nightly-1.2b9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: torchmanager-nightly
-Version: 1.2b8
-Summary: PyTorch Training Manager v1.2 (Beta 8)
+Version: 1.2b9
+Summary: PyTorch Training Manager v1.2 (Beta 9)
 Home-page: https://github.com/kisonho/torchmanager.git
 Author: Qisheng He
 Author-email: Qisheng.He@wayne.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: scipy
 Provides-Extra: tensorboard
+Requires-Dist: shutil
 Requires-Dist: torch
 Requires-Dist: tqdm
 Project-URL: Repository, https://github.com/kisonho/torchmanager.git
```

