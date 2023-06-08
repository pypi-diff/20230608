# Comparing `tmp/wizata-dsapi-0.1.80.tar.gz` & `tmp/wizata-dsapi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.1.80.tar", last modified: Thu Jun  8 13:39:30 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.1.9.tar", last modified: Thu Apr 13 18:30:46 2023, max compression
```

## Comparing `wizata-dsapi-0.1.80.tar` & `wizata-dsapi-0.1.9.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 13:39:30.629674 wizata-dsapi-0.1.80/
--rw-rw-rw-   0        0        0    11556 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.80/LICENSE.txt
--rw-rw-rw-   0        0        0      177 2023-06-08 13:39:30.627703 wizata-dsapi-0.1.80/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-05-24 07:05:28.000000 wizata-dsapi-0.1.80/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-08 13:39:30.630170 wizata-dsapi-0.1.80/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-06-08 13:39:26.000000 wizata-dsapi-0.1.80/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:39:30.604079 wizata-dsapi-0.1.80/wizata_dsapi/
--rw-rw-rw-   0        0        0      916 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.80/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.80/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     2958 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.80/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     5714 2023-06-08 13:31:54.000000 wizata-dsapi-0.1.80/wizata_dsapi/datapoint.py
--rw-rw-rw-   0        0        0     1877 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.80/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.80/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    13823 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.80/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3810 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.80/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     6159 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.80/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.80/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0     7984 2023-05-24 07:05:28.000000 wizata-dsapi-0.1.80/wizata_dsapi/pipeline.py
--rw-rw-rw-   0        0        0     2136 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.80/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0    13260 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.80/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     8607 2023-05-19 12:04:56.000000 wizata-dsapi-0.1.80/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0     3929 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.80/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0     2597 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.80/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2701 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.80/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.80/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    50245 2023-05-24 16:23:15.000000 wizata-dsapi-0.1.80/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:39:30.625718 wizata-dsapi-0.1.80/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      177 2023-06-08 13:39:30.000000 wizata-dsapi-0.1.80/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2023-06-08 13:39:30.000000 wizata-dsapi-0.1.80/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 13:39:30.000000 wizata-dsapi-0.1.80/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-06-08 13:39:30.000000 wizata-dsapi-0.1.80/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-08 13:39:30.000000 wizata-dsapi-0.1.80/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 18:30:46.558856 wizata-dsapi-0.1.9/
+-rw-rw-rw-   0        0        0    11556 2023-03-17 16:15:58.000000 wizata-dsapi-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      246 2023-04-13 18:30:46.557865 wizata-dsapi-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-03-17 16:15:58.000000 wizata-dsapi-0.1.9/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-13 18:30:46.559353 wizata-dsapi-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2023-04-13 18:30:41.000000 wizata-dsapi-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:30:46.534553 wizata-dsapi-0.1.9/wizata_dsapi/
+-rw-rw-rw-   0        0        0      756 2023-04-13 17:52:10.000000 wizata-dsapi-0.1.9/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-03-24 09:46:21.000000 wizata-dsapi-0.1.9/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     2958 2023-04-10 07:55:31.000000 wizata-dsapi-0.1.9/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     1856 2023-04-03 07:22:42.000000 wizata-dsapi-0.1.9/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-03-21 09:56:23.000000 wizata-dsapi-0.1.9/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    13455 2023-04-13 15:54:05.000000 wizata-dsapi-0.1.9/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3555 2023-04-06 06:19:02.000000 wizata-dsapi-0.1.9/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     5447 2023-04-06 06:19:02.000000 wizata-dsapi-0.1.9/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-04-06 06:19:02.000000 wizata-dsapi-0.1.9/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0     2136 2023-03-27 08:16:15.000000 wizata-dsapi-0.1.9/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0     9756 2023-04-10 07:55:31.000000 wizata-dsapi-0.1.9/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     6914 2023-04-03 07:22:42.000000 wizata-dsapi-0.1.9/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0      392 2023-04-13 17:47:12.000000 wizata-dsapi-0.1.9/wizata_dsapi/sql_dto.py
+-rw-rw-rw-   0        0        0     3563 2023-04-13 15:54:05.000000 wizata-dsapi-0.1.9/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0      952 2023-04-13 17:47:12.000000 wizata-dsapi-0.1.9/wizata_dsapi/twin.py
+-rw-rw-rw-   0        0        0     2256 2023-04-13 18:30:41.000000 wizata-dsapi-0.1.9/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-03-27 08:16:15.000000 wizata-dsapi-0.1.9/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    33193 2023-04-07 15:57:41.000000 wizata-dsapi-0.1.9/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:30:46.555384 wizata-dsapi-0.1.9/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      246 2023-04-13 18:30:46.000000 wizata-dsapi-0.1.9/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-04-13 18:30:46.000000 wizata-dsapi-0.1.9/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 18:30:46.000000 wizata-dsapi-0.1.9/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-04-13 18:30:46.000000 wizata-dsapi-0.1.9/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 18:30:46.000000 wizata-dsapi-0.1.9/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.1.80/LICENSE.txt` & `wizata-dsapi-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.80/setup.py` & `wizata-dsapi-0.1.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.1.80',
+    version='0.1.9',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.1.9/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.1.9/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.1.9/wizata_dsapi/ds_dataframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
     A DS Dataframe is a definition of a pandas Dataframe that can be stored and shared on Wizata.
 
     :ivar df_id: The UUID of the dataframe.
     :ivar generatedById: The UUID of the Execution from which the dataframe was created.
     :ivar dataframe: Pandas Dataframe.
     """
 
-    def __init__(self, df_id=None, dataframe=None):
+    def __init__(self, df_id=None):
         if df_id is None:
             self.df_id = uuid.uuid4()
         else:
             self.df_id = df_id
         self.generatedById = None
-        self.dataframe = dataframe
+        self.dataframe = None
 
     def api_id(self) -> str:
         """
         Id of the dataframe (df_id)
 
         :return: string formatted UUID of the dataframe.
         """
```

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.1.9/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi/execution.py` & `wizata-dsapi-0.1.9/wizata_dsapi/execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,18 +261,18 @@
             self.execution_id = uuid.UUID(obj["id"])
         if "experimentId" in obj.keys() and obj["experimentId"] is not None:
             self.experiment_id = uuid.UUID(obj["experimentId"])
         if "request" in obj.keys() and obj["request"] is not None:
             self.request = Request()
             if isinstance(obj["request"], str):
                 self.request.from_json(json.loads(obj["request"]))
-                self.copy_properties(json.loads(obj["request"]))
+                self.add_properties(json.loads(obj["request"]))
             else:
                 self.request.from_json(obj["request"])
-                self.copy_properties(obj["request"])
+                self.add_properties(obj["request"])
         if "properties" in obj.keys() and obj["properties"] is not None:
             if isinstance(obj["properties"], str):
                 self.add_properties(json.loads(obj["properties"]))
             else:
                 self.add_properties(obj["properties"])
         if "dataframe" in obj.keys() and obj["dataframe"] is not None:
             if isinstance(obj["dataframe"], str):
@@ -313,34 +313,22 @@
     def to_pickle(self):
         """
         Convert the Execution to a pickle object.
         :return: Pickle object.
         """
         return pickle.dumps(self)
 
-    def add_properties(self, obj: dict):
+    def add_properties(self, obj: dict, replace=True):
         """
         load properties from a dictionary
 
         :param obj: dictionary with potential properties
         """
-        for key in obj.keys():
-            if self.properties is None:
-                self.properties = {}
-            self.properties[key] = obj[key]
-
-    def copy_properties(self, obj: dict):
-        """
-        copy properties from a dictionary originating from a Request object.
-        filtering on specific properties (Execution.keys)
-
-        :param obj: dictionary with potential properties
-        """
         for key in Execution.keys:
-            if key in obj:
+            if key in obj and (replace or key not in self.properties):
                 if self.properties is None:
                     self.properties = {}
                 self.properties[key] = obj[key]
 
     def get_interval(self) -> int:
         """
         Determine interval from either request, properties or loaded dataframe.
