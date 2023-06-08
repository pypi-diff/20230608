# Comparing `tmp/pipeline_ai-0.5.0b2.tar.gz` & `tmp/pipeline_ai-0.5.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_ai-0.5.0b2.tar", max compression
+gzip compressed data, was "pipeline_ai-0.5.0b3.tar", max compression
```

## Comparing `pipeline_ai-0.5.0b2.tar` & `pipeline_ai-0.5.0b3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0    10176 2023-06-07 10:41:11.051565 pipeline_ai-0.5.0b2/LICENSE
--rw-r--r--   0        0        0     6130 2023-06-07 10:41:11.051565 pipeline_ai-0.5.0b2/README.md
--rw-r--r--   0        0        0      434 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/__init__.py
--rw-r--r--   0        0        0      135 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/__main__.py
--rw-r--r--   0        0        0       62 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/api/__init__.py
--rw-r--r--   0        0        0       62 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/api/asyncio/__init__.py
--rw-r--r--   0        0        0     8380 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/api/asyncio/cloud.py
--rw-r--r--   0        0        0    29923 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/api/cloud.py
--rw-r--r--   0        0        0      974 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/api/environments.py
--rw-r--r--   0        0        0     3247 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/configuration/__init__.py
--rw-r--r--   0        0        0    11693 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/console/__init__.py
--rw-r--r--   0        0        0     8254 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/console/environments.py
--rw-r--r--   0        0        0     2587 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/console/remote.py
--rw-r--r--   0        0        0     2011 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/console/runs.py
--rw-r--r--   0        0        0     4838 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/console/tags.py
--rw-r--r--   0        0        0     4868 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/docker/__init__.py
--rw-r--r--   0        0        0      276 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/exceptions/InvalidSchema.py
--rw-r--r--   0        0        0      283 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/exceptions/MissingActiveToken.py
--rw-r--r--   0        0        0      312 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/exceptions/NonChargeableProfile.py
--rw-r--r--   0        0        0      309 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/exceptions/PipelineNotDeployed.py
--rw-r--r--   0        0        0      546 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/__init__.py
--rw-r--r--   0        0        0     4752 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/decorators.py
--rw-r--r--   0        0        0     1528 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/environment/__init__.py
--rw-r--r--   0        0        0     2015 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/function.py
--rw-r--r--   0        0        0    10909 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/graph.py
--rw-r--r--   0        0        0      877 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/graph_node.py
--rw-r--r--   0        0        0     1091 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/huggingface/TransformersModelForCausalLM.py
--rw-r--r--   0        0        0        0 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/huggingface/__init__.py
--rw-r--r--   0        0        0     1161 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/model.py
--rw-r--r--   0        0        0     3474 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/pipeline.py
--rw-r--r--   0        0        0     1861 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/variable.py
--rw-r--r--   0        0        0     1712 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/wrappers.py
--rw-r--r--   0        0        0        0 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/schemas/__init__.py
--rw-r--r--   0        0        0     1821 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/schemas/base.py
--rw-r--r--   0        0        0      369 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/schemas/compute_requirements.py
--rw-r--r--   0        0        0      558 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/schemas/data.py
--rw-r--r--   0        0        0      573 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/schemas/deployment.py
--rw-r--r--   0        0        0      516 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/schemas/environment.py
--rw-r--r--   0        0        0      714 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/schemas/file.py
--rw-r--r--   0        0        0     2426 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/function.py
--rw-r--r--   0        0        0     5236 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/metrics.py
--rw-r--r--   0        0        0      569 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/milestones_register.py
--rw-r--r--   0        0        0     1599 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/model.py
--rw-r--r--   0        0        0      739 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/onboarding.py
--rw-r--r--   0        0        0      944 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/pagination.py
--rw-r--r--   0        0        0     5817 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/pipeline.py
--rw-r--r--   0        0        0     1261 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/pipeline_file.py
--rw-r--r--   0        0        0      537 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/project.py
--rw-r--r--   0        0        0        0 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/redis/__init__.py
--rw-r--r--   0        0        0      234 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/redis/command.py
--rw-r--r--   0        0        0      337 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/request.py
--rw-r--r--   0        0        0      261 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/resource.py
--rw-r--r--   0        0        0     3839 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/run.py
--rw-r--r--   0        0        0     1031 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/runnable.py
--rw-r--r--   0        0        0      167 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/tag.py
--rw-r--r--   0        0        0     1668 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/token.py
--rw-r--r--   0        0        0     3827 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/user.py
--rw-r--r--   0        0        0     2493 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/validators.py
--rw-r--r--   0        0        0      320 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/worker.py
--rw-r--r--   0        0        0     1924 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/util/__init__.py
--rw-r--r--   0        0        0     1129 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/util/logging.py
--rw-r--r--   0        0        0      241 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/util/torch_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/v3/__init__.py
--rw-r--r--   0        0        0      287 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/v3/environments.py
--rw-r--r--   0        0        0     3131 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/v3/http.py
--rw-r--r--   0        0        0     3701 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/v3/pipelines.py
--rw-r--r--   0        0        0        0 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/v3/schemas/__init__.py
--rw-r--r--   0        0        0     2172 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/v3/schemas/runs.py
--rw-r--r--   0        0        0     4571 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/v3/uploading.py
--rw-r--r--   0        0        0     1249 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pyproject.toml
--rw-r--r--   0        0        0     7132 1970-01-01 00:00:00.000000 pipeline_ai-0.5.0b2/PKG-INFO
+-rw-r--r--   0        0        0    10176 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/LICENSE
+-rw-r--r--   0        0        0     6130 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/README.md
+-rw-r--r--   0        0        0      434 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/__init__.py
+-rw-r--r--   0        0        0      135 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/__main__.py
+-rw-r--r--   0        0        0       62 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/api/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/api/asyncio/__init__.py
+-rw-r--r--   0        0        0     8380 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/api/asyncio/cloud.py
+-rw-r--r--   0        0        0    29923 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/api/cloud.py
+-rw-r--r--   0        0        0      974 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/api/environments.py
+-rw-r--r--   0        0        0     3247 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/configuration/__init__.py
+-rw-r--r--   0        0        0    11693 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/console/__init__.py
+-rw-r--r--   0        0        0     8254 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/console/environments.py
+-rw-r--r--   0        0        0     2587 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/console/remote.py
+-rw-r--r--   0        0        0     2011 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/console/runs.py
+-rw-r--r--   0        0        0     4838 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/console/tags.py
+-rw-r--r--   0        0        0     4868 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/docker/__init__.py
+-rw-r--r--   0        0        0      276 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/exceptions/InvalidSchema.py
+-rw-r--r--   0        0        0      283 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/exceptions/MissingActiveToken.py
+-rw-r--r--   0        0        0      312 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/exceptions/NonChargeableProfile.py
+-rw-r--r--   0        0        0      309 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/exceptions/PipelineNotDeployed.py
+-rw-r--r--   0        0        0      546 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/__init__.py
+-rw-r--r--   0        0        0     4752 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/decorators.py
+-rw-r--r--   0        0        0     1528 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/environment/__init__.py
+-rw-r--r--   0        0        0     2015 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/function.py
+-rw-r--r--   0        0        0    10909 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/graph.py
+-rw-r--r--   0        0        0      877 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/graph_node.py
+-rw-r--r--   0        0        0     1091 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/huggingface/TransformersModelForCausalLM.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/huggingface/__init__.py
+-rw-r--r--   0        0        0     1161 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/model.py
+-rw-r--r--   0        0        0     3488 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/pipeline.py
+-rw-r--r--   0        0        0     1861 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/variable.py
+-rw-r--r--   0        0        0     1712 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/objects/wrappers.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:28:01.979241 pipeline_ai-0.5.0b3/pipeline/schemas/__init__.py
+-rw-r--r--   0        0        0     1821 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/base.py
+-rw-r--r--   0        0        0      369 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/compute_requirements.py
+-rw-r--r--   0        0        0      558 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/data.py
+-rw-r--r--   0        0        0      573 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/deployment.py
+-rw-r--r--   0        0        0      516 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/environment.py
+-rw-r--r--   0        0        0      714 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/file.py
+-rw-r--r--   0        0        0     2426 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/function.py
+-rw-r--r--   0        0        0     5236 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/metrics.py
+-rw-r--r--   0        0        0      569 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/milestones_register.py
+-rw-r--r--   0        0        0     1599 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/model.py
+-rw-r--r--   0        0        0      739 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/onboarding.py
+-rw-r--r--   0        0        0      944 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/pagination.py
+-rw-r--r--   0        0        0     5817 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/pipeline.py
+-rw-r--r--   0        0        0     1261 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/pipeline_file.py
+-rw-r--r--   0        0        0      537 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/project.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/redis/__init__.py
+-rw-r--r--   0        0        0      234 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/redis/command.py
+-rw-r--r--   0        0        0      337 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/request.py
+-rw-r--r--   0        0        0      261 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/resource.py
+-rw-r--r--   0        0        0     3839 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/run.py
+-rw-r--r--   0        0        0     1031 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/runnable.py
+-rw-r--r--   0        0        0      167 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/tag.py
+-rw-r--r--   0        0        0     1668 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/token.py
+-rw-r--r--   0        0        0     3827 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/user.py
+-rw-r--r--   0        0        0     2493 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/validators.py
+-rw-r--r--   0        0        0      320 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/schemas/worker.py
+-rw-r--r--   0        0        0     1924 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/util/__init__.py
+-rw-r--r--   0        0        0     1129 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/util/logging.py
+-rw-r--r--   0        0        0      241 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/util/torch_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/v3/__init__.py
+-rw-r--r--   0        0        0      287 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/v3/environments.py
+-rw-r--r--   0        0        0     3131 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/v3/http.py
+-rw-r--r--   0        0        0     4354 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/v3/pipelines.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/v3/schemas/__init__.py
+-rw-r--r--   0        0        0     3769 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/v3/schemas/runs.py
+-rw-r--r--   0        0        0     4571 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pipeline/v3/uploading.py
+-rw-r--r--   0        0        0     1249 2023-06-08 16:28:01.983241 pipeline_ai-0.5.0b3/pyproject.toml
+-rw-r--r--   0        0        0     7132 1970-01-01 00:00:00.000000 pipeline_ai-0.5.0b3/PKG-INFO
```

### Comparing `pipeline_ai-0.5.0b2/LICENSE` & `pipeline_ai-0.5.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/README.md` & `pipeline_ai-0.5.0b3/README.md`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/api/asyncio/cloud.py` & `pipeline_ai-0.5.0b3/pipeline/api/asyncio/cloud.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/api/cloud.py` & `pipeline_ai-0.5.0b3/pipeline/api/cloud.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/api/environments.py` & `pipeline_ai-0.5.0b3/pipeline/api/environments.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/configuration/__init__.py` & `pipeline_ai-0.5.0b3/pipeline/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/console/__init__.py` & `pipeline_ai-0.5.0b3/pipeline/console/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/console/environments.py` & `pipeline_ai-0.5.0b3/pipeline/console/environments.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/console/remote.py` & `pipeline_ai-0.5.0b3/pipeline/console/remote.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/console/runs.py` & `pipeline_ai-0.5.0b3/pipeline/console/runs.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/console/tags.py` & `pipeline_ai-0.5.0b3/pipeline/console/tags.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/docker/__init__.py` & `pipeline_ai-0.5.0b3/pipeline/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/objects/__init__.py` & `pipeline_ai-0.5.0b3/pipeline/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/objects/decorators.py` & `pipeline_ai-0.5.0b3/pipeline/objects/decorators.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/objects/environment/__init__.py` & `pipeline_ai-0.5.0b3/pipeline/objects/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/objects/function.py` & `pipeline_ai-0.5.0b3/pipeline/objects/function.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/objects/graph.py` & `pipeline_ai-0.5.0b3/pipeline/objects/graph.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/objects/graph_node.py` & `pipeline_ai-0.5.0b3/pipeline/objects/graph_node.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/objects/huggingface/TransformersModelForCausalLM.py` & `pipeline_ai-0.5.0b3/pipeline/objects/huggingface/TransformersModelForCausalLM.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/objects/model.py` & `pipeline_ai-0.5.0b3/pipeline/objects/model.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/objects/pipeline.py` & `pipeline_ai-0.5.0b3/pipeline/objects/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 from pipeline.objects.function import Function
 from pipeline.objects.graph import Graph
 from pipeline.objects.graph_node import GraphNode
 from pipeline.objects.variable import Variable
 
 
 class Pipeline:
@@ -70,15 +71,14 @@
             return Pipeline.defined_pipelines[graph_name]
         else:
             raise Exception("No Pipeline graph found with name '%s'" % graph_name)
 
     @staticmethod
     def add_variable(variable: Variable) -> None:
         if Pipeline._pipeline_context_active:
-
             if variable not in Pipeline._current_pipeline.variables:
                 Pipeline._current_pipeline.variables.append(variable)
         else:
             raise Exception("Cant add a variable when not defining a pipeline!")
 
     @staticmethod
     def add_variables(*variables: Variable) -> None:
```

