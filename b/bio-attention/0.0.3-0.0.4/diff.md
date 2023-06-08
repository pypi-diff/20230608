# Comparing `tmp/bio-attention-0.0.3.tar.gz` & `tmp/bio-attention-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-attention-0.0.3.tar", last modified: Fri Jun  2 14:30:19 2023, max compression
+gzip compressed data, was "bio-attention-0.0.4.tar", last modified: Thu Jun  8 09:51:50 2023, max compression
```

## Comparing `bio-attention-0.0.3.tar` & `bio-attention-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:30:19.129676 bio-attention-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:30:19.125676 bio-attention-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:30:19.125676 bio-attention-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-02 14:30:11.000000 bio-attention-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-02 14:30:11.000000 bio-attention-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-02 14:30:11.000000 bio-attention-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-02 14:30:19.129676 bio-attention-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-02 14:30:11.000000 bio-attention-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:30:19.125676 bio-attention-0.0.3/bio_attention/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:30:11.000000 bio-attention-0.0.3/bio_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15822 2023-06-02 14:30:11.000000 bio-attention-0.0.3/bio_attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-02 14:30:11.000000 bio-attention-0.0.3/bio_attention/embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:30:19.129676 bio-attention-0.0.3/bio_attention/img/
--rw-r--r--   0 runner    (1001) docker     (123)  2372654 2023-06-02 14:30:11.000000 bio-attention-0.0.3/bio_attention/img/2Dslidingwindow-attention.png
--rw-r--r--   0 runner    (1001) docker     (123)   118589 2023-06-02 14:30:11.000000 bio-attention-0.0.3/bio_attention/img/windowed_implementation.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21699 2023-06-02 14:30:11.000000 bio-attention-0.0.3/bio_attention/positional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:30:19.125676 bio-attention-0.0.3/bio_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-02 14:30:19.000000 bio-attention-0.0.3/bio_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-02 14:30:19.000000 bio-attention-0.0.3/bio_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:30:19.000000 bio-attention-0.0.3/bio_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 14:30:19.000000 bio-attention-0.0.3/bio_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 14:30:19.000000 bio-attention-0.0.3/bio_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:30:11.000000 bio-attention-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-02 14:30:19.129676 bio-attention-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:51:50.585416 bio-attention-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:51:50.581416 bio-attention-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:51:50.581416 bio-attention-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 09:51:39.000000 bio-attention-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-08 09:51:39.000000 bio-attention-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-08 09:51:39.000000 bio-attention-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-08 09:51:50.585416 bio-attention-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-08 09:51:39.000000 bio-attention-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:51:50.581416 bio-attention-0.0.4/bio_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:51:39.000000 bio-attention-0.0.4/bio_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-06-08 09:51:39.000000 bio-attention-0.0.4/bio_attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-08 09:51:39.000000 bio-attention-0.0.4/bio_attention/embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:51:50.585416 bio-attention-0.0.4/bio_attention/img/
+-rw-r--r--   0 runner    (1001) docker     (123)  2372654 2023-06-08 09:51:39.000000 bio-attention-0.0.4/bio_attention/img/2Dslidingwindow-attention.png
+-rw-r--r--   0 runner    (1001) docker     (123)   118589 2023-06-08 09:51:39.000000 bio-attention-0.0.4/bio_attention/img/windowed_implementation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22849 2023-06-08 09:51:39.000000 bio-attention-0.0.4/bio_attention/positional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:51:50.581416 bio-attention-0.0.4/bio_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-08 09:51:50.000000 bio-attention-0.0.4/bio_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-08 09:51:50.000000 bio-attention-0.0.4/bio_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:51:50.000000 bio-attention-0.0.4/bio_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 09:51:50.000000 bio-attention-0.0.4/bio_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 09:51:50.000000 bio-attention-0.0.4/bio_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-08 09:51:39.000000 bio-attention-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-08 09:51:50.585416 bio-attention-0.0.4/setup.cfg
```

### Comparing `bio-attention-0.0.3/.github/workflows/publish.yml` & `bio-attention-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.3/.gitignore` & `bio-attention-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.3/LICENSE` & `bio-attention-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.3/PKG-INFO` & `bio-attention-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-attention
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple implementations of attention modules adapted for the biological data domain
 Home-page: https://github.com/gdewael/bio-attention
 Author: Gaetan De Waele
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -62,10 +62,12 @@
   - [x] Windowed
   - [x] Random
   - [x] Performer
   - [x] Encoder
   - [x] Decoder
   - [ ] Cross
   - [x] Support for multi-dim inputs