```

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi/experiment.py` & `wizata-dsapi-0.1.9/wizata_dsapi/experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         if experiment_id is None:
             self.experiment_id = uuid.uuid4()
         else:
             self.experiment_id = experiment_id
         self.key = key
         self.name = name
         self.description = description
-        self.templateId = None
         self.twinId = None
         self.twinGraphId = None
         self.createdById = None
         self.createdDate = None
         self.updatedById = None
         self.updatedDate = None
 
@@ -50,16 +49,14 @@
         }
         if self.key is not None:
             obj["key"] = str(self.key)
         if self.name is not None:
             obj["name"] = str(self.name)
         if self.description is not None:
             obj["description"] = str(self.description)
-        if self.templateId is not None:
-            obj["templateId"] = str(self.templateId)
         if self.twinId is not None:
             obj["twinId"] = str(self.twinId)
         if self.twinGraphId is not None:
             obj["twinGraphId"] = str(self.twinGraphId)
         if self.createdById is not None:
             obj["createdById"] = str(self.createdById)
         if self.createdDate is not None:
@@ -78,20 +75,18 @@
             self.experiment_id = uuid.UUID(obj["id"])
         if "key" in obj.keys() and obj["key"] is not None:
             self.key = obj["key"]
         if "name" in obj.keys() and obj["name"] is not None:
             self.name = obj["name"]
         if "description" in obj.keys() and obj["description"] is not None:
             self.description = obj["description"]
-        if "templateId" in obj.keys() and obj["templateId"] is not None:
-            self.templateId = obj["templateId"]
         if "twinId" in obj.keys() and obj["twinId"] is not None:
             self.twinId = obj["twinId"]
         if "twinGraphId" in obj.keys() and obj["twinGraphId"] is not None:
-            self.twinGraphId = obj["twinGraphId"]
+            self.twinId = obj["twinGraphId"]
         if "createdById" in obj.keys() and obj["createdById"] is not None:
             self.createdById = obj["createdById"]
         if "createdDate" in obj.keys() and obj["createdDate"] is not None:
             self.createdDate = obj["createdDate"]
         if "updatedById" in obj.keys() and obj["updatedById"] is not None:
             self.updatedById = obj["updatedById"]
         if "updatedDate" in obj.keys() and obj["updatedDate"] is not None:
```

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.1.9/wizata_dsapi/mlmodel.py`

 * *Files 13% similar despite different names*

```diff
@@ -105,33 +105,21 @@
         if "inputColumns" in obj.keys():
             self.input_columns = json.loads(obj["inputColumns"])
         if "outputColumns" in obj.keys():
             self.output_columns = json.loads(obj["outputColumns"])
         if "labelCount" in obj.keys():
             self.label_counts = int(obj["labelCount"])
         if "hasAnomalies" in obj.keys():
-            if isinstance(obj["hasAnomalies"], str) and obj["hasAnomalies"].lower() == "false":
-                self.has_anomalies = False
-            else:
-                self.has_anomalies = bool(obj["hasAnomalies"])
+            self.has_anomalies = bool(obj["hasAnomalies"])
         if "hasTargetFeat" in obj.keys():
-            if isinstance(obj["hasTargetFeat"], str) and obj["hasTargetFeat"].lower() == "false":
-                self.has_target_feat = False
-            else:
-                self.has_target_feat = bool(obj["hasTargetFeat"])
+            self.has_target_feat = bool(obj["hasTargetFeat"])
         if "needExactColumnNumbers" in obj.keys():
-            if isinstance(obj["needExactColumnNumbers"], str) and obj["needExactColumnNumbers"].lower() == "false":
-                self.needExactColumnNumbers = False
-            else:
-                self.needExactColumnNumbers = bool(obj["needExactColumnNumbers"])
+            self.needExactColumnNumbers = bool(obj["needExactColumnNumbers"])
         if "needExactColumnNames" in obj.keys():
-            if isinstance(obj["needExactColumnNames"], str) and obj["needExactColumnNames"].lower() == "false":
-                self.needExactColumnNames = False
-            else:
-                self.needExactColumnNames = bool(obj["needExactColumnNames"])
+            self.needExactColumnNames = bool(obj["needExactColumnNames"])
 
     def get_sample_payload(self):
         """
         Get a JSON formatted sample payload to call the ML Model.
         :return: JSON formatted sample payload.
         """
         pl_columns = {"timestamp": "[timestamp]"}
