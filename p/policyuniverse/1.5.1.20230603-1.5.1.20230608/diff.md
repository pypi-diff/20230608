# Comparing `tmp/policyuniverse-1.5.1.20230603.tar.gz` & `tmp/policyuniverse-1.5.1.20230608.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "policyuniverse-1.5.1.20230603.tar", last modified: Sun Jun  4 03:23:38 2023, max compression
+gzip compressed data, was "policyuniverse-1.5.1.20230608.tar", last modified: Thu Jun  8 14:00:28 2023, max compression
```

## Comparing `policyuniverse-1.5.1.20230603.tar` & `policyuniverse-1.5.1.20230608.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 03:23:38.872851 policyuniverse-1.5.1.20230603/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-06-04 03:23:38.872851 policyuniverse-1.5.1.20230603/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 03:23:38.872851 policyuniverse-1.5.1.20230603/policyuniverse/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/action_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/arn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/common.py
--rw-r--r--   0 runner    (1001) docker     (123)  7810249 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/data.json
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/expander_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/policyuniverse/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 03:23:38.872851 policyuniverse-1.5.1.20230603/policyuniverse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-06-04 03:23:38.000000 policyuniverse-1.5.1.20230603/policyuniverse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-04 03:23:38.000000 policyuniverse-1.5.1.20230603/policyuniverse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 03:23:38.000000 policyuniverse-1.5.1.20230603/policyuniverse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 03:23:38.000000 policyuniverse-1.5.1.20230603/policyuniverse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-04 03:23:38.000000 policyuniverse-1.5.1.20230603/policyuniverse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-04 03:23:38.000000 policyuniverse-1.5.1.20230603/policyuniverse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-04 03:23:38.872851 policyuniverse-1.5.1.20230603/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-04 03:23:29.000000 policyuniverse-1.5.1.20230603/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:00:28.743653 policyuniverse-1.5.1.20230608/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-06-08 14:00:28.743653 policyuniverse-1.5.1.20230608/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:00:28.739653 policyuniverse-1.5.1.20230608/policyuniverse/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/action_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/arn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7833102 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/expander_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/policyuniverse/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:00:28.743653 policyuniverse-1.5.1.20230608/policyuniverse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-06-08 14:00:28.000000 policyuniverse-1.5.1.20230608/policyuniverse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-08 14:00:28.000000 policyuniverse-1.5.1.20230608/policyuniverse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:00:28.000000 policyuniverse-1.5.1.20230608/policyuniverse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:00:28.000000 policyuniverse-1.5.1.20230608/policyuniverse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 14:00:28.000000 policyuniverse-1.5.1.20230608/policyuniverse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 14:00:28.000000 policyuniverse-1.5.1.20230608/policyuniverse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 14:00:28.743653 policyuniverse-1.5.1.20230608/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-08 14:00:18.000000 policyuniverse-1.5.1.20230608/setup.py
```

### Comparing `policyuniverse-1.5.1.20230603/LICENSE` & `policyuniverse-1.5.1.20230608/LICENSE`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230603/PKG-INFO` & `policyuniverse-1.5.1.20230608/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyuniverse
-Version: 1.5.1.20230603
+Version: 1.5.1.20230608
 Summary: Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.
 Home-page: https://github.com/Netflix-Skunkworks/policyuniverse
 Author: Patrick Kelley
 Author-email: patrickbarrettkelley@gmail.com
 Keywords: iam,arn,action_groups,condition,policy,statement,wildcard
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
```

### Comparing `policyuniverse-1.5.1.20230603/README.md` & `policyuniverse-1.5.1.20230608/README.md`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230603/policyuniverse/__init__.py` & `policyuniverse-1.5.1.20230608/policyuniverse/__init__.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230603/policyuniverse/action.py` & `policyuniverse-1.5.1.20230608/policyuniverse/action.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230603/policyuniverse/action_categories.py` & `policyuniverse-1.5.1.20230608/policyuniverse/action_categories.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230603/policyuniverse/arn.py` & `policyuniverse-1.5.1.20230608/policyuniverse/arn.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230603/policyuniverse/common.py` & `policyuniverse-1.5.1.20230608/policyuniverse/common.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230603/policyuniverse/data.json` & `policyuniverse-1.5.1.20230608/policyuniverse/data.json`

 * *Files 0% similar despite different names*

