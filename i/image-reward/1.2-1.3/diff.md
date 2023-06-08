# Comparing `tmp/image-reward-1.2.tar.gz` & `tmp/image-reward-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image-reward-1.2.tar", last modified: Mon May  1 02:43:28 2023, max compression
+gzip compressed data, was "dist/image-reward-1.3.tar", last modified: Thu Jun  8 02:03:49 2023, max compression
```

## Comparing `image-reward-1.2.tar` & `image-reward-1.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 02:43:28.000000 image-reward-1.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 02:43:28.000000 image-reward-1.2/ImageReward/
--rw-r--r--   0 root         (0) root         (0)     6044 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/ImageReward.py
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 02:43:28.000000 image-reward-1.2/ImageReward/models/
--rw-r--r--   0 root         (0) root         (0)     2614 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/AestheticScore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 02:43:28.000000 image-reward-1.2/ImageReward/models/BLIP/
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/BLIP/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3125 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/BLIP/blip.py
--rw-r--r--   0 root         (0) root         (0)     1502 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/BLIP/blip_pretrain.py
--rw-r--r--   0 root         (0) root         (0)    41498 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/BLIP/med.py
--rw-r--r--   0 root         (0) root         (0)    14061 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/BLIP/vit.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/BLIPScore.py
--rw-r--r--   0 root         (0) root         (0)     2165 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/CLIPScore.py
--rw-r--r--   0 root         (0) root         (0)       99 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5868 2023-05-01 02:33:51.000000 image-reward-1.2/ImageReward/utils.py
--rw-r--r--   0 root         (0) root         (0)    11351 2023-05-01 02:33:51.000000 image-reward-1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7185 2023-05-01 02:43:28.000000 image-reward-1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6876 2023-05-01 02:33:51.000000 image-reward-1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 02:43:28.000000 image-reward-1.2/image_reward.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7185 2023-05-01 02:43:28.000000 image-reward-1.2/image_reward.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      580 2023-05-01 02:43:28.000000 image-reward-1.2/image_reward.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-01 02:43:28.000000 image-reward-1.2/image_reward.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-01 02:43:28.000000 image-reward-1.2/image_reward.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-01 02:43:28.000000 image-reward-1.2/image_reward.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 02:43:28.000000 image-reward-1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      980 2023-05-01 02:42:34.000000 image-reward-1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:03:49.000000 image-reward-1.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:03:49.000000 image-reward-1.3/ImageReward/
+-rw-r--r--   0 root         (0) root         (0)     6969 2023-05-25 09:11:16.000000 image-reward-1.3/ImageReward/ImageReward.py
+-rw-r--r--   0 root         (0) root         (0)    36541 2023-06-07 14:04:32.000000 image-reward-1.3/ImageReward/ReFL.py
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-25 08:38:24.000000 image-reward-1.3/ImageReward/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:03:49.000000 image-reward-1.3/ImageReward/models/
+-rw-r--r--   0 root         (0) root         (0)     3167 2023-05-25 08:52:49.000000 image-reward-1.3/ImageReward/models/AestheticScore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:03:49.000000 image-reward-1.3/ImageReward/models/BLIP/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-25 05:25:59.000000 image-reward-1.3/ImageReward/models/BLIP/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-05-25 13:23:56.000000 image-reward-1.3/ImageReward/models/BLIP/blip.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2023-05-25 05:25:59.000000 image-reward-1.3/ImageReward/models/BLIP/blip_pretrain.py
+-rw-r--r--   0 root         (0) root         (0)    41498 2023-05-25 05:25:59.000000 image-reward-1.3/ImageReward/models/BLIP/med.py
+-rw-r--r--   0 root         (0) root         (0)    14061 2023-05-25 05:25:59.000000 image-reward-1.3/ImageReward/models/BLIP/vit.py
+-rw-r--r--   0 root         (0) root         (0)     3840 2023-05-25 08:53:13.000000 image-reward-1.3/ImageReward/models/BLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-05-25 08:53:34.000000 image-reward-1.3/ImageReward/models/CLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-05-25 05:25:59.000000 image-reward-1.3/ImageReward/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5923 2023-06-07 13:27:42.000000 image-reward-1.3/ImageReward/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11351 2023-05-25 05:25:59.000000 image-reward-1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11883 2023-06-08 02:03:49.000000 image-reward-1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11574 2023-06-07 14:30:23.000000 image-reward-1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:03:49.000000 image-reward-1.3/image_reward.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11883 2023-06-08 02:03:49.000000 image-reward-1.3/image_reward.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-08 02:03:49.000000 image-reward-1.3/image_reward.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-08 02:03:49.000000 image-reward-1.3/image_reward.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-06-08 02:03:49.000000 image-reward-1.3/image_reward.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-08 02:03:49.000000 image-reward-1.3/image_reward.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 02:03:49.000000 image-reward-1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-06-07 14:30:09.000000 image-reward-1.3/setup.py
```

### Comparing `image-reward-1.2/ImageReward/ImageReward.py` & `image-reward-1.3/ImageReward/ImageReward.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,14 +77,33 @@
         self.preprocess = _transform(224)
         self.mlp = MLP(768)
         
         self.mean = 0.16717362830052426
         self.std = 1.0333394966054072
 
 