```

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.1.9/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.1.9/wizata_dsapi/script.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,223 +1,185 @@
+import json
 import uuid
-
+import dill
+import os
+import types
 from .api_dto import ApiDto
-from .script import ScriptConfig
-
-from enum import Enum
+import inspect
+from collections import OrderedDict
 
 
-class StepType(Enum):
-    QUERY = 'query'
-    SCRIPT = 'script'
-    MODEL = 'model'
+class Script(ApiDto):
+    """
+    A piece of python code that can either transform data, generate plot or train Machine Learning Models.
 
+    Scripts once validated can be used from Python or directly inside Wizata App by users.
 
-class PipelineStep(ApiDto):
-    """
-    Step of a pipeline.
+    :ivar script_id: The UUID of the ML Model.
+    :ivar description: Provide an insight-full description of what does your script.
+    :ivar status: 'draft', 'valid' or 'invalid' - to validate your script use client validate method.
+    :ivar needExactColumnNumbers: False by default, define if the model requires exact columns numbers to be executed.
+    :ivar needExactColumnNames: False by default, define if the model requires exact columns names to be executed.
+    :ivar canGeneratePlot: Set during validation, inform if the script generate plotly figures from dataframe.
+    :ivar canGenerateData: Set during validation, inform if the script transform input dataframe into another one.
+    :ivar canGenerateModel: Set during validation, inform if the script trains Machine Learning models from dataframe.
+    :ivar inputColumns: list of all columns used to call the script the model.
+    :ivar outputColumns: list of all columns generated by the script if it generates data.
+    :ivar function: Dill object containing the function code and decorators, please use copy()
     """
 
-    def __init__(self,
-                 step_id: uuid.UUID = None,
-                 step_type: StepType = None,
-                 config=None,
-                 inputs=None,
-                 outputs=None):
-
-        if outputs is None:
-            outputs = []
-        if step_id is None:
-            step_id = uuid.uuid4()
-        self.step_id = step_id
-        self.step_type = step_type
-        self.config = config
-        self.inputs = inputs
-        self.outputs = outputs
+    def __init__(self, script_id=None, description=None, function=None,
+                 exact_names=False, exact_numbers=False):
 
-    def from_json(self, obj):
+        # Id
+        if script_id is None:
+            script_id = uuid.uuid4()
+        self.script_id = script_id
+        self._name = None
+
+        # Properties
+        self.description = description
+        self.needExactColumnNumbers = exact_numbers
+        self.needExactColumnNames = exact_names
+
+        # Validation Properties
+        self.canGeneratePlot = False
+        self.canGenerateModel = False
+        self.canGenerateData = False
+        self.status = "draft"
+        self.inputColumns = []
+        self.outputColumns = []
+
+        # Source code property
+        self.source = None
+
+        # Function properties (code)
+        self.function = None
+        if function is not None:
+            self.copy(function)
+
+
+    @property
+    def name(self):
         """
-        load from JSON dictionary representation
+        Name of the function
+        :return: name of the function
         """
-        if "id" in obj.keys():
-            self.step_id = uuid.UUID(obj["id"])
+        return self._name
+
+    def api_id(self) -> str:
+        """
+        Id of the script (script_id)
+
+        :return: string formatted UUID of the script.
+        """
+        return str(self.script_id).upper()
 
-        if "type" in obj.keys():
-            if obj["type"] in ['query', 'script', 'model']:
-                self.step_type = StepType(obj["type"])
-            else:
-                raise TypeError(f'unsupported step type {obj["type"]}')
-        else:
-            raise TypeError(f'pipeline step must have a type.')
-        if "config" in obj.keys():
-            if self.step_type == StepType.SCRIPT:
-                self.config = ScriptConfig()
-                self.config.from_json(obj['config'])
-            else:
-                self.config = obj['config']
-        self.inputs = []
-        if "inputs" in obj.keys():
-            for step_input in obj["inputs"]:
-                if isinstance(step_input, dict):
-                    self.inputs.append(step_input)
-                else:
-                    raise TypeError(f'unsupported input type {step_input.__class__.__name__}')
-
-        self.outputs = []
-        if "outputs" in obj.keys():
-            for step_output in obj["outputs"]:
-                if isinstance(step_output, dict):
-                    self.outputs.append(step_output)
-                else:
-                    raise TypeError(f'unsupported output type {step_output.__class__.__name__}')
-
-    def inputs_names(self, f_type: str = None) -> list:
-        """
-        get a list str representing inputs names
-        :param f_type: filter on a type
-        :return: list str
-        """
-        names = []
-        for d_key in self.inputs:
-            if not isinstance(d_key, dict):
-                raise TypeError(f'unsupported output type {d_key} expected dataframe or model')
-            if "dataframe" in d_key.keys() and (f_type is None or f_type == 'dataframe'):
-                names.append(d_key["dataframe"])
-            elif "model" in d_key.keys() and (f_type is None or f_type == 'model'):
-                names.append(d_key["model"])
-            elif f_type is None:
-                raise TypeError(f'unsupported input type {d_key} expected dataframe or model')
-        return names
-
-    def outputs_names(self, f_type: str = None) -> list:
-        """
-        get a list str representing outputs names
-        :param f_type: filter on a type
-        :return: list str
-        """
-        names = []
-        for d_key in self.outputs:
-            if not isinstance(d_key, dict):
-                raise TypeError(f'unsupported output type {d_key} expected dataframe or model')
-            elif "dataframe" in d_key.keys() and (f_type is None or f_type == 'dataframe'):
-                names.append(d_key["dataframe"])
-            elif "model" in d_key.keys() and (f_type is None or f_type == 'model'):
-                names.append(d_key["model"])
-            elif f_type is None:
-                raise TypeError(f'unsupported output type {d_key} expected dataframe or model')
-        return names
-
-    def get_input(self, name: str) -> dict:
-        """
-        get input dict based on value name.
-        :param name: value name to find.
-        :return: input dict
-        """
-        for d_input in self.inputs:
-            if name in d_input.values():
-                return d_input
-
-    def get_output(self, name: str) -> dict:
-        """
-        get output dict based on value name.
-        :param name: value name to find.
-        :return: input dict
-        """
-        for d_output in self.outputs:
-            if name in d_output.values():
-                return d_output
-
-
-class Pipeline(ApiDto):
-
-    def __init__(self,
-                 pipeline_id: uuid.UUID = None,
-                 key: str = None,
-                 variables: dict = None,
-                 steps: [] = None):
-
-        if pipeline_id is None:
-            pipeline_id = uuid.uuid4()
-        self.pipeline_id = pipeline_id
-        self.key = key
-        self.variables = variables
-        if steps is not None:
-            for step in steps:
-                if not isinstance(step, PipelineStep):
-                    raise TypeError(f'step expected PipelineStep but received {step.__class__.__name__}')
-            self.steps = steps
-        else:
-            self.steps = []
-
-    def check_path(self) -> bool:
-        """
-        validate that steps create a valid path.
-        return true if path is valid, otherwise raise errors
-        """
-
-        followed = []  # all steps already followed
-        produced = []  # all outputs already produced
-
-        steps_to_follow = self._next_steps(followed, produced)
-        if len(steps_to_follow) == 0:
-            raise ValueError('path does not contains any initial steps producing outputs')
-
-        while len(steps_to_follow) > 0:
-            for step in steps_to_follow:
-                self._follow_step(step, followed, produced)
-            steps_to_follow = []
-            if len(followed) < len(self.steps):
-                steps_to_follow = self._next_steps(followed, produced)
-
-        if len(followed) == len(self.steps):
-            return True
-        else:
-            raise RuntimeError(f'missing {len(self.steps)-len(followed)} step(s) that could not be followed')
-
-    def _follow_step(self,
-                     step: PipelineStep,
-                     followed: list,
-                     produced: list):
-        """
-        simulate that step have been followed.
-        """
-        if step in followed:
-            raise RuntimeError(f'path cannot pass two times through same step {step.step_id}')
-        followed.append(step)
-        for output in step.outputs_names():
-            if step.step_type == StepType.QUERY and len(step.outputs) != 1:
-                raise RuntimeError(f'query step must have exactly one output and be of type dataframe')
-            if output in produced:
-                raise RuntimeError(f'output {output} is already produced.')
-            produced.append(output)
-
-    def _next_steps(self, followed, produced):
-        """
-        find all next steps that are ready to be executed
-        """
-        next_steps = []
-        step: PipelineStep
-        for step in self.steps:
-            if all(s_input in produced for s_input in step.inputs_names()) and step not in followed:
-                next_steps.append(step)
-        return next_steps
+    def endpoint(self) -> str:
+        """
+        Name of the endpoints used to manipulate scripts.
+        :return: Endpoint name.
+        """
+        return "Scripts"
+
+    def to_json(self):
+        """
+        Convert the script to a dictionary compatible to JSON format.
+
+        :return: dictionary representation of the Script object.
+        """
+        obj = {
+            "id": str(self.script_id),
+            "canGeneratePlot": str(self.canGeneratePlot),
+            "canGenerateModel": str(self.canGenerateModel),
+            "canGenerateData": str(self.canGenerateData),
+            "status": str(self.status),
+            "needExactColumnNumbers": str(self.needExactColumnNumbers),
+            "needExactColumnNames": str(self.needExactColumnNames),
+            "inputColumns": json.dumps(list(self.inputColumns)),
+            "outputColumns": json.dumps(list(self.outputColumns))
+        }
+        if self.name is not None:
+            obj["name"] = str(self.name)
+        if self.name is not None:
+            obj["description"] = str(self.description)
+        return obj
 
     def from_json(self, obj):
         """
-        load from JSON dictionary representation
+        Load the Script entity from a dictionary representation of the Script.
+
+        :param obj: Dict version of the Script.
         """
         if "id" in obj.keys():
-            self.pipeline_id = uuid.UUID(obj["id"])
-        if "key" in obj.keys():
-            self.key = str(obj['key'])
-        if "id" not in obj.keys() and "key" not in obj.keys():
-            raise KeyError("at least id or key must be set on a pipeline")
-        if "variables" in obj.keys():
-            self.variables = obj['variables']
-        if "steps" in obj.keys():
-            for obj_step in obj["steps"]:
-                step = PipelineStep()
-                step.from_json(obj_step)
-                self.steps.append(step)
+            self.script_id = uuid.UUID(obj["id"])
+        if "name" in obj.keys():
+            self._name = obj["name"]
+        if "description" in obj.keys():
+            if obj["description"] != "None":
+                self.description = obj["description"]
+        if "canGeneratePlot" in obj.keys():
+            self.canGeneratePlot = bool(obj["canGeneratePlot"])
+        if "canGenerateModel" in obj.keys():
+            self.canGenerateModel = bool(obj["canGenerateModel"])
+        if "canGenerateData" in obj.keys():
+            self.canGenerateData = bool(obj["canGenerateData"])
+        if "status" in obj.keys():
+            self.status = str(obj["status"]).lower()
+        if "needExactColumnNumbers" in obj.keys():
+            self.needExactColumnNumbers = bool(obj["needExactColumnNumbers"])
+        if "needExactColumnNames" in obj.keys():
+            self.needExactColumnNames = bool(obj["needExactColumnNames"])
+        if "inputColumns" in obj.keys():
+            self.inputColumns = json.loads(obj["inputColumns"])
+        if "outputColumns" in obj.keys():
+            self.outputColumns = json.loads(obj["outputColumns"])
+
+    def copy(self, myfunction):
+        """
+        Copy your function code and decorators to a format executable by the Wizata App.
+        :param myfunction: your function - pass the function itself as parameter
+        """
+
+        if myfunction.__code__.co_argcount < 1:
+            raise ValueError('your function must contains at least one parameter')
+
+        self.function = Function()
+
+        self.function.id = myfunction.__name__
+        self.function.params = inspect.signature(myfunction).parameters
+
+        self._name = myfunction.__name__
+
+        self.function.code = myfunction.__code__
+
+        f_globals = myfunction.__globals__
+        self.function.globals = []
+        for k_global in f_globals:
+            if isinstance(myfunction.__globals__[k_global], types.ModuleType):
+                module = f_globals[k_global]
+                self.function.globals.append({
+                    "var": k_global,
+                    "module": str(module.__name__)
+                })
+
+        if myfunction.__code__.co_filename is not None:
+            if os.path.exists(myfunction.__code__.co_filename):
+                with open(myfunction.__code__.co_filename, "r") as f:
+                    source_code = f.read()
+                self.source = source_code
 
 
+class Function:
+    """
+    Python Code Function
+
+    :ivar id: technical name and then id of the function
+    :ivar code: code of the function __code__
+    :ivar globals: modules references __globals__
+    """
 
+    def __init__(self):
+        self.id = None
+        self.code = None
+        self.globals = None
+        self.params = OrderedDict()
```

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi/plot.py` & `wizata-dsapi-0.1.9/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi/request.py` & `wizata-dsapi-0.1.9/wizata_dsapi/request.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 import uuid
-from datetime import datetime, timedelta, timezone
+from datetime import datetime, timedelta
 
 
 class Request:
     """
     A Request to fetch dataframes from Wizata App.
 
     To execute the request please use a DS API client.
 
     :ivar equipments: List of Equipments containing Digital Twin item and datapoints to fetch.
-
-    :ivar template_id: UUID of the template.
-    :ivar template: str unique id of the template.
-    :ivar twin_id: UUID of the Digital Twin.
-    :ivar twin: str hardware id of the Digital Twin.
-
     :ivar start: Datetime defining beginning of period.
     :ivar end: Datetime defining end of period.
     :ivar aggregation: Aggregation method to fetch, accept "mean" and "stddev".
     :ivar interval: Interval in seconds between each aggregation.
     :ivar filters: Filter to apply on the query (not yet fully implemented).
     :ivar connections: Connections rules between equipment to align data in time (not yet fully implemented).
     :ivar null: By default at 'drop' and dropping NaN values. If not intended behavior please set it to 'ignore' or 'all'.
@@ -26,51 +20,28 @@
 
     def __init__(self,
                  datapoints=None,
                  start=None,
                  end=None,
                  agg_method='mean',
                  interval=None,
-                 null='drop',
-                 template_id=None,
-                 template=None,
-                 twin_id=None,
-                 twin=None,
-                 request_id=None,
-                 filters=None,
-                 options=None):
-        if request_id is None:
-            request_id = uuid.uuid4()
-        self.request_id = request_id
+                 null='drop'):
         self.function = None
-
-        # Equipments & Data Points
         self.equipments = []
         if datapoints is not None:
             self.add_datapoints(datapoints)
 
-        # Template & Registration
-        self.template = None
-        self.select_template(
-             template_id=template_id,
-             template_key=template,
-             twin_id=twin_id,
-             twin_hardware_id=twin
-        )
-
         self.start = start
         self.end = end
 
         self.aggregation = agg_method
         if interval is not None:
             self.interval = int(interval) / 1000
 
-        self.filters = filters
-        self.options = options
-
+        self.filters = None
         self.on_off_sensor = None
         self.restart_time = None
         self.sensitivity = None
         self.dataframe = None
         self.extra_data = None
         self.target_feat = None
         self.connections = None
@@ -81,16 +52,14 @@
     def prepare(self):
         """
         prepare a dict JSON compatible only for the QUERY part of the request.
 
         :return: a dict JSON compatible
         """
         query = {}
-        if self.request_id is not None:
-            query["id"] = str(self.request_id)
         if self.equipments is not None:
             query["equipments_list"] = self.equipments
         else:
             raise KeyError("Missing data points inside the query - add_datapoints")
         if self.start is not None and self.end is not None:
             query["timeframe"] = {
                 "start": self.__format_date(self.start),
@@ -103,20 +72,14 @@
                 "agg_method": self.aggregation,
                 "interval": self.interval * 1000
             }
         else:
             raise KeyError("Missing aggregations information inside the request")
         if self.null is not None and self.null != 'drop':
             query['null'] = self.null
-        if self.template is not None:
-            query['template'] = self.template
-        if self.filters is not None:
-            query['filters'] = self.filters
-        if self.options is not None:
-            query['options'] = self.options
         return query
 
     def __format_date(self, dt_to_format):
         if isinstance(dt_to_format, datetime):
             millisec = dt_to_format.timestamp() * 1000
             return int(millisec)
         else:
@@ -174,56 +137,21 @@
         :param method: 'mean' or 'stddev'
         :param interval: interval in ms (will be stored in seconds)
         """
         self.aggregation = method
         if interval is not None:
             self.interval = int(interval) / 1000
 