```diff
@@ -29891,28 +29891,56 @@
         "description": "Grants permission to create or update a subscription filter and associates it with the specified log group",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_PutSubscriptionFilter.html"
         }
       },
+      "StartLiveTail": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to start a livetail session in CloudWatch Logs",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}AmazonCloudWatch/latest/logs/CloudWatchLogs_LiveTail.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/CloudWatchLogs_LiveTail.html"
+        }
+      },
       "StartQuery": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to schedule a query of a log group using CloudWatch Logs Insights",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_StartQuery.html"
         }
       },
+      "StopLiveTail": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to stop a CloudWatch Logs livetail session that is in progress",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}AmazonCloudWatch/latest/logs/CloudWatchLogs_LiveTail.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/CloudWatchLogs_LiveTail.html"
+        }
+      },
       "StopQuery": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -33293,14 +33321,15 @@
       "UntagResource": {
         "aws_action_groups": [
           "Tagging",
           "ReadWrite"
         ],
         "calculated_action_group": "Tagging",
         "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
           "aws:TagKeys"
         ],
         "description": "Grants permission to disassociate resource tags from a CodeCommit resource ARN",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/codecommit/latest/APIReference/API_UntagResource.html"
@@ -33472,16 +33501,16 @@
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}auth-and-access-control-permissions-reference.html#aa-acp",
           "doc_page_rel": "https://docs.aws.amazon.com/codecommit/latest/userguide/auth-and-access-control-permissions-reference.html#aa-acp"
         }
       }
     },
-    "arn_format": "arn:aws:codecommit:${Region}:${Account}:${RepositoryName}",
-    "arn_regex": "^arn:aws:codecommit:.+",
+    "arn_format": "arn:${Partition}:codecommit:${Region}:${Account}:${RepositoryName}",
+    "arn_regex": "^arn:${Partition}:codecommit:.+",
     "description": "AWS CodeCommit",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/codecommit/latest/APIReference/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/codecommit/latest/APIReference/Welcome.html",
       "authz_doc_page": "https://docs.aws.amazon.com/codecommit/latest/userguide/auth-and-access-control-permissions-reference.html",
@@ -82905,14 +82934,27 @@
       "concepts_doc_root": "https://docs.aws.amazon.com/fsx/latest/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/fsx/latest/WindowsGuide/access-control-manage-access-intro.html"
     },
     "prefix": "fsx"
   },
   "FinSpace": {
     "actions": {
+      "ConnectKxCluster": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to connect to a kdb cluster",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}finspace/latest/userguide/interacting-with-kdb-clusters.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/userguide/interacting-with-kdb-clusters.html"
+        }
+      },
       "CreateEnvironment": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
@@ -82921,14 +82963,91 @@
         "description": "Grants permission to create a FinSpace environment",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_CreateEnvironment.html"
         }
       },
+      "CreateKxChangeset": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to create a changeset for a kdb database",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_CreateKxChangeset.html"
+        }
+      },
+      "CreateKxCluster": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create a cluster in a managed kdb environment",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_CreateKxCluster.html"
+        }
+      },
+      "CreateKxDatabase": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create a kdb database in a managed kdb environment",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_CreateKxDatabase.html"
+        }
+      },
+      "CreateKxEnvironment": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create a managed kdb environment",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_CreateKxEnvironment.html"
+        }
+      },
+      "CreateKxUser": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create a user in a managed kdb environment",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_CreateKxUser.html"
+        }
+      },
       "CreateUser": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
@@ -82950,28 +83069,164 @@
         "description": "Grants permission to delete a FinSpace environment",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_DeleteEnvironment.html"
         }
       },
+      "DeleteKxCluster": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a kdb cluster",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_DeleteKxCluster.html"
+        }
+      },
+      "DeleteKxDatabase": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a kdb database",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_DeleteKxDatabase.html"
+        }
+      },
+      "DeleteKxEnvironment": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a managed kdb environment",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_DeleteKxEnvironment.html"
+        }
+      },
+      "DeleteKxUser": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a kdb user",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_DeleteKxUser.html"
+        }
+      },
       "GetEnvironment": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to describe a FinSpace environment",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_GetEnvironment.html"
         }
       },
+      "GetKxChangeset": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to describe a changeset for a kdb database",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_GetKxChangeset.html"
+        }
+      },
+      "GetKxCluster": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to describe a cluster in a managed kdb environment",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_GetKxCluster.html"
+        }
+      },
+      "GetKxConnectionString": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve a connection string for kdb clusters",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_GetKxConnectionString.html"
+        }
+      },
+      "GetKxDatabase": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to describe a kdb database",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_GetKxDatabase.html"
+        }
+      },
+      "GetKxEnvironment": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to describe a managed kdb environment",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_GetKxEnvironment.html"
+        }
+      },
+      "GetKxUser": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to describe a kdb user",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_GetKxUser.html"
+        }
+      },
       "GetLoadSampleDataSetGroupIntoEnvironmentStatus": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -83007,20 +83262,111 @@
         "description": "Grants permission to list FinSpace environments in the AWS account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_ListEnvironments.html"
         }
       },
-      "ListTagsForResource": {
+      "ListKxChangesets": {
         "aws_action_groups": [
+          "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
-        "calculated_action_group": "Read",
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list changesets for a kdb database",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_ListKxChangesets.html"
+        }
+      },
+      "ListKxClusterNodes": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list cluster nodes in a managed kdb environment",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_ListKxClusterNodes.html"
+        }
+      },
+      "ListKxClusters": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list clusters in a managed kdb environment",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_ListKxClusters.html"
+        }
+      },
+      "ListKxDatabases": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list kdb databases in a managed kdb environment",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_ListKxDatabases.html"
+        }
+      },
+      "ListKxEnvironments": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list managed kdb environments",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_ListKxEnvironments.html"
+        }
+      },
+      "ListKxUsers": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list users in a managed kdb environment",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_ListKxUsers.html"
+        }
+      },
+      "ListTagsForResource": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite",
+          "ListOnly"
+        ],
+        "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to return a list of tags for a resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_ListTagsForResource.html"
         }
@@ -83049,14 +83395,27 @@
         "description": "Grants permission to load sample data bundle into your FinSpace environment",
         "docs": {
           "api_doc": "",
           "doc_page": "${DocHomeURL}finspace/latest/userguide/finspace-what-is.html",
           "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/userguide/finspace-what-is.html"
         }
       },
+      "MountKxDatabase": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to mount a database to a kdb cluster",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}finspace/latest/userguide/finspace-managed-kdb-db.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/userguide/finspace-managed-kdb-db.html"
+        }
+      },
       "ResetUserPassword": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to reset the password for a FinSpace user",
@@ -83068,29 +83427,34 @@
       },
       "TagResource": {
         "aws_action_groups": [
           "Tagging",
           "ReadWrite"
         ],
         "calculated_action_group": "Tagging",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
         "description": "Grants permission to tag a resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_TagResource.html"
         }
       },
       "UntagResource": {
         "aws_action_groups": [
           "Tagging",
           "ReadWrite"
         ],
         "calculated_action_group": "Tagging",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:TagKeys"
+        ],
         "description": "Grants permission to untag a resource",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_UntagResource.html"
         }
       },
@@ -83103,14 +83467,79 @@
         "description": "Grants permission to update a FinSpace environment",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_UpdateEnvironment.html"
         }
       },
+      "UpdateKxClusterDatabases": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update databases for a cluster in a managed kdb environment",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_UpdateKxClusterDatabases.html"
+        }
+      },
+      "UpdateKxDatabase": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update a kdb database",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_UpdateKxDatabase.html"
+        }
+      },
+      "UpdateKxEnvironment": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update a managed kdb environment",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_UpdateKxEnvironment.html"
+        }
+      },
+      "UpdateKxEnvironmentNetwork": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update the network for a managed kdb environment",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_UpdateKxEnvironmentNetwork.html"
+        }
+      },
+      "UpdateKxUser": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update a kdb user",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/finspace/latest/management-api/API_UpdateKxUser.html"
+        }
+      },
       "UpdateUser": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update a FinSpace user",
@@ -105348,15 +105777,15 @@
           "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
         "description": "Grants permission to create a fleet metric",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/iot-indexing.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_CreateFleetMetric.html"
         }
       },
       "CreateJob": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -105429,14 +105858,48 @@
         "description": "Grants permission to create an OTA update job",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_CreateOTAUpdate.html"
         }
       },
+      "CreatePackage": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create a software package that you can deploy to your devices",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_CreatePackage.html"
+        }
+      },
+      "CreatePackageVersion": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create a version under the specified package",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_CreatePackageVersion.html"
+        }
+      },
       "CreatePolicy": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
@@ -105802,15 +106265,15 @@
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete the specified fleet metric",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/iot-indexing.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_DeleteFleetMetric.html"
         }
       },
       "DeleteJob": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -105880,14 +106343,44 @@
         "description": "Grants permission to delete an OTA update job",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_DeleteOTAUpdate.html"
         }
       },
+      "DeletePackage": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to delete a package",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_DeletePackage.html"
+        }
+      },
+      "DeletePackageVersion": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to delete a version of the specified package",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_DeletePackageVersion.html"
+        }
+      },
       "DeletePolicy": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
@@ -106372,15 +106865,15 @@
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to get information about the specified fleet metric",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/iot-indexing.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_DescribeFleetMetric.html"
         }
       },
       "DescribeIndex": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
@@ -106745,15 +107238,15 @@
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to get buckets aggregation for IoT fleet index",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/iot-indexing.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_GetBucketsAggregation.html"
         }
       },
       "GetCardinality": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
@@ -106836,14 +107329,60 @@
         "description": "Grants permission to get the information about the OTA update job",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_GetOTAUpdate.html"
         }
       },
+      "GetPackage": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to get the information about the package",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_GetPackage.html"
+        }
+      },
+      "GetPackageConfiguration": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get the package configuration of the account",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_GetPackageConfiguration.html"
+        }
+      },
+      "GetPackageVersion": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to get the version of the package",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_GetPackageVersion.html"
+        }
+      },
       "GetPercentiles": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -107251,15 +107790,15 @@
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to list the fleet metrics in your account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/iot-indexing.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_ListFleetMetrics.html"
         }
       },
       "ListIndices": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
@@ -107352,15 +107891,15 @@
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
-        "description": "Adds support to list metric datapoints collected for IoT devices",
+        "description": "Grants permissions to list the metric values for a thing based on the metricName, and dimension if specified",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_ListMetricValues.html"
         }
       },
       "ListMitigationActions": {
@@ -107419,14 +107958,44 @@
         "description": "Grants permission to list certificates that are being transfered but not yet accepted",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_ListOutgoingCertificates.html"
         }
       },
+      "ListPackageVersions": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list versions for a package in the account",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_ListPackageVersions.html"
+        }
+      },
+      "ListPackages": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list packages in the account",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_ListPackages.html"
+        }
+      },
       "ListPolicies": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
@@ -108505,15 +109074,15 @@
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update a fleet metric",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/iot-indexing.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_UpdateFleetMetric.html"
         }
       },
       "UpdateIndexingConfiguration": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -108551,14 +109120,57 @@
         "description": "Grants permission to update the definition for the specified mitigation action",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_UpdateMitigationAction.html"
         }
       },
+      "UpdatePackage": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to update a package",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_UpdatePackage.html"
+        }
+      },
+      "UpdatePackageConfiguration": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update the package configuration of the account",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_UpdatePackageConfiguration.html"
+        }
+      },
+      "UpdatePackageVersion": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}"
+        ],
+        "description": "Grants permission to update the version of the specified package",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/iot/latest/apireference/API_UpdatePackageVersion.html"
+        }
+      },
       "UpdateProvisioningTemplate": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
@@ -117704,14 +118316,15 @@
           "kms:CallerAccount",
           "kms:KeyOrigin",
           "kms:KeySpec",
           "kms:KeyUsage",
           "kms:MultiRegion",
           "kms:MultiRegionKeyType",
           "kms:ResourceAliases",
+          "kms:ScheduleKeyDeletionPendingWindowInDays",
           "kms:ViaService"
         ],
         "description": "Controls permission to schedule deletion of an AWS KMS key",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/kms/latest/APIReference/API_ScheduleKeyDeletion.html"
@@ -192182,17 +192795,17 @@
     "arn_regex": "^arn:${Partition}:securitylake:.+:.+:.+",
     "description": "Amazon Security Lake",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/security-lake/latest/APIReference/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/security-lake/latest/APIReference/",
-      "authz_doc_page": "https://docs.aws.amazon.com/AmazonSecurityLake/latest/access_policies.html",
-      "concepts_doc_root": "https://docs.aws.amazon.com/AmazonSecurityLake/latest/",
-      "context_keys_doc_root": "https://docs.aws.amazon.com/AmazonSecurityLake/latest/"
+      "authz_doc_page": "https://docs.aws.amazon.com/security-lake/latest/userguide/security-iam.html",
+      "concepts_doc_root": "https://docs.aws.amazon.com/security-lake/latest/",
+      "context_keys_doc_root": "https://docs.aws.amazon.com/security-lake/latest/"
     },
     "prefix": "securitylake"
   },
   "ServerMigrationService": {
     "actions": {
       "CreateApp": {
         "aws_action_groups": [
@@ -195472,14 +196085,28 @@
         "description": "Grants permission to return information about a specific Signing Job",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/signer/latest/api/API_DescribeSigningJob.html"
         }
       },
+      "GetRevocationStatus": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to query revocation info of signing resources",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/signer/latest/api/API_GetRevocationStatus.html"
+        }
+      },
       "GetSigningPlatform": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -195636,14 +196263,29 @@
         "description": "Grants permission to change the state of a Signing Profile to REVOKED",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/signer/latest/api/API_RevokeSigningProfile.html"
         }
       },
+      "SignPayload": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "signer:ProfileVersion"
+        ],
+        "description": "Grants permission to initiate a Signing Job on the provided payload",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/signer/latest/api/API_SignPayload.html"
+        }
+      },
       "StartSigningJob": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "signer:ProfileVersion"
@@ -209955,14 +210597,42 @@
         "description": "Grants permission to delete a WebACL",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/waf/latest/APIReference/API_DeleteWebACL.html"
         }
       },
+      "DescribeAllManagedProducts": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve product information for a managed rule group",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/waf/latest/APIReference/API_DescribeAllManagedProducts.html"
+        }
+      },
+      "DescribeManagedProductsByVendor": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to retrieve product information for a managed rule group by a given vendor",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/waf/latest/APIReference/API_DescribeManagedProductsByVendor.html"
+        }
+      },
       "DescribeManagedRuleGroup": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
```