### Comparing `pipeline_ai-0.5.0b2/pipeline/objects/variable.py` & `pipeline_ai-0.5.0b3/pipeline/objects/variable.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/objects/wrappers.py` & `pipeline_ai-0.5.0b3/pipeline/objects/wrappers.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/base.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/base.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/data.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/data.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/deployment.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/deployment.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/environment.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/environment.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/file.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/file.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/function.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/function.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/metrics.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/metrics.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/milestones_register.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/milestones_register.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/model.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/model.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/onboarding.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/onboarding.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/pagination.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/pagination.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/pipeline.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/pipeline.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/pipeline_file.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/pipeline_file.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/project.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/project.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/run.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/run.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/runnable.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/runnable.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/token.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/token.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/user.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/user.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/schemas/validators.py` & `pipeline_ai-0.5.0b3/pipeline/schemas/validators.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/util/__init__.py` & `pipeline_ai-0.5.0b3/pipeline/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/util/logging.py` & `pipeline_ai-0.5.0b3/pipeline/util/logging.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/v3/http.py` & `pipeline_ai-0.5.0b3/pipeline/v3/http.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pipeline/v3/pipelines.py` & `pipeline_ai-0.5.0b3/pipeline/v3/pipelines.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import cloudpickle as cp
 import httpx
 
 from pipeline.objects import Graph, PipelineFile
 from pipeline.util.logging import _print
 from pipeline.v3 import http