-    def select_template(self,
-                        template_id=None,
-                        template_key=None,
-                        twin_id=None,
-                        twin_hardware_id=None):
-        """
-        Select a template and its registration.
-        :param template_id: template UUID
-        :param template_key: template key ( ignored if template_id specified )
-        :param twin_id: Digital Twin UUID
-        :param twin_hardware_id: hardware ID of Digital Twin ( ignored if twin_id specified )
-        """
-        if template_id is None and template_key is None and twin_id is None and twin_hardware_id is None:
-            self.template = None
-            return
-        else:
-            self.template = {}
-
-            if template_id is not None:
-                self.template['template_id'] = uuid.UUID(template_id)
-            elif template_key is not None:
-                self.template['template_key'] = str(template_key)
-            else:
-                raise ValueError('A twin can only be specified with its template')
-
-            if twin_id is not None:
-                self.template['twin_id'] = uuid.UUID(twin_id)
-            elif twin_hardware_id is not None:
-                self.template['twin_hardware_id'] = str(twin_hardware_id)
-            else:
-                raise ValueError('A template can only be specified with its registered twin')
-
     def to_json(self):
         """
         convert to a dict JSON compatible for all properties. For query only, use prepare().
 
         :return: a dict JSON compatible
         """
-
-        # Prepare is 'to_json' without future obsolete properties
         obj = self.prepare()
-
         if self.target_feat is not None:
             obj["target_feat"] = {
                 "sensor": self.target_feat["sensor"],
                 "operator": self.target_feat["operator"],
                 "threshold": self.target_feat["threshold"]
             }
         if self.on_off_sensor is not None and self.restart_time is not None:
@@ -242,67 +170,45 @@
 
     def from_json(self, json_data):
         """
         load a request based on dict from a JSON file.
 
         :param json_data: JSON formatted dictionnary object representing a query.
         """
-        if "id" in json_data.keys():
-            self.request_id = uuid.UUID(json_data["id"])
-
         if "name" in json_data.keys():
             self.name = json_data["name"]
 
-        found_dps = False
-        if "equipments_list" in json_data.keys():
-            self.equipments = json_data["equipments_list"]
-            for equipment in self.equipments:
-                if "datapoints" not in equipment.keys():
-                    raise KeyError("No 'data points' have been provided for equipment with id '" +
-                                   str(equipment["id"]) + "'")
-                else:
-                    found_dps = True
-        if "template" in json_data.keys():
-            self.template = json_data["template"]
-            found_dps = True
-
-        if not found_dps:
-            raise KeyError('no equipments lists nor template specified.')
+        if "equipments_list" not in json_data.keys():
+            raise KeyError("No 'twin unit' nor 'data points' selected please select some and re-try.")
+        self.equipments = json_data["equipments_list"]
 
         if "timeframe" not in json_data.keys():
             raise KeyError("No 'time range' have been selected, please set it up and re-try.")
 
         if "start" not in json_data["timeframe"].keys():
             raise KeyError("No 'start time' have been selected, please set it up and re-try.")
-        self.start = datetime.fromtimestamp(json_data["timeframe"]["start"] / 1000, timezone.utc)
+        self.start = datetime.fromtimestamp(json_data["timeframe"]["start"] / 1000)
 
         if "end" not in json_data["timeframe"].keys():
             raise KeyError("No 'end time' have been selected, please set it up and re-try.")
-        self.end = datetime.fromtimestamp(json_data["timeframe"]["end"] / 1000, timezone.utc)
+        self.end = datetime.fromtimestamp(json_data["timeframe"]["end"] / 1000)
 
         if "aggregations" not in json_data.keys():
             raise KeyError("No 'aggregations' have been selected, please set it up and re-try.")
 
         if "agg_method" not in json_data["aggregations"].keys():
             raise KeyError("No 'Aggregation Method' have been selected, please set it up and re-try.")
         self.aggregation = json_data["aggregations"]["agg_method"]
 
         if "interval" not in json_data["aggregations"].keys():
             raise KeyError("No 'Aggregation Interval' have been selected, please set it up and re-try.")
         self.interval = int(json_data["aggregations"]["interval"] / 1000)
 
         if "filters" in json_data.keys():
             self.filters = json_data["filters"]
-        else:
-            self.filters = {}
-
-        if "options" in json_data.keys():
-            self.options = json_data["options"]
-        else:
-            self.options = {}
 
         if "connections" in json_data.keys():
             self.connections = json_data["connections"]
 
         if "null" in json_data.keys():
             self.null = json_data["null"]
 
@@ -321,8 +227,7 @@
 
         if "sensitivity" in json_data.keys():
             self.sensitivity = json_data["sensitivity"]
 
         if "extra_data" in json_data.keys():
             self.extra_data = json_data["extra_data"]
 
