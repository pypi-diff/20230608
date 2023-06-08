# Comparing `tmp/finetuner-0.7.7.tar.gz` & `tmp/finetuner-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finetuner-0.7.7.tar", last modified: Wed May 24 07:37:52 2023, max compression
+gzip compressed data, was "finetuner-0.7.8.tar", last modified: Thu Jun  8 13:51:59 2023, max compression
```

## Comparing `finetuner-0.7.7.tar` & `finetuner-0.7.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:37:52.469937 finetuner-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-05-24 07:37:44.000000 finetuner-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 07:37:44.000000 finetuner-0.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-05-24 07:37:52.469937 finetuner-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-05-24 07:37:44.000000 finetuner-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:37:52.465937 finetuner-0.7.7/finetuner/
--rw-r--r--   0 runner    (1001) docker     (123)    26507 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:37:52.469937 finetuner-0.7.7/finetuner/client/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/excepts.py
--rw-r--r--   0 runner    (1001) docker     (123)    14355 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/finetuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/hubble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-05-24 07:37:44.000000 finetuner-0.7.7/finetuner/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:37:52.465937 finetuner-0.7.7/finetuner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-05-24 07:37:52.000000 finetuner-0.7.7/finetuner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-24 07:37:52.000000 finetuner-0.7.7/finetuner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:37:52.000000 finetuner-0.7.7/finetuner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:37:52.000000 finetuner-0.7.7/finetuner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-24 07:37:52.000000 finetuner-0.7.7/finetuner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 07:37:52.000000 finetuner-0.7.7/finetuner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-24 07:37:44.000000 finetuner-0.7.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-24 07:37:52.469937 finetuner-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-24 07:37:44.000000 finetuner-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:51:59.280786 finetuner-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-06-08 13:51:50.000000 finetuner-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-08 13:51:50.000000 finetuner-0.7.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-06-08 13:51:59.280786 finetuner-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-06-08 13:51:50.000000 finetuner-0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:51:59.280786 finetuner-0.7.8/finetuner/
+-rw-r--r--   0 runner    (1001) docker     (123)    27892 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:51:59.280786 finetuner-0.7.8/finetuner/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/excepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12521 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/finetuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/hubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-08 13:51:50.000000 finetuner-0.7.8/finetuner/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:51:59.280786 finetuner-0.7.8/finetuner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-06-08 13:51:58.000000 finetuner-0.7.8/finetuner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-08 13:51:59.000000 finetuner-0.7.8/finetuner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:51:58.000000 finetuner-0.7.8/finetuner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:51:58.000000 finetuner-0.7.8/finetuner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-08 13:51:58.000000 finetuner-0.7.8/finetuner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 13:51:58.000000 finetuner-0.7.8/finetuner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-08 13:51:50.000000 finetuner-0.7.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-08 13:51:59.280786 finetuner-0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-08 13:51:50.000000 finetuner-0.7.8/setup.py
```

### Comparing `finetuner-0.7.7/LICENSE` & `finetuner-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.7/PKG-INFO` & `finetuner-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuner
-Version: 0.7.7
+Version: 0.7.8
 Summary: Task-oriented finetuning for better embeddings on neural search.
 Home-page: https://github.com/jina-ai/finetuner/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finetuner Version: 0.7.7 Summary: Task-oriented
+Metadata-Version: 2.1 Name: finetuner Version: 0.7.8 Summary: Task-oriented
 finetuning for better embeddings on neural search. Home-page: https://
 github.com/jina-ai/finetuner/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai Project-URL: Source,
 https://github.com/jina-ai/finetuner/ Project-URL: Tracker, https://github.com/
 jina-ai/finetuner/issues Description:
