# Comparing `tmp/openlayer-0.0.0a9.tar.gz` & `tmp/openlayer-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlayer-0.0.0a9.tar", last modified: Wed Mar  8 09:24:27 2023, max compression
+gzip compressed data, was "openlayer-0.1.0a0.tar", last modified: Thu Jun  8 05:37:50 2023, max compression
```

## Comparing `openlayer-0.0.0a9.tar` & `openlayer-0.1.0a0.tar`

### file list

```diff
@@ -1,27 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 09:24:27.829157 openlayer-0.0.0a9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-08 09:24:27.829157 openlayer-0.0.0a9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 09:24:27.825157 openlayer-0.0.0a9/openlayer/
--rw-r--r--   0 runner    (1001) docker     (123)    48105 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    54794 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/openlayer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 09:24:27.829157 openlayer-0.0.0a9/openlayer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-08 09:24:27.000000 openlayer-0.0.0a9/openlayer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-08 09:24:27.000000 openlayer-0.0.0a9/openlayer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 09:24:27.000000 openlayer-0.0.0a9/openlayer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 09:24:27.000000 openlayer-0.0.0a9/openlayer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-08 09:24:27.000000 openlayer-0.0.0a9/openlayer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-08 09:24:27.000000 openlayer-0.0.0a9/openlayer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-08 09:24:27.829157 openlayer-0.0.0a9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-08 09:23:49.000000 openlayer-0.0.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:37:50.221126 openlayer-0.1.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-08 05:37:50.221126 openlayer-0.1.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:37:50.217126 openlayer-0.1.0a0/openlayer/
+-rw-r--r--   0 runner    (1001) docker     (123)    53715 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:37:50.217126 openlayer-0.1.0a0/openlayer/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/validators/base_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/validators/baseline_model_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25443 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/validators/commit_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27173 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/validators/dataset_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/validators/model_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/validators/project_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/openlayer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:37:50.217126 openlayer-0.1.0a0/openlayer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-08 05:37:50.000000 openlayer-0.1.0a0/openlayer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-08 05:37:50.000000 openlayer-0.1.0a0/openlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:37:50.000000 openlayer-0.1.0a0/openlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:37:50.000000 openlayer-0.1.0a0/openlayer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-08 05:37:50.000000 openlayer-0.1.0a0/openlayer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 05:37:50.000000 openlayer-0.1.0a0/openlayer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-08 05:37:50.221126 openlayer-0.1.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:37:50.221126 openlayer-0.1.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-08 05:37:06.000000 openlayer-0.1.0a0/tests/test_openlayer.py
```

### Comparing `openlayer-0.0.0a9/LICENSE` & `openlayer-0.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `openlayer-0.0.0a9/PKG-INFO` & `openlayer-0.1.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlayer
-Version: 0.0.0a9
+Version: 0.1.0a0
 Summary: The official Python API library for Openlayer: the Testing and Debugging Platform for AI
 Home-page: https://github.com/openlayer-ai/openlayer-python
 Author: Unbox Inc.
 Project-URL: Documentation, https://docs.openlayer.com/
 Project-URL: Openlayer User Slack Group, https://l.linklyhq.com/l/1DG73
 Keywords: MLOps,AI,Openlayer
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: <=3.9,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="left">
   <img src="docs/source/_static/logo-purple-text.svg"><br>
 </div>
```

### Comparing `openlayer-0.0.0a9/README.md` & `openlayer-0.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `openlayer-0.0.0a9/openlayer/__init__.py` & `openlayer-0.1.0a0/openlayer/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,54 @@
+"""
+Openlayer Python SDK.
+
+Defines the core OpenlayerClient class that users can use to interact
+with the Openlayer platform.
+
+Typical usage example:
+
+    import openlayer
+
+    client = openlayer.OpenlayerClient("YOUR_API_KEY")
+    project = client.create_project("My Project")
+    project.add_dataframe(
+        dataset_df=training_set,
+        dataset_config_file_path="training_dataset_config.yaml",
+    )
+    project.add_dataframe(
+        dataset_df=validation_set,
+        dataset_config_file_path="validation_dataset_config.yaml",
+    )
+    project.status()
+    project.push()
+"""
 import os
 import shutil
 import tarfile
 import tempfile
 import time
 import uuid
-from typing import List, Optional
+from typing import Optional
 
 import pandas as pd
 import yaml
 
-from . import api, exceptions, utils, validators
+from . import api, exceptions, utils
 from .projects import Project
 from .schemas import BaselineModelSchema, DatasetSchema, ModelSchema
 from .tasks import TaskType
+
+# from validators import models as model_validators
+from .validators import (
+    baseline_model_validators,
+    commit_validators,
+    dataset_validators,
+    model_validators,
+    project_validators,
+)
 from .version import __version__  # noqa: F401
 
 OPENLAYER_DIR = os.path.join(os.path.expanduser("~"), ".openlayer")
 VALID_RESOURCE_NAMES = {"model", "training", "validation"}
 
 
 class OpenlayerClient(object):
@@ -87,25 +119,31 @@
         """
         # Validate project
         project_config = {
             "name": name,
             "description": description,
             "task_type": task_type,
         }
-        project_validator = validators.ProjectValidator(project_config=project_config)
+        project_validator = project_validators.ProjectValidator(
+            project_config=project_config
+        )
         failed_validations = project_validator.validate()
 
         if failed_validations:
             raise exceptions.OpenlayerValidationError(
                 "There are issues with the project. \n"
                 "Make sure to fix all of the issues listed above before creating it.",
             ) from None
 
         endpoint = "projects"
-        payload = dict(name=name, description=description, taskType=task_type.value)
+        payload = {
+            "name": name,
+            "description": description,
+            "taskType": task_type.value,
+        }
         project_data = self.api.post_request(endpoint, body=payload)
 
         project = Project(project_data, self.api.upload, self)
 
         # Check if the staging area exists
         project_dir = os.path.join(OPENLAYER_DIR, f"{project.id}/staging")
         os.makedirs(project_dir)
@@ -212,14 +250,15 @@
             return self.create_project(
                 name=name, task_type=task_type, description=description
             )
 
     def add_model(
         self,
         model_config_file_path: str,
+        task_type: TaskType,
         model_package_dir: Optional[str] = None,
         sample_data: Optional[pd.DataFrame] = None,
         force: bool = False,
         project_id: str = None,
     ):
         """Adds a model to a project's staging area.
 