-
```

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi/template.py` & `wizata-dsapi-0.1.9/wizata_dsapi/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,13 @@
 import uuid
 import json
 from .api_dto import ApiDto
 
 
 class Template(ApiDto):
-    """
-    Template of a solution and/or asset.
-
-    :ivar template_id: UUID of the Template.
-    :ivar key: str unique id identifying the Template.
-    :ivar name: logical display name of the Template.
-    :ivar properties: list of Property { type , name } of the solution.
-
-    Properties only support type 'datapoint', 'float', 'integer' or 'string'
-    """
 
     def __init__(self, template_id=None, key=None, name=None, properties=None):
         if template_id is None:
             self.template_id = uuid.uuid4()
         else:
             self.template_id = template_id
         self.key = key
@@ -94,17 +84,16 @@
             if existing_property["name"] == property_value["name"]:
                 raise ValueError(f'property {property_value["name"]} already exists in template.')
         self.properties.append(property_value)
 
     def remove_property(self, name):
         """
         remove a property from the list based on its name
-        :param name: property to remove
+        :param name: name of property to remove
         """
         found_property = None
         for existing_property in self.properties:
             if existing_property["name"] == name:
                 found_property = existing_property
         if self.properties is not None and found_property is not None:
             self.properties.remove(found_property)
 
-
```

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.1.9/wizata_dsapi/twinregistration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,13 @@
 import uuid
 import json
 from .api_dto import ApiDto
 
 
 class TwinRegistration(ApiDto):
-    """
-    Registration of a Digital Twin on a solution Template.
-
-    :ivar twin_registration_id: UUID of the registration
-    :ivar twin_id: UUID of registered Digital Twin
-    :ivar template_id: UUID of the solution template.
-    :ivar properties: list of Properties { name , datapoint, float, integer, string }
-
-    A property must contains a name and the hardwareId of the datapoint or the value corresponding to the right type.
-    """
 
     def __init__(self, twin_registration_id=None, twin_id=None, template_id=None, properties=None):
         if twin_registration_id is None:
             self.twin_registration_id = uuid.uuid4()
         else:
             self.twin_registration_id = twin_registration_id
         self.twin_id = twin_id
@@ -43,18 +33,18 @@
         """
         Load the Registration entity from a dictionary.
 
         :param obj: Dict version of the Registration.
         """
         if "id" in obj.keys():
             self.twin_registration_id = uuid.UUID(obj["id"])
-        if "twinId" in obj.keys() and obj["twinId"] is not None:
-            self.twin_id = obj["twinId"]
-        if "templateId" in obj.keys() and obj["templateId"] is not None:
-            self.template_id = obj["templateId"]
+        if "twin_id" in obj.keys() and obj["twin_id"] is not None:
+            self.twin_id = obj["twin_id"]
+        if "template_id" in obj.keys() and obj["template_id"] is not None:
+            self.template_id = obj["template_id"]
         if "properties" in obj.keys() and obj["properties"] is not None:
             if isinstance(obj["properties"], str):
                 self.properties = json.loads(obj["properties"])
             else:
                 self.properties = obj["properties"]
 
     def to_json(self):
@@ -63,14 +53,14 @@
 
         :return: dictionary representation of the Registration object.
         """
         obj = {
             "id": str(self.twin_registration_id)
         }
         if self.twin_id is not None:
-            obj["twinId"] = str(self.twin_id)
+            obj["twin_id"] = str(self.twin_id)
         if self.template_id is not None:
-            obj["templateId"] = str(self.template_id)
+            obj["template_id"] = str(self.template_id)
         if self.properties is not None:
             obj["properties"] = json.dumps(self.properties)
         return obj
```

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.1.9/wizata_dsapi/wizata_dsapi_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,30 +25,26 @@
 from .mlmodel import MLModel
 from .experiment import Experiment
 from .script import Script
 from .execution import Execution
 from .dsapi_json_encoder import DSAPIEncoder
 from .ds_dataframe import DSDataFrame
 from .model_toolkit import predict
-from .template import Template
-from .twinregistration import TwinRegistration
-from .twin import Twin
 
 
 class WizataDSAPIClient:
 
     def __init__(self,
                  client_id=None,
                  scope=None,
                  tenant_id=None,
                  username=None,
                  password=None,
                  domain="localhost",
-                 protocol="https",
-                 client_secret=None):
+                 protocol="https"):
 
         # properties
         self.domain = domain
         self.protocol = protocol
 
         # authentication
         self.__username = username
@@ -57,81 +53,51 @@
         self.__client_id = client_id
         self.__tenant_id = tenant_id
         if tenant_id is not None:
             self.__authority = "https://login.microsoftonline.com/" + tenant_id
         self.__scopes = [scope]
 
         self.__interactive_token = None
-        self.__daemon = False
-
-        if client_secret is not None:
-            self.__daemon = True
-            self.__confidential_app = msal.ConfidentialClientApplication(
-                client_id=self.__client_id,
-                client_credential=client_secret,
-                authority=self.__authority
-            )
 
         self.__app = msal.PublicClientApplication(
             client_id=self.__client_id,
             authority=self.__authority
         )
 
     def authenticate(self):
         result = self.__app.acquire_token_interactive(
             scopes=self.__scopes,
             success_template="""<html><body>You are authenticated and your code is running, you can close this page.<script>setTimeout(function(){window.close()}, 3000);</script></body></html> """
         )
-        self.__daemon = False
         self.__interactive_token = result["access_token"]
 
     def __url(self):
         return self.protocol + "://" + self.domain + "/dsapi/"
 
     def __token(self):
         # Interactive Authentication
         if self.__interactive_token is not None:
             return self.__interactive_token
 
-        if not self.__daemon:
-            # Silent Authentication
-            result = None
-            accounts = self.__app.get_accounts(username=self.__username)
-            if accounts:
-                # If there is an account in the cache, try to get the token silently
-                result = self.__app.acquire_token_silent(scopes=self.__scopes, account=accounts[0])
-
-            if not result:
-                # If there is no cached token, try to get a new token using the provided username and password
-                result = self.__app.acquire_token_by_username_password(
-                    username=self.__username,
-                    password=self.__password,
-                    scopes=self.__scopes
-                )
-
-            if "error_description" in result.keys():
-                raise RuntimeError(str(result["error_description"]))
-
-            if "access_token" in result.keys():
-                return result["access_token"]
-            else:
-                raise RuntimeError(str(result))
-        else:
-            result = self.__confidential_app.acquire_token_silent(scopes=self.__scopes, account=None)
-
-            if not result:
-                result = self.__confidential_app.acquire_token_for_client(scopes=self.__scopes)
-
-            if "error_description" in result.keys():
-                raise RuntimeError(str(result["error_description"]))
-
-            if "access_token" in result.keys():
-                return result["access_token"]
+        # Silent Authentication
+        result = None
+        accounts = self.__app.get_accounts(username=self.__username)
+        if accounts:
+            # If there is an account in the cache, try to get the token silently
+            result = self.__app.acquire_token_silent(scopes=self.__scopes, account=accounts[0])
+
+        if not result:
+            # If there is no cached token, try to get a new token using the provided username and password
+            result = self.__app.acquire_token_by_username_password(
+                username=self.__username,
+                password=self.__password,
+                scopes=self.__scopes
+            )
 
-            return result
+        return result["access_token"]
 
     def __header(self):
         return {
             'Content-Type': 'application/json',
             'Authorization': f'Bearer {self.__token()}'
         }
 
@@ -196,49 +162,25 @@
                 json_dfs = response.json()
                 dfs = []
                 for json_model in json_dfs:
                     dfs.append(DSDataFrame(uuid.UUID(json_model["id"])))
                 return dfs
             else:
                 raise self.__raise_error(response)
-        elif str_type == "templates":
-            response = requests.request("GET",
-                                        self.__url() + "templates/",
-                                        headers=self.__header()
-                                        )
-            if response.status_code == 200:
-                templates_json = response.json()
-                templates = []
-                for template_json in templates_json:
-                    template = Template()
-                    template.from_json(template_json)
-                    templates.append(template)
-                return templates
-            else:
-                raise self.__raise_error(response)
         else:
             raise TypeError("Type not supported.")
 
-    def get(self,
-            obj=None,
-            script_name=None,
-            experiment_key=None,
-            model_key=None,
-            template_key=None,
-            twin_hardware_id=None):
+    def get(self, obj=None, script_name=None, experiment_key=None, model_key=None):
         """
         get full content of an object identified with is id.
 
         :param obj: object of a supported entity with at list its id
         :param script_name: alternatively you can use a function name to get a script
         :param experiment_key: alternatively you can use an experiment key to get an experiment