+- [ ] Add a warning if non-increasing positional indices are used with a decoder attention
+- [ ] Add docs clarifying that clf tokens are automatically accounted for if no pos is provided for them
 - [ ] Tests
 - [ ] Typing
 - [ ] Docs
```

### Comparing `bio-attention-0.0.3/README.md` & `bio-attention-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -52,10 +52,12 @@
   - [x] Windowed
   - [x] Random
   - [x] Performer
   - [x] Encoder
   - [x] Decoder
   - [ ] Cross
   - [x] Support for multi-dim inputs
+- [ ] Add a warning if non-increasing positional indices are used with a decoder attention
+- [ ] Add docs clarifying that clf tokens are automatically accounted for if no pos is provided for them
 - [ ] Tests
 - [ ] Typing
 - [ ] Docs
```

### Comparing `bio-attention-0.0.3/bio_attention/attention.py` & `bio-attention-0.0.4/bio_attention/attention.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,16 +29,14 @@
         self.use_context_manager = not all(
             [enable_math, enable_flash, enable_mem_efficient]
         )
 
     def forward(self, q, k, v, mask=None, causal=False):
         """Default attention layer
 
-        NOTE: causal attention will erase input masks
-
         Parameters
         ----------
         q : B, *, L1, NH, H
             queries
         k : B, *, L2, NH, H
             keys
         v : B, *, L2, NH, H
@@ -53,40 +51,46 @@
         _type_
             _description_
         """
         q_shape = q.shape
         q, k, v = map(
             lambda t: rearrange(t, "b ... x n h -> (b ...) x n h").permute(0, 2, 1, 3),
             (q, k, v),
-        )
+        ) # (B...), NH, L, H
         if mask is not None:
-            mask = rearrange(mask, "b ... n q k -> (b ...) n q k")
+            mask = rearrange(mask, "b ... n q k -> (b ...) n q k") # (B...), NH, L1, L2
+
+        if causal:
+            causal_mask = torch.ones(q.shape[-2], k.shape[-2], dtype=torch.bool)
+            causal_mask = causal_mask.triu(diagonal=0).expand(q.shape[0], q.shape[1], -1, -1)
+            mask = (mask if mask is not None else (causal_mask).to(q)).masked_fill(causal_mask, -float('inf'))
+
         if self.use_context_manager:
             with torch.backends.cuda.sdp_kernel(**self.context_manager):
                 return (
                     F.scaled_dot_product_attention(
                         q,
                         k,
                         v,
                         dropout_p=(self.dropout if self.training else 0),
                         attn_mask=mask,
-                        is_causal=causal,
+                        is_causal=False,
                     )
                     .permute(0, 2, 1, 3)
                     .view(*q_shape)
                 )
         else:
             return (
                 F.scaled_dot_product_attention(
                     q,
                     k,
                     v,
                     dropout_p=(self.dropout if self.training else 0),
                     attn_mask=mask,
-                    is_causal=causal,
+                    is_causal=False,
                 )
                 .permute(0, 2, 1, 3)
                 .view(*q_shape)
             )
 
 
 class RandomAttention(nn.Module):
@@ -437,15 +441,15 @@
         )
 
     def forward(self, x, pos=None, mask=None, causal=False, **mod_kwargs):
         x = self.attn(self.norm(x), pos=pos, mask=mask, causal=causal, **mod_kwargs) + x
         return self.ff(x)
 
 
-class TransformerEncoder(nn.Module):
+class Transformer(nn.Module):
     def __init__(
         self,
         depth,
         dim,
         nh,
         attentiontype="vanilla",
         attention_args={},
@@ -492,40 +496,44 @@
                 nh,
                 plugin=plugin,
                 dropout=dropout,
                 glu_ff=glu_ff,
                 activation=activation,
             )
         )