```

### Comparing `finetuner-0.7.7/README.md` & `finetuner-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.7/finetuner/__init__.py` & `finetuner-0.7.8/finetuner/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inspect
 import os
 import warnings
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, TextIO, Union
+from urllib.parse import urlparse
 
 from _finetuner.runner.stubs import model as model_stub
 from docarray import Document, DocumentArray  # noqa F401
 
 from finetuner.constants import (
     DEFAULT_FINETUNER_HOST,
     DEFAULT_HUBBLE_REGISTRY,
@@ -21,14 +22,15 @@
     os.environ[HOST] = DEFAULT_FINETUNER_HOST
 
 if HUBBLE_REGISTRY not in os.environ:
     os.environ[HUBBLE_REGISTRY] = DEFAULT_HUBBLE_REGISTRY
 
 from finetuner import callback, model
 from finetuner.console import print_model_table
+from finetuner.constants import HF_ORG_PREFIX, HF_URL_PREFIX
 from finetuner.data import build_encoding_dataset
 from finetuner.experiment import Experiment
 from finetuner.finetuner import Finetuner
 from finetuner.model import list_model_classes
 
 if TYPE_CHECKING:
     import numpy as np
@@ -277,15 +279,15 @@
 
 
 @login_required
 def synthesize(
     query_data: Union[str, List[str], DocumentArray],
     corpus_data: Union[str, List[str], DocumentArray],
     models: SynthesisModels,
-    num_relations: int = 3,
+    num_relations: int = 10,
     run_name: Optional[str] = None,
     description: Optional[str] = None,
     experiment_name: Optional[str] = None,
     device: str = 'cuda',
     num_workers: int = 4,
     csv_options: Optional[CSVOptions] = None,
     public: bool = False,
@@ -513,32 +515,56 @@
         return ONNXRuntimeInferenceEngine(
             artifact=model,
             batch_size=batch_size,
             device=device,
         )
 
 
+def _download_huggingface_model(model_name: str, token: Optional[str] = None) -> str:
+    """Download a model from the HuggingFace Hub.
+
+    :param model_name: Either a URL or a model identifier from the HuggingFace Hub.
+    :param token: Optional token to access private models.
+    :return: The local path to the downloaded model.
+    """
+    from huggingface_hub import hf_hub_download, list_repo_files
+
+    repo_id = urlparse(model_name).path
+    if repo_id.startswith('/'):
+        repo_id = repo_id[1:]
+    filenames = list_repo_files(
+        repo_id=repo_id, repo_type='model', use_auth_token=token
+    )
+    for fname in filenames:
+        dest_filename = hf_hub_download(
+            repo_id=repo_id, filename=fname, repo_type='model', use_auth_token=token
+        )
+    local_dir_path = dest_filename[: -len(filenames[-1])]
+    return local_dir_path
+
+
 def get_model(
     artifact: str,
     token: Optional[str] = None,
     batch_size: int = 32,
     select_model: Optional[str] = None,
     device: Optional[str] = None,
     logging_level: str = 'WARNING',
     is_onnx: bool = False,
 ) -> 'InferenceEngine':
     """Re-build the model based on the model inference session with ONNX.
 
     :param artifact: Specify a finetuner run artifact. Can be a path to a local
-        directory, a path to a local zip file, or a Hubble artifact ID. Individual
-        model artifacts (model sub-folders inside the run artifacts) can also be
-        specified using this argument.
-    :param token: A Jina authentication token required for pulling artifacts from
-        Hubble. If not provided, the Hubble client will try to find one either in a
-        local cache folder or in the environment.
+        directory, a path to a local zip file, a Hubble artifact ID, or a huggingface
+        model created with finetuner. Individual model artifacts (model sub-folders
+        inside the run artifacts) can also be specified using this argument.
+    :param token: A Jina authentication token (required for pulling artifacts from
+        Hubble) or a HuggingFace authentication token (required only when downloading
+        private models from huggingface). If not provided, the Hubble client might try
+        to find one either in a local cache folder or in the environment.
     :param batch_size: Incoming documents are fed to the graph in batches, both to
         speed-up inference and avoid memory errors. This argument controls the
         number of documents that will be put in each batch.
     :param select_model: Finetuner run artifacts might contain multiple models. In
         such cases you can select which model to deploy using this argument. For CLIP
         fine-tuning, you can choose either `clip-vision` or `clip-text`.
     :param device: Whether to use the CPU, if set to `cuda`, a Nvidia GPU will be used.
@@ -564,14 +590,20 @@
 
     if device == 'cuda' and is_onnx:
         warnings.warn(
             message='You are using cuda device for ONNX inference, please consider'
             'calling `pip install onnxruntime-gpu` to speed up inference.',
             category=RuntimeWarning,
         )
+
+    if artifact.startswith(HF_URL_PREFIX) or artifact.startswith(HF_ORG_PREFIX):
+        artifact = _download_huggingface_model(artifact, token=token)
+        token = None  # hf token is not needed for local models and can not be used for
+        # inference engine
+
     if is_onnx:
         inference_engine = ONNXRuntimeInferenceEngine(
             artifact=artifact,
             token=token,
             batch_size=batch_size,
             select_model=select_model,
             device=device,
```

### Comparing `finetuner-0.7.7/finetuner/client/base.py` & `finetuner-0.7.8/finetuner/client/base.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.7/finetuner/client/client.py` & `finetuner-0.7.8/finetuner/client/client.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.7/finetuner/client/session.py` & `finetuner-0.7.8/finetuner/client/session.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.7/finetuner/console.py` & `finetuner-0.7.8/finetuner/console.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.7/finetuner/constants.py` & `finetuner-0.7.8/finetuner/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -90,7 +90,9 @@
 CROSS_ENCODER = 'cross_encoder'
 QUERIES = 'queries'
 CORPUS = 'corpus'
 MODELS = 'models'
 NUM_RELATIONS = 'num_relations'
 TRAIN_DATA = 'train_data'
 MAX_NUM_DOCS = 'max_num_docs'
+HF_URL_PREFIX = 'https://huggingface.co/jinaai/'
+HF_ORG_PREFIX = 'jinaai/'
```

### Comparing `finetuner-0.7.7/finetuner/data.py` & `finetuner-0.7.8/finetuner/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
         task: str,
         options: Optional[CSVOptions] = None,
     ):
         super().__init__(file, task, options)
 
     def parse(self):
         with self._file_ctx as fp:
-
             lines = csv.reader(fp, dialect=self._options.dialect)
 
             for columns in _subsample(
                 lines, self._options.size, self._options.sampling_rate
             ):
                 col1, col2 = columns
                 modality_col1, modality_col2 = check_columns(self._task, col1, col2)
@@ -121,15 +120,14 @@
         task: str,
         options: Optional[CSVOptions] = None,
     ):
         super().__init__(file, task, options)
 
     def parse(self):
         with self._file_ctx as fp:
-
             queries = {}
             artificial_label = 0
             modality_col1, modality_col2 = None, None
             lines = csv.reader(fp, dialect=self._options.dialect)
 
             for columns in _subsample(
                 lines, self._options.size, self._options.sampling_rate
@@ -193,15 +191,14 @@
         task: str,
         options: Optional[CSVOptions] = None,
     ):
         super().__init__(file, task, options)
 
     def parse(self):
         with self._file_ctx as fp:
-
             lines = csv.reader(fp, dialect=self._options.dialect)
 
             for columns in _subsample(
                 lines, self._options.size, self._options.sampling_rate
             ):
                 col1, col2, col3 = columns
                 modality_col1, modality_col2 = check_columns(self._task, col1, col2)
```

### Comparing `finetuner-0.7.7/finetuner/experiment.py` & `finetuner-0.7.8/finetuner/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -225,36 +225,36 @@
         return run
 
     def create_synthesis_run(
         self,
         query_data: Union[str, List[str], DocumentArray],
         corpus_data: Union[str, List[str], DocumentArray],
         models: SynthesisModels,
-        num_relations: int = 3,
+        num_relations: int = 10,
         run_name: Optional[str] = None,
         csv_options: Optional[CSVOptions] = None,
         **kwargs,
     ) -> Run:
         """Create a :class:`Run` inside the :class:`Experiment` with the
         task of 'generation' (data synthesis).
         """
         if not run_name:
             run_name = get_random_name()
 
         csv_context = CSVContext(None, options=csv_options)
-        query_data = (
-            csv_context.build_dataset(data=query_data)
-            if isinstance(query_data, str)
-            else DocumentArray([Document(text=data) for data in query_data])
-        )
-        corpus_data = (
-            csv_context.build_dataset(data=corpus_data)
-            if isinstance(query_data, str)
-            else DocumentArray([Document(text=data) for data in corpus_data])
-        )
+        if isinstance(query_data, str):
+            query_data = csv_context.build_dataset(data=query_data)
+        elif isinstance(query_data, list):
+            query_data = DocumentArray([Document(text=data) for data in query_data])
+
+        if isinstance(corpus_data, str):
+            corpus_data = csv_context.build_dataset(data=corpus_data)
+        elif isinstance(corpus_data, list):
+            corpus_data = DocumentArray([Document(text=data) for data in corpus_data])
+
         query_data, corpus_data = push_synthesis_data(
             experiment_name=self._name,
             run_name=run_name,
             query_data=query_data,
             corpus_data=corpus_data,
         )
```

### Comparing `finetuner-0.7.7/finetuner/finetuner.py` & `finetuner-0.7.8/finetuner/finetuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
 
     @login_required
     def create_synthesis_run(
         self,
         query_data: Union[str, List[str], DocumentArray],
         corpus_data: Union[str, List[str], DocumentArray],
         models: SynthesisModels,
-        num_relations: int = 3,
+        num_relations: int = 10,
         run_name: Optional[str] = None,
         description: Optional[str] = None,
         experiment_name: Optional[str] = None,
         device: str = 'cuda',
         num_workers: int = 4,
         csv_options: Optional[CSVOptions] = None,
         public: bool = False,
```

### Comparing `finetuner-0.7.7/finetuner/hubble.py` & `finetuner-0.7.8/finetuner/hubble.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.7/finetuner/model.py` & `finetuner-0.7.8/finetuner/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,7 +49,12 @@
     cross_encoder: str
 
 
 synthesis_model_en = SynthesisModels(
     relation_miner='sbert-base-en',
     cross_encoder='crossencoder-base-en',
 )
+
+synthesis_model_multi = SynthesisModels(
+    relation_miner='distiluse-base-multi',
+    cross_encoder='crossencoder-base-ml',
+)
```

### Comparing `finetuner-0.7.7/finetuner/names.py` & `finetuner-0.7.8/finetuner/names.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.7/finetuner/run.py` & `finetuner-0.7.8/finetuner/run.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.7/finetuner.egg-info/PKG-INFO` & `finetuner-0.7.8/finetuner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuner
-Version: 0.7.7
+Version: 0.7.8
 Summary: Task-oriented finetuning for better embeddings on neural search.
 Home-page: https://github.com/jina-ai/finetuner/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finetuner Version: 0.7.7 Summary: Task-oriented
+Metadata-Version: 2.1 Name: finetuner Version: 0.7.8 Summary: Task-oriented
 finetuning for better embeddings on neural search. Home-page: https://
 github.com/jina-ai/finetuner/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai Project-URL: Source,
 https://github.com/jina-ai/finetuner/ Project-URL: Tracker, https://github.com/
 jina-ai/finetuner/issues Description:
```

### Comparing `finetuner-0.7.7/finetuner.egg-info/SOURCES.txt` & `finetuner-0.7.8/finetuner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.7/setup.py` & `finetuner-0.7.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,25 +25,25 @@
         long_description=_long_description,
         long_description_content_type='text/markdown',
         zip_safe=False,
         setup_requires=['setuptools>=18.0', 'wheel'],
         install_requires=[
             'docarray[common]<0.30.0',
             'trimesh==3.16.4',
-            'finetuner-stubs==0.13.6',
+            'finetuner-stubs==0.13.7',
             'jina-hubble-sdk==0.33.1',
         ],
         extras_require={
             'full': [
-                'finetuner-commons==0.13.6',
+                'finetuner-commons==0.13.7',
             ],
             'test': [
-                'black==22.3.0',
-                'flake8==5.0.4',
-                'isort==5.10.1',
+                'black==23.3.0',
+                'flake8==6.0.0',
+                'isort==5.12.0',
                 'pytest==7.0.0',
                 'pytest-cov==3.0.0',
                 'pytest-mock==3.7.0',
             ],
         },
         python_requires='>=3.8.0',
         classifiers=[
```