-        :param model_key: model key you want to get.
-        :param template_key: template key you want to get.
-        :param twin_hardware_id: twin hardware id you want to get.
-        :return: object completed with all properties on server (None if not found or raise Error if with id)
+        :return: object completed with all properties on server.
         """
         if script_name is not None:
             response = requests.request("GET",
                                         self.__url() + "scripts/" + str(script_name) + "/",
                                         headers=self.__header()
                                         )
             if response.status_code == 200:
@@ -251,70 +193,34 @@
                                         self.__url() + "experiments/",
                                         params={
                                             'key': experiment_key
                                         },
                                         headers=self.__header()
                                         )
             if response.status_code == 200:
+                obj = Experiment()
                 for obj_json in response.json():
-                    obj = Experiment()
                     obj.from_json(obj_json)
-                    return obj
-                return None
+                return obj
             else:
                 raise self.__raise_error(response)
 
         elif model_key is not None:
             response = requests.request("GET",
                                         self.__url() + "mlmodels/",
                                         params={
                                             'key': model_key
                                         },
                                         headers=self.__header()
                                         )
             if response.status_code == 200:
+                obj = MLModel()
                 for obj_json in response.json():
-                    obj = MLModel()
-                    obj.from_json(obj_json)
-                    return obj
-                return None
-            else:
-                raise self.__raise_error(response)
-
-        elif template_key is not None:
-            response = requests.request("GET",
-                                        self.__url() + "templates/",
-                                        params={
-                                            'key': template_key
-                                        },
-                                        headers=self.__header()
-                                        )
-            if response.status_code == 200:
-                for obj_json in response.json():
-                    obj = Template()
-                    obj.from_json(obj_json)
-                    return obj
-                return None
-            else:
-                raise self.__raise_error(response)
-
-        elif twin_hardware_id is not None:
-            response = requests.request("GET",
-                                        self.__url() + "twins/",
-                                        params={
-                                            'key': twin_hardware_id
-                                        },
-                                        headers=self.__header()
-                                        )
-            if response.status_code == 200:
-                for obj_json in response.json():
-                    obj = Twin()
                     obj.from_json(obj_json)
-                    return obj
-                return None
+                return obj
             else:
                 raise self.__raise_error(response)
 
         elif obj is not None:
             if isinstance(obj, Execution):
                 response = requests.request("GET",
                                             self.__url() + "execute/" + str(obj.execution_id) + "/",
@@ -379,36 +285,26 @@
                                             headers=self.__header()
                                             )
                 if response.status_code == 200:
                     obj.from_json(response.json())
                     return obj
                 else:
                     raise self.__raise_error(response)
-            elif isinstance(obj, Template):
-                response = requests.request("GET",
-                                            self.__url() + "templates/" + str(obj.template_id) + "/",
-                                            headers=self.__header()
-                                            )
-                if response.status_code == 200:
-                    obj.from_json(response.json())
-                    return obj
-                else:
-                    raise self.__raise_error(response)
             else:
                 raise TypeError("Type not supported.")
 
     def create(self, obj):
         """
         create and save an object on the server
 
         :param obj: object to save on the server (any id is ignored and replaced)
         :return: id of created object
         """
         if callable(obj) and isinstance(obj, types.FunctionType):
-            obj = Script(
+            obj = wizata_dsapi.Script(
                 function=obj
             )
         if isinstance(obj, Script):
             response = requests.post(self.__url() + "scripts/",
                                      headers=self.__header(),
                                      data=dill.dumps(obj))
             if response.status_code == 200:
@@ -420,34 +316,26 @@
             response = requests.post(self.__url() + "experiments/",
                                      headers=self.__header(),
                                      data=json.dumps(obj.to_json()))
             if response.status_code == 200:
                 return
             else:
                 raise self.__raise_error(response)
-        elif isinstance(obj, Template):
-            response = requests.post(self.__url() + "templates/",
-                                     headers=self.__header(),
-                                     data=json.dumps(obj.to_json()))
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
         else:
             raise TypeError("Type not supported.")
 
     def update(self, obj):
         """
         update and save an object on the server
 
         :param obj: object to update on the server
         :return: None
         """
         if callable(obj) and isinstance(obj, types.FunctionType):
-            obj = Script(
+            obj = wizata_dsapi.Script(
                 function=obj
             )
         if isinstance(obj, Script):
             response = requests.put(self.__url() + "scripts/" + str(obj.script_id) + "/",
                                     headers=self.__header(),
                                     data=dill.dumps(obj))
             if response.status_code == 200:
@@ -458,35 +346,27 @@
             response = requests.put(self.__url() + "experiments/" + str(obj.experiment_id) + "/",
                                     headers=self.__header(),
                                     data=json.dumps(obj.to_json()))
             if response.status_code == 200:
                 return
             else:
                 raise self.__raise_error(response)
-        elif isinstance(obj, Template):
-            response = requests.put(self.__url() + "templates/" + str(obj.template_id) + "/",
-                                     headers=self.__header(),
-                                     data=json.dumps(obj.to_json()))
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
         else:
             raise TypeError("Type not supported.")
 
     def upsert(self, obj):
         """
         upsert on object on the server
         work with Script, MLModel or directly a function name
 
         :param obj: object to upsert on the server
         :return: ID of the object created or updated
         """
         if callable(obj) and isinstance(obj, types.FunctionType):
-            obj = Script(
+            obj = wizata_dsapi.Script(
                 function=obj
             )
         if isinstance(obj, Script):
             response = requests.put(self.__url() + "scripts/",
                                     headers=self.__header(),
                                     data=dill.dumps(obj))
             if response.status_code == 200:
@@ -499,16 +379,14 @@
                                     headers=self.__header(),
                                     data=pickle.dumps(obj))
             if response.status_code == 200:
                 obj.model_id = uuid.UUID(response.json()['id'])
                 return obj.model_id
             else:
                 raise self.__raise_error(response)
-        if isinstance(obj, Template):
-            return self.upsert_template(obj.key, obj.name)
         else:
             raise TypeError("Type not supported.")
 
     def delete(self, obj):
         """
         delete an object on the server
 
@@ -546,107 +424,72 @@
         elif isinstance(obj, DSDataFrame):
             response = requests.delete(self.__url() + "dataframes" + "/" + str(obj.df_id) + "/",
                                        headers=self.__header())
             if response.status_code == 200:
                 return
             else:
                 raise self.__raise_error(response)
-        elif isinstance(obj, Template):
-            response = requests.delete(self.__url() + "templates" + "/" + str(obj.template_id) + "/",
-                                       headers=self.__header())
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
         else:
             raise TypeError("Type not supported.")
 
     def query(self,
-              datapoints: list[str] = None,
-              start: datetime = None,
-              end: datetime = None,
-              interval: int = None,
+              datapoints: list[str],
+              start: datetime,
+              end: datetime,
+              interval: int,
               agg_method: str = "mean",
-              template: str = None,
-              twin: str = None,
-              null: str = None,
-              filters: dict = None,
-              options: dict = None) -> pandas.DataFrame:
+              null: str = None) -> pandas.DataFrame:
         """
         Query a dataframe from API.
         :param agg_method:
         :param datapoints: list of datapoints to fetch.
         :param start: start datetime of range to fetch
         :param end: end datetime of range to fetch
         :param interval: interval in milliseconds.
-        :param template: template to fetch.
-        :param twin: hardware ID of twin to fetch based on template.
         :param null: By default at 'drop' and dropping NaN values. If not intended behavior please set it to 'ignore' or 'all'.
-        :param filters: dict of filters.
-        :param options: dict of options.
         :return: dataframe
         """
-        request = Request()
+        request = wizata_dsapi.Request()
 
         if datapoints is not None:
             request.add_datapoints(datapoints)
 
         if start is not None:
             request.start = start
-        else:
-            raise ValueError('start datetime is required.')
 
         if end is not None:
             request.end = end
-        else:
-            raise ValueError('end datetime is required.')
 
         if null is not None:
             request.null = null
 
-        if interval is None:
-            raise ValueError('interval is required.')
         request.set_aggregation(agg_method, interval)
 