-        if only_apply_plugin_at_first:
-            for _ in range(depth - 1):
-                layers.append(
-                    TransformerLayer(
-                        attn_op,
-                        dim,
-                        nh,
-                        plugin=plugin,
-                        dropout=dropout,
-                        glu_ff=glu_ff,
-                        activation=activation,
-                    )
-                )
-        else:
-            for _ in range(depth - 1):
-                layers.append(
-                    TransformerLayer(
-                        attn_op,
-                        dim,
-                        nh,
-                        plugin=None,
-                        dropout=dropout,
-                        glu_ff=glu_ff,
-                        activation=activation,
-                    )
+        
+        for _ in range(depth - 1):
+            layers.append(
+                TransformerLayer(
+                    attn_op,
+                    dim,
+                    nh,
+                    plugin=(None if only_apply_plugin_at_first else plugin),
+                    dropout=dropout,
+                    glu_ff=glu_ff,
+                    activation=activation,
                 )
+            )
+    
 
         self.layers = nn.ModuleList(layers)
 
     def forward(self, x, pos=None, mask=None, causal=False, **mod_kwargs):
         for layer in self.layers:
             x = layer(x, pos=pos, mask=mask, causal=causal, **mod_kwargs)
         return x
+
+class TransformerEncoder(Transformer):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+    def forward(self, x, pos=None, mask=None, **mod_kwargs):
+        for layer in self.layers:
+            x = layer(x, pos=pos, mask=mask, causal=False, **mod_kwargs)
+        return x
+    
+class TransformerDecoder(Transformer):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+    def forward(self, x, pos=None, mask=None, **mod_kwargs):
+        for layer in self.layers:
+            x = layer(x, pos=pos, mask=mask, causal=True, **mod_kwargs)
+        return x
```

### Comparing `bio-attention-0.0.3/bio_attention/embed.py` & `bio-attention-0.0.4/bio_attention/embed.py`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.3/bio_attention/img/2Dslidingwindow-attention.png` & `bio-attention-0.0.4/bio_attention/img/2Dslidingwindow-attention.png`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.3/bio_attention/img/windowed_implementation.svg` & `bio-attention-0.0.4/bio_attention/img/windowed_implementation.svg`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.3/bio_attention/positional.py` & `bio-attention-0.0.4/bio_attention/positional.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import torch
 import torch.nn as nn
+import torch.nn.functional as F
 from einops import rearrange, repeat, einsum
 import math
 
 
 class Base(nn.Module):
     def __init__(self, divide=1.0, learned=False):
         super().__init__()
@@ -50,35 +51,41 @@
         inv_freq = 1 / (10000 ** (torch.arange(0.0, dim, 2) / dim))
         self.register_buffer("inv_freq", inv_freq)
 
     def mod_x(self, x, pos=None, mask=None, **kwargs):
         """
         Args:
             x (torch.tensor): (B,*,L,H)
-            pos (torch.tensor, optional): (B,*,L). Defaults to None for computing positions from 0 to L-1 (only possible for 1-D sequence inputs x B,L,H).
+            pos (torch.tensor, optional): (B,*,L). Defaults to None for computing positions from 0 to L-1
             mask (torch.tensor, optional): (B,*,L). A boolean mask to indicate where positions should not have positional encodings added.
                 Defaults to None for no masking
             **kwargs: ignored. Kept for compatibility.
 
         Returns:
             torch.tensor: x with added sinusoidal embeddings.
         """
-        shp = x.shape
+        shp = list(x.shape)
+        l = shp[-2]
         assert shp[-1] == self.dim
 
         pos_emb = self.default_pos_x(x).to(self.inv_freq) if pos is None else pos
+        shp[-2] = pos_emb.shape[-2]
+
         sinusoid_inp = self.apply_pos_division(pos_emb.unsqueeze(-1) * self.inv_freq)
         pos_emb = (
             torch.stack((sinusoid_inp.sin(), sinusoid_inp.cos()), dim=-1)
             .view(*shp)
             .to(x.dtype)
         )
         if mask is not None:
             pos_emb = pos_emb * mask.unsqueeze(-1)
 
+        if l != shp[-2]:
+            pos_emb = F.pad(pos_emb, (0, 0, l-shp[-2], 0))
+
         return x + pos_emb
 
 
 class LearnedVocab(Base):
     def __init__(self, dim, max_seq_len):
         """Learned vocab as in Devlin et al. (2018)
         Supports specifying positions and masking.
@@ -90,30 +97,35 @@
         """
         super().__init__()
         self.emb = nn.Embedding(max_seq_len, dim)
 
     def mod_x(self, x, pos=None, mask=None, **kwargs):
         """
         Args:
-            x (torch.tensor): (B,*,H)
-            pos (torch.tensor, optional): (B,*). Defaults to None for computing positions from 0 to L-1 (only possible for 1-D sequence inputs x B,L,H).
-            mask (torch.tensor, optional): (B,*). A boolean mask to indicate where positions should not have positional encodings added.
+            x (torch.tensor): (B,*,L,H)
+            pos (torch.tensor, optional): (B,*,L). Defaults to None for computing positions from 0 to L-1
+            mask (torch.tensor, optional): (B,*,L). A boolean mask to indicate where positions should not have positional encodings added.
                 Defaults to None for no masking
             **kwargs: ignored. Kept for compatibility.
 
         Returns:
             torch.tensor: x with added learned embeddings.
         """
-        shp = x.shape
+        shp = list(x.shape)
         assert shp[-1] == self.emb.embedding_dim
         pos = self.default_pos_x(x).long() if pos is None else pos
 
         pos_emb = self.emb(pos)
         if mask is not None:
             pos_emb = pos_emb * mask.unsqueeze(-1)
+
+        l = pos_emb.shape[-2]
+        if l != shp[-2]:
+            pos_emb = F.pad(pos_emb, (0, 0, shp[-2]-l, 0))
+
         return x + pos_emb
 
 
 class LearnedContinuous(Base):
     def __init__(self, dim, depth=3, norm=False, divide=1.0, learned_div=False):
         """Learned embeddings with a continuity between absolute positional indices, as learned by a series of linear layers.
         Supports specifying positions, masking, and division of positional range.
@@ -143,31 +155,37 @@
                     nn.LayerNorm(dim) if norm else nn.Identity(),
                 )
             )
 
     def mod_x(self, x, pos=None, mask=None, **kwargs):
         """
         Args:
-            x (torch.tensor): (B,*,H)
-            pos (torch.tensor, optional): (B,*). Defaults to None for computing positions from 0 to L-1 (only possible for 1-D sequence inputs x B,L,H).
-            mask (torch.tensor, optional): (B,*). A boolean mask to indicate where positions should not have positional encodings added.
+            x (torch.tensor): (B,*,L,H)
+            pos (torch.tensor, optional): (B,*,L). Defaults to None for computing positions from 0 to L-1
+            mask (torch.tensor, optional): (B,*,L). A boolean mask to indicate where positions should not have positional encodings added.
                 Defaults to None for no masking
             **kwargs: ignored. Kept for compatibility.
         Returns:
             torch.tensor: x with added learned embeddings.
         """
+        shp = list(x.shape)
 
         pos = self.default_pos_x(x).to(x) if pos is None else pos
 
         pos_emb = self.apply_pos_division(pos).unsqueeze(-1)
         for layer in self.mlp:
             pos_emb = layer(pos_emb)
 
         if mask is not None:
             pos_emb = pos_emb * mask.unsqueeze(-1)
+
+        l = pos_emb.shape[-2]
+        if l != shp[-2]:
+            pos_emb = F.pad(pos_emb, (0, 0, shp[-2]-l, 0))
+
         return x + pos_emb
 
 
 class Rotary(Base):
     def __init__(self, head_dim, n_dims=None, divide=1.0, learned_div=False):
         """Rotary embedding as in RoFormer / RoPE
         Supports specifying positions and division of positional range.
@@ -198,42 +216,54 @@
         pos_q=None,
         pos_k=None,
         self_attn_mode=True,
         **kwargs,
     ):
         """
         Args:
-            q (torch.tensor): (B,*,NH,H)
-            k (torch.tensor): (B,*,NH,H)
-            v (torch.tensor): (B,*,NH,H)
-            pos_q_k (torch.tensor, optional): (B, L). Positions of q and k in self attention mode. Requires L1 = L2.
-                Defaults to None for computing positions from 0 to L-1 (only possible for 1-D sequence inputs x B,L,H).
-            pos_q (torch.tensor, optional): (B, L1). Positions of q in cross attention mode.
-                Defaults to None for computing positions from 0 to L1-1 (only possible for 1-D sequence inputs x B,L,H).
-            pos_k (torch.tensor, optional): (B, L2). Positions of k in cross attention mode.
-                Defaults to None for computing positions from 0 to L2-1 (only possible for 1-D sequence inputs x B,L,H).
+            q (torch.tensor): (B,*,L1,NH,H)
+            k (torch.tensor): (B,*,L2,NH,H)
+            v (torch.tensor): (B,*,L2,NH,H)
+            pos_q_k (torch.tensor, optional): (B,*,L). Positions of q and k in self attention mode. Requires L1 = L2.
+                Defaults to None for computing positions from 0 to L-1
+            pos_q (torch.tensor, optional): (B,*,L1). Positions of q in cross attention mode.
+                Defaults to None for computing positions from 0 to L1-1
+            pos_k (torch.tensor, optional): (B,*,L2). Positions of k in cross attention mode.
+                Defaults to None for computing positions from 0 to L2-1
             self_attn_mode (bool, optional): Whether to use the same positions for q and k (pos_q_k),
                 or use different positions for each (pos_q) and (pos_k).
                 Defaults to True.
             **kwargs: ignored. Kept for compatibility.
         Returns:
             q, k, v (all torch.tensor)
         """
         if self_attn_mode:
+            assert q.shape[-3] == k.shape[-3]
             pos_q_k = self.default_pos_x(q[..., 0, :]) if pos_q_k is None else pos_q_k
             sin, cos = self.get_rotations(pos_q_k)
 
+            l_sin, l_q = sin.shape[-3], q.shape[-3]
+            if l_sin != l_q:
+                sin, cos = map(lambda t: F.pad(t, (0, 0, 0, 0, l_q-l_sin, 0), (sin, cos)))
+
             q = q * cos.to(q) + self.rotate_every_two(q) * sin.to(q)
             k = k * cos.to(k) + self.rotate_every_two(k) * sin.to(k)
         else:
             pos_q = self.default_pos_x(q[..., 0, :]) if pos_q is None else pos_q
             pos_k = self.default_pos_x(k[..., 0, :]) if pos_k is None else pos_k
             sin_q, cos_q = self.get_rotations(pos_q)
             sin_k, cos_k = self.get_rotations(pos_k)
 
+            l_sin, l_q = sin_q.shape[-3], q.shape[-3]
+            if l_sin != l_q:
+                sin_q, cos_q = map(lambda t: F.pad(t, (0, 0, 0, 0, l_q-l_sin, 0), (sin_q, cos_q)))
+            l_sin, l_k = sin_k.shape[-3], k.shape[-3]
+            if l_sin != l_k:
+                sin_k, cos_k = map(lambda t: F.pad(t, (0, 0, 0, 0, l_k-l_sin, 0), (sin_k, cos_k)))
+
             q = q * cos_q.to(q) + self.rotate_every_two(q) * sin_q.to(q)
             k = k * cos_k.to(k) + self.rotate_every_two(k) * sin_k.to(k)
 
         return q, k, v
 
     def get_rotations(self, pos):
         mthetas = (
@@ -293,25 +323,25 @@
 
         self.div = divide
 
     def mod_mask(self, mask, q, k, v, pos_q_k=None, pos_q=None, pos_k=None, **kwargs):
         """
         Args:
             mask (torch.tensor): B, *, NH, L1, L2, optional, eg B, NH, L1, L2, or for multi-dim: B, S, NH, L1, L2
-            q (torch.tensor): (B,*,NH,H)
-            k (torch.tensor): (B,*,NH,H)
-            v (torch.tensor): (B,*,NH,H)
-            pos_q_k (torch.tensor, optional): (B, *) eg (B, L). Positions of q and k in self attention mode. Requires L1 = L2.
-                Defaults to None for computing positions from 0 to L-1 (only possible for 1-D sequence inputs x B,L,H).
-            pos_q (torch.tensor, optional): (B, *) eg (B, L1). Positions of q in cross attention mode.
+            q (torch.tensor): (B,*,L1,NH,H)
+            k (torch.tensor): (B,*,L2,NH,H)
+            v (torch.tensor): (B,*,L2,NH,H)
+            pos_q_k (torch.tensor, optional): (B, *, L). Positions of q and k in self attention mode. Requires L1 = L2 =L.
+                Defaults to None for computing positions from 0 to L-1.
+            pos_q (torch.tensor, optional): (B, *, L) eg (B, L1). Positions of q in cross attention mode.
                 Ignored if pos_q_k is specified
-                Defaults to None for computing positions from 0 to L1-1 (only possible for 1-D sequence inputs x B,L,H).
-            pos_k (torch.tensor, optional): (B, *) eg (B, L2). Positions of k in cross attention mode.
+                Defaults to None for computing positions from 0 to L1-1.
+            pos_k (torch.tensor, optional): (B, *, L) eg (B, L2). Positions of k in cross attention mode.
                 Ignored if pos_q_k is specified
-                Defaults to None for computing positions from 0 to L2-1 (only possible for 1-D sequence inputs x B,L,H).
+                Defaults to None for computing positions from 0 to L2-1.
             **kwargs: ignored. Kept for compatibility.
         Returns:
             mask (torch.tensor): (B, *, NH, L1, L2)
         """
 
         if pos_q_k is not None:
             pos_q = pos_k = pos_q_k
@@ -323,14 +353,19 @@
         relative_pos = pos_q[..., :, None] - pos_k[..., None, :]
         bias = self.apply_pos_division(relative_pos.unsqueeze(-3) * self.slopes)
 
         if self.asymmetric:
             bias = self.asymmetric_bias(bias)
         bias = torch.abs(bias)
 
+        l1, l2 = q.shape[-3], k.shape[-3]
+        mask_l1, mask_l2 = mask.shape[-2], mask.shape[-1]
+        if (l1 != mask_l1) or (l2 != mask_l2):
+            mask = F.pad(mask, (l2-mask_l2, 0, l1-mask_l1, 0))
+
         return (0 if mask is None else mask) - bias
 
     @staticmethod
     def _get_slopes(heads):
         def get_slopes_power_of_2(n):
             start = 2 ** (-(2 ** -(math.log2(n) - 3)))
             ratio = start
@@ -396,23 +431,23 @@
 
         self.div = divide
 
     def mod_mask(self, mask, q, k, v, pos_q_k=None, pos_q=None, pos_k=None, **kwargs):
         """
         Args:
             mask (torch.tensor): B, *, NH, L1, L2, optional, eg B, NH, L1, L2, or for multi-dim: B, S, NH, L1, L2
-            q (torch.tensor): (B,*,NH,H)
-            k (torch.tensor): (B,*,NH,H)
-            v (torch.tensor): (B,*,NH,H)
-            pos_q_k (torch.tensor, optional): (B, *). Positions of q and k in self attention mode. Requires L1 = L2.
-                Defaults to None for computing positions from 0 to L-1 (only possible for 1-D sequence inputs x B,L,H).
-            pos_q (torch.tensor, optional): (B, *). Positions of q in cross attention mode.
-                Defaults to None for computing positions from 0 to L1-1 (only possible for 1-D sequence inputs x B,L,H).
-            pos_k (torch.tensor, optional): (B, *). Positions of k in cross attention mode.
-                Defaults to None for computing positions from 0 to L2-1 (only possible for 1-D sequence inputs x B,L,H).
+            q (torch.tensor): (B,*,L1,NH,H)
+            k (torch.tensor): (B,*,L2,NH,H)
+            v (torch.tensor): (B,*,L2,NH,H)
+            pos_q_k (torch.tensor, optional): (B, *,L). Positions of q and k in self attention mode. Requires L1 = L2 = L.
+                Defaults to None for computing positions from 0 to L-1
+            pos_q (torch.tensor, optional): (B, *,L1). Positions of q in cross attention mode.
+                Defaults to None for computing positions from 0 to L1-1
+            pos_k (torch.tensor, optional): (B, *,L2). Positions of k in cross attention mode.
+                Defaults to None for computing positions from 0 to L2-1
             **kwargs: ignored. Kept for compatibility.
         Returns:
             mask (torch.tensor): (B, *, NH, L1, L2)
         """
         if pos_q_k is not None:
             pos_q = pos_k = pos_q_k
         elif (pos_q is None) and (pos_k is None):
@@ -423,14 +458,19 @@
             ..., None
         ].to(q)
 
         for layer in self.mlp:
             bias = layer(bias)
         bias = bias.transpose(-1, -2).transpose(-2, -3).to(q)
 
+        l1, l2 = q.shape[-3], k.shape[-3]
+        mask_l1, mask_l2 = mask.shape[-2], mask.shape[-1]
+        if (l1 != mask_l1) or (l2 != mask_l2):
+            mask = F.pad(mask, (l2-mask_l2, 0, l1-mask_l1, 0))
+
         return (0 if mask is None else mask) - bias
 
 
 class XL(Base):
     def __init__(self, dim, n_heads, divide=1, learned_div=False):
         """Relative positional biases as in Transformer-XL (Dai et al 2019)
         Supports specifying positions and division of positional range
@@ -454,34 +494,34 @@
         inv_freq = 1 / (10000 ** (torch.arange(0.0, dim, 2) / dim))
         self.register_buffer("inv_freq", inv_freq)
         self.div = divide
 
     def mod_qkv(self, q, k, v, **kwargs):
         """
         Args:
-            q (torch.tensor): (B,*,NH,H)
-            k (torch.tensor): (B,*,NH,H)
-            v (torch.tensor): (B,*,NH,H)
+            q (torch.tensor): (B,*,L1,NH,H)
+            k (torch.tensor): (B,*,L2,NH,H)
+            v (torch.tensor): (B,*,L2,NH,H)
         Returns:
             q, k, v (all torch.tensor)
         """
         return q + self.bias_r_w, k, v
 
     def mod_mask(self, mask, q, k, v, pos_q_k=None, pos_q=None, pos_k=None, **kwargs):
         """
         Args:
             mask (torch.tensor): B, *, NH, L1, L2, optional, eg B, NH, L1, L2, or for multi-dim: B, S, NH, L1, L2
-            q (torch.tensor): (B,*,NH,H)
-            k (torch.tensor): (B,*,NH,H)
-            v (torch.tensor): (B,*,NH,H)
-            pos_q_k (torch.tensor, optional): (B, *). Positions of q and k in self attention mode. Requires L1 = L2.
+            q (torch.tensor): (B,*,L1,NH,H)
+            k (torch.tensor): (B,*,L2,NH,H)
+            v (torch.tensor): (B,*,L2,NH,H)
+            pos_q_k (torch.tensor, optional): (B, *, L). Positions of q and k in self attention mode. Requires L1 = L2 = L.
                 Defaults to None for computing positions from 0 to L-1.
-            pos_q (torch.tensor, optional): (B, *). Positions of q in cross attention mode.
+            pos_q (torch.tensor, optional): (B, *, L1). Positions of q in cross attention mode.
                 Defaults to None for computing positions from 0 to L1-1
-            pos_k (torch.tensor, optional): (B, *). Positions of k in cross attention mode.
+            pos_k (torch.tensor, optional): (B, *, L2). Positions of k in cross attention mode.
                 Defaults to None for computing positions from 0 to L2-1
             **kwargs: ignored. Kept for compatibility.
         Returns:
             mask (torch.tensor): (B, *, NH, L1, L2)
         """
         if pos_q_k is not None:
             pos_q = pos_k = pos_q_k
@@ -500,14 +540,20 @@
 
         r = rearrange(
             self.embed_lin(pos_emb),
             "... (nh h) -> ... nh h",
             nh=self.n_heads,
             h=q.shape[-1],
         )
+
+        l1, l2 = q.shape[-3], k.shape[-3]
+        r_l1, r_l2 = r.shape[-2], r.shape[-1]
+        if (l1 != r_l1) or (l2 != r_l2):
+            r = F.pad(r, (0, 0, 0, 0, l2-r_l2, 0, l1-r_l1, 0))
+
         q_r = q + self.bias_r_w
         BD = einsum(q_r, r, "... q n h, ... q k n h -> ... n q k")
         return (0 if mask is None else mask) + BD
 
     def _init_bias(self, bias):
         bound = 1 / bias.size(1) ** 0.5
         return nn.init.uniform_(bias, -bound, bound)
```

### Comparing `bio-attention-0.0.3/bio_attention.egg-info/PKG-INFO` & `bio-attention-0.0.4/bio_attention.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-attention
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple implementations of attention modules adapted for the biological data domain
 Home-page: https://github.com/gdewael/bio-attention
 Author: Gaetan De Waele
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -62,10 +62,12 @@
   - [x] Windowed
   - [x] Random
   - [x] Performer
   - [x] Encoder
   - [x] Decoder
   - [ ] Cross
   - [x] Support for multi-dim inputs
+- [ ] Add a warning if non-increasing positional indices are used with a decoder attention
+- [ ] Add docs clarifying that clf tokens are automatically accounted for if no pos is provided for them
 - [ ] Tests
 - [ ] Typing
 - [ ] Docs
```