### Comparing `policyuniverse-1.5.1.20230603/policyuniverse/expander_minimizer.py` & `policyuniverse-1.5.1.20230608/policyuniverse/expander_minimizer.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230603/policyuniverse/organization.py` & `policyuniverse-1.5.1.20230608/policyuniverse/organization.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230603/policyuniverse/policy.py` & `policyuniverse-1.5.1.20230608/policyuniverse/policy.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230603/policyuniverse/statement.py` & `policyuniverse-1.5.1.20230608/policyuniverse/statement.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230603/policyuniverse.egg-info/PKG-INFO` & `policyuniverse-1.5.1.20230608/policyuniverse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyuniverse
-Version: 1.5.1.20230603
+Version: 1.5.1.20230608
 Summary: Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.
 Home-page: https://github.com/Netflix-Skunkworks/policyuniverse
 Author: Patrick Kelley
 Author-email: patrickbarrettkelley@gmail.com
 Keywords: iam,arn,action_groups,condition,policy,statement,wildcard
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
```

### Comparing `policyuniverse-1.5.1.20230603/policyuniverse.egg-info/SOURCES.txt` & `policyuniverse-1.5.1.20230608/policyuniverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230603/setup.py` & `policyuniverse-1.5.1.20230608/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ROOT = os.path.realpath(os.path.join(os.path.dirname(__file__)))
 
 tests_require = ["pytest", "coveralls", "bandit"]
 dev_require = ["pre-commit", "black"]
 
 setup(
     name="policyuniverse",
-    version="1.5.1.20230603",
+    version="1.5.1.20230608",
     description="Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.",
     long_description=open(os.path.join(ROOT, "README.md")).read(),
     long_description_content_type="text/markdown",
     author="Patrick Kelley",
     author_email="patrickbarrettkelley@gmail.com",
     url="https://github.com/Netflix-Skunkworks/policyuniverse",
     keywords=[
```