-from pipeline.v3.schemas.runs import Run
+from pipeline.v3.schemas.runs import Run, RunInput, RunIOType, RunCreate
 
 
 def upload_pipeline(
     graph: Graph,
     environment_id_or_name: t.Union[str, int],
 ):
     if graph._has_run_startup:
@@ -64,30 +64,50 @@
     )
 
     graph_file.close()
 
     return res
 
 
+def _data_to_run_input(data: t.Any) -> t.List[RunInput]:
+    input_array = []
+
+    for item in data:
+        input_type = RunIOType.from_object(item)
+        if input_type == RunIOType.file:
+            raise NotImplementedError("File input not yet supported")
+        elif input_type == RunIOType.pkl:
+            raise NotImplementedError("Python object input not yet supported")
+
+        input_schema = RunInput(
+            type=input_type,
+            value=item,
+        )
+        input_array.append(input_schema)
+
+    return input_array
+
+
 def run_pipeline(
-    graph_id: str,
-    data: t.Any,
-    *,
-    return_response: bool = False,
+    pipeline_id_or_tag: t.Union[str, int],
+    *data,
     async_run: bool = False,
+    return_response: bool = False,
 ) -> t.Union[Run, httpx.Response]:
     data_obj = io.BytesIO(cp.dumps(data))
 
