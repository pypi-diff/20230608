# Comparing `tmp/irisml-tasks-transformers-0.0.2.tar.gz` & `tmp/irisml-tasks-transformers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-tasks-transformers-0.0.2.tar", last modified: Wed Jun  7 06:18:36 2023, max compression
+gzip compressed data, was "irisml-tasks-transformers-0.0.3.tar", last modified: Wed Jun  7 23:08:10 2023, max compression
```

## Comparing `irisml-tasks-transformers-0.0.2.tar` & `irisml-tasks-transformers-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:18:36.477649 irisml-tasks-transformers-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-07 06:18:36.477649 irisml-tasks-transformers-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:18:36.477649 irisml-tasks-transformers-0.0.2/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:18:36.477649 irisml-tasks-transformers-0.0.2/irisml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/irisml/tasks/cache_transformers_model_on_azure_blob.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/irisml/tasks/create_transformers_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/irisml/tasks/create_transformers_text_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/irisml/tasks/create_transformers_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:18:36.477649 irisml-tasks-transformers-0.0.2/irisml_tasks_transformers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-07 06:18:36.000000 irisml-tasks-transformers-0.0.2/irisml_tasks_transformers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-07 06:18:36.000000 irisml-tasks-transformers-0.0.2/irisml_tasks_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:18:36.000000 irisml-tasks-transformers-0.0.2/irisml_tasks_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-07 06:18:36.000000 irisml-tasks-transformers-0.0.2/irisml_tasks_transformers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 06:18:36.000000 irisml-tasks-transformers-0.0.2/irisml_tasks_transformers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-07 06:18:36.477649 irisml-tasks-transformers-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:18:36.477649 irisml-tasks-transformers-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/test/test_cache_transformers_model_on_azure_blob.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/test/test_create_transformers_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/test/test_create_transformers_text_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-07 06:15:56.000000 irisml-tasks-transformers-0.0.2/test/test_create_transformers_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:08:10.730944 irisml-tasks-transformers-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-07 23:05:38.000000 irisml-tasks-transformers-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-07 23:08:10.730944 irisml-tasks-transformers-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-07 23:05:38.000000 irisml-tasks-transformers-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:08:10.730944 irisml-tasks-transformers-0.0.3/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:08:10.730944 irisml-tasks-transformers-0.0.3/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-07 23:05:38.000000 irisml-tasks-transformers-0.0.3/irisml/tasks/cache_transformers_model_on_azure_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-07 23:05:38.000000 irisml-tasks-transformers-0.0.3/irisml/tasks/create_transformers_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-07 23:05:38.000000 irisml-tasks-transformers-0.0.3/irisml/tasks/create_transformers_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-07 23:05:38.000000 irisml-tasks-transformers-0.0.3/irisml/tasks/create_transformers_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:08:10.730944 irisml-tasks-transformers-0.0.3/irisml_tasks_transformers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-07 23:08:10.000000 irisml-tasks-transformers-0.0.3/irisml_tasks_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-07 23:08:10.000000 irisml-tasks-transformers-0.0.3/irisml_tasks_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 23:08:10.000000 irisml-tasks-transformers-0.0.3/irisml_tasks_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-07 23:08:10.000000 irisml-tasks-transformers-0.0.3/irisml_tasks_transformers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 23:08:10.000000 irisml-tasks-transformers-0.0.3/irisml_tasks_transformers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-07 23:05:38.000000 irisml-tasks-transformers-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-07 23:08:10.730944 irisml-tasks-transformers-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:08:10.730944 irisml-tasks-transformers-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 23:05:38.000000 irisml-tasks-transformers-0.0.3/test/test_cache_transformers_model_on_azure_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-07 23:05:38.000000 irisml-tasks-transformers-0.0.3/test/test_create_transformers_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-07 23:05:38.000000 irisml-tasks-transformers-0.0.3/test/test_create_transformers_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-07 23:05:38.000000 irisml-tasks-transformers-0.0.3/test/test_create_transformers_tokenizer.py
```

### Comparing `irisml-tasks-transformers-0.0.2/LICENSE` & `irisml-tasks-transformers-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-transformers-0.0.2/PKG-INFO` & `irisml-tasks-transformers-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-transformers
-Version: 0.0.2
+Version: 0.0.3
 Summary: IrisML tasks for transformers library
 Home-page: https://github.com/microsoft/irisml-tasks-transformers
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-transformers-0.0.2/README.md` & `irisml-tasks-transformers-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `irisml-tasks-transformers-0.0.2/irisml/tasks/cache_transformers_model_on_azure_blob.py` & `irisml-tasks-transformers-0.0.3/irisml/tasks/cache_transformers_model_on_azure_blob.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-transformers-0.0.2/irisml/tasks/create_transformers_model.py` & `irisml-tasks-transformers-0.0.3/irisml/tasks/create_transformers_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-transformers-0.0.2/irisml/tasks/create_transformers_text_model.py` & `irisml-tasks-transformers-0.0.3/irisml/tasks/create_transformers_text_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,61 +8,61 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Task(irisml.core.TaskBase):
     """Create a text-generation model using transformers library.
 
-    # TODO Add a feature to load from local file.
+    Config:
+        name (str): Name of the model to load. See https://huggingface.co/models for a list of available models.
+        azure_blob_container_url (str): Azure blob container URL to download the model from.
+        azure_blob_path_prefix (str): Azure blob path prefix to download the model from.
     """
-    VERSION = '0.1.0'
+    VERSION = '0.2.0'
 
     @dataclasses.dataclass
     class Config:
         name: str
-        pretrained: bool = False
         azure_blob_container_url: Optional[str] = None
         azure_blob_path_prefix: Optional[str] = None
 
     @dataclasses.dataclass
     class Outputs:
         model: torch.nn.Module
 
     def execute(self, inputs):
         self._check_config()
 
+        if 'blip2' in self.config.name:
+            model_class = transformers.Blip2ForConditionalGeneration
+        else:
+            model_class = transformers.AutoModel
+
         if self.config.azure_blob_container_url:
             prefix = self.config.name if not self.config.azure_blob_path_prefix else f'{self.config.azure_blob_path_prefix}/{self.config.name}'
             with with_azure_directory(self.config.azure_blob_container_url, prefix) as temp_dir:
-                model = transformers.AutoModel.from_pretrained(temp_dir)
+                model = model_class.from_pretrained(temp_dir)
                 processor = transformers.AutoProcessor.from_pretrained(temp_dir)
         else:
+            model = model_class.from_pretrained(self.config.name)
             processor = transformers.AutoProcessor.from_pretrained(self.config.name)
-            if self.config.pretrained:
-                model = transformers.AutoModel.from_pretrained(self.config.name)
-            else:
-                config = transformers.AutoConfig.from_pretrained(self.config.name)
-                model = transformers.AutoModel.from_config(config)
 
         if not isinstance(model, transformers.Blip2PreTrainedModel):
             raise RuntimeError(f"The model type {type(model)} is not supported. Please submit a pull request.")
 
         return self.Outputs(TextGenerationModel(model, processor))
 
     def dry_run(self, inputs):
         self._check_config()
         return self.Outputs(FakeModel())
 
     def _check_config(self):
         if not self.config.name:
             raise ValueError("name is required")
 
-        if self.config.pretrained and self.config.azure_blob_container_url:
-            raise ValueError("pretrained and azure_blob_container_url are mutually exclusive")
-
         if not self.config.azure_blob_container_url and self.config.azure_blob_path_prefix:
             raise ValueError("azure_blob_path_prefix requires azure_blob_container_url")
 
 
 class TextGenerationModel(torch.nn.Module):
     """Model that generates text.
 
@@ -73,21 +73,24 @@
     """
     def __init__(self, model, processor):
         super().__init__()
         self._model = model
         self._processor = processor
         self._dtype = torch.float16
         self._device = torch.device('cpu')
+        self._model.to(self._dtype)
 
     def forward(self, inputs: List[Tuple[str, List[torch.Tensor]]]) -> List[str]:
         results = []
         for text, images in inputs:
             inputs = self._processor(images=torch.stack(images) * 255, text=text, return_tensors='pt', padding=True).to(self._device, self._dtype)
             generated_ids = self._model.generate(**inputs)
-            results.append(self._processor.batch_decode(generated_ids, skip_special_tokens=True))
+            generated_text = self._processor.batch_decode(generated_ids, skip_special_tokens=True)[0].strip()
+            logger.debug(f"Generated text: {repr(generated_text)}")
+            results.append(generated_text)
         return results
 
     def to(self, device, *args, **kwargs):
         if not isinstance(device, torch.device):
             raise NotImplementedError("Only torch.device is supported")
         self._device = device
         return super().to(device, *args, **kwargs)
```