-        if template is not None and twin is not None:
-            request.select_template(
-                template_key=template,
-                twin_hardware_id=twin
-            )
-
-        if filters is not None:
-            request.filters = filters
-
-        if options is not None:
-            request.options = options
-
         return self.get(request)
 
     def execute(self,
                 execution: Execution = None,
                 request: Request = None,
                 dataframe=None,
                 script=None,
                 ml_model=None,
                 isAnomalyDetection=False,
                 function=None,
-                experiment=None,
-                properties: dict = None
+                experiment=None
                 ) -> Execution:
         """
         execute an experimentation on the server.
         :param execution: Execution to execute on the server with configuration (Request, Script, ML Model, ...)
         :param request: Request to use to generate a dataframe
         :param dataframe: dataframe to be used as input (pandas or DS API type)
         :param script: Script to be executed (accept Script,uuid or script function name)
         :param ml_model: MLModel to be executed (accept MLModel, ml_model(id) or uuid)
         :param isAnomalyDetection: set to true to execute automatic anomaly detection
         :param function: set to name of a built-in function to execute it
         :param experiment: ID or experiment to link the execution too
-        :param properties: dictionary of properties.
         :return: Execution updated with expected content (Data, Anomalies, Plots, ML Models, ...)
         """
         # Prepare
         if execution is None:
             execution = Execution()
         if request is not None:
             execution.request = request
@@ -676,16 +519,14 @@
         if experiment is not None:
             if isinstance(experiment, uuid.UUID):
                 execution.experiment_id = experiment
             elif isinstance(experiment, str):
                 execution.experiment_id = self.get(experiment_key=experiment).experiment_id
             elif isinstance(experiment, Experiment):
                 execution.experiment_id = experiment.experiment_id
-        if properties is not None and isinstance(properties, dict):
-            execution.properties = properties
 
         # Execute
         if isinstance(execution, Execution):
             response = requests.post(self.__url() + "execute/",
                                      headers=self.__header(),
                                      data=json.dumps(execution.to_json(), cls=DSAPIEncoder))
 
@@ -708,26 +549,24 @@
         else:
             raise TypeError("No execution have been loaded from parameters.")
 
     def validate(self,
                  execution: Execution = None,
                  request: Request = None,
                  dataframe=None,
-                 script=None,
-                 properties: dict = None) -> Script:
+                 script=None) -> Script:
         """
         run an execution to validate the script used.
         Do not store anything on the DS API nor return anything.
         In case of error, set the Script as invalid.
 
         :param execution: Execution to validate - must contain a dataframe or a query and a script
         :param request: Request to use to generate a dataframe
         :param dataframe: dataframe to be used as input (pandas or DS API type)
         :param script: Script to be executed (accept Script, string(id) or uuid)
-        :param properties: dictionary of properties.
         :return: validated script properties (do not use update or it will invalidate the script)
         """
         if execution is None:
             execution = Execution()
         if request is not None:
             execution.request = request
         if dataframe is not None:
@@ -738,18 +577,14 @@
         if script is not None:
             if isinstance(script, uuid.UUID):
                 execution.script = Script(script)
             elif isinstance(script, str):
                 execution.script = self.get(script_name=script)
             elif isinstance(script, Script):
                 execution.script = script
-
-        if properties is not None and isinstance(properties, dict):
-            execution.properties = properties
-
         if isinstance(execution, Execution):
             if execution.script is None:
                 raise ValueError("Execution must contains at least a Script.")
             response = requests.post(self.__url() + "execute/validate",
                                      headers=self.__header(),
                                      data=json.dumps(execution.to_json(), cls=DSAPIEncoder))
             if response.status_code == 200:
@@ -764,30 +599,28 @@
     def test(self,
              execution: Execution = None,
              request: Request = None,
              dataframe=None,
              script=None,
              ml_model=None,
              detect_anomalies=False,
-             function=None,
-             properties: dict = None
+             function=None
              ) -> Execution:
         """
         test an experimentation on the server.
 
         DO NOT STORE ANYTHING ON SERVER.
 
         :param execution: Execution to execute on the server with configuration (Request, Script, ML Model, ...)
         :param request: Request to use to generate a dataframe
         :param dataframe: dataframe to be used as input (pandas or DS API type)
         :param script: Script to be executed (accept Script, string(id) or uuid)
         :param ml_model: MLModel to be executed (accept MLModel, ml_model(id) or uuid)
         :param detect_anomalies: set to true to execute automatic anomaly detection
         :param function: set to name of a built-in function to execute it
-        :param properties: dictionary of properties.
         :return: Execution updated with expected content (Data, Anomalies, Plots, ML Models, ...)
         """
         # Prepare
         if execution is None:
             execution = Execution()
         if request is not None:
             execution.request = request
@@ -811,32 +644,29 @@
             elif isinstance(ml_model, MLModel):
                 execution.ml_model = ml_model
         if detect_anomalies:
             execution.isAnomalyDetection = True
         if function is not None:
             execution.function = function
 
-        if properties is not None and isinstance(properties, dict):
-            execution.properties = properties
-
         # Execute
         if isinstance(execution, Execution):
             if execution.script is None and execution.ml_model is None:
                 raise ValueError("Execution must contains at least a Script or a Model")
             response = requests.post(self.__url() + "execute/test",
                                      headers=self.__header(),
                                      data=json.dumps(execution.to_json(), cls=DSAPIEncoder))
             if response.status_code == 200:
                 return dill.loads(response.content)
             else:
                 raise self.__raise_error(response)
         else:
             raise TypeError("Type not supported.")
 
-    def plot(self, plot_id: str = None, plot: Plot = None, figure=None,):
+    def plot(self, plot_id: str = None, plot: wizata_dsapi = None, figure=None,):
         """
         Fetch and show plot.
         :param plot: Wizata Plot Object
         :param figure: JSON Figure
         :param plot_id: Plot Id
         :return:
         """
@@ -847,15 +677,15 @@
             if plot.figure is not None:
                 return plotly.io.from_json(plot.figure)
             else:
                 raise ValueError('No plot has been fetch.')
         elif figure is not None:
             return plotly.io.from_json(plot.figure)
         elif id is not None:
-            plot = self.get(Plot(plot_id=plot_id))
+            plot = self.get(wizata_dsapi.Plot(plot_id=plot_id))
             if plot.figure is not None:
                 return plotly.io.from_json(plot.figure)
             else:
                 raise ValueError('No plot has been fetch.')
         else:
             raise KeyError('No valid arguments.')
 
@@ -883,15 +713,15 @@
             raise ValueError('Please provide a str Model Key to identify the model.')
         if train_model is None:
             raise ValueError('Trained Machine Learning model should not be null')
         elif df is None:
             raise ValueError('A sample dataframe must be provided')
 
         # Create a ML Model object
-        ml_model = MLModel()
+        ml_model = wizata_dsapi.MLModel()
         ml_model.trained_model = train_model
         if scaler is not None:
             ml_model.scaler = scaler
         ml_model.has_anomalies = has_anomalies
         ml_model.has_target_feat = has_target_feat
         ml_model.input_columns = df.columns
         ml_model.key = model_key
@@ -906,261 +736,34 @@
                 self.upsert(ml_model)
                 return ml_model, result_df
             else:
                 raise RuntimeError('no dataframe was generated by your model while testing predict capabilities')
         except Exception as e:
             raise RuntimeError('not able to validated the model : ' + str(e))
 