-    res = http.post_files(
+    run_create_schema = RunCreate(
+        pipeline_id_or_tag=pipeline_id_or_tag,
+        input_data=_data_to_run_input(data),
+        async_run=async_run,
+    )
+
+    res = http.post(
         "/v3/runs",
-        params=dict(
-            graph_id=graph_id,
-            async_run=async_run,
-        ),
-        files=dict(input_data=data_obj),
+        json_data=run_create_schema.dict(),
     )
 
     if return_response:
         return res
 
     if res.status_code == 500:
         _print(
```

### Comparing `pipeline_ai-0.5.0b2/pipeline/v3/schemas/runs.py` & `pipeline_ai-0.5.0b3/pipeline/v3/schemas/runs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import io
 import typing as t
 from datetime import datetime
 from enum import Enum
+import json
 
 from pydantic import BaseModel
 
 
 class RunState(int, Enum):
     created: int = 0
     routing: int = 1
@@ -74,32 +76,101 @@
     path: str
 
     class Config:
         # use_enum_values = True
         orm_mode = True
 
 
+class RunIOType(str, Enum):
+    integer: str = "integer"
+    string: str = "string"
+    fp: str = "fp"
+    dictionary: str = "dictionary"
+    boolean: str = "boolean"
+    none: str = "none"
+
+    pkl: str = "pkl"
+    file: str = "file"
+
+    @classmethod
+    def from_object(cls, obj: t.Any):
+        # Get the enum type for the object.
+        if isinstance(obj, int):
+            return cls.integer
+        elif isinstance(obj, float):
+            return cls.fp
+        elif isinstance(obj, str):
+            return cls.string
+        elif isinstance(obj, bool):
+            return cls.boolean
+        elif obj is None:
+            return cls.none
+        elif isinstance(obj, dict):
+            try:
+                json.dumps(obj)
+            except (TypeError, OverflowError):
+                return cls.pkl
+            return cls.dictionary
+        elif isinstance(obj, io.BufferedIOBase):
+            return cls.file
+        else:
+            return cls.pkl
+
+
+class RunOutputFile(BaseModel):
+    name: str
+    path: str
+    url: str
+    size: int
+
+
+class RunOutput(BaseModel):
+    type: RunIOType
+    value: t.Optional[t.Any]
+    file: t.Optional[RunOutputFile]
+
+
+class RunResult(BaseModel):
+    run_id: int
+    outputs: t.List[RunOutput]
+
+    def result_array(self) -> t.List[t.Any]:
+        return [output.value for output in self.outputs]
+
+
 class Run(BaseModel):
     id: int
 
+    created_at: datetime
+
     pipeline_id: int
     environment_id: int
     environment_hash: str
 
     state: RunState
     error: t.Optional[RunError]
 
-    result: t.Optional[t.Any]
-
-    files: t.Optional[t.List[RunFile]]
-
-    created_at: datetime
+    result: t.Optional[RunResult]
 
     class Config:
         # use_enum_values = True
         orm_mode = True
 
 
 class RunStateTransition(BaseModel):
     run_id: int
     new_state: RunState
     time: datetime
+
+
+class RunInput(BaseModel):
+    type: RunIOType
+    value: t.Any
+
+    file_name: t.Optional[str]
+    file_path: t.Optional[str]
+
+
+class RunCreate(BaseModel):
+    pipeline_id_or_tag: t.Union[int, str]
+    input_data: t.List[RunInput]
+    async_run: bool = False
```

### Comparing `pipeline_ai-0.5.0b2/pipeline/v3/uploading.py` & `pipeline_ai-0.5.0b3/pipeline/v3/uploading.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b2/pyproject.toml` & `pipeline_ai-0.5.0b3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipeline-ai"
-version = "0.5.0b2"
+version = "0.5.0b3"
 
 description = "Pipelines for machine learning workloads."
 authors = [
   "Paul Hetherington <ph@mystic.ai>",
   "Alex Pearwin <alex@mystic.ai>",
   "Neil Wang <neil@mystic.ai>",
   "Ross Gray <ross@mystic.ai>",
```

### Comparing `pipeline_ai-0.5.0b2/PKG-INFO` & `pipeline_ai-0.5.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-ai
-Version: 0.5.0b2
+Version: 0.5.0b3
 Summary: Pipelines for machine learning workloads.
 License: Apache-2.0
 Author: Paul Hetherington
 Author-email: ph@mystic.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

