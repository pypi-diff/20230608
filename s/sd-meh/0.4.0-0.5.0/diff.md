# Comparing `tmp/sd_meh-0.4.0.tar.gz` & `tmp/sd_meh-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_meh-0.4.0.tar", max compression
+gzip compressed data, was "sd_meh-0.5.0.tar", max compression
```

## Comparing `sd_meh-0.4.0.tar` & `sd_meh-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-05-31 15:54:41.675357 sd_meh-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1585 2023-05-31 15:54:41.675357 sd_meh-0.4.0/README.md
--rw-r--r--   0        0        0      390 2023-05-31 15:54:41.675357 sd_meh-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-31 15:54:41.675357 sd_meh-0.4.0/sd_meh/__init__.py
--rw-r--r--   0        0        0     7957 2023-05-31 15:54:41.675357 sd_meh-0.4.0/sd_meh/merge.py
--rw-r--r--   0        0        0     2416 2023-05-31 15:54:41.675357 sd_meh-0.4.0/sd_meh/merge_methods.py
--rw-r--r--   0        0        0     1465 2023-05-31 15:54:41.675357 sd_meh-0.4.0/sd_meh/model.py
--rw-r--r--   0        0        0    83125 2023-05-31 15:54:41.675357 sd_meh-0.4.0/sd_meh/rebasin.py
--rw-r--r--   0        0        0     2109 1970-01-01 00:00:00.000000 sd_meh-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-08 08:32:25.972422 sd_meh-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1896 2023-06-08 08:32:25.972422 sd_meh-0.5.0/README.md
+-rw-r--r--   0        0        0      390 2023-06-08 08:32:25.972422 sd_meh-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-08 08:32:25.972422 sd_meh-0.5.0/sd_meh/__init__.py
+-rw-r--r--   0        0        0    11589 2023-06-08 08:32:25.972422 sd_meh-0.5.0/sd_meh/merge.py
+-rw-r--r--   0        0        0     5353 2023-06-08 08:32:25.972422 sd_meh-0.5.0/sd_meh/merge_methods.py
+-rw-r--r--   0        0        0     1521 2023-06-08 08:32:25.972422 sd_meh-0.5.0/sd_meh/model.py
+-rw-r--r--   0        0        0    83404 2023-06-08 08:32:25.972422 sd_meh-0.5.0/sd_meh/rebasin.py
+-rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 sd_meh-0.5.0/PKG-INFO
```

### Comparing `sd_meh-0.4.0/LICENSE.txt` & `sd_meh-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd_meh-0.4.0/README.md` & `sd_meh-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -26,29 +26,33 @@
 ```
 Usage: merge_models.py [OPTIONS]
 
 Options:
   -a, --model_a TEXT
   -b, --model_b TEXT
   -c, --model_c TEXT
-  -m, --merging_method [weighted_sum|add_difference|weighted_subtraction|sum_twice|triple_sum|tensor_sum|similarity_add_difference|transmogrify_distribution]
+  -m, --merging_method [weighted_sum|add_difference|weighted_subtraction|sum_twice|triple_sum|tensor_sum|similarity_add_difference|transmogrify_distribution|multiply_difference|distribution_crossover|euclidean_add_difference|ties_add_difference]
   -wc, --weights_clip
   -p, --precision INTEGER
   -o, --output_path TEXT
   -f, --output_format [safetensors|ckpt]
   -wa, --weights_alpha TEXT
   -ba, --base_alpha FLOAT
   -wb, --weights_beta TEXT
   -bb, --base_beta FLOAT
   -rb, --re_basin
   -rbi, --re_basin_iterations INTEGER
+  -d, --device [cpu|cuda]
+  -pr, --prune
   --help                          Show this message and exit.
 ```
 
 ## Features
 
-- weights matching
+- gpu merging
+- prune model before merging (and un-prune at the end)
+- weights matching aka re-basin
 - weights clipping
 - registered pypi package
 - block merge
-- merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`, `similarity_add_difference`, `transmogrify_distribution`
+- merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`, `similarity_add_difference`, `transmogrify_distribution`, `distribution_crossover`, `multiply_difference`, `euclidean_add_difference`, `ties_add_difference`
 - `fp16` and `fp32`
