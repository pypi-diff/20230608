# Comparing `tmp/onefuzztypes-8.2.0.tar.gz` & `tmp/onefuzztypes-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onefuzztypes-8.2.0.tar", last modified: Wed May 24 18:19:51 2023, max compression
+gzip compressed data, was "dist/onefuzztypes-8.3.0.tar", last modified: Tue Jun  6 20:27:13 2023, max compression
```

## Comparing `onefuzztypes-8.2.0.tar` & `onefuzztypes-8.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 18:19:51.000000 onefuzztypes-8.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-05-24 18:19:51.000000 onefuzztypes-8.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 18:19:51.000000 onefuzztypes-8.2.0/onefuzztypes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/_monkeypatch.py
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/consts.py
--rw-r--r--   0 runner    (1001) docker     (122)    11852 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     8387 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5118 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/job_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)    25283 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/primitives.py
--rw-r--r--   0 runner    (1001) docker     (122)     5821 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/requests.py
--rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/responses.py
--rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/validators.py
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 18:19:51.000000 onefuzztypes-8.2.0/onefuzztypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-05-24 18:19:50.000000 onefuzztypes-8.2.0/onefuzztypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      768 2023-05-24 18:19:51.000000 onefuzztypes-8.2.0/onefuzztypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 18:19:50.000000 onefuzztypes-8.2.0/onefuzztypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 18:19:50.000000 onefuzztypes-8.2.0/onefuzztypes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-24 18:19:50.000000 onefuzztypes-8.2.0/onefuzztypes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-24 18:19:50.000000 onefuzztypes-8.2.0/onefuzztypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/requirements-lint.txt
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 18:19:51.000000 onefuzztypes-8.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1366 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 18:19:51.000000 onefuzztypes-8.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      556 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/tests/test_alnum_filter.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/tests/test_container_def.py
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/tests/test_instance_config_update.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2947 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 20:27:13.000000 onefuzztypes-8.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-06-06 20:27:13.000000 onefuzztypes-8.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 20:27:13.000000 onefuzztypes-8.3.0/onefuzztypes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/onefuzztypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/onefuzztypes/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/onefuzztypes/_monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/onefuzztypes/consts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11877 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/onefuzztypes/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8387 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/onefuzztypes/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5118 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/onefuzztypes/job_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25439 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/onefuzztypes/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/onefuzztypes/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5821 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/onefuzztypes/requests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/onefuzztypes/responses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/onefuzztypes/validators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/onefuzztypes/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 20:27:13.000000 onefuzztypes-8.3.0/onefuzztypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-06-06 20:27:12.000000 onefuzztypes-8.3.0/onefuzztypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      768 2023-06-06 20:27:13.000000 onefuzztypes-8.3.0/onefuzztypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 20:27:12.000000 onefuzztypes-8.3.0/onefuzztypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 20:27:12.000000 onefuzztypes-8.3.0/onefuzztypes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-06 20:27:12.000000 onefuzztypes-8.3.0/onefuzztypes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-06 20:27:12.000000 onefuzztypes-8.3.0/onefuzztypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/requirements-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-06 20:27:13.000000 onefuzztypes-8.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1366 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 20:27:13.000000 onefuzztypes-8.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      556 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/tests/test_alnum_filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/tests/test_container_def.py
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/tests/test_instance_config_update.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2947 2023-06-06 20:27:07.000000 onefuzztypes-8.3.0/tests/test_models.py
```

### Comparing `onefuzztypes-8.2.0/PKG-INFO` & `onefuzztypes-8.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzztypes
-Version: 8.2.0
+Version: 8.3.0
 Summary: Onefuzz Types Library
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # Python types used by OneFuzz
```

### Comparing `onefuzztypes-8.2.0/README.md` & `onefuzztypes-8.3.0/README.md`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.2.0/onefuzztypes/_monkeypatch.py` & `onefuzztypes-8.3.0/onefuzztypes/_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.2.0/onefuzztypes/enums.py` & `onefuzztypes-8.3.0/onefuzztypes/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,14 +287,15 @@
     ADO_VALIDATION_INVALID_PAT = 478
     ADO_VALIDATION_INVALID_FIELDS = 479
     GITHUB_VALIDATION_INVALID_PAT = 480
     GITHUB_VALIDATION_INVALID_REPOSITORY = 481
     UNEXPECTED_DATA_SHAPE = 482
     UNABLE_TO_SEND = 483
     NODE_DELETED = 484
+    TASK_CANCELLED = 485
     # NB: if you update this enum, also update Enums.cs
 
 
 class HeartbeatType(Enum):
     MachineAlive = "MachineAlive"
     TaskAlive = "TaskAlive"
```

### Comparing `onefuzztypes-8.2.0/onefuzztypes/events.py` & `onefuzztypes-8.3.0/onefuzztypes/events.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.2.0/onefuzztypes/job_templates.py` & `onefuzztypes-8.3.0/onefuzztypes/job_templates.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.2.0/onefuzztypes/models.py` & `onefuzztypes-8.3.0/onefuzztypes/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from .consts import ONE_HOUR, SEVEN_DAYS
 from .enums import (
     OS,
     Architecture,
     Compare,
     ContainerPermission,
     ContainerType,
-    ErrorCode,
     GithubIssueSearchMatch,
     GithubIssueState,
     HeartbeatType,
     JobState,
     NodeState,
     NodeTaskState,
     PoolState,
@@ -91,15 +90,19 @@
         if len(some) > 1:
             raise ValueError("multiple values set for enum: %s" % some)
 
         return values
 
 
 class Error(BaseModel):
-    code: ErrorCode
+    # the code here is from ErrorCodes.cs, but we don't
+    # want to validate the error code on the client-side
+    code: int
+    # a human-readable version of the error code
+    title: str
     errors: List[str]
 
 
 OkType = TypeVar("OkType")
 Result = Union[OkType, Error]
```

### Comparing `onefuzztypes-8.2.0/onefuzztypes/primitives.py` & `onefuzztypes-8.3.0/onefuzztypes/primitives.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.2.0/onefuzztypes/requests.py` & `onefuzztypes-8.3.0/onefuzztypes/requests.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.2.0/onefuzztypes/responses.py` & `onefuzztypes-8.3.0/onefuzztypes/responses.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.2.0/onefuzztypes/validators.py` & `onefuzztypes-8.3.0/onefuzztypes/validators.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.2.0/onefuzztypes/webhooks.py` & `onefuzztypes-8.3.0/onefuzztypes/webhooks.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.2.0/onefuzztypes.egg-info/PKG-INFO` & `onefuzztypes-8.3.0/onefuzztypes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzztypes
-Version: 8.2.0
+Version: 8.3.0
 Summary: Onefuzz Types Library
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # Python types used by OneFuzz
```

### Comparing `onefuzztypes-8.2.0/onefuzztypes.egg-info/SOURCES.txt` & `onefuzztypes-8.3.0/onefuzztypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.2.0/setup.py` & `onefuzztypes-8.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.2.0/tests/test_alnum_filter.py` & `onefuzztypes-8.3.0/tests/test_alnum_filter.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.2.0/tests/test_container_def.py` & `onefuzztypes-8.3.0/tests/test_container_def.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.2.0/tests/test_instance_config_update.py` & `onefuzztypes-8.3.0/tests/test_instance_config_update.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.2.0/tests/test_models.py` & `onefuzztypes-8.3.0/tests/test_models.py`

 * *Files identical despite different names*