@@ -228,30 +267,37 @@
         model_config_file_path : str
             Path to the model configuration YAML file.
 
             .. admonition:: What's on the model config file?
 
                 The model configuration YAML file must contain the following fields:
 
-                - ``name`` : str
+                name : str
                     Name of the model.
-                - ``architectureType`` : str
+                architectureType : str
                     The model's framework. Must be one of the supported frameworks
                     on :obj:`ModelType`.
-                - ``classNames`` : List[str]
+                classNames : List[str]
                     List of class names corresponding to the outputs of your predict function.
                     E.g. ``['positive', 'negative']``.
-                - ``featureNames`` : List[str], default []
+                featureNames : List[str], default []
                     List of input feature names. Only applicable if your ``task_type`` is
                     :obj:`TaskType.TabularClassification` or :obj:`TaskType.TabularRegression`.
-                - ``categoricalFeatureNames`` : List[str], default []
+                categoricalFeatureNames : List[str], default []
                     A list containing the names of all categorical features used by the model.
                     E.g. ``["Gender", "Geography"]``. Only applicable if your ``task_type`` is
                     :obj:`TaskType.TabularClassification` or :obj:`TaskType.TabularRegression`.
-                - ``metadata`` : Dict[str, any], default {}
+                predictionThreshold : float, default None
+                    The threshold used to determine the predicted class. Only applicable if you
+                    are using a binary classifier and you provided the ``predictionScoresColumnName``
+                    with the lists of class probabilities in your datasets (refer to :obj:`add_dataframe`).
+
+                    If you provided ``predictionScoresColumnName`` but not ``predictionThreshold``,
+                    the predicted class is defined by the argmax of the lists in ``predictionScoresColumnName``.
+                metadata : Dict[str, any], default {}
                     Dictionary containing metadata about the model. This is the metadata that
                     will be displayed on the Openlayer platform.
 
 
         model_package_dir : str, default None
             Path to the directory containing the model package. **Only needed if you are
             interested in adding the model's artifacts.**
@@ -259,16 +305,16 @@
             .. admonition:: What's inside `model_package_dir`?
 
                 The model package directory must contain the following files:
 
                 - ``prediction_interface.py``
                     The prediction interface file.
                 - ``model artifacts``
-                    The model artifacts. This can be a single file or a directory containing
-                    multiple files. The model artifacts must be compatible with the
+                    The model artifacts. This can be a single file, multiple files or a directory.
+                    The model artifacts must be compatible with the
                     prediction interface file.
                 - ``requirements.txt``
                     The requirements file. This file contains the dependencies needed to run
                     the prediction interface file.
 
                 For instructions on how to create a model package, refer to
                 the documentation.
@@ -385,30 +431,31 @@
             elif len(sample_data) < 2:
                 raise ValueError(
                     "The sample data must contain at least 2 rows, but only"
                     f"{len(sample_data)} rows were provided."
                 )
 
         # Validate model package