+    def score_gard(self, prompt_ids, prompt_attention_mask, image):
+
+        image_embeds = self.blip.visual_encoder(image)
+        # text encode cross attention with image
+        image_atts = torch.ones(image_embeds.size()[:-1],dtype=torch.long).to(self.device)
+        text_output = self.blip.text_encoder(prompt_ids,
+                                                    attention_mask = prompt_attention_mask,
+                                                    encoder_hidden_states = image_embeds,
+                                                    encoder_attention_mask = image_atts,
+                                                    return_dict = True,
+                                                )
+        
+        txt_features = text_output.last_hidden_state[:,0,:] # (feature_dim)
+        rewards = self.mlp(txt_features)
+        rewards = (rewards - self.mean) / self.std
+        
+        return rewards
+
+
     def score(self, prompt, image):
         
         if (type(image).__name__=='list'):
             _, rewards = self.inference_rank(prompt, image)
             return rewards
             
         # text encode
```

### Comparing `image-reward-1.2/ImageReward/models/AestheticScore.py` & `image-reward-1.3/ImageReward/models/AestheticScore.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,14 +54,29 @@
             self.clip_model.float()
         else:
             clip.model.convert_weights(self.clip_model) # Actually this line is unnecessary since clip by default already on float16
 
         # have clip.logit_scale require no grad.
         self.clip_model.logit_scale.requires_grad_(False)
         
+    def score(self, prompt, image_path):
+        
+        if (type(image_path).__name__=='list'):
+            _, rewards = self.inference_rank(prompt, image_path)
+            return rewards
+            
+        # image encode
+        pil_image = Image.open(image_path)
+        image = self.preprocess(pil_image).unsqueeze(0).to(self.device)
+        image_features = F.normalize(self.clip_model.encode_image(image)).float()
+        
+        # score
+        rewards = self.mlp(image_features)
+        
+        return rewards.detach().cpu().numpy().item()
 
     def inference_rank(self, prompt, generations_list):
         
         img_set = []
         for generations in generations_list:
             # image encode
             img_path = generations
```

### Comparing `image-reward-1.2/ImageReward/models/BLIP/blip.py` & `image-reward-1.3/ImageReward/models/BLIP/blip.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.2/ImageReward/models/BLIP/blip_pretrain.py` & `image-reward-1.3/ImageReward/models/BLIP/blip_pretrain.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.2/ImageReward/models/BLIP/med.py` & `image-reward-1.3/ImageReward/models/BLIP/med.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.2/ImageReward/models/BLIP/vit.py` & `image-reward-1.3/ImageReward/models/BLIP/vit.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.2/ImageReward/models/BLIPScore.py` & `image-reward-1.3/ImageReward/models/BLIPScore.py`

 * *Files 19% similar despite different names*

```diff
@@ -43,14 +43,37 @@
         super().__init__()
         self.device = device
         
         self.preprocess = _transform(224)
         self.blip = BLIP_Pretrain(image_size=224, vit='large', med_config=med_config)
 
 
+    def score(self, prompt, image_path):
+        
+        if (type(image_path).__name__=='list'):
+            _, rewards = self.inference_rank(prompt, image_path)
+            return rewards
+            
+        # text encode
+        text_input = self.blip.tokenizer(prompt, padding='max_length', truncation=True, max_length=35, return_tensors="pt").to(self.device)
+        text_output = self.blip.text_encoder(text_input.input_ids, attention_mask = text_input.attention_mask, mode='text')  
+        txt_feature = F.normalize(self.blip.text_proj(text_output.last_hidden_state[:,0,:]))
+        
+        # image encode
+        pil_image = Image.open(image_path)
+        image = self.preprocess(pil_image).unsqueeze(0).to(self.device)
+        image_embeds = self.blip.visual_encoder(image)
+        image_features = F.normalize(self.blip.vision_proj(image_embeds[:,0,:]), dim=-1)    
+        
+        # score
+        rewards = torch.sum(torch.mul(txt_feature, image_features), dim=1, keepdim=True)
+        
+        return rewards.detach().cpu().numpy().item()
+
+
     def inference_rank(self, prompt, generations_list):
     
         text_input = self.blip.tokenizer(prompt, padding='max_length', truncation=True, max_length=35, return_tensors="pt").to(self.device)
         text_output = self.blip.text_encoder(text_input.input_ids, attention_mask = text_input.attention_mask, mode='text')  
         txt_feature = F.normalize(self.blip.text_proj(text_output.last_hidden_state[:,0,:]))
         
         txt_set = []
