# Comparing `tmp/bio-attention-0.0.4.tar.gz` & `tmp/bio-attention-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-attention-0.0.4.tar", last modified: Thu Jun  8 09:51:50 2023, max compression
+gzip compressed data, was "bio-attention-0.0.5.tar", last modified: Thu Jun  8 11:46:23 2023, max compression
```

## Comparing `bio-attention-0.0.4.tar` & `bio-attention-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:51:50.585416 bio-attention-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:51:50.581416 bio-attention-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:51:50.581416 bio-attention-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 09:51:39.000000 bio-attention-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-08 09:51:39.000000 bio-attention-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-08 09:51:39.000000 bio-attention-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-08 09:51:50.585416 bio-attention-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-08 09:51:39.000000 bio-attention-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:51:50.581416 bio-attention-0.0.4/bio_attention/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:51:39.000000 bio-attention-0.0.4/bio_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-06-08 09:51:39.000000 bio-attention-0.0.4/bio_attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-08 09:51:39.000000 bio-attention-0.0.4/bio_attention/embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:51:50.585416 bio-attention-0.0.4/bio_attention/img/
--rw-r--r--   0 runner    (1001) docker     (123)  2372654 2023-06-08 09:51:39.000000 bio-attention-0.0.4/bio_attention/img/2Dslidingwindow-attention.png
--rw-r--r--   0 runner    (1001) docker     (123)   118589 2023-06-08 09:51:39.000000 bio-attention-0.0.4/bio_attention/img/windowed_implementation.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22849 2023-06-08 09:51:39.000000 bio-attention-0.0.4/bio_attention/positional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:51:50.581416 bio-attention-0.0.4/bio_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-08 09:51:50.000000 bio-attention-0.0.4/bio_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-08 09:51:50.000000 bio-attention-0.0.4/bio_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:51:50.000000 bio-attention-0.0.4/bio_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 09:51:50.000000 bio-attention-0.0.4/bio_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 09:51:50.000000 bio-attention-0.0.4/bio_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-08 09:51:39.000000 bio-attention-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-08 09:51:50.585416 bio-attention-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:46:23.452710 bio-attention-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:46:23.440709 bio-attention-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:46:23.444710 bio-attention-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 11:46:11.000000 bio-attention-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-08 11:46:11.000000 bio-attention-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-08 11:46:11.000000 bio-attention-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-08 11:46:23.452710 bio-attention-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-08 11:46:11.000000 bio-attention-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:46:23.444710 bio-attention-0.0.5/bio_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:46:11.000000 bio-attention-0.0.5/bio_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-06-08 11:46:11.000000 bio-attention-0.0.5/bio_attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-08 11:46:11.000000 bio-attention-0.0.5/bio_attention/embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:46:23.452710 bio-attention-0.0.5/bio_attention/img/
+-rw-r--r--   0 runner    (1001) docker     (123)  2372654 2023-06-08 11:46:11.000000 bio-attention-0.0.5/bio_attention/img/2Dslidingwindow-attention.png
+-rw-r--r--   0 runner    (1001) docker     (123)   118589 2023-06-08 11:46:11.000000 bio-attention-0.0.5/bio_attention/img/windowed_implementation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22849 2023-06-08 11:46:11.000000 bio-attention-0.0.5/bio_attention/positional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:46:23.448710 bio-attention-0.0.5/bio_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-08 11:46:23.000000 bio-attention-0.0.5/bio_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-08 11:46:23.000000 bio-attention-0.0.5/bio_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:46:23.000000 bio-attention-0.0.5/bio_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 11:46:23.000000 bio-attention-0.0.5/bio_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 11:46:23.000000 bio-attention-0.0.5/bio_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-08 11:46:11.000000 bio-attention-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-08 11:46:23.452710 bio-attention-0.0.5/setup.cfg
```

### Comparing `bio-attention-0.0.4/.github/workflows/publish.yml` & `bio-attention-0.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.4/.gitignore` & `bio-attention-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.4/LICENSE` & `bio-attention-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.4/PKG-INFO` & `bio-attention-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-attention
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple implementations of attention modules adapted for the biological data domain
 Home-page: https://github.com/gdewael/bio-attention
 Author: Gaetan De Waele
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bio-attention-0.0.4/README.md` & `bio-attention-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.4/bio_attention/attention.py` & `bio-attention-0.0.5/bio_attention/attention.py`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.4/bio_attention/embed.py` & `bio-attention-0.0.5/bio_attention/embed.py`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.4/bio_attention/img/2Dslidingwindow-attention.png` & `bio-attention-0.0.5/bio_attention/img/2Dslidingwindow-attention.png`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.4/bio_attention/img/windowed_implementation.svg` & `bio-attention-0.0.5/bio_attention/img/windowed_implementation.svg`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.4/bio_attention/positional.py` & `bio-attention-0.0.5/bio_attention/positional.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             torch.tensor: x with added sinusoidal embeddings.
         """
         shp = list(x.shape)
         l = shp[-2]
         assert shp[-1] == self.dim
 
         pos_emb = self.default_pos_x(x).to(self.inv_freq) if pos is None else pos
-        shp[-2] = pos_emb.shape[-2]
+        shp[-2] = pos_emb.shape[-1]
 
         sinusoid_inp = self.apply_pos_division(pos_emb.unsqueeze(-1) * self.inv_freq)
         pos_emb = (
             torch.stack((sinusoid_inp.sin(), sinusoid_inp.cos()), dim=-1)
             .view(*shp)
             .to(x.dtype)
         )
```

### Comparing `bio-attention-0.0.4/bio_attention.egg-info/PKG-INFO` & `bio-attention-0.0.5/bio_attention.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-attention
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple implementations of attention modules adapted for the biological data domain
 Home-page: https://github.com/gdewael/bio-attention
 Author: Gaetan De Waele
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