```

### Comparing `sd_meh-0.4.0/sd_meh/merge.py` & `sd_meh-0.5.0/sd_meh/merge.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+import gc
 import os
 import re
+from contextlib import contextmanager
 from pathlib import Path
 from typing import Dict, Optional, Tuple
 
 import safetensors.torch
 import torch
 from tqdm import tqdm
 
 from sd_meh import merge_methods
 from sd_meh.model import SDModel
 from sd_meh.rebasin import (
-    SPECIAL_KEYS,
     apply_permutation,
     sdunet_permutation_spec,
     step_weights_and_bases,
+    update_model_a,
     weight_matching,
 )
 
 MAX_TOKENS = 77
 NUM_INPUT_BLOCKS = 12
 NUM_MID_BLOCK = 1
 NUM_OUTPUT_BLOCKS = 12
@@ -38,15 +40,15 @@
     "cond_stage_model.transformer.embeddings.": "cond_stage_model.transformer.text_model.embeddings.",
     "cond_stage_model.transformer.encoder.": "cond_stage_model.transformer.text_model.encoder.",
     "cond_stage_model.transformer.final_layer_norm.": "cond_stage_model.transformer.text_model.final_layer_norm.",
 }
 
 
 def fix_clip(model: Dict) -> Dict:
-    if KEY_POSITION_IDS in model:
+    if KEY_POSITION_IDS in model.keys():
         model[KEY_POSITION_IDS] = torch.tensor(
             [list(range(MAX_TOKENS))], dtype=torch.int64
         )
 
     return model
 
 
@@ -57,87 +59,177 @@
             del model[key]
 
     return model
 
 
 # https://github.com/j4ded/sdweb-merge-block-weighted-gui/blob/master/scripts/mbw/merge_block_weighted.py#L115
 def fix_model(model: Dict) -> Dict:
-    for k in model:
+    for k in model.keys():
         model = fix_key(model, k)
     return fix_clip(model)
 
 
 def load_sd_model(model: os.PathLike | str, device: str = "cpu") -> Dict:
     if isinstance(model, str):
         model = Path(model)
 
     return SDModel(model, device).load_model()
 
 
+def prune_sd_model(model: Dict) -> Dict:
+    keys = list(model.keys())
+    for k in keys:
+        if (
+            not k.startswith("model.diffusion_model.")
+            and not k.startswith("first_stage_model.")
+            and not k.startswith("cond_stage_model.")
+        ):
+            del model[k]
+    return model
+
+
+def restore_sd_model(original_model: Dict, merged_model: Dict) -> Dict:
+    for k in original_model:
+        if k not in merged_model:
+            merged_model[k] = original_model[k]
+    return merged_model
+
+
+def log_vram(txt=""):
+    alloc = torch.cuda.memory_allocated(0)
+    print(f"{txt}: {alloc*1e-9:5.3f}")
+
+
+def load_thetas(
+    models: Dict[str, os.PathLike | str],
+    prune: bool,
+    device: str,
+    precision: int,
+) -> Dict:
+    log_vram("before loading models")
+    if prune:
+        thetas = {k: prune_sd_model(load_sd_model(m, "cpu")) for k, m in models.items()}
+    else:
+        thetas = {k: load_sd_model(m, device) for k, m in models.items()}
+
+    if device == "cuda":
+        for model_key, model in thetas.items():
+            for key, block in model.items():
+                if precision == 16:
+                    thetas[model_key].update({key: block.to(device).half()})
+                else:
+                    thetas[model_key].update({key: block.to(device)})
+
+    log_vram("models loaded")
+    return thetas
+
+
 def merge_models(
     models: Dict[str, os.PathLike | str],
     weights: Dict,
     bases: Dict,
     merge_mode: str,
     precision: int = 16,
     weights_clip: bool = False,
     re_basin: bool = False,
     iterations: int = 1,
+    device: str = "cpu",
+    prune: bool = False,
 ) -> Dict:
-    thetas = {k: load_sd_model(m) for k, m in models.items()}
+    thetas = load_thetas(models, prune, device, precision)
 
     if re_basin:
