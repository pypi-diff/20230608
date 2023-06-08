# Comparing `tmp/daam-0.0.8.tar.gz` & `tmp/daam-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daam-0.0.8.tar", last modified: Wed Nov 30 17:59:09 2022, max compression
+gzip compressed data, was "daam-0.0.9.tar", last modified: Wed Nov 30 18:18:52 2022, max compression
```

## Comparing `daam-0.0.8.tar` & `daam-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2022-11-30 17:59:09.279506 daam-0.0.8/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     1066 2022-11-30 04:07:37.000000 daam-0.0.8/LICENSE
--rw-rw-r--   0 ralph     (1000) ralph     (1000)       25 2022-11-30 17:57:37.000000 daam-0.0.8/MANIFEST.in
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      284 2022-11-30 17:59:09.279506 daam-0.0.8/PKG-INFO
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     4042 2022-11-30 17:50:24.000000 daam-0.0.8/README.md
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2022-11-30 17:59:09.279506 daam-0.0.8/daam/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      112 2022-11-30 04:07:37.000000 daam-0.0.8/daam/__init__.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)       22 2022-11-30 17:58:54.000000 daam-0.0.8/daam/_version.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     3350 2022-11-30 17:11:02.000000 daam-0.0.8/daam/evaluate.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)    13631 2022-11-30 17:50:24.000000 daam-0.0.8/daam/experiment.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     3685 2022-11-30 17:10:08.000000 daam-0.0.8/daam/hook.py
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2022-11-30 17:59:09.279506 daam-0.0.8/daam/run/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2022-11-30 04:07:37.000000 daam-0.0.8/daam/run/__init__.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     3274 2022-11-30 04:07:37.000000 daam-0.0.8/daam/run/evaluate.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     8895 2022-11-30 17:50:24.000000 daam-0.0.8/daam/run/generate.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)    10620 2022-11-30 17:50:24.000000 daam-0.0.8/daam/trace.py
--rw-rw-r--   0 ralph     (1000) ralph     (1000)     3536 2022-11-30 17:10:08.000000 daam-0.0.8/daam/utils.py
-drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2022-11-30 17:59:09.279506 daam-0.0.8/daam.egg-info/
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      284 2022-11-30 17:59:09.000000 daam-0.0.8/daam.egg-info/PKG-INFO
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      399 2022-11-30 17:59:09.000000 daam-0.0.8/daam.egg-info/SOURCES.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        1 2022-11-30 17:59:09.000000 daam-0.0.8/daam.egg-info/dependency_links.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)       48 2022-11-30 17:59:09.000000 daam-0.0.8/daam.egg-info/entry_points.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      102 2022-11-30 17:59:09.000000 daam-0.0.8/daam.egg-info/requires.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)        5 2022-11-30 17:59:09.000000 daam-0.0.8/daam.egg-info/top_level.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      102 2022-11-30 17:10:08.000000 daam-0.0.8/requirements.txt
--rw-rw-r--   0 ralph     (1000) ralph     (1000)       38 2022-11-30 17:59:09.279506 daam-0.0.8/setup.cfg
--rw-rw-r--   0 ralph     (1000) ralph     (1000)      602 2022-11-30 17:10:08.000000 daam-0.0.8/setup.py
+drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2022-11-30 18:18:52.236800 daam-0.0.9/
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     1066 2022-11-30 04:07:37.000000 daam-0.0.9/LICENSE
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)       25 2022-11-30 17:57:37.000000 daam-0.0.9/MANIFEST.in
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      284 2022-11-30 18:18:52.236800 daam-0.0.9/PKG-INFO
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     4042 2022-11-30 17:50:24.000000 daam-0.0.9/README.md
+drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2022-11-30 18:18:52.236800 daam-0.0.9/daam/
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      112 2022-11-30 04:07:37.000000 daam-0.0.9/daam/__init__.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)       22 2022-11-30 18:18:29.000000 daam-0.0.9/daam/_version.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     3350 2022-11-30 17:11:02.000000 daam-0.0.9/daam/evaluate.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)    13631 2022-11-30 17:50:24.000000 daam-0.0.9/daam/experiment.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     3685 2022-11-30 17:10:08.000000 daam-0.0.9/daam/hook.py
+drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2022-11-30 18:18:52.236800 daam-0.0.9/daam/run/
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)        0 2022-11-30 04:07:37.000000 daam-0.0.9/daam/run/__init__.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     3274 2022-11-30 04:07:37.000000 daam-0.0.9/daam/run/evaluate.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     8895 2022-11-30 18:17:13.000000 daam-0.0.9/daam/run/generate.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)    12293 2022-11-30 18:17:10.000000 daam-0.0.9/daam/trace.py
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)     3536 2022-11-30 17:10:08.000000 daam-0.0.9/daam/utils.py
+drwxrwxr-x   0 ralph     (1000) ralph     (1000)        0 2022-11-30 18:18:52.236800 daam-0.0.9/daam.egg-info/
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      284 2022-11-30 18:18:52.000000 daam-0.0.9/daam.egg-info/PKG-INFO
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      399 2022-11-30 18:18:52.000000 daam-0.0.9/daam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)        1 2022-11-30 18:18:52.000000 daam-0.0.9/daam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)       48 2022-11-30 18:18:52.000000 daam-0.0.9/daam.egg-info/entry_points.txt
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      102 2022-11-30 18:18:52.000000 daam-0.0.9/daam.egg-info/requires.txt
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)        5 2022-11-30 18:18:52.000000 daam-0.0.9/daam.egg-info/top_level.txt
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      102 2022-11-30 17:10:08.000000 daam-0.0.9/requirements.txt
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)       38 2022-11-30 18:18:52.236800 daam-0.0.9/setup.cfg
+-rw-rw-r--   0 ralph     (1000) ralph     (1000)      602 2022-11-30 17:10:08.000000 daam-0.0.9/setup.py
```

### Comparing `daam-0.0.8/LICENSE` & `daam-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `daam-0.0.8/README.md` & `daam-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `daam-0.0.8/daam/evaluate.py` & `daam-0.0.9/daam/evaluate.py`

 * *Files identical despite different names*

### Comparing `daam-0.0.8/daam/experiment.py` & `daam-0.0.9/daam/experiment.py`

 * *Files identical despite different names*

### Comparing `daam-0.0.8/daam/hook.py` & `daam-0.0.9/daam/hook.py`

 * *Files identical despite different names*

### Comparing `daam-0.0.8/daam/run/evaluate.py` & `daam-0.0.9/daam/run/evaluate.py`

 * *Files identical despite different names*

### Comparing `daam-0.0.8/daam/run/generate.py` & `daam-0.0.9/daam/run/generate.py`

 * *Files identical despite different names*

### Comparing `daam-0.0.8/daam/trace.py` & `daam-0.0.9/daam/trace.py`

 * *Files 13% similar despite different names*

```diff
@@ -222,14 +222,48 @@
                 map_ = map_.view(map_.size(0), h, w)
                 map_ = map_[map_.size(0) // 2:]  # Filter out unconditional
                 maps.append(map_)
 
         maps = torch.stack(maps, 0)  # shape: (tokens, heads, height, width)
         return maps.permute(1, 0, 2, 3).contiguous()  # shape: (heads, tokens, height, width)
 
+    def _hooked_sliced_attention(hk_self, self, query, key, value, sequence_length, dim):
+        batch_size_attention = query.shape[0]
+        hidden_states = torch.zeros(
+            (batch_size_attention, sequence_length, dim // self.heads), device=query.device, dtype=query.dtype
+        )
+        slice_size = self._slice_size if self._slice_size is not None else hidden_states.shape[0]
+        for i in range(hidden_states.shape[0] // slice_size):
+            start_idx = i * slice_size
+            end_idx = (i + 1) * slice_size
+            attn_slice = torch.baddbmm(
+                torch.empty(slice_size, query.shape[1], key.shape[1], dtype=query.dtype, device=query.device),
+                query[start_idx:end_idx],
+                key[start_idx:end_idx].transpose(-1, -2),
+                beta=0,
+                alpha=self.scale,
+            )
+            attn_slice = attn_slice.softmax(dim=-1)
+            factor = int(math.sqrt(hk_self.latent_hw // attn_slice.shape[1]))
+
+            if attn_slice.shape[-1] == hk_self.context_size:
+                # shape: (batch_size, 64 // factor, 64 // factor, 77)
+                maps = hk_self._unravel_attn(attn_slice)
+
+                for head_idx, heatmap in enumerate(maps):
+                    hk_self.heat_maps.update(factor, hk_self.layer_idx, head_idx, heatmap)
+
+            attn_slice = torch.bmm(attn_slice, value[start_idx:end_idx])
+
+            hidden_states[start_idx:end_idx] = attn_slice
+
+        # reshape hidden_states
+        hidden_states = self.reshape_batch_dim_to_heads(hidden_states)
+        return hidden_states
+
     def _hooked_attention(hk_self, self, query, key, value):
         """
         Monkey-patched version of :py:func:`.CrossAttention._attention` to capture attentions and aggregate them.
 
         Args:
             hk_self (`UNetCrossAttentionHooker`): pointer to the hook itself.
             self (`CrossAttention`): pointer to the module.
@@ -260,14 +294,15 @@
 
         # reshape hidden_states
         hidden_states = self.reshape_batch_dim_to_heads(hidden_states)
         return hidden_states
 
     def _hook_impl(self):
         self.monkey_patch('_attention', self._hooked_attention)
+        self.monkey_patch('_sliced_attention', self._hooked_sliced_attention)
 
     @property
     def num_heat_maps(self):
         return len(next(iter(self.heat_maps.values())))
 
 
 trace: Type[DiffusionHeatMapHooker] = DiffusionHeatMapHooker
```

### Comparing `daam-0.0.8/daam/utils.py` & `daam-0.0.9/daam/utils.py`

 * *Files identical despite different names*

### Comparing `daam-0.0.8/setup.py` & `daam-0.0.9/setup.py`

 * *Files identical despite different names*