-    def upsert_template(self, key: str, name: str):
-        """
-        Upsert a template.
-        :param key: unique key identifying the template.
-        :param name: display name of the template
-        :return: upserted template.
-        """
-
-        template = self.get(template_key=key)
-        if template is not None:
-            found = True
-        else:
-            template = Template(
-                key=key,
-                name=name
-            )
-            found = False
-
-        if not found:
-            return self.create(template)
-        else:
-            return self.update(template)
-
-    def add_template_property(self, template, property_name: str, property_type: str = "datapoint"):
-
-        if property_type not in ['datapoint', 'float', 'integer', 'string']:
-            raise ValueError('property type must be datapoint, float, integer or string')
-
-        if isinstance(template, str):
-            template = self.get(template_key=template)
-        elif not isinstance(template, Template):
-            raise TypeError('template must be a key str referring template or a proper wizata_dsapi Template')
-
-        if property_name is None:
-            raise ValueError('please provide a valid name for the property')
-
-        property_dict = {
-            "type": property_type,
-            "name": property_name
-        }
-
-        response = requests.post(self.__url() + "templates/" + str(template.template_id) + '/properties/',
-                                 headers=self.__header(),
-                                 data=json.dumps(property_dict))
-        if response.status_code == 200:
-            return
-        else:
-            raise self.__raise_error(response)
-
-    def remove_template_property(self, template, property_name: str):
-
-        if isinstance(template, str):
-            template = self.get(template_key=template)
-        elif not isinstance(template, Template):
-            raise TypeError('template must be a key str referring template or a proper wizata_dsapi Template')
-
-        if property_name is None:
-            raise ValueError('please provide a valid name for the property')
-
-        property_dict = {
-            "name": property_name
-        }
-
-        response = requests.delete(self.__url() + "templates/" + str(template.template_id) + '/properties/',
-                                   headers=self.__header(),
-                                   data=json.dumps(property_dict))
-        if response.status_code == 200:
-            return
-        else:
-            raise self.__raise_error(response)
-
-    def get_registrations(self, template) -> list:
-        """
-        retrieve all registrations for
-        :param template: template object, UUID or str key.
-        :return: list of twin registration.
-        """
-
-        if template is None:
-            raise ValueError('template must be specified.')
-        elif isinstance(template, uuid.UUID):
-            template = self.get(wizata_dsapi.Template(template_id=template))
-        elif isinstance(template, str):
-            template = self.get(template_key=template)
-        elif not isinstance(template, Template):
-            raise TypeError('template must be UUID, a key str referring template or a proper wizata_dsapi Template')
-        if template is None:
-            raise ValueError('template cannot be found on server')
-
-        response = requests.get(self.__url() + "templates/" + str(template.template_id) + '/registrations/',
-                                headers=self.__header())
-        if response.status_code == 200:
-            registrations_json = response.json()
-            registrations = []
-            for twin_registration_json in registrations_json:
-                registration = TwinRegistration()
-                registration.from_json(twin_registration_json)
-                registrations.append(registration)
-            return registrations
-        else:
-            raise self.__raise_error(response)
-
-    def register_twin(self, template, twin, properties: dict, override=True):
-        """
-        register a twin on a specific template using a map.
-        :param template: template object, UUID or str key.
-        :param twin: twin object, UUID or str key.
-        :param properties: dict where key = template property and value = datapoint name or const value (str, int or float).
-        :param override: by default at True - allow overriding any existing subscription
-        """
-
-        if template is None:
-            raise ValueError('template must be specified.')
-        elif isinstance(template, uuid.UUID):
-            template = self.get(wizata_dsapi.Template(template_id=template))
-        elif isinstance(template, str):
-            template = self.get(template_key=template)
-        elif not isinstance(template, Template):
-            raise TypeError('template must be UUID, a key str referring template or a proper wizata_dsapi Template')
-
-        if template is None:
-            raise ValueError('template cannot be found on server')
-
-        if twin is None:
-            raise ValueError('twin must be specified.')
-        elif isinstance(twin, uuid.UUID):
-            twin_id = twin
-        elif isinstance(twin, str):
-            twin_id = self.get(twin_hardware_id=twin).twin_id
-        elif isinstance(twin, Twin):
-            twin_id = twin.twin_id
-        else:
-            raise TypeError('twin must be UUID, a key str referring hardware ID or a proper wizata_dsapi Twin')
-
-        if template.properties is None or len(template.properties) == 0:
-            raise ValueError('template chosen does not contains any properties')
-
-        if properties is None or len(properties.keys()) == 0:
-            raise ValueError('your map dictionary must contains properties matching template')
-
-        twin_properties = {
-            "properties": []
-        }
-        for key in properties.keys():
-            property_type = None
-            for template_property in template.properties:
-                if key == template_property['name']:
-                    property_type = template_property['type']
-            if property_type is None:
-                raise ValueError(f'cannot find property {key} in template or cannot determine its type')
-            twin_properties["properties"].append({
-                'name': key,
-                property_type: properties[key]
-            })
-
-        # Check if already exist
-        exists = False
-        response_exists = requests.get(self.__url() + "templates/" + str(template.template_id)
-                                       + '/registrations/' + str(twin_id) + '/',
-                                       headers=self.__header())
-        if response_exists.status_code == 200:
-            exists = True
-
-        if exists and not override:
-            raise ValueError("registration already exists and override not allowed.")
-
-        if exists and override:
-            response = requests.put(self.__url() + "templates/" + str(template.template_id)
-                                    + '/registrations/' + str(twin_id) + '/',
-                                    headers=self.__header(),
-                                    data=json.dumps(twin_properties))
-        else:
-            response = requests.post(self.__url() + "templates/" + str(template.template_id)
-                                     + '/registrations/' + str(twin_id) + '/',
-                                     headers=self.__header(),
-                                     data=json.dumps(twin_properties))
-
-        if response.status_code == 200:
-            return
-        else:
-            raise self.__raise_error(response)
-
-    def unregister_twin(self, template, twin):
-        """
-        un-register a twin from a specific template.
-        :param template: template object, UUID or str key.
-        :param twin: twin object, UUID or str key.
-        """
-
-        if template is None:
-            raise ValueError('template must be specified.')
-        elif isinstance(template, uuid.UUID):
-            template = self.get(wizata_dsapi.Template(template_id=template))
-        elif isinstance(template, str):
-            template = self.get(template_key=template)
-        elif not isinstance(template, Template):
-            raise TypeError('template must be UUID, a key str referring template or a proper wizata_dsapi Template')
-
-        if twin is None:
-            raise ValueError('twin must be specified.')
-        elif isinstance(twin, uuid.UUID):
-            twin_id = twin
-        elif isinstance(twin, str):
-            twin_id = self.get(twin_hardware_id=twin).twin_id
-        elif isinstance(twin, Twin):
-            twin_id = twin.twin_id
-        else:
-            raise TypeError('twin must be UUID, a key str referring hardware ID or a proper wizata_dsapi Twin')
-
-        response = requests.delete(self.__url() + "templates/" + str(template.template_id)
-                                   + '/registrations/' + str(twin_id) + '/',
-                                   headers=self.__header())
-        if response.status_code == 200:
-            return
-        else:
-            raise self.__raise_error(response)
-
 
 def api() -> WizataDSAPIClient:
     """
     Create a WizataDSAPIClient from environment variables.
     :return: client
     """
     protocol = 'https'
 
     if os.environ.get('WIZATA_PROTOCOL') is not None:
         protocol = os.environ.get('WIZATA_PROTOCOL')
 
-    if os.environ.get('WIZATA_CLIENT_SECRET') is not None:
-        return WizataDSAPIClient(
-            tenant_id=os.environ.get('WIZATA_TENANT_ID'),
-            client_id=os.environ.get('WIZATA_CLIENT_ID'),
-            client_secret=os.environ.get('WIZATA_CLIENT_SECRET'),
-            scope=os.environ.get('WIZATA_CLIENT_ID') + '/.default',
-            domain=os.environ.get('WIZATA_DOMAIN'),
-            protocol=protocol
-        )
-    else:
-        return WizataDSAPIClient(
-            tenant_id=os.environ.get('WIZATA_TENANT_ID'),
-            client_id=os.environ.get('WIZATA_CLIENT_ID'),
-            scope=os.environ.get('WIZATA_SCOPE'),
-            username=os.environ.get('WIZATA_USERNAME'),
-            password=os.environ.get('WIZATA_PASSWORD'),
-            domain=os.environ.get('WIZATA_DOMAIN'),
-            protocol=protocol
-        )
+    return WizataDSAPIClient(
+        tenant_id=os.environ.get('WIZATA_TENANT_ID'),
+        client_id=os.environ.get('WIZATA_CLIENT_ID'),
+        scope=os.environ.get('WIZATA_SCOPE'),
+        username=os.environ.get('WIZATA_USERNAME'),
+        password=os.environ.get('WIZATA_PASSWORD'),
+        domain=os.environ.get('WIZATA_DOMAIN'),
+        protocol=protocol
+    )
 
 
 def is_valid_uuid(val):
     try:
         uuid.UUID(str(val))
         return True
     except ValueError:
```

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.1.9/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 LICENSE.txt
 README.rst
 setup.py
 wizata_dsapi/__init__.py
 wizata_dsapi/api_dto.py
 wizata_dsapi/dataframe_toolkit.py
-wizata_dsapi/datapoint.py
 wizata_dsapi/ds_dataframe.py
 wizata_dsapi/dsapi_json_encoder.py
 wizata_dsapi/execution.py
 wizata_dsapi/experiment.py
 wizata_dsapi/mlmodel.py
 wizata_dsapi/model_toolkit.py
-wizata_dsapi/pipeline.py
 wizata_dsapi/plot.py
 wizata_dsapi/request.py
 wizata_dsapi/script.py
+wizata_dsapi/sql_dto.py
 wizata_dsapi/template.py
 wizata_dsapi/twin.py
 wizata_dsapi/twinregistration.py
 wizata_dsapi/wizard_function.py
 wizata_dsapi/wizata_dsapi_client.py
 wizata_dsapi.egg-info/PKG-INFO
 wizata_dsapi.egg-info/SOURCES.txt
```

### Comparing `wizata-dsapi-0.1.80/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.1.9/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