-        return rebasin_merge(
+        merged = rebasin_merge(
             thetas,
             weights,
             bases,
             merge_mode,
             precision=precision,
-            weights_clip=weights_clip,
+            weights_clip=False,
             iterations=iterations,
-            device="cpu",
+            device=device,
         )
+        # clip only after the last re-basin iteration
+        if weights_clip:
+            merged = clip_weights(thetas, merged)
     else:
-        return simple_merge(
+        merged = simple_merge(
             thetas,
             weights,
             bases,
             merge_mode,
             precision=precision,
             weights_clip=weights_clip,
         )
 
+    return un_prune_model(merged, thetas, models, device, prune, precision)
+
+
+def un_prune_model(
+    merged: Dict,
+    thetas: Dict,
+    models: Dict,
+    device: str,
+    prune: bool,
+    precision: int,
+) -> Dict:
+    if prune:
+        del thetas
+        gc.collect()
+        log_vram("remove thetas")
+        original_a = load_sd_model(models["model_a"], device)
+        for key in tqdm(original_a.keys(), desc="un-prune model a"):
+            if KEY_POSITION_IDS in key:
+                continue
+            if "model" in key and key not in merged.keys():
+                merged.update({key: original_a[key]})
+                if precision == 16:
+                    merged.update({key: merged[key].half()})
+        del original_a
+        gc.collect()
+        log_vram("remove original_a")
+        original_b = load_sd_model(models["model_b"], device)
+        for key in tqdm(original_b.keys(), desc="un-prune model b"):
+            if KEY_POSITION_IDS in key:
+                continue
+            if "model" in key and key not in merged.keys():
+                merged.update({key: original_b[key]})
+                if precision == 16:
+                    merged.update({key: merged[key].half()})
+        del original_b
+
+    return fix_model(merged)
+
 
 def simple_merge(
     thetas: Dict[str, Dict],
     weights: Dict,
     bases: Dict,
     merge_mode: str,
     precision: int = 16,
     weights_clip: bool = False,
 ) -> Dict:
     for key in tqdm(thetas["model_a"].keys(), desc="stage 1"):
-        if result := merge_key(
-            key,
-            thetas,
-            weights,
-            bases,
-            merge_mode,
-            precision,
-            weights_clip,
-        ):
-            thetas["model_a"][key] = result[1]
+        with merge_key_context(
+            key, thetas, weights, bases, merge_mode, precision, weights_clip
+        ) as result:
+            if result is not None:
+                thetas["model_a"].update({key: result.detach().clone()})
+
+    log_vram("after stage 1")
 
     for key in tqdm(thetas["model_b"].keys(), desc="stage 2"):
         if KEY_POSITION_IDS in key:
             continue
-        if "model" in key and key not in thetas["model_a"]:
+        if "model" in key and key not in thetas["model_a"].keys():
             thetas["model_a"].update({key: thetas["model_b"][key]})
             if precision == 16:
-                thetas["model_a"][key] = thetas["model_a"][key].half()
+                thetas["model_a"].update({key: thetas["model_a"][key].half()})
+
+    log_vram("after stage 2")
 
     return fix_model(thetas["model_a"])
 
 
 def rebasin_merge(
     thetas: Dict[str, os.PathLike | str],
     weights: Dict,
@@ -146,57 +238,68 @@
     precision: int = 16,
     weights_clip: bool = False,
     iterations: int = 1,
     device="cpu",
 ):
     # WARNING: not sure how this does when 3 models are involved...
 
-    model_a = thetas["model_a"].copy()
+    model_a = thetas["model_a"].clone()
     perm_spec = sdunet_permutation_spec()
 
     print("permuting")
     for it in range(iterations):
-        print(it)
+        # print(it)
+        log_vram(f"{it} iteration start")
         new_weights, new_bases = step_weights_and_bases(weights, bases, it, iterations)
+        log_vram("weights & bases, before simple merge")
 
         # normal block merge we already know and love
         thetas["model_a"] = simple_merge(
             thetas, new_weights, new_bases, merge_mode, precision, weights_clip
         )
 
+        log_vram("simple merge done")
+
         # find permutations
         perm_1, y = weight_matching(
             perm_spec,
             model_a,
             thetas["model_a"],
             max_iter=it,
             init_perm=None,
             usefp16=precision == 16,
             device=device,
         )
+
+        log_vram("weight matching #1 done")
+
         thetas["model_a"] = apply_permutation(perm_spec, perm_1, thetas["model_a"])
+
+        log_vram("apply perm 1 done")
+
         perm_2, z = weight_matching(
             perm_spec,
             thetas["model_b"],
             thetas["model_a"],
             max_iter=it,
             init_perm=None,
             usefp16=precision == 16,
             device=device,
         )
-        theta_3 = apply_permutation(perm_spec, perm_2, thetas["model_a"])
 
-        # is this correct for block merge?
+        log_vram("weight matching #2 done")
+
         new_alpha = torch.nn.functional.normalize(
             torch.sigmoid(torch.Tensor([y, z])), p=1, dim=0
         ).tolist()[0]
-        for key in SPECIAL_KEYS:
-            thetas["model_a"][key] = (1 - new_alpha) * (
-                thetas["model_a"][key]
-            ) + new_alpha * theta_3[key]
+        thetas["model_a"] = update_model_a(
+            perm_spec, perm_2, thetas["model_a"], new_alpha
+        )
+
+        log_vram("model a updated")
 
     return thetas["model_a"]
 
 
 def merge_key(
     key: str,
     thetas: Dict,
@@ -206,15 +309,15 @@
     precision: int = 16,
     weights_clip: bool = False,
 ) -> Optional[Tuple[str, Dict]]:
     if KEY_POSITION_IDS in key:
         return
 
     for theta in thetas.values():
-        if key not in theta:
+        if key not in theta.keys():
             return
 
     if "model" in key:
         current_bases = bases
 
         if "model.diffusion_model." in key:
             weight_index = -1
@@ -253,15 +356,33 @@
             t1 = thetas["model_b"][key]
             threshold = torch.maximum(torch.abs(t0), torch.abs(t1))
             merged_key = torch.minimum(torch.maximum(merged_key, -threshold), threshold)
 
         if precision == 16:
             merged_key = merged_key.half()
 
-        return key, merged_key
+        return merged_key
+
+
+def clip_weights(thetas, merged):
+    for k, t0 in thetas["model_a"].items():
+        t1 = thetas["model_b"][k]
+        th = torch.maximum(torch.abs(t0), torch.abs(t1))
+        merged.update({k: torch.minimum(torch.maximum(merged[k], -th), th)})
+    return merged
+
+
+@contextmanager
+def merge_key_context(*args, **kwargs):
+    result = merge_key(*args, **kwargs)
+    try:
+        yield result
+    finally:
+        if result is not None:
+            del result
 
 
 def get_merge_method_args(current_bases: Dict, thetas: Dict, key: str) -> Dict:
     merge_method_args = {
         "a": thetas["model_a"][key],
         "b": thetas["model_b"][key],
         **current_bases,
@@ -270,13 +391,16 @@
     if "model_c" in thetas:
         merge_method_args["c"] = thetas["model_c"][key]
 
     return merge_method_args
 
 
 def save_model(model, output_file, file_format) -> None:
+    print(f"saving {output_file}")
     if file_format == "safetensors":
         safetensors.torch.save_file(
-            model, f"{output_file}.safetensors", metadata={"format": "pt"}
+            model if type(model) == dict else model.to_dict(),
+            f"{output_file}.safetensors",
+            metadata={"format": "pt"},
         )
     else:
         torch.save({"state_dict": model}, f"{output_file}.ckpt")
```

### Comparing `sd_meh-0.4.0/sd_meh/model.py` & `sd_meh-0.5.0/sd_meh/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from dataclasses import dataclass
 
 import safetensors
 import torch
+from tensordict import TensorDict
 
 
 @dataclass
 class SDModel:
     model_path: os.PathLike
     device: str
 
@@ -16,15 +17,15 @@
             ckpt = safetensors.torch.load_file(
                 self.model_path,
                 device=self.device,
             )
         else:
             ckpt = torch.load(self.model_path, map_location=self.device)
 
-        return get_state_dict_from_checkpoint(ckpt)
+        return TensorDict.from_dict(get_state_dict_from_checkpoint(ckpt))
 
 
 # TODO: tidy up
 # from: stable-diffusion-webui/modules/sd_models.py
 def get_state_dict_from_checkpoint(pl_sd):
     pl_sd = pl_sd.pop("state_dict", pl_sd)
     pl_sd.pop("state_dict", None)
```

### Comparing `sd_meh-0.4.0/sd_meh/rebasin.py` & `sd_meh-0.5.0/sd_meh/rebasin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1620,15 +1620,20 @@
             **conv("first_stage_model.quant_conv", "P_bg361", "P_bg362"),
             **conv("first_stage_model.post_quant_conv", "P_bg363", "P_bg364"),
             **skip(
                 "cond_stage_model.transformer.text_model.embeddings.position_ids",
                 None,
                 None,
             ),
-            #  **dense("cond_stage_model.transformer.text_model.embeddings.token_embedding","P_bg365", "P_bg366",bias=False),
+            **dense(
+                "cond_stage_model.transformer.text_model.embeddings.token_embedding",
+                "P_bg365",
+                "P_bg366",
+                bias=False,
+            ),
             **dense(
                 "cond_stage_model.transformer.text_model.embeddings.token_embedding",
                 None,
                 None,
             ),
             **dense(
                 "cond_stage_model.transformer.text_model.embeddings.position_embedding",
@@ -2177,126 +2182,135 @@
     w = params[k]
     for axis, p in enumerate(ps.axes_to_perm[k]):
         # Skip the axis we're trying to permute.
         if axis == except_axis:
             continue
 
         # None indicates that there is no permutation relevant to that axis.
-        if p is not None:
+        if p:
             w = torch.index_select(w, axis, perm[p].int())
 
     return w
 
 
 def apply_permutation(ps: PermutationSpec, perm, params):
     """Apply a `perm` to `params`."""
     return {k: get_permuted_param(ps, perm, k, params) for k in params.keys()}
 
 
+def update_model_a(ps: PermutationSpec, perm, model_a, new_alpha):
+    for k in model_a:
+        model_a[k] = model_a[k] * (1 - new_alpha) + new_alpha * get_permuted_param(
+            ps, perm, k, model_a
+        )
+    return model_a
+
+
 def inner_matching(
     n,
     ps,
     p,
     params_a,
     params_b,
     usefp16,
     progress,
     number,
     linear_sum,
     perm,
     device,
 ):
     A = torch.zeros((n, n), dtype=torch.float16) if usefp16 else torch.zeros((n, n))
+    A = A.to(device)
 
     for wk, axis in ps.perm_to_axes[p]:
         w_a = params_a[wk]
         w_b = get_permuted_param(ps, perm, wk, params_b, except_axis=axis)
         w_a = torch.moveaxis(w_a, axis, 0).reshape((n, -1)).to(device)
         w_b = torch.moveaxis(w_b, axis, 0).reshape((n, -1)).T.to(device)
 
         if usefp16:
-            w_a = w_a.half()
-            w_b = w_b.half()
+            w_a = w_a.half().to(device)
+            w_b = w_b.half().to(device)
 
         try:
             A += torch.matmul(w_a, w_b)
         except RuntimeError:
             A += torch.matmul(torch.dequantize(w_a), torch.dequantize(w_b))
 
     A = A.cpu()
     ri, ci = linear_sum_assignment(A.detach().numpy(), maximize=True)
-
-    if device == "cuda":
-        A = A.cuda()
+    A = A.to(device)
 
     assert (torch.tensor(ri) == torch.arange(len(ri))).all()
 
+    eye_tensor = torch.eye(n).to(device)
+
     oldL = torch.vdot(
-        torch.flatten(A).float(), torch.flatten(torch.eye(n)[perm[p].long()])
+        torch.flatten(A).float(), torch.flatten(eye_tensor[perm[p].long()])
     )
-    newL = torch.vdot(torch.flatten(A).float(), torch.flatten(torch.eye(n)[ci, :]))
+    newL = torch.vdot(torch.flatten(A).float(), torch.flatten(eye_tensor[ci, :]))
 
     if usefp16:
         oldL = oldL.half()
         newL = newL.half()
 
     if newL - oldL != 0:
         linear_sum += abs((newL - oldL).item())
         number += 1
         print(f" > {p}: {newL - oldL}")
 
     progress = progress or newL > oldL + 1e-12
 
-    perm[p] = torch.Tensor(ci)
+    perm[p] = torch.Tensor(ci).to(device)
 
     return linear_sum, number, perm, progress
 
 
 def weight_matching(
     ps: PermutationSpec,
     params_a,
     params_b,
     max_iter=1,
     init_perm=None,
     usefp16=False,
     device="cpu",
 ):
     perm_sizes = {
-        p: params_a[axes[0][0]].shape[axes[0][1]] for p, axes in ps.perm_to_axes.items()
+        p: params_a[axes[0][0]].shape[axes[0][1]]
+        for p, axes in ps.perm_to_axes.items()
+        if axes[0][0] in params_a.keys()
     }
     perm = {}
     perm = (
-        {p: torch.arange(n) for p, n in perm_sizes.items()}
+        {p: torch.arange(n).to(device) for p, n in perm_sizes.items()}
         if init_perm is None
         else init_perm
     )
-    perm_names = list(perm.keys())
+
     linear_sum = 0
     number = 0
 
-    special_layers = ["P_bg358", "P_bg324", "P_bg337"]
+    special_layers = ["P_bg324", "P_bg358", "P_bg337"]
     for _ in range(max_iter):
         progress = False
         shuffle(special_layers)
-        for p_ix in special_layers:
-            p = p_ix
-            if p in special_layers:
-                n = perm_sizes[p]
-
-                linear_sum, number, perm, progress = inner_matching(
-                    n,
-                    ps,
-                    p,
-                    params_a,
-                    params_b,
-                    usefp16,
-                    progress,
-                    number,
-                    linear_sum,
-                    perm,
-                    device,
-                )
+        for p in special_layers:
+            n = perm_sizes[p]
+
+            linear_sum, number, perm, progress = inner_matching(
+                n,
+                ps,
+                p,
+                params_a,
+                params_b,
+                usefp16,
+                progress,
+                number,
+                linear_sum,
+                perm,
+                device,
+            )
         if not progress:
             break
 
     average = linear_sum / number if number > 0 else 0
     return (perm, average)
```

### Comparing `sd_meh-0.4.0/PKG-INFO` & `sd_meh-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-meh
-Version: 0.4.0
+Version: 0.5.0
 Summary: stable diffusion merging execution helper
 Home-page: https://github.com/s1dlx/meh
 License: MIT
 Author: s1dlx
 Author-email: s1dlx@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -42,30 +42,34 @@
 ```
 Usage: merge_models.py [OPTIONS]
 
 Options:
   -a, --model_a TEXT
   -b, --model_b TEXT
   -c, --model_c TEXT
-  -m, --merging_method [weighted_sum|add_difference|weighted_subtraction|sum_twice|triple_sum|tensor_sum|similarity_add_difference|transmogrify_distribution]
+  -m, --merging_method [weighted_sum|add_difference|weighted_subtraction|sum_twice|triple_sum|tensor_sum|similarity_add_difference|transmogrify_distribution|multiply_difference|distribution_crossover|euclidean_add_difference|ties_add_difference]
   -wc, --weights_clip
   -p, --precision INTEGER
   -o, --output_path TEXT
   -f, --output_format [safetensors|ckpt]
   -wa, --weights_alpha TEXT
   -ba, --base_alpha FLOAT
   -wb, --weights_beta TEXT
   -bb, --base_beta FLOAT
   -rb, --re_basin
   -rbi, --re_basin_iterations INTEGER
+  -d, --device [cpu|cuda]
+  -pr, --prune
   --help                          Show this message and exit.
 ```
 
 ## Features
 
-- weights matching
+- gpu merging
+- prune model before merging (and un-prune at the end)
+- weights matching aka re-basin
 - weights clipping
 - registered pypi package
 - block merge
-- merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`, `similarity_add_difference`, `transmogrify_distribution`
+- merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`, `similarity_add_difference`, `transmogrify_distribution`, `distribution_crossover`, `multiply_difference`, `euclidean_add_difference`, `ties_add_difference`
 - `fp16` and `fp32`
```