### Comparing `irisml-tasks-transformers-0.0.2/irisml/tasks/create_transformers_tokenizer.py` & `irisml-tasks-transformers-0.0.3/irisml/tasks/create_transformers_tokenizer.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-transformers-0.0.2/irisml_tasks_transformers.egg-info/PKG-INFO` & `irisml-tasks-transformers-0.0.3/irisml_tasks_transformers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-transformers
-Version: 0.0.2
+Version: 0.0.3
 Summary: IrisML tasks for transformers library
 Home-page: https://github.com/microsoft/irisml-tasks-transformers
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-transformers-0.0.2/irisml_tasks_transformers.egg-info/SOURCES.txt` & `irisml-tasks-transformers-0.0.3/irisml_tasks_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irisml-tasks-transformers-0.0.2/setup.cfg` & `irisml-tasks-transformers-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = irisml-tasks-transformers
-version = 0.0.2
+version = 0.0.3
 url = https://github.com/microsoft/irisml-tasks-transformers
 description = IrisML tasks for transformers library
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = irisdev
 license = MIT
```

### Comparing `irisml-tasks-transformers-0.0.2/test/test_cache_transformers_model_on_azure_blob.py` & `irisml-tasks-transformers-0.0.3/test/test_cache_transformers_model_on_azure_blob.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-transformers-0.0.2/test/test_create_transformers_model.py` & `irisml-tasks-transformers-0.0.3/test/test_create_transformers_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-transformers-0.0.2/test/test_create_transformers_text_model.py` & `irisml-tasks-transformers-0.0.3/test/test_create_transformers_text_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-transformers-0.0.2/test/test_create_transformers_tokenizer.py` & `irisml-tasks-transformers-0.0.3/test/test_create_transformers_tokenizer.py`

 * *Files identical despite different names*