```

### Comparing `image-reward-1.2/ImageReward/models/CLIPScore.py` & `image-reward-1.3/ImageReward/models/CLIPScore.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,35 @@
         else:
             clip.model.convert_weights(self.clip_model) # Actually this line is unnecessary since clip by default already on float16
 
         # have clip.logit_scale require no grad.
         self.clip_model.logit_scale.requires_grad_(False)
 
 
+    def score(self, prompt, image_path):
+        
+        if (type(image_path).__name__=='list'):
+            _, rewards = self.inference_rank(prompt, image_path)
+            return rewards
+            
+        # text encode
+        text = clip.tokenize(prompt, truncate=True).to(self.device)
+        txt_features = F.normalize(self.clip_model.encode_text(text))
+        
+        # image encode
+        pil_image = Image.open(image_path)
+        image = self.preprocess(pil_image).unsqueeze(0).to(self.device)
+        image_features = F.normalize(self.clip_model.encode_image(image))
+        
+        # score
+        rewards = torch.sum(torch.mul(txt_features, image_features), dim=1, keepdim=True)
+        
+        return rewards.detach().cpu().numpy().item()
+
+
     def inference_rank(self, prompt, generations_list):
         
         text = clip.tokenize(prompt, truncate=True).to(self.device)
         txt_feature = F.normalize(self.clip_model.encode_text(text))
         
         txt_set = []
         img_set = []
```

### Comparing `image-reward-1.2/ImageReward/utils.py` & `image-reward-1.3/ImageReward/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     os.makedirs(root, exist_ok=True)
     filename = os.path.basename(url)
     download_target = os.path.join(root, filename)
     hf_hub_download(repo_id="THUDM/ImageReward", filename=filename, local_dir=root)
     return download_target
 
 
-def load(name: str = "ImageReward-v1.0", device: Union[str, torch.device] = "cuda" if torch.cuda.is_available() else "cpu", download_root: str = None):
+def load(name: str = "ImageReward-v1.0", device: Union[str, torch.device] = "cuda" if torch.cuda.is_available() else "cpu", download_root: str = None, med_config: str = None):
     """Load a ImageReward model
 
     Parameters
     ----------
     name : str
         A model name listed by `ImageReward.available_models()`, or the path to a model checkpoint containing the state_dict
 
@@ -68,15 +68,16 @@
     else:
         raise RuntimeError(f"Model {name} not found; available models = {available_models()}")
 
     print('load checkpoint from %s'%model_path)
     state_dict = torch.load(model_path, map_location='cpu')
     
     # med_config
-    med_config = ImageReward_download("https://huggingface.co/THUDM/ImageReward/blob/main/med_config.json", download_root or os.path.expanduser("~/.cache/ImageReward"))
+    if med_config is None:
+        med_config = ImageReward_download("https://huggingface.co/THUDM/ImageReward/blob/main/med_config.json", download_root or os.path.expanduser("~/.cache/ImageReward"))
     
     model = ImageReward(device=device, med_config=med_config).to(device)
     msg = model.load_state_dict(state_dict,strict=False)
     print("checkpoint loaded")
     model.eval()
 
     return model
```

### Comparing `image-reward-1.2/LICENSE` & `image-reward-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `image-reward-1.2/image_reward.egg-info/SOURCES.txt` & `image-reward-1.3/image_reward.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 ImageReward/ImageReward.py
+ImageReward/ReFL.py
 ImageReward/__init__.py
 ImageReward/utils.py
 ImageReward/models/AestheticScore.py
 ImageReward/models/BLIPScore.py
 ImageReward/models/CLIPScore.py
 ImageReward/models/__init__.py
 ImageReward/models/BLIP/__init__.py
```

### Comparing `image-reward-1.2/setup.py` & `image-reward-1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,27 +6,30 @@
 long_description = (Path(__file__).parent / "README.md").read_text()
 DESCRIPTION = 'ImageReward'
 
 # 配置
 setup(
         name="image-reward", 
         py_modules = ["ImageReward"],
-        version="1.2",
+        version="1.3",
         author="Jiazheng Xu, et al.",
         author_email="<xjz22@mails.tsinghua.edu.cn>",
         url="https://github.com/THUDM/ImageReward",
         description=DESCRIPTION,
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=find_packages(exclude=["tests*"]),
         install_requires=[
             'timm==0.6.13',
             'transformers==4.27.4',
             'fairscale==0.4.13',
             'huggingface_hub==0.13.4',
+            'diffusers==0.16.0',
+            'accelerate==0.16.0',
+            'datasets==2.11.0',
         ],
         dependency_links = [
             "clip @ git+https://github.com/openai/CLIP.git",
         ],
         python_requires=">=3.5",
         license="Apache 2.0 license"
 )
```

