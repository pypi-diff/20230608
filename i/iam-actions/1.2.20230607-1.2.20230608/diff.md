# Comparing `tmp/iam_actions-1.2.20230607.tar.gz` & `tmp/iam_actions-1.2.20230608.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230607.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230608.tar", max compression
```

## Comparing `iam_actions-1.2.20230607.tar` & `iam_actions-1.2.20230608.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/README.md
--rw-r--r--   0        0        0      228 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/__init__.py
--rw-r--r--   0        0        0  4294396 2023-06-07 02:50:27.539640 iam_actions-1.2.20230607/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-07 02:48:33.539629 iam_actions-1.2.20230607/iam_actions/generate/services.py
--rw-r--r--   0        0        0   552341 2023-06-07 02:50:27.539640 iam_actions-1.2.20230607/iam_actions/policies.json
--rw-r--r--   0        0        0   195776 2023-06-07 02:50:27.539640 iam_actions-1.2.20230607/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   535757 2023-06-07 02:50:27.539640 iam_actions-1.2.20230607/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-07 02:50:28.327637 iam_actions-1.2.20230607/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230607/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230607/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-08 02:47:50.052026 iam_actions-1.2.20230608/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-08 02:47:50.052026 iam_actions-1.2.20230608/README.md
+-rw-r--r--   0        0        0      228 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4297233 2023-06-08 02:49:24.485743 iam_actions-1.2.20230608/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-08 02:47:50.056026 iam_actions-1.2.20230608/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   552341 2023-06-08 02:49:24.485743 iam_actions-1.2.20230608/iam_actions/policies.json
+-rw-r--r--   0        0        0   196565 2023-06-08 02:49:24.485743 iam_actions-1.2.20230608/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   535757 2023-06-08 02:49:24.485743 iam_actions-1.2.20230608/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-08 02:49:25.257757 iam_actions-1.2.20230608/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230608/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230608/PKG-INFO
```

### Comparing `iam_actions-1.2.20230607/LICENSE` & `iam_actions-1.2.20230608/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230607/README.md` & `iam_actions-1.2.20230608/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230607/iam_actions/actions.json` & `iam_actions-1.2.20230608/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998478711675816%*

 * *Differences: {"'finspace'": "{'ListTagsForResource': {'access_level': 'List', 'resources': {insert: [(1, "*

 * *               "'kxCluster'), (2, 'kxDatabase'), (3, 'kxEnvironment'), (4, 'kxUser')]}}, "*

 * *               "'TagResource': {'condition_keys': ['aws:RequestTag/${TagKey}', 'aws:TagKeys'], "*

 * *               "'resources': {insert: [(1, 'kxCluster'), (2, 'kxDatabase'), (3, 'kxEnvironment'), "*

 * *               "(4, 'kxUser')]}}, 'UntagResource': {'condition_keys': ['aws:TagKeys'], "*

 * *               "'resources': {insert: [(1 […]*

```diff
@@ -60059,20 +60059,22 @@
             "resources": [
                 "execute-api-general"
             ]
         }
     },
     "finspace": {
         "ConnectKxCluster": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ConnectKxCluster",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to connect to a kdb cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxCluster"
+            ]
         },
         "CreateEnvironment": {
             "access_level": "Write",
             "action": "CreateEnvironment",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -60080,52 +60082,72 @@
             "description": "Grants permission to create a FinSpace environment",
             "orphan": false,
             "resources": [
                 "environment"
             ]
         },
         "CreateKxChangeset": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateKxChangeset",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create a changeset for a kdb database",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxDatabase"
+            ]
         },
         "CreateKxCluster": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateKxCluster",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a cluster in a managed kdb environment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxCluster"
+            ]
         },
         "CreateKxDatabase": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateKxDatabase",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a kdb database in a managed kdb environment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxDatabase"
+            ]
         },
         "CreateKxEnvironment": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateKxEnvironment",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a managed kdb environment",
             "orphan": false,
             "resources": []
         },
         "CreateKxUser": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateKxUser",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a user in a managed kdb environment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxEnvironment"
+            ]
         },
         "CreateUser": {
             "access_level": "Write",
             "action": "CreateUser",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -60144,102 +60166,122 @@
             "description": "Grants permission to delete a FinSpace environment",
             "orphan": false,
             "resources": [
                 "environment"
             ]
         },
         "DeleteKxCluster": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteKxCluster",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a kdb cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxCluster"
+            ]
         },
         "DeleteKxDatabase": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteKxDatabase",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a kdb database",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxDatabase"
+            ]
         },
         "DeleteKxEnvironment": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteKxEnvironment",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a managed kdb environment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxEnvironment"
+            ]
         },
         "DeleteKxUser": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteKxUser",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a kdb user",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxUser"
+            ]
         },
         "GetEnvironment": {
             "access_level": "Read",
             "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Grants permission to describe a FinSpace environment",
             "orphan": false,
             "resources": [
                 "environment"
             ]
         },
         "GetKxChangeset": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetKxChangeset",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe a changeset for a kdb database",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxDatabase"
+            ]
         },
         "GetKxCluster": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetKxCluster",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe a cluster in a managed kdb environment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxCluster"
+            ]
         },
         "GetKxConnectionString": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetKxConnectionString",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve a connection string for kdb clusters",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxCluster"
+            ]
         },
         "GetKxDatabase": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetKxDatabase",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe a kdb database",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxDatabase"
+            ]
         },
         "GetKxEnvironment": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetKxEnvironment",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe a managed kdb environment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxEnvironment"
+            ]
         },
         "GetKxUser": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetKxUser",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe a kdb user",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxUser"
+            ]
         },
         "GetLoadSampleDataSetGroupIntoEnvironmentStatus": {
             "access_level": "Read",
             "action": "GetLoadSampleDataSetGroupIntoEnvironmentStatus",
             "condition_keys": [],
             "description": "Grants permission to request status of the loading of sample data bundle",
             "orphan": false,
@@ -60265,69 +60307,83 @@
             "description": "Grants permission to list FinSpace environments in the AWS account",
             "orphan": false,
             "resources": [
                 "environment"
             ]
         },
         "ListKxChangesets": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListKxChangesets",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list changesets for a kdb database",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxDatabase"
+            ]
         },
         "ListKxClusterNodes": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListKxClusterNodes",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list cluster nodes in a managed kdb environment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxCluster"
+            ]
         },
         "ListKxClusters": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListKxClusters",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list clusters in a managed kdb environment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxEnvironment"
+            ]
         },
         "ListKxDatabases": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListKxDatabases",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list kdb databases in a managed kdb environment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxEnvironment"
+            ]
         },
         "ListKxEnvironments": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListKxEnvironments",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list managed kdb environments",
             "orphan": false,
             "resources": []
         },
         "ListKxUsers": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListKxUsers",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list users in a managed kdb environment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxEnvironment"
+            ]
         },
         "ListTagsForResource": {
-            "access_level": "Read",
+            "access_level": "List",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to return a list of tags for a resource",
             "orphan": false,
             "resources": [
-                "environment"
+                "environment",
+                "kxCluster",
+                "kxDatabase",
+                "kxEnvironment",
+                "kxUser"
             ]
         },
         "ListUsers": {
             "access_level": "List",
             "action": "ListUsers",
             "condition_keys": [],
             "description": "Grants permission to list FinSpace users in an environment",
@@ -60344,20 +60400,22 @@
             "description": "Grants permission to load sample data bundle into your FinSpace environment",
             "orphan": false,
             "resources": [
                 "environment"
             ]
         },
         "MountKxDatabase": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "MountKxDatabase",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to mount a database to a kdb cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxDatabase"
+            ]
         },
         "ResetUserPassword": {
             "access_level": "Write",
             "action": "ResetUserPassword",
             "condition_keys": [],
             "description": "Grants permission to reset the password for a FinSpace user",
             "orphan": false,
@@ -60365,80 +60423,103 @@
                 "environment",
                 "user"
             ]
         },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
             "description": "Grants permission to tag a resource",
             "orphan": false,
             "resources": [
-                "environment"
+                "environment",
+                "kxCluster",
+                "kxDatabase",
+                "kxEnvironment",
+                "kxUser"
             ]
         },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:TagKeys"
+            ],
             "description": "Grants permission to untag a resource",
             "orphan": false,
             "resources": [
-                "environment"
+                "environment",
+                "kxCluster",
+                "kxDatabase",
+                "kxEnvironment",
+                "kxUser"
             ]
         },
         "UpdateEnvironment": {
             "access_level": "Write",
             "action": "UpdateEnvironment",
             "condition_keys": [],
             "description": "Grants permission to update a FinSpace environment",
             "orphan": false,
             "resources": [
                 "environment"
             ]
         },
         "UpdateKxClusterDatabases": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateKxClusterDatabases",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update databases for a cluster in a managed kdb environment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxCluster"
+            ]
         },
         "UpdateKxDatabase": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateKxDatabase",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a kdb database",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxDatabase"
+            ]
         },
         "UpdateKxEnvironment": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateKxEnvironment",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a managed kdb environment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxEnvironment"
+            ]
         },
         "UpdateKxEnvironmentNetwork": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateKxEnvironmentNetwork",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update the network for a managed kdb environment",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxEnvironment"
+            ]
         },
         "UpdateKxUser": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateKxUser",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a kdb user",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "kxUser"
+            ]
         },
         "UpdateUser": {
             "access_level": "Write",
             "action": "UpdateUser",
             "condition_keys": [],
             "description": "Grants permission to update a FinSpace user",
             "orphan": false,
@@ -73740,14 +73821,15 @@
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to list tags for an Image Builder resource",
             "orphan": false,
             "resources": [
                 "component",
+                "containerRecipe",
                 "distributionConfiguration",
                 "image",
                 "imagePipeline",
                 "imageRecipe",
                 "infrastructureConfiguration"
             ]
         },
@@ -75071,28 +75153,39 @@
             "description": "Grants permission to create an OTA update job",
             "orphan": false,
             "resources": [
                 "otaupdate"
             ]
         },
         "CreatePackage": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreatePackage",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a software package that you can deploy to your devices",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "package"
+            ]
         },
         "CreatePackageVersion": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreatePackageVersion",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a version under the specified package",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "package",
+                "packageversion"
+            ]
         },
         "CreatePolicy": {
             "access_level": "Write",
             "action": "CreatePolicy",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -75414,28 +75507,33 @@
             "description": "Grants permission to delete an OTA update job",
             "orphan": false,
             "resources": [
                 "otaupdate"
             ]
         },
         "DeletePackage": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeletePackage",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a package",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "package"
+            ]
         },
         "DeletePackageVersion": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeletePackageVersion",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a version of the specified package",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "package",
+                "packageversion"
+            ]
         },
         "DeletePolicy": {
             "access_level": "Write",
             "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Grants permission to delete the specified policy",
             "orphan": false,
@@ -76057,36 +76155,41 @@
             "description": "Grants permission to get the information about the OTA update job",
             "orphan": false,
             "resources": [
                 "otaupdate"
             ]
         },
         "GetPackage": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetPackage",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get the information about the package",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "package"
+            ]
         },
         "GetPackageConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetPackageConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get the package configuration of the account",
             "orphan": false,
             "resources": []
         },
         "GetPackageVersion": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetPackageVersion",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get the version of the package",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "package",
+                "packageversion"
+            ]
         },
         "GetPercentiles": {
             "access_level": "Read",
             "action": "GetPercentiles",
             "condition_keys": [],
             "description": "Grants permission to get percentiles for IoT fleet index",
             "orphan": false,
@@ -76381,15 +76484,15 @@
             "orphan": false,
             "resources": []
         },
         "ListMetricValues": {
             "access_level": "List",
             "action": "ListMetricValues",
             "condition_keys": [],
-            "description": "Adds support to list metric datapoints collected for IoT devices",
+            "description": "Grants permissions to list the metric values for a thing based on the metricName, and dimension if specified",
             "orphan": false,
             "resources": [
                 "thing"
             ]
         },
         "ListMitigationActions": {
             "access_level": "List",
@@ -76422,26 +76525,26 @@
             "action": "ListOutgoingCertificates",
             "condition_keys": [],
             "description": "Grants permission to list certificates that are being transfered but not yet accepted",
             "orphan": false,
             "resources": []
         },
         "ListPackageVersions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListPackageVersions",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list versions for a package in the account",
             "orphan": false,
             "resources": []
         },
         "ListPackages": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListPackages",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list packages in the account",
             "orphan": false,
             "resources": []
         },
         "ListPolicies": {
             "access_level": "List",
             "action": "ListPolicies",
             "condition_keys": [],
@@ -76999,14 +77102,16 @@
                 "domainconfiguration",
                 "dynamicthinggroup",
                 "fleetmetric",
                 "job",
                 "jobtemplate",
                 "mitigationaction",
                 "otaupdate",
+                "package",
+                "packageversion",
                 "policy",
                 "provisioningtemplate",
                 "rolealias",
                 "rule",
                 "scheduledaudit",
                 "securityprofile",
                 "stream",
@@ -77061,14 +77166,16 @@
                 "domainconfiguration",
                 "dynamicthinggroup",
                 "fleetmetric",
                 "job",
                 "jobtemplate",
                 "mitigationaction",
                 "otaupdate",
+                "package",
+                "packageversion",
                 "policy",
                 "provisioningtemplate",
                 "rolealias",
                 "rule",
                 "scheduledaudit",
                 "securityprofile",
                 "stream",
@@ -77216,36 +77323,41 @@
             "description": "Grants permission to update the definition for the specified mitigation action",
             "orphan": false,
             "resources": [
                 "mitigationaction"
             ]
         },
         "UpdatePackage": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdatePackage",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a package",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "package"
+            ]
         },
         "UpdatePackageConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdatePackageConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update the package configuration of the account",
             "orphan": false,
             "resources": []
         },
         "UpdatePackageVersion": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdatePackageVersion",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update the version of the specified package",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "package",
+                "packageversion"
+            ]
         },
         "UpdateProvisioningTemplate": {
             "access_level": "Write",
             "action": "UpdateProvisioningTemplate",
             "condition_keys": [],
             "description": "Grants permission to update a fleet provisioning template",
             "orphan": false,
@@ -134496,20 +134608,23 @@
             "description": "Grants permission to return information about a specific Signing Job",
             "orphan": false,
             "resources": [
                 "signing-job"
             ]
         },
         "GetRevocationStatus": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetRevocationStatus",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to query revocation info of signing resources",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "signing-job",
+                "signing-profile"
+            ]
         },
         "GetSigningPlatform": {
             "access_level": "Read",
             "action": "GetSigningPlatform",
             "condition_keys": [],
             "description": "Grants permission to return information about a specific Signing Platform",
             "orphan": false,
@@ -134615,20 +134730,24 @@
             "description": "Grants permission to change the state of a Signing Profile to REVOKED",
             "orphan": false,
             "resources": [
                 "signing-profile"
             ]
         },
         "SignPayload": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "SignPayload",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "signer:ProfileVersion"
+            ],
+            "description": "Grants permission to initiate a Signing Job on the provided payload",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "signing-profile"
+            ]
         },
         "StartSigningJob": {
             "access_level": "Write",
             "action": "StartSigningJob",
             "condition_keys": [
                 "signer:ProfileVersion"
             ],
```

### Comparing `iam_actions-1.2.20230607/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230608/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230607/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230608/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230607/iam_actions/generate/generate.py` & `iam_actions-1.2.20230608/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230607/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230608/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230607/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230608/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230607/iam_actions/generate/services.py` & `iam_actions-1.2.20230608/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230607/iam_actions/policies.json` & `iam_actions-1.2.20230608/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230607/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230608/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998984468339307%*

 * *Differences: {"'finspace'": "{'kxEnvironment': OrderedDict([('arn_pattern', "*

 * *               "'arn:*:finspace:*:*:kxEnvironment/*'), ('condition_keys', "*

 * *               "'aws:ResourceTag/${TagKey}')]), 'kxUser': OrderedDict([('arn_pattern', "*

 * *               "'arn:*:finspace:*:*:kxEnvironment/*/kxUser/*'), ('condition_keys', "*

 * *               "'aws:ResourceTag/${TagKey}')]), 'kxCluster': OrderedDict([('arn_pattern', "*

 * *               "'arn:*:finspace:*:*:kxEnvironment/*/kxCluster/*'), ('condition_keys', "*

 * *               "' […]*

```diff
@@ -2597,14 +2597,30 @@
         }
     },
     "finspace": {
         "environment": {
             "arn_pattern": "arn:*:finspace:*:*:environment/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "kxCluster": {
+            "arn_pattern": "arn:*:finspace:*:*:kxEnvironment/*/kxCluster/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
+        "kxDatabase": {
+            "arn_pattern": "arn:*:finspace:*:*:kxEnvironment/*/kxDatabase/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
+        "kxEnvironment": {
+            "arn_pattern": "arn:*:finspace:*:*:kxEnvironment/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
+        "kxUser": {
+            "arn_pattern": "arn:*:finspace:*:*:kxEnvironment/*/kxUser/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "user": {
             "arn_pattern": "arn:*:finspace:*:*:user/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "finspace-api": {},
     "firehose": {
@@ -3349,14 +3365,22 @@
             "arn_pattern": "arn:*:iot:*:*:mitigationaction/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "otaupdate": {
             "arn_pattern": "arn:*:iot:*:*:otaupdate/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "package": {
+            "arn_pattern": "arn:*:iot:*:*:package/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
+        "packageversion": {
+            "arn_pattern": "arn:*:iot:*:*:package/*/version/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "policy": {
             "arn_pattern": "arn:*:iot:*:*:policy/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "provisioningtemplate": {
             "arn_pattern": "arn:*:iot:*:*:provisioningtemplate/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
```

### Comparing `iam_actions-1.2.20230607/iam_actions/services.json` & `iam_actions-1.2.20230608/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230607/pyproject.toml` & `iam_actions-1.2.20230608/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230607"
+version = "1.2.20230608"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230607/setup.py` & `iam_actions-1.2.20230608/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230607',
+    'version': '1.2.20230608',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230607/PKG-INFO` & `iam_actions-1.2.20230608/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230607
+Version: 1.2.20230608
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