-        model_package_validator = validators.ModelValidator(
+        model_validator = model_validators.get_validator(
+            task_type=task_type,
             model_package_dir=model_package_dir,
             model_config_file_path=model_config_file_path,
             sample_data=sample_data,
         )
-        failed_validations = model_package_validator.validate()
+        failed_validations = model_validator.validate()
 
         if failed_validations:
             raise exceptions.OpenlayerValidationError(
                 "There are issues with the model package. \n"
                 "Make sure to fix all of the issues listed above before the upload.",
             ) from None
 
         # Load model config and augment with defaults
         model_config = utils.read_yaml(model_config_file_path)
-        model_data = ModelSchema().load(model_config)
+        model_data = ModelSchema().load({"task_type": task_type.value, **model_config})
 
         # Copy relevant resources to temp directory
         with tempfile.TemporaryDirectory() as temp_dir:
             if model_package_dir:
                 shutil.copytree(model_package_dir, temp_dir, dirs_exist_ok=True)
                 utils.write_python_version(temp_dir)
                 model_data["modelType"] = "full"
@@ -463,15 +510,17 @@
         """
         if task_type is not TaskType.TabularClassification:
             raise exceptions.OpenlayerException(
                 "Only tabular classification is supported for model baseline for now."
             )
 
         # Validate the baseline model
-        baseline_model_validator = validators.BaselineModelValidator(
+
+        baseline_model_validator = baseline_model_validators.get_validator(
+            task_type=task_type,
             model_config_file_path=model_config_file_path,
         )
         failed_validations = baseline_model_validator.validate()
 
         if failed_validations:
             raise exceptions.OpenlayerValidationError(
                 "There are issues with the baseline model. \n"
@@ -479,15 +528,17 @@
             ) from None
 
         # Load model config and augment with defaults
         model_config = {}
         if model_config_file_path is not None:
             model_config = utils.read_yaml(model_config_file_path)
         model_config["modelType"] = "baseline"
-        model_data = BaselineModelSchema().load(model_config)
+        model_data = BaselineModelSchema().load(
+            {"task_type": task_type.value, **model_config}
+        )
 
         # Copy relevant resources to temp directory
         with tempfile.TemporaryDirectory() as temp_dir:
             utils.write_yaml(model_data, f"{temp_dir}/model_config.yaml")
 
             self._stage_resource(
                 resource_name="model",
@@ -495,14 +546,15 @@
                 project_id=project_id,
                 force=force,
             )
 
     def add_dataset(
         self,
         file_path: str,
+        task_type: TaskType,
         dataset_config_file_path: str,
         project_id: str = None,
         force: bool = False,
     ):
         r"""Adds a dataset to a project's staging area (from a csv).
 
         Parameters
@@ -512,54 +564,71 @@
         dataset_config_file_path : str
             Path to the dataset configuration YAML file.
 
             .. admonition:: What's on the dataset config file?
 
                 The YAML file with the dataset config must have the following fields:
 
-                - ``columnNames`` : List[str]
+                columnNames : List[str]
                     List of the dataset's column names.
-                - ``classNames`` : List[str]
+                classNames : List[str]
                     List of class names indexed by label integer in the dataset.
                     E.g. ``[negative, positive]`` when ``[0, 1]`` are in your label column.
-                - ``labelColumnName`` : str
+                labelColumnName : str
                     Column header in the csv containing the labels.
 
                     .. important::
                         The labels in this column must be zero-indexed integer values.
-                - ``label`` : str
+                label : str
                     Type of dataset. E.g. ``'training'`` or
                     ``'validation'``.
-                - ``featureNames`` : List[str], default []
+                featureNames : List[str], default []
                     List of input feature names. Only applicable if your ``task_type`` is
                     :obj:`TaskType.TabularClassification` or :obj:`TaskType.TabularRegression`.
-                - ``textColumnName`` : str, default None
+                textColumnName : str, default None
                     Column header in the csv containing the input text. Only applicable if
                     your ``task_type`` is :obj:`TaskType.TextClassification`.
-                - ``predictionsColumnName`` : str, default None
-                    Column header in the csv containing the predictions. Only applicable if you
-                    are uploading a model as well with the :obj:`add_model` method.
+                predictionsColumnName : str, default None
+                    Column header in the csv containing the model's predictions as **zero-indexed
+                    integers**. Only applicable if you are uploading a model as well with the
+                    :obj:`add_model` method.
+
+                    This is optional if you provide a ``predictionScoresColumnName``.
+
+                    .. important::
+                        The values in this column must be zero-indexed integer values.
+                predictionScoresColumnName : str, default None
+                    Column header in the csv containing the model's predictions as **lists of
+                    class probabilities**. Only applicable if you are uploading a model as well with
+                    the :obj:`add_model` method.
+
+                    This is optional if you provide a ``predictionsColumnName``.
 
                     .. important::
                         Each cell in this column must contain a list of
                         class probabilities. For example, for a binary classification
-                        task, the cell values should look like this:
-                        .. csv-table::
-                            :header: ..., predictions
-                            ..., "[0.6650292861587155, 0.3349707138412845]"
-                            ..., "[0.8145561636482788, 0.18544383635172124]"
+                        task, the column with the predictions should look like this:
+
+                        **prediction_scores**
+
+                        ``[0.1, 0.9]``
+
+                        ``[0.8, 0.2]``
 
-                - ``categoricalFeatureNames`` : List[str], default []
+                        ``...``
+
+                categoricalFeatureNames : List[str], default []
                     A list containing the names of all categorical features in the dataset.
                     E.g. ``["Gender", "Geography"]``. Only applicable if your ``task_type`` is
                     :obj:`TaskType.TabularClassification` or :obj:`TaskType.TabularRegression`.
-                - ``language`` : str, default 'en'
+                language : str, default 'en'
                     The language of the dataset in ISO 639-1 (alpha-2 code) format.
-                - ``sep`` : str, default ','
+                sep : str, default ','
                     Delimiter to use. E.g. `'\\t'`.
+
         force : bool
             If :obj:`add_dataset` is called when there is already a dataset of the same type
             in the staging area, when ``force=True``, the existing staged dataset will be
             overwritten by the new one. When ``force=False``, the user will be prompted
             to confirm the overwrite.
 
         Notes
@@ -675,29 +744,32 @@
         right away with a commit message, you can use the :obj:`commit` and
         :obj:`push` methods:
 
         >>> project.commit("Initial dataset commit.")
         >>> project.push()
         """
         # Validate dataset
-        dataset_validator = validators.DatasetValidator(
+        dataset_validator = dataset_validators.get_validator(
+            task_type=task_type,
             dataset_config_file_path=dataset_config_file_path,
             dataset_file_path=file_path,
         )
         failed_validations = dataset_validator.validate()
 
         if failed_validations:
             raise exceptions.OpenlayerValidationError(
                 "There are issues with the dataset and its config. \n"
                 "Make sure to fix all of the issues listed above before the upload.",
             ) from None
 
         # Load dataset config and augment with defaults
         dataset_config = utils.read_yaml(dataset_config_file_path)
-        dataset_data = DatasetSchema().load(dataset_config)
+        dataset_data = DatasetSchema().load(
+            {"task_type": task_type.value, **dataset_config}
+        )
 
         # Copy relevant resources to temp directory
         with tempfile.TemporaryDirectory() as temp_dir:
             shutil.copy(file_path, f"{temp_dir}/dataset.csv")
             utils.write_yaml(dataset_data, f"{temp_dir}/dataset_config.yaml")
 
             self._stage_resource(
@@ -706,14 +778,15 @@
                 project_id=project_id,
                 force=force,
             )
 
     def add_dataframe(
         self,
         dataset_df: pd.DataFrame,
+        task_type: TaskType,
         dataset_config_file_path: str,
         project_id: str = None,
         force: bool = False,
     ):
         r"""Adds a dataset to a project's staging area (from a pandas DataFrame).
 
         Parameters
@@ -723,54 +796,71 @@
         dataset_config_file_path : str
             Path to the dataset configuration YAML file.
 
             .. admonition:: What's on the dataset config file?
 
                 The YAML file with the dataset config must have the following fields:
 
-                - ``columnNames`` : List[str]
+                columnNames : List[str]
                     List of the dataset's column names.
-                - ``classNames`` : List[str]
+                classNames : List[str]
                     List of class names indexed by label integer in the dataset.
                     E.g. ``[negative, positive]`` when ``[0, 1]`` are in your label column.
-                - ``labelColumnName`` : str
-                    Column header in the csv containing the labels.
+                labelColumnName : str
+                    Column header in the dataframe containing the labels.
 
                     .. important::
                         The labels in this column must be zero-indexed integer values.
-                - ``label`` : str
+                label : str
                     Type of dataset. E.g. ``'training'`` or
                     ``'validation'``.
-                - ``featureNames`` : List[str], default []
+                featureNames : List[str], default []
                     List of input feature names. Only applicable if your ``task_type`` is
                     :obj:`TaskType.TabularClassification` or :obj:`TaskType.TabularRegression`.
-                - ``textColumnName`` : str, default None
-                    Column header in the csv containing the input text. Only applicable if your
-                    ``task_type`` is :obj:`TaskType.TextClassification`.
-                - ``predictionsColumnName`` : str, default None
-                    Column header in the csv containing the predictions. Only applicable if you
-                    are uploading a model as well with the :obj:`add_model` method.
+                textColumnName : str, default None
+                    Column header in the dataframe containing the input text. Only applicable if
+                    your ``task_type`` is :obj:`TaskType.TextClassification`.
+                predictionsColumnName : str, default None
+                    Column header in the dataframe containing the model's predictions as **zero-indexed
+                    integers**. Only applicable if you are uploading a model as well with the
+                    :obj:`add_model` method.
+
+                    This is optional if you provide a ``predictionScoresColumnName``.
+
+                    .. important::
+                        The values in this column must be zero-indexed integer values.
+                predictionScoresColumnName : str, default None
+                    Column header in the dataframe containing the model's predictions as **lists of
+                    class probabilities**. Only applicable if you are uploading a model as well with
+                    the :obj:`add_model` method.
+
+                    This is optional if you provide a ``predictionsColumnName``.
 
                     .. important::
                         Each cell in this column must contain a list of
                         class probabilities. For example, for a binary classification
-                        task, the cell values should look like this:
-                        .. csv-table::
-                            :header: ..., predictions
-                            ..., "[0.6650292861587155, 0.3349707138412845]"
-                            ..., "[0.8145561636482788, 0.18544383635172124]"
+                        task, the column with the predictions should look like this:
 
-                - ``categoricalFeatureNames`` : List[str], default []
+                        **prediction_scores**
+
+                        ``[0.1, 0.9]``
+
+                        ``[0.8, 0.2]``
+
+                        ``...``
+
+                categoricalFeatureNames : List[str], default []
                     A list containing the names of all categorical features in the dataset.
                     E.g. ``["Gender", "Geography"]``. Only applicable if your ``task_type`` is
                     :obj:`TaskType.TabularClassification` or :obj:`TaskType.TabularRegression`.
-                - ``language`` : str, default 'en'
+                language : str, default 'en'
                     The language of the dataset in ISO 639-1 (alpha-2 code) format.
-                - ``sep`` : str, default ','
+                sep : str, default ','
                     Delimiter to use. E.g. `'\\t'`.
+
         force : bool
             If :obj:`add_dataframe` is called when there is already a dataset of the same
             type in the staging area, when ``force=True``, the existing staged dataset will
             be overwritten by the new one. When ``force=False``, the user will be prompted
             to confirm the overwrite.
 
         Notes
@@ -897,14 +987,15 @@
             file_path = os.path.join(tmp_dir, str(uuid.uuid1()))
             dataset_df.to_csv(file_path, index=False)
             return self.add_dataset(
                 file_path=file_path,
                 project_id=project_id,
                 dataset_config_file_path=dataset_config_file_path,
                 force=force,
+                task_type=task_type,
             )
 
     def commit(self, message: str, project_id: int, force: bool = False):
         """Adds a commit message to staged resources.
 
         Parameters
         ----------
@@ -936,15 +1027,15 @@
 
         After adding the commit message, the resources are ready to be pushed to the platform.
         You use the :obj:`push` method to do so:
 
         >>> project.push()
         """
         # Validate commit
-        commit_validator = validators.CommitValidator(commit_message=message)
+        commit_validator = commit_validators.CommitValidator(commit_message=message)
         failed_validations = commit_validator.validate()
 
         if failed_validations:
             raise exceptions.OpenlayerValidationError(
                 "There are issues with the commit message specified. \n"
                 "Make sure to fix all of the issues listed above before committing.",
             ) from None
@@ -977,27 +1068,30 @@
                 print("Overwriting commit message...")
                 os.remove(f"{project_dir}/commit.yaml")
 
             else:
                 print("Keeping the existing commit message.")
                 return
 
-        commit = dict(message=message, date=time.ctime())
+        commit = {
+            "message": message,
+            "date": time.ctime(),
+        }
         with open(f"{project_dir}/commit.yaml", "w", encoding="UTF-8") as commit_file:
             yaml.dump(commit, commit_file)
 
         print("Committed!")
 
-    def push(self, project_id: int):
+    def push(self, project_id: int, task_type: TaskType):
         """Pushes the commited resources to the platform.
 
         Notes
         -----
         - To use this method, you must first have committed your changes with the :obj:`commit`
-        method.
+            method.
 
         Examples
         --------
 
         Let's say you have a project with a model and a dataset staged and committed. You can
         confirm these resources are indeed in the staging area using the :obj:`status` method:
 
@@ -1007,71 +1101,137 @@
 
         Now, you can push the resources to the platform with:
 
         >>> project.push()
         """
         project_dir = f"{OPENLAYER_DIR}/{project_id}/staging"
 
+        if self._ready_for_push(project_dir=project_dir, task_type=task_type):
+            with open(
+                f"{project_dir}/commit.yaml", "r", encoding="UTF-8"
+            ) as commit_file:
+                commit = yaml.safe_load(commit_file)
+
+            # Tar the project's staging area
+            with tempfile.TemporaryDirectory() as tmp_dir:
+                tar_file_path = os.path.join(tmp_dir, "tarfile")
+                with tarfile.open(tar_file_path, mode="w:gz") as tar:
+                    tar.add(project_dir, arcname=os.path.basename(project_dir))
+
+                # Upload the tar file
+                print(
+                    "Pushing changes to the platform with the commit message: \n"
+                    f"\t - Message: {commit['message']} \n"
+                    f"\t - Date: {commit['date']}"
+                )
+                payload = {"commit": {"message": commit["message"]}}
+                self.api.upload(
+                    endpoint=f"projects/{project_id}/versions",
+                    file_path=tar_file_path,
+                    object_name="tarfile",
+                    body=payload,
+                )
+
+            self._post_push_cleanup(project_dir=project_dir)
+            print("Pushed!")
+
+    def _ready_for_push(self, project_dir: str, task_type: TaskType) -> bool:
+        """Checks if the project's staging area is ready to be pushed to the platform.
+
+        Parameters
+        ----------
+        project_dir : str
+            Directory path to the project's staging area.
+
+        Returns
+        -------
+        bool
+            Indicates whether the project's staging area is ready to be pushed to the platform.
+        """
         if not os.listdir(project_dir):
             print(
                 "The staging area is clean and there is nothing committed to push. "
                 "Please add model and/or datasets first, and then commit before pushing."
             )
-            return
+            return False
 
         if not os.path.exists(f"{project_dir}/commit.yaml"):
             print(
                 "There are resources staged, but you haven't committed them yet. "
                 "Please commit before pushing"
             )
-            return
-
-        with open(f"{project_dir}/commit.yaml", "r", encoding="UTF-8") as commit_file:
-            commit = yaml.safe_load(commit_file)
+            return False
 
         # Validate bundle resources
-        commit_bundle_validator = validators.CommitBundleValidator(
+        commit_bundle_validator = commit_validators.get_validator(
+            task_type=task_type,
             bundle_path=project_dir,
             skip_dataset_validation=True,
             skip_model_validation=False,  # Don't skip because the sample data is different
         )
         failed_validations = commit_bundle_validator.validate()
 
         if failed_validations:
             raise exceptions.OpenlayerValidationError(
                 "There are issues with the staged resources. \n"
                 "Make sure to fix all of the issues listed above before pushing.",
             ) from None
 
-        print(
-            "Pushing changes to the platform with the commit message: \n"
-            f"\t - Message: {commit['message']} \n"
-            f"\t - Date: {commit['date']}"
-        )
+        return True
 
-        # Tar the project's staging area
-        with tempfile.TemporaryDirectory() as tmp_dir:
-            tar_file_path = os.path.join(tmp_dir, "staging")
-            with tarfile.open(tar_file_path, mode="w:gz") as tar:
-                tar.add(project_dir, arcname=os.path.basename(project_dir))
-
-            # Upload the tar file
-            payload = {"commit": {"message": commit["message"]}}
-            self.api.upload(
-                endpoint=f"projects/{project_id}/versions",
-                file_path=tar_file_path,
-                object_name="tarfile",
-                body=payload,
-            )
-
-        # Clean up the staging area
+    def _post_push_cleanup(self, project_dir: str) -> None:
+        """Cleans up and re-creates the project's staging area after a push."""
         shutil.rmtree(project_dir)
         os.makedirs(project_dir, exist_ok=True)
 
-        print("Pushed!")
+    def export(self, destination_dir: str, project_id: int):
+        """Exports the commited resources as a tarfile to the location specified
+        by ``destination_dir``.
+
+        This is useful if you want to drag and drop the tarfile into the platform's
+        UI to upload it instead of using the :obj:`push` method.
+
+        Parameters
+        ----------
+        destination_dir : str
+            Directory path to where the project's staging area should be exported.
+
+        Notes
+        -----
+        - To use this method, you must first have committed your changes with the :obj:`commit`
+            method.
+
+        Examples
+        --------
+
+        Let's say you have a project with a model and a dataset staged and committed. You can
+        confirm these resources are indeed in the staging area using the :obj:`status` method:
+
+        >>> project.status()
+
+        You should see the staged resources as well as the commit message associated with them.
+
+        Now, you can export the resources to a speficied location with:
+
+        >>> project.export(destination_dir="/path/to/destination")
+        """
+        project_dir = f"{OPENLAYER_DIR}/{project_id}/staging"
+
+        if self._ready_for_push(project_dir=project_dir):
+            # Tar the project's staging area
+            with tempfile.TemporaryDirectory() as tmp_dir:
+                tar_file_path = os.path.join(tmp_dir, "tarfile")
+                with tarfile.open(tar_file_path, mode="w:gz") as tar:
+                    tar.add(project_dir, arcname=os.path.basename(project_dir))
+
+                print(f"Exporting staging area to {destination_dir}.")
+                shutil.copy(tar_file_path, os.path.expanduser(destination_dir))
+
+            self._post_push_cleanup(project_dir=project_dir)
+            print("Exported tarfile!")
 
     def status(self, project_id: int):
         """Shows the state of the staging area.
 
         Examples
         --------
```

### Comparing `openlayer-0.0.0a9/openlayer/api.py` & `openlayer-0.1.0a0/openlayer/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+"""Module that contains the core functionality of the Openlayer Python SDK.
+
+This module mainly defines the Api class, which is used by the OpenlayerClient
+to make requests to the Openlayer API.
+The StorageType enum is also defined here, which is used to specify what kind
+of storage the OpenlayerClient should use for uploads.
+
+Typical usage example:
+
+    from . import api
+
+    self.api = api.Api(api_key)
+    endpoint = "projects"
+    payload = {
+        "name": name,
+        "description": description,
+        "taskType": task_type.value,
+    }
+    project_data = self.api.post_request(endpoint, body=payload)
+
+"""
 import os
 import shutil
 from enum import Enum
 
 import requests
 from requests.adapters import HTTPAdapter, Response, Retry
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
@@ -14,27 +35,31 @@
 # Parameters for HTTP retry
 HTTP_TOTAL_RETRIES = 3  # Number of total retries
 HTTP_RETRY_BACKOFF_FACTOR = 2  # Wait 1, 2, 4 seconds between retries
 HTTP_STATUS_FORCE_LIST = [408, 429] + list(range(500, 504)) + list(range(506, 531))
 HTTP_RETRY_ALLOWED_METHODS = frozenset({"GET", "PUT", "POST"})
 
 CLIENT_METADATA = {"version": __version__}
+REQUESTS_TIMEOUT = 60 * 60 * 3  # 3 hours
 
 
 class StorageType(Enum):
     """Storage options for uploads."""
 
     ONPREM = "local"
     AWS = "s3"
     GCP = "gcs"
     AZURE = "azure"
 
 
 STORAGE = StorageType.AWS
 OPENLAYER_ENDPOINT = "https://api.openlayer.com/v1"
+# Controls the `verify` parameter on requests in case a custom
+# certificate is needed or needs to be disabled altogether
+VERIFY_REQUESTS = True
 
 
 class Api:
     """Internal class to handle http requests"""
 
     def __init__(self, api_key: str):
         if api_key == "" or api_key is None:
@@ -90,15 +115,14 @@
 
                 return res
             except Exception as err:
                 raise OpenlayerException(err) from err
 
     @staticmethod
     def _raise_on_respose(res: Response):
-
         try:
             message = res.json().get("error", res.text)
         except ValueError:
             message = res.text
 
         exception = ExceptionMap.get(res.status_code, OpenlayerException)
         raise exception(message, res.status_code)
@@ -191,21 +215,27 @@
             unit_scale=True,
             unit_divisor=1024,
             colour="BLUE",
         ) as t:
             with open(file_path, "rb") as f:
                 # Avoid logging here as it will break the progress bar
                 fields = presigned_json["fields"]
-                fields["file"] = (presigned_json["id"], f)
+                fields["file"] = (presigned_json["id"], f, "application/x-tar")
                 e = MultipartEncoder(fields=fields)
                 m = MultipartEncoderMonitor(
                     e, lambda monitor: t.update(min(t.total, monitor.bytes_read) - t.n)
                 )
                 headers = {"Content-Type": m.content_type}
-                res = requests.post(presigned_json["url"], data=m, headers=headers)
+                res = requests.post(
+                    presigned_json["url"],
+                    data=m,
+                    headers=headers,
+                    verify=VERIFY_REQUESTS,
+                    timeout=REQUESTS_TIMEOUT,
+                )
 
         if res.ok:
             body["storageUri"] = presigned_json["storageUri"]
             return self.post_request(f"{endpoint}", body=body)
         else:
             self._raise_on_respose(res)
 
@@ -225,14 +255,16 @@
                 unit_divisor=1024,
             ) as t:
                 wrapped_file = CallbackIOWrapper(t.update, f, "read")
                 res = requests.put(
                     presigned_json["url"],
                     data=wrapped_file,
                     headers={"Content-Type": "application/x-gzip"},
+                    verify=VERIFY_REQUESTS,
+                    timeout=REQUESTS_TIMEOUT,
                 )
         if res.ok:
             body["storageUri"] = presigned_json["storageUri"]
             return self.post_request(f"{endpoint}", body=body)
         else:
             self._raise_on_respose(res)
 
@@ -255,14 +287,16 @@
                 res = requests.put(
                     presigned_json["url"],
                     data=wrapped_file,
                     headers={
                         "Content-Type": "application/x-gzip",
                         "x-ms-blob-type": "BlockBlob",
                     },
+                    verify=VERIFY_REQUESTS,
+                    timeout=REQUESTS_TIMEOUT,
                 )
         if res.ok:
             body["storageUri"] = presigned_json["storageUri"]
             return self.post_request(f"{endpoint}", body=body)
         else:
             self._raise_on_respose(res)
 
@@ -272,12 +306,12 @@
         """
         params = {"storageInterface": "local", "objectName": object_name}
         presigned_json = self.get_request(f"{endpoint}/presigned-url", params=params)
         blob_path = presigned_json["storageUri"].replace("local://", "")
         dir_path = os.path.dirname(blob_path)
         try:
             os.makedirs(dir_path, exist_ok=True)
-        except OSError:
-            raise OpenlayerException(f"Directory {dir_path} cannot be created")
+        except OSError as exc:
+            raise OpenlayerException(f"Directory {dir_path} cannot be created") from exc
         shutil.copyfile(file_path, blob_path)
         body["storageUri"] = presigned_json["storageUri"]
         return self.post_request(f"{endpoint}", body=body)
```

### Comparing `openlayer-0.0.0a9/openlayer/exceptions.py` & `openlayer-0.1.0a0/openlayer/exceptions.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.0.0a9/openlayer/models.py` & `openlayer-0.1.0a0/openlayer/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,39 @@
+# pylint: disable=invalid-name,broad-exception-raised, consider-using-with
+"""
+Module that contains structures relevant to interfacing models with Openlayer.
+
+The ModelType enum chooses between different machine learning modeling frameworks.
+The Model object contains information about a model on the Openlayer platform.
+The CondaEnv object contains conda environment metadata relevant to the
+Openlayer platform.
+The ModelRunner runs input data through the model in a consistent Conda environment.
+
+Typical usage example:
+
+    validate=validate.OneOf(
+        [model_framework.value for model_framework in ModelType],
+        error=f"`model_type` must be one of the supported frameworks.",
+    )
+
+"""
 import ast
+import datetime
 import logging
 import os
 import shutil
 import subprocess
 import tempfile
+from abc import ABC, abstractmethod
 from enum import Enum
 from typing import List, Optional, Set
 
 import pandas as pd
 
-from . import utils
+from . import tasks, utils
 
 
 class ModelType(Enum):
     """A selection of machine learning modeling frameworks supported by Openlayer.
 
     .. note::
         Our `sample notebooks <https://github.com/openlayer-ai/openlayer-python/tree/main/examples>`_
@@ -22,14 +42,16 @@
 
     #: For custom built models.
     custom = "custom"
     #: For models built with `fastText <https://fasttext.cc/>`_.
     fasttext = "fasttext"
     #: For models built with `Keras <https://keras.io/>`_.
     keras = "keras"
+    #: For large language models (LLMs), such as GPT
+    llm = "llm"
     #: For models built with `PyTorch <https://pytorch.org/>`_.
     pytorch = "pytorch"
     #: For models built with `rasa <https://rasa.com/>`_.
     rasa = "rasa"
     #: For models built with `scikit-learn <https://scikit-learn.org/>`_.
     sklearn = "sklearn"
     #: For models built with `TensorFlow <https://www.tensorflow.org/>`_.
@@ -301,26 +323,26 @@
 
         with process.stdout:
             utils.log_subprocess_output(self.logger, process.stdout)
         exitcode = process.wait()
         return exitcode
 
 
-class ModelRunner:
+class BaseModelRunner(ABC):
     """Wraps the model package and provides a uniform run method."""
 
     def __init__(self, model_package: str, logger: Optional[logging.Logger] = None):
         self.model_package = model_package
 
         # Use validators logger if no logger is provided
         self.logger = logger or logging.getLogger("validators")
 
         # TODO: change env name to the model id
         self._conda_environment = CondaEnvironment(
-            env_name="new-openlayer",
+            env_name=f"model-runner-env-{datetime.datetime.now().strftime('%m-%d-%H-%M-%S-%f')}",
             requirements_file_path=f"{model_package}/requirements.txt",
             python_version_file_path=f"{model_package}/python_version",
             logger=self.logger,
         )
 
     def __del__(self):
         self._conda_environment.delete()
@@ -338,18 +360,16 @@
         -------
         pd.DataFrame
             Output from the model. The output is a dataframe with a single
             column named 'prediction' and lists of class probabilities as values.
         """
         # Copy the prediction job script to the model package
         current_file_dir = os.path.dirname(os.path.abspath(__file__))
-        shutil.copy(
-            f"{current_file_dir}/prediction_job.py",
-            f"{self.model_package}/prediction_job.py",
-        )
+
+        self._copy_prediction_job_script(current_file_dir)
 
         with tempfile.TemporaryDirectory() as temp_dir:
             # Save the input data to a csv file
             input_data.to_csv(f"{temp_dir}/input_data.csv", index=False)
 
             # Run the model in the conda environment
             with self._conda_environment as env:
@@ -374,13 +394,85 @@
                         "Failed to run the model in the conda environment."
                     ) from None
 
             self.logger.info("Successfully ran data through the model!")
             # Read the output data from the csv file
             output_data = pd.read_csv(f"{temp_dir}/output_data.csv")
 
-            # Make the items list of floats (and not strings)
-            output_data["predictions"] = output_data["predictions"].apply(
-                ast.literal_eval
-            )
+            output_data = self._post_process_output(output_data)
 
         return output_data
+
+    @abstractmethod
+    def _copy_prediction_job_script(self, current_file_dir: str):
+        """Copies the correct prediction job script to the model package."""
+        pass
+
+    @abstractmethod
+    def _post_process_output(self, output_data: pd.DataFrame) -> pd.DataFrame:
+        """Performs any post-processing on the output data."""
+        pass
+
+
+class ClassificationModelRunner(BaseModelRunner):
+    """ "Wraps classification models."""
+
+    def _copy_prediction_job_script(self, current_file_dir: str):
+        """Copies the classification prediction job script to the model package."""
+        shutil.copy(
+            f"{current_file_dir}/prediction_jobs/classification_prediction_job.py",
+            f"{self.model_package}/prediction_job.py",
+        )
+
+    def _post_process_output(self, output_data: pd.DataFrame) -> pd.DataFrame:
+        """Post-processes the output data."""
+        processed_output_data = output_data.copy()
+
+        # Make the items list of floats (and not strings)
+        processed_output_data["predictions"] = processed_output_data[
+            "predictions"
+        ].apply(ast.literal_eval)
+
+        return processed_output_data
+
+
+class RegressionModelRunner(BaseModelRunner):
+    """Wraps regression models."""
+
+    def _copy_prediction_job_script(self, current_file_dir: str):
+        """Copies the regression prediction job script to the model package."""
+        shutil.copy(
+            f"{current_file_dir}/prediction_jobs/regression_prediction_job.py",
+            f"{self.model_package}/prediction_job.py",
+        )
+
+    def _post_process_output(self, output_data: pd.DataFrame) -> pd.DataFrame:
+        """Post-processes the output data."""
+        return output_data
+
+
+# ----------------------------- Factory function ----------------------------- #
+def get_model_runner(
+    task_type: tasks.TaskType,
+    model_package: str,
+    logger: Optional[logging.Logger] = None,
+) -> BaseModelRunner:
+    """Factory function to get the correct model runner for the specified task type.
+
+    Parameters
+    ----------
+    task_type : tasks.TaskType
+        Task type of the model.
+    model_package : str
+        Path to the model package.
+    logger : Optional[logging.Logger], optional
+        Logger to use, by default None
+    """
+    if (
+        task_type == tasks.TaskType.TabularClassification
+        or task_type == tasks.TaskType.TextClassification
+    ):
+        return ClassificationModelRunner(model_package, logger)
+    elif task_type == tasks.TaskType.TabularRegression:
+        return RegressionModelRunner(model_package, logger)
+    else:
+        raise ValueError(f"Task type `{task_type}` is not supported.")
```

### Comparing `openlayer-0.0.0a9/openlayer/projects.py` & `openlayer-0.1.0a0/openlayer/projects.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 
     def add_model(
         self,
         *args,
         **kwargs,
     ):
         """Adds a model to a project's staging area."""
-        return self.client.add_model(*args, project_id=self.id, **kwargs)
+        return self.client.add_model(
+            *args, project_id=self.id, task_type=tasks.TaskType(self.taskType), **kwargs
+        )
 
     def add_baseline_model(
         self,
         *args,
         **kwargs,
     ):
         """Adds a baseline model to the project."""
@@ -57,27 +59,37 @@
 
     def add_dataset(
         self,
         *args,
         **kwargs,
     ):
         """Adds a dataset to a project's staging area (from a csv)."""
-        return self.client.add_dataset(*args, project_id=self.id, **kwargs)
+        return self.client.add_dataset(
+            *args, project_id=self.id, task_type=tasks.TaskType(self.taskType), **kwargs
+        )
 
     def add_dataframe(self, *args, **kwargs):
         """Adds a dataset to a project's staging area (from a pandas DataFrame)."""
-        return self.client.add_dataframe(*args, project_id=self.id, **kwargs)
+        return self.client.add_dataframe(
+            *args, project_id=self.id, task_type=tasks.TaskType(self.taskType), **kwargs
+        )
 
     def commit(self, *args, **kwargs):
         """Adds a commit message to staged resources."""
         return self.client.commit(*args, project_id=self.id, **kwargs)
 
     def push(self, *args, **kwargs):
         """Pushes the commited resources to the platform."""
-        return self.client.push(*args, project_id=self.id, **kwargs)
+        return self.client.push(
+            *args, project_id=self.id, task_type=tasks.TaskType(self.taskType), **kwargs
+        )
+
+    def export(self, *args, **kwargs):
+        """Exports the commited resources to a specified location."""
+        return self.client.export(*args, project_id=self.id, **kwargs)
 
     def status(self, *args, **kwargs):
         """Shows the state of the staging area."""
         return self.client.status(*args, project_id=self.id, **kwargs)
 
     def restore(self, *args, **kwargs):
         """Removes the resource specified by ``resource_name`` from the staging area."""
```

### Comparing `openlayer-0.0.0a9/openlayer/utils.py` & `openlayer-0.1.0a0/openlayer/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 """
 import io
 import logging
 import os
 import sys
 import traceback
 import warnings
+from typing import Any, Dict
 
+import pandas as pd
 import yaml
 
 
 # -------------------------- Helper context managers ------------------------- #
 class LogStdout:
     """Helper class that suppresses the prints and writes them to the `log_file_path` file."""
 
     def __init__(self, log_file_path: str):
         self.log_file_path = log_file_path
 
     def __enter__(self):
         self._original_stdout = sys.stdout
-        sys.stdout = open(self.log_file_path, "w")
+        sys.stdout = open(self.log_file_path, "w", encoding="utf-8")
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         sys.stdout.close()
         sys.stdout = self._original_stdout
 
 
 class HidePrints:
@@ -32,15 +34,15 @@
 
     Used as a context manager to hide the print / warning statements that can be inside the user's
     function while we test it.
     """
 
     def __enter__(self):
         self._original_stdout = sys.stdout
-        sys.stdout = open(os.devnull, "w")
+        sys.stdout = open(os.devnull, "w", encoding="utf-8")
         sys._jupyter_stdout = sys.stdout
         warnings.filterwarnings("ignore")
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         sys.stdout.close()
         sys.stdout = self._original_stdout
         sys._jupyter_stdout = sys.stdout
@@ -124,15 +126,73 @@
     Args:
         bundle_path (str): the path to the bundle.
 
     Returns:
         list: the list of resources in the bundle.
     """
     # TODO: factor out list of valid resources
+    # pylint: disable=invalid-name
     VALID_RESOURCES = {"baseline-model", "model", "training", "validation"}
 
     resources = []
 
     for resource in os.listdir(bundle_path):
         if resource in VALID_RESOURCES:
             resources.append(resource)
     return resources
+
+
+def load_dataset_from_bundle(bundle_path: str, label: str) -> pd.DataFrame:
+    """Loads a dataset from a commit bundle.
+
+    Parameters
+    ----------
+    label : str
+        The type of the dataset. Can be either "training" or "validation".
+
+    Returns
+    -------
+    pd.DataFrame
+        The dataset.
+    """
+    dataset_file_path = f"{bundle_path}/{label}/dataset.csv"
+
+    dataset_df = pd.read_csv(dataset_file_path)
+
+    return dataset_df
+
+
+def load_dataset_config_from_bundle(bundle_path: str, label: str) -> Dict[str, Any]:
+    """Loads a dataset config from a commit bundle.
+
+    Parameters
+    ----------
+    label : str
+        The type of the dataset. Can be either "training" or "validation".
+
+    Returns
+    -------
+    Dict[str, Any]
+        The dataset config.
+    """
+    dataset_config_file_path = f"{bundle_path}/{label}/dataset_config.yaml"
+
+    with open(dataset_config_file_path, "r", encoding="UTF-8") as stream:
+        dataset_config = yaml.safe_load(stream)
+
+    return dataset_config
+
+
+def load_model_config_from_bundle(bundle_path: str) -> Dict[str, Any]:
+    """Loads a model config from a commit bundle.
+
+    Returns
+    -------
+    Dict[str, Any]
+        The model config.
+    """
+    model_config_file_path = f"{bundle_path}/model/model_config.yaml"
+
+    with open(model_config_file_path, "r", encoding="UTF-8") as stream:
+        model_config = yaml.safe_load(stream)
+
+    return model_config
```

### Comparing `openlayer-0.0.0a9/openlayer.egg-info/PKG-INFO` & `openlayer-0.1.0a0/openlayer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlayer
-Version: 0.0.0a9
+Version: 0.1.0a0
 Summary: The official Python API library for Openlayer: the Testing and Debugging Platform for AI
 Home-page: https://github.com/openlayer-ai/openlayer-python
 Author: Unbox Inc.
 Project-URL: Documentation, https://docs.openlayer.com/
 Project-URL: Openlayer User Slack Group, https://l.linklyhq.com/l/1DG73
 Keywords: MLOps,AI,Openlayer
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: <=3.9,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="left">
   <img src="docs/source/_static/logo-purple-text.svg"><br>
 </div>
```

### Comparing `openlayer-0.0.0a9/setup.cfg` & `openlayer-0.1.0a0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+[isort]
+profile = black
+
+[flake8]
+count = True
+max-line-length = 192
+
+[tool:pytest]
+testpaths = 
+	tests
+
 [metadata]
 name = openlayer
 version = attr: openlayer.version.__version__
 description = The official Python API library for Openlayer: the Testing and Debugging Platform for AI
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/openlayer-ai/openlayer-python
@@ -18,25 +29,28 @@
 	Topic :: Software Development :: Libraries
 keywords = MLOps, AI, Openlayer
 project_urls = 
 	Documentation = https://docs.openlayer.com/
 	Openlayer User Slack Group = https://l.linklyhq.com/l/1DG73
 
 [options]
-packages = openlayer
+packages = 
+	openlayer
+	openlayer.validators
 install_requires = 
 	jupyter
 	pandas
 	requests
 	tqdm
 	marshmallow
+	marshmallow_oneofschema
 	requests_toolbelt
 	requests>=2.28.2
 	urllib3>=1.26.14
-python_requires = >=3.7, <=3.9
+python_requires = >=3.7
 include_package_data = True
 setup_requires = 
 	setuptools>=59.0
 	wheel
 zip_safe = False
 
 [egg_info]
```

