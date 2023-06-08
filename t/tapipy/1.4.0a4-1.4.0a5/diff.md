# Comparing `tmp/tapipy-1.4.0a4.tar.gz` & `tmp/tapipy-1.4.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapipy-1.4.0a4.tar", max compression
+gzip compressed data, was "tapipy-1.4.0a5.tar", max compression
```

## Comparing `tapipy-1.4.0a4.tar` & `tapipy-1.4.0a5.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0     1539 2022-05-17 23:01:20.810838 tapipy-1.4.0a4/LICENSE.md
--rw-r--r--   0        0        0     8639 2023-05-31 22:55:27.557819 tapipy-1.4.0a4/README.md
--rw-r--r--   0        0        0      972 2023-06-05 18:15:49.843865 tapipy-1.4.0a4/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-02 22:48:04.288915 tapipy-1.4.0a4/tapipy/__init__.py
--rw-r--r--   0        0        0    13502 2023-05-31 22:55:11.637942 tapipy-1.4.0a4/tapipy/actors.py
--rw-r--r--   0        0        0     2071 2023-05-31 22:55:27.557819 tapipy-1.4.0a4/tapipy/errors.py
--rw-r--r--   0        0        0    38703 2023-06-02 16:26:38.119280 tapipy-1.4.0a4/tapipy/resources/openapi_v3-actors.yml
--rw-r--r--   0        0        0    65123 2023-05-31 22:55:27.557819 tapipy-1.4.0a4/tapipy/resources/openapi_v3-apps.yml
--rw-r--r--   0        0        0    23782 2023-05-31 22:55:27.557819 tapipy-1.4.0a4/tapipy/resources/openapi_v3-authenticator.yml
--rw-r--r--   0        0        0    73802 2023-06-02 22:48:04.288915 tapipy-1.4.0a4/tapipy/resources/openapi_v3-files.yml
--rw-r--r--   0        0        0    65915 2023-05-31 22:55:27.557819 tapipy-1.4.0a4/tapipy/resources/openapi_v3-jobs.yml
--rw-r--r--   0        0        0    28625 2023-05-31 20:34:22.484233 tapipy-1.4.0a4/tapipy/resources/openapi_v3-meta.yml
--rw-r--r--   0        0        0    52055 2023-05-31 22:55:27.557819 tapipy-1.4.0a4/tapipy/resources/openapi_v3-notifications.yml
--rw-r--r--   0        0        0    33814 2023-05-31 22:55:27.557819 tapipy-1.4.0a4/tapipy/resources/openapi_v3-pgrest.yml
--rw-r--r--   0        0        0    63213 2023-05-31 22:55:27.557819 tapipy-1.4.0a4/tapipy/resources/openapi_v3-pods.yml
--rw-r--r--   0        0        0   145319 2023-05-31 22:55:27.561818 tapipy-1.4.0a4/tapipy/resources/openapi_v3-sk.yml
--rw-r--r--   0        0        0   108752 2023-05-31 22:55:27.561818 tapipy-1.4.0a4/tapipy/resources/openapi_v3-streams.yml
--rw-r--r--   0        0        0    95703 2023-05-31 22:55:27.561818 tapipy-1.4.0a4/tapipy/resources/openapi_v3-systems.yml
--rw-r--r--   0        0        0    25448 2023-05-31 20:34:25.512199 tapipy-1.4.0a4/tapipy/resources/openapi_v3-tenants.yml
--rw-r--r--   0        0        0     8406 2023-05-31 22:55:27.561818 tapipy-1.4.0a4/tapipy/resources/openapi_v3-tokens.yml
--rw-r--r--   0        0        0    87325 2023-06-02 22:48:04.288915 tapipy-1.4.0a4/tapipy/resources/openapi_v3-workflows.yml
--rw-r--r--   0        0        0   727593 2023-06-02 22:52:17.418459 tapipy-1.4.0a4/tapipy/resources/openapi_v3-workflows.ymlraw.yml
--rw-r--r--   0        0        0      785 2023-06-02 22:48:04.288915 tapipy-1.4.0a4/tapipy/resources/resource_etags.json
--rw-r--r--   0        0        0    61852 2023-06-02 22:48:04.288915 tapipy-1.4.0a4/tapipy/specs/tapis-project-tapipy-main-tapipy-resources-openapi_v3-pods.pickle
--rw-r--r--   0        0        0    27037 2023-06-02 22:48:04.288915 tapipy-1.4.0a4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle
--rw-r--r--   0        0        0    69940 2023-06-02 22:48:04.288915 tapipy-1.4.0a4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle
--rw-r--r--   0        0        0    17736 2023-06-02 22:48:04.288915 tapipy-1.4.0a4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle
--rw-r--r--   0        0        0    54861 2023-06-02 22:48:04.288915 tapipy-1.4.0a4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle
--rw-r--r--   0        0        0    57550 2023-06-02 22:48:04.288915 tapipy-1.4.0a4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle
--rw-r--r--   0        0        0    14366 2023-06-02 22:48:04.288915 tapipy-1.4.0a4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle
--rw-r--r--   0        0        0    36903 2023-06-02 22:48:04.288915 tapipy-1.4.0a4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle
--rw-r--r--   0        0        0    23333 2023-06-02 22:48:04.288915 tapipy-1.4.0a4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle
--rw-r--r--   0        0        0    99591 2023-06-02 22:48:04.288915 tapipy-1.4.0a4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle
--rw-r--r--   0        0        0    75745 2023-06-02 22:48:04.288915 tapipy-1.4.0a4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle
--rw-r--r--   0        0        0    77699 2023-06-02 22:48:04.292915 tapipy-1.4.0a4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle
--rw-r--r--   0        0        0    20306 2023-06-02 22:48:04.292915 tapipy-1.4.0a4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle
--rw-r--r--   0        0        0     5985 2023-06-02 22:48:04.292915 tapipy-1.4.0a4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle
--rw-r--r--   0        0        0   156006 2023-06-02 22:48:04.292915 tapipy-1.4.0a4/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle
--rw-r--r--   0        0        0    71157 2023-06-05 18:16:02.795707 tapipy-1.4.0a4/tapipy/tapis.py
--rw-r--r--   0        0        0     3297 2023-06-02 22:48:04.292915 tapipy-1.4.0a4/tapipy/util.py
--rw-r--r--   0        0        0    10020 1970-01-01 00:00:00.000000 tapipy-1.4.0a4/setup.py
--rw-r--r--   0        0        0    10003 1970-01-01 00:00:00.000000 tapipy-1.4.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1539 2023-06-08 15:22:35.013634 tapipy-1.4.0a5/LICENSE.md
+-rw-r--r--   0        0        0     8639 2023-06-08 15:22:20.913795 tapipy-1.4.0a5/README.md
+-rwxr-xr-x   0        0        0      972 2023-06-08 15:51:10.775620 tapipy-1.4.0a5/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-08 15:21:55.962079 tapipy-1.4.0a5/tapipy/__init__.py
+-rw-r--r--   0        0        0    13502 2023-06-08 15:21:46.714184 tapipy-1.4.0a5/tapipy/actors.py
+-rw-r--r--   0        0        0     2071 2023-06-08 15:21:58.470050 tapipy-1.4.0a5/tapipy/errors.py
+-rw-r--r--   0        0        0    38703 2023-06-08 03:44:21.351648 tapipy-1.4.0a5/tapipy/resources/openapi_v3-actors.yml
+-rw-r--r--   0        0        0    65816 2023-06-08 15:51:10.775620 tapipy-1.4.0a5/tapipy/resources/openapi_v3-apps.yml
+-rw-r--r--   0        0        0    23782 2023-06-08 03:44:21.935642 tapipy-1.4.0a5/tapipy/resources/openapi_v3-authenticator.yml
+-rw-r--r--   0        0        0    74553 2023-06-08 15:51:10.775620 tapipy-1.4.0a5/tapipy/resources/openapi_v3-files.yml
+-rw-r--r--   0        0        0    65915 2023-06-08 03:44:29.879560 tapipy-1.4.0a5/tapipy/resources/openapi_v3-jobs.yml
+-rw-r--r--   0        0        0    28625 2023-06-08 03:44:22.571636 tapipy-1.4.0a5/tapipy/resources/openapi_v3-meta.yml
+-rw-r--r--   0        0        0    52671 2023-06-08 15:51:10.775620 tapipy-1.4.0a5/tapipy/resources/openapi_v3-notifications.yml
+-rw-r--r--   0        0        0    33814 2023-06-08 03:44:28.195577 tapipy-1.4.0a5/tapipy/resources/openapi_v3-pgrest.yml
+-rw-r--r--   0        0        0    62115 2023-06-08 15:51:10.775620 tapipy-1.4.0a5/tapipy/resources/openapi_v3-pods.yml
+-rw-r--r--   0        0        0   145319 2023-06-08 03:44:24.443616 tapipy-1.4.0a5/tapipy/resources/openapi_v3-sk.yml
+-rw-r--r--   0        0        0   108752 2023-06-08 03:44:25.403606 tapipy-1.4.0a5/tapipy/resources/openapi_v3-streams.yml
+-rw-r--r--   0        0        0    97327 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/resources/openapi_v3-systems.yml
+-rw-r--r--   0        0        0    25448 2023-06-08 03:44:26.931591 tapipy-1.4.0a5/tapipy/resources/openapi_v3-tenants.yml
+-rw-r--r--   0        0        0     8406 2023-06-08 03:44:27.499585 tapipy-1.4.0a5/tapipy/resources/openapi_v3-tokens.yml
+-rw-r--r--   0        0        0    87200 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/resources/openapi_v3-workflows.yml
+-rw-r--r--   0        0        0      907 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/resources/resource_etags.json
+-rw-r--r--   0        0        0    33491 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/specs/tapis-project-tapipy-main-tapipy-resources-openapi_v3-pods.pickle
+-rw-r--r--   0        0        0    15308 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-actors.pickle
+-rw-r--r--   0        0        0    31045 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-apps.pickle
+-rw-r--r--   0        0        0    11279 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-authenticator.pickle
+-rw-r--r--   0        0        0    33817 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-files.pickle
+-rw-r--r--   0        0        0    39032 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-jobs.pickle
+-rw-r--r--   0        0        0    13263 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-meta.pickle
+-rw-r--r--   0        0        0    26238 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-notifications.pickle
+-rw-r--r--   0        0        0    13256 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-pgrest.pickle
+-rw-r--r--   0        0        0    68833 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-sk.pickle
+-rw-r--r--   0        0        0    57952 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-streams.pickle
+-rw-r--r--   0        0        0    50661 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-systems.pickle
+-rw-r--r--   0        0        0    12036 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tenants.pickle
+-rw-r--r--   0        0        0     4540 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-tokens.pickle
+-rw-r--r--   0        0        0    36855 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/specs/tapis-project-tapipy-prod-tapipy-resources-openapi_v3-workflows.pickle
+-rwxr-xr-x   0        0        0    71061 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/tapis.py
+-rwxr-xr-x   0        0        0     3129 2023-06-08 15:51:10.779620 tapipy-1.4.0a5/tapipy/util.py
+-rw-r--r--   0        0        0    10020 1970-01-01 00:00:00.000000 tapipy-1.4.0a5/setup.py
+-rw-r--r--   0        0        0    10003 1970-01-01 00:00:00.000000 tapipy-1.4.0a5/PKG-INFO
```

### Comparing `tapipy-1.4.0a4/LICENSE.md` & `tapipy-1.4.0a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a4/README.md` & `tapipy-1.4.0a5/README.md`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a4/pyproject.toml` & `tapipy-1.4.0a5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tapipy"
-version = "1.4.0a4"
+version = "1.4.0a5"
 description = "Python lib for interacting with an instance of the Tapis API Framework"
 license = "BSD-4-Clause"
 authors = ["Joe Stubbs <jstubbs@tacc.utexas.edu>"]
 maintainers = ["Joe Stubbs <jstubbs@tacc.utexas.edu>",
 			   "Christian Garcia <cgarcia@tacc.utexas.edu>"]
 readme = "README.md"
 repository = "https://github.com/tapis-project/tapipy"
@@ -15,16 +15,16 @@
 python = "^3.7"
 certifi = ">= 2020.11.8"
 six = "^1.10"
 python_dateutil = "^2.5.3"
 setuptools = ">= 21.0.0"
 urllib3 = "^1.26.5"
 PyJWT = ">= 1.7.1"
-openapi_core = "^0.17"
-openapi_spec_validator = "^0.5.0"
+openapi_core = "^0.12"
+openapi_spec_validator = "^0.4.0"
 requests = "^2.20.0"
 atomicwrites = "^1.4.0"
 cryptography = ">= 3.3.2"
 # jsonschema from 4.0.0 -> 4.3.0 slows tapipy import to 8+ seconds.
 jsonschema = ">= 3.2.0"
 pyyaml = ">= 5.4"
 cloudpickle = ">= 1.6.0"
```

### Comparing `tapipy-1.4.0a4/tapipy/actors.py` & `tapipy-1.4.0a5/tapipy/actors.py`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a4/tapipy/errors.py` & `tapipy-1.4.0a5/tapipy/errors.py`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a4/tapipy/resources/openapi_v3-actors.yml` & `tapipy-1.4.0a5/tapipy/resources/openapi_v3-actors.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a4/tapipy/resources/openapi_v3-apps.yml` & `tapipy-1.4.0a5/tapipy/resources/openapi_v3-apps.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1846,27 +1846,35 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           type: object
         metadata:
           type: object
     RespBoolean:
       type: object
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/ResultBoolean'
         metadata:
           type: object
     ResultBoolean:
       type: object
       properties:
@@ -1877,14 +1885,18 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/ResultNameArray'
         metadata:
           type: object
     ResultNameArray:
       type: object
       properties:
@@ -1897,14 +1909,18 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/ResultChangeCount'
         metadata:
           type: object
     ResultChangeCount:
       type: object
       properties:
@@ -1916,14 +1932,18 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/ResultResourceUrl'
         metadata:
           type: object
     ResultResourceUrl:
       type: object
       properties:
@@ -1934,27 +1954,35 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/TapisApp'
         metadata:
           type: object
     RespApps:
       type: object
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           type: array
           items:
             $ref: '#/components/schemas/TapisApp'
         metadata:
           type: object
           properties:
@@ -1975,14 +2003,18 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           type: array
           minItems: 1
           items:
             $ref: '#/components/schemas/AppHistory'
         metadata:
           type: object
@@ -1991,14 +2023,18 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/ShareInfo'
         metadata:
           type: object
     # -------------------------------------------------------------------------
     # --- Enums ---------------------------------------------------------------
     # -------------------------------------------------------------------------
```

### Comparing `tapipy-1.4.0a4/tapipy/resources/openapi_v3-authenticator.yml` & `tapipy-1.4.0a5/tapipy/resources/openapi_v3-authenticator.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a4/tapipy/resources/openapi_v3-files.yml` & `tapipy-1.4.0a5/tapipy/resources/openapi_v3-files.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 openapi: 3.0.3
 info:
   title: Tapis Files API
   description: The Tapis Files API provides for management of file resources on Tapis systems
-  version: '1.3.5'
+  version: '1.3.6'
   termsOfService: "https://tapis-project.org"
   contact:
     name: "Files API - CICSupport"
     url: "https://tapis-project.org"
     email: "cicsupport@tacc.utexas.edu"
   license:
     name: 3-Clause BSD License
@@ -23,19 +23,24 @@
     variables: {}
 security:
   - TapisJWT: []
 tags:
   - name: General
     description: General service health and readiness
   - name: File Operations
-    description: Manage file resources on Tapis systems. List, upload, copy, native operations, etc.
+    description: |
+      Manage file resources on Tapis systems. List, upload, copy, native operations, etc.
+      Note that not all operations are supported for all system types.
   - name: Content
-    description: Download a file or directory.
+    description: Download a file or directory. Not supported for all system types.
   - name: Transfers
-    description: Manage file transfers. Initiate, cancel and retrieve status.
+    description: |
+      Manage file transfers between two systems. Initiate, cancel and retrieve status.
+      Note that not all combinations of system types are supported. For example, transfers involving a GLOBUS
+      system must be GLOBUS to GLOBUS.
   - name: Permissions
     description: |
       The permissions model allows for fine grained access control of paths on a Tapis system. The system owner
       may grant READ and MODIFY permission to specific users. MODIFY implies READ.
   
       Please note that Tapis also supports a higher level approach to granting access known as *Sharing*.
 
@@ -193,16 +198,16 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/FileStringResponse'
     put:
       tags:
         - File Operations
       description: |
-        Move or copy a file, directory or object on {systemID} at path {path}. Not all operations supported for all
-        system types.
+        Move or copy a file, directory or object on {systemID} at path {path}.
+        Not all operations supported for all system types.
       operationId: moveCopy
       parameters:
         - name: systemId
           in: path
           description: System ID
           required: true
           schema:
@@ -383,19 +388,21 @@
                 $ref: '#/components/schemas/FileStringResponse'
   /v3/files/ops/{systemId}:
     post:
       tags:
         - File Operations
       description: |
         Create a directory on the system at the given path. Not supported for all system types. Currently supported
-        for LINUX and IRODS type systems.
+        for LINUX, IRODS and GLOBUS type systems.
 
         Certain services may use the query parameter *sharedCtx* to indicate that the request is in a shared
         context. *sharedCtx* must be set to the share grantor.
         Tapis will include the share grantor as part of authorization checks.
+
+        If the path already exists as a directory, no error will be returned.
       operationId: mkdir
       parameters:
         - name: systemId
           in: path
           description: System ID
           required: true
           schema:
@@ -579,15 +586,15 @@
                 $ref: '#/components/schemas/FileStringResponse'
 
   /v3/files/utils/linux/facl/{systemId}/{path}:
     get:
       tags:
         - File Operations
       description: |
-        Get file ACLs for files or directories.
+        Get file ACLs for files or directories for a system of type LINUX.
       operationId: getFacl
       parameters:
         - name: systemId
           in: path
           description: System ID
           required: true
           schema:
@@ -631,15 +638,15 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/FileStringResponse'
     post:
       tags:
         - File Operations
       description: |
-        Set file ACLs for files or directories.
+        Set file ACLs for files or directories for a system of type LINUX.
 
         This can be used for a single file or directory, or can be recursive.  If recursion is
         used, it can be made to follow symlinks, or not follow symlinks.
 
         The operations support adding or removing Acl Entries as well as removing all acls or all
         default acls
       operationId: setFacl
@@ -812,14 +819,16 @@
               schema:
                 $ref: '#/components/schemas/TransferTaskListResponse'
     post:
       tags:
         - Transfers
       description: |
         Create a background task which will transfer files between systems.
+        Note that not all combinations of system types are supported. For example, transfers involving a GLOBUS
+        system must be GLOBUS to GLOBUS.
       operationId: createTransferTask
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/ReqTransfer'
         required: true
@@ -1671,15 +1680,15 @@
     # --- FileInfo -----------------------------------------------------------------
     FileInfo:
       type: object
       properties:
         mimeType:
           type: string
         type:
-          type: string
+          $ref: '#/components/schemas/FileTypeEnum'
         owner:
           type: string
         group:
           type: string
         nativePermissions:
           type: string
         url:
@@ -2452,8 +2461,16 @@
         - MODIFY
     ListTypeEnum:
       type: string
       default: OWNED
       enum:
         - OWNED
         - ALL
+    FileTypeEnum:
+      type: string
+      enum:
+        - file
+        - dir
+        - symbolic_link
+        - other
+        - unknown
```

### Comparing `tapipy-1.4.0a4/tapipy/resources/openapi_v3-jobs.yml` & `tapipy-1.4.0a5/tapipy/resources/openapi_v3-jobs.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a4/tapipy/resources/openapi_v3-meta.yml` & `tapipy-1.4.0a5/tapipy/resources/openapi_v3-meta.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a4/tapipy/resources/openapi_v3-notifications.yml` & `tapipy-1.4.0a5/tapipy/resources/openapi_v3-notifications.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1340,27 +1340,35 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           type: object
         metadata:
           type: object
     RespBoolean:
       type: object
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/ResultBoolean'
         metadata:
           type: object
     ResultBoolean:
       type: object
       properties:
@@ -1371,14 +1379,18 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/ResultNameArray'
         metadata:
           type: object
     ResultNameArray:
       type: object
       properties:
@@ -1391,14 +1403,18 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/ResultChangeCount'
         metadata:
           type: object
     ResultChangeCount:
       type: object
       properties:
@@ -1410,14 +1426,18 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/ResultResourceUrl'
         metadata:
           type: object
     ResultResourceUrl:
       type: object
       properties:
@@ -1428,27 +1448,35 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/TapisSubscription'
         metadata:
           type: object
     RespSubscriptions:
       type: object
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           type: array
           items:
             $ref: '#/components/schemas/TapisSubscription'
         metadata:
           type: object
           properties:
@@ -1469,14 +1497,18 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/TestSequence'
         metadata:
           type: object
     # -------------------------------------------------------------------------
     # --- Enums ---------------------------------------------------------------
     # -------------------------------------------------------------------------
```

### Comparing `tapipy-1.4.0a4/tapipy/resources/openapi_v3-pgrest.yml` & `tapipy-1.4.0a5/tapipy/resources/openapi_v3-pgrest.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a4/tapipy/resources/openapi_v3-pods.yml` & `tapipy-1.4.0a5/tapipy/resources/openapi_v3-pods.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1052,83 +1052,65 @@
           description: Validation Error
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/HTTPValidationError'
   /traefik-config:
     get:
-      summary: Api Traefik Config
+      tags:
+        - Misc
+      summary: traefik_config
       description: >-
         Supplies traefik-config to service. Returns json traefik-config object
         for
 
         traefik to use with the http provider. Dynamic configs don't work well
         in 
 
         Kubernetes.
-      operationId: api_traefik_config_traefik_config_get
+      operationId: traefik_config
       responses:
         '200':
           description: Successful Response
           content:
             application/json:
               schema: {}
   /healthcheck:
     get:
-      summary: Api Healthcheck
+      tags:
+        - Misc
+      summary: healthcheck
       description: |-
         Health check for service. Returns healthy when api is running.
         Should add database health check, should add kubernetes health check
-      operationId: api_healthcheck_healthcheck_get
+      operationId: healthcheck
       responses:
         '200':
           description: Successful Response
           content:
             application/json:
               schema: {}
   '/error-handler/{status}':
     get:
-      summary: Error Codes
+      tags:
+        - Misc
+      summary: error_handler
       description: Handles all error codes from Traefik.
-      operationId: error_codes_error_handler__status__get
+      operationId: error_handler
       parameters:
         - required: true
           schema:
             title: Status
           name: status
           in: path
       responses:
         '200':
           description: Successful Response
           content:
             application/json:
-              schema:
-                $ref: '#/components/schemas/TapisApiModel'
-        '422':
-          description: Validation Error
-          content:
-            application/json:
-              schema:
-                $ref: '#/components/schemas/HTTPValidationError'
-  /error-handler:
-    get:
-      summary: Error Codes
-      description: Handles all error codes from Traefik.
-      operationId: error_codes_error_handler_get
-      parameters:
-        - required: true
-          schema:
-            title: Status
-          name: status
-          in: query
-      responses:
-        '200':
-          description: Successful Response
-          content:
-            application/json:
               schema: {}
         '422':
           description: Validation Error
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/HTTPValidationError'
@@ -1776,25 +1758,23 @@
           description: Inherited roles required to view this pod
           default: []
         creation_ts:
           title: Creation Ts
           type: string
           description: Time (UTC) that this pod was created.
           format: date-time
-          default: '2023-05-25T20:51:46.112775Z'
         update_ts:
           title: Update Ts
           type: string
           description: Time (UTC) that this pod was updated.
           format: date-time
-          default: '2023-05-25T20:51:46.112782Z'
         start_instance_ts:
           title: Start Instance Ts
           type: string
-          description: Time (UTC) that this pod instance was started.
+          description: Time (UdTC) that this pod instance was started.
           format: date-time
       additionalProperties: false
       description: Response object for Pod class.
     PodsResponse:
       title: PodsResponse
       required:
         - message
@@ -1980,21 +1960,19 @@
           description: Current status of snapshot.
           default: REQUESTED
         creation_ts:
           title: Creation Ts
           type: string
           description: Time (UTC) that this snapshot was created.
           format: date-time
-          default: '2023-05-25T20:51:46.092862Z'
         update_ts:
           title: Update Ts
           type: string
           description: Time (UTC) that this snapshot was updated.
           format: date-time
-          default: '2023-05-25T20:51:46.092887Z'
       additionalProperties: false
       description: Response object for Snapshot class.
     SnapshotsResponse:
       title: SnapshotsResponse
       required:
         - message
         - metadata
@@ -2017,19 +1995,14 @@
         status:
           title: Status
           type: string
         version:
           title: Version
           type: string
       additionalProperties: false
-    TapisApiModel:
-      title: TapisApiModel
-      type: object
-      properties: {}
-      additionalProperties: false
     UpdatePod:
       title: UpdatePod
       type: object
       properties:
         description:
           title: Description
           type: string
@@ -2274,28 +2247,26 @@
           title: Size
           type: integer
           description: Size of volume currently in MB
           default: 0
         status:
           title: Status
           type: string
-          description: Current status of snapshot.
+          description: Current status of volume.
           default: REQUESTED
         creation_ts:
           title: Creation Ts
           type: string
-          description: Time (UTC) that this snapshot was created.
+          description: Time (UTC) that this volume was created.
           format: date-time
-          default: '2023-05-25T20:51:45.865346Z'
         update_ts:
           title: Update Ts
           type: string
-          description: Time (UTC) that this snapshot was updated.
+          description: Time (UTC) that this volume was updated.
           format: date-time
-          default: '2023-05-25T20:51:45.865353Z'
       additionalProperties: false
       description: Response object for Volume class.
     VolumesResponse:
       title: VolumesResponse
       required:
         - message
         - metadata
```

### Comparing `tapipy-1.4.0a4/tapipy/resources/openapi_v3-sk.yml` & `tapipy-1.4.0a5/tapipy/resources/openapi_v3-sk.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a4/tapipy/resources/openapi_v3-streams.yml` & `tapipy-1.4.0a5/tapipy/resources/openapi_v3-streams.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a4/tapipy/resources/openapi_v3-systems.yml` & `tapipy-1.4.0a5/tapipy/resources/openapi_v3-systems.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 openapi: 3.0.3
 info:
   title: Tapis Systems API
   description: The Tapis Systems API provides for management of Tapis Systems including permissions, credentials and Scheduler Profiles.
-  version: '1.3.2'
+  version: '1.3.3'
   termsOfService: "https://tapis-project.org"
   contact:
     name: "Systems API - CICSupport"
     url: "https://tapis-project.org"
     email: "cicsupport@tacc.utexas.edu"
   license:
     name: 3-Clause BSD License
@@ -236,15 +236,15 @@
         '500':
           description: Server error.
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/RespBasic'
 
-  '/v3/systems/createChildSystem':
+  '/v3/systems/{parentId}/createChildSystem':
     post:
       tags:
         - Child Systems
       description: |
         Create a child system.  The child system gets all of it's attributes from it's parent except for the following
         fields:
           - *id*
@@ -1070,15 +1070,15 @@
           in: query
           description: Unlink all children from the parent. Default is false.
           schema:
             type: boolean
             default: false
       requestBody:
         required: false
-        description: A JSON object specifying credentials.
+        description: A JSON object containing information about which systems should be unlinked.
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/ReqUnlinkChildren'
       responses:
         '200':
           description: System separated from parent.
@@ -1208,25 +1208,25 @@
         - name: userName
           in: path
           required: true
           schema:
             $ref: '#/components/schemas/UserNameString'
         - name: skipCredentialCheck
           in: query
-          description: Bypass initial credential validation (for LINUX and S3). Default is false.
+          description: Bypass initial credential validation. Default is false.
           schema:
             type: boolean
             default: false
       requestBody:
         required: true
         description: A JSON object specifying credentials.
         content:
           application/json:
             schema:
-              $ref: '#/components/schemas/Credential'
+              $ref: '#/components/schemas/ReqUpdateCredential'
       responses:
         '200':
           description: Credentials updated.
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/RespBasic'
@@ -2654,14 +2654,35 @@
           type: string
         accessToken:
           type: string
         refreshToken:
           type: string
         certificate:
           type: string
+    ReqUpdateCredential:
+      type: object
+      properties:
+        loginUser:
+          $ref: '#/components/schemas/UserNameString'
+        password:
+          type: string
+        privateKey:
+          type: string
+        publicKey:
+          type: string
+        accessKey:
+          type: string
+        accessSecret:
+          type: string
+        accessToken:
+          type: string
+        refreshToken:
+          type: string
+        certificate:
+          type: string
     ReqPerms:
       type: object
       required:
         - permissions
       properties:
         permissions:
           type: array
@@ -2718,14 +2739,15 @@
           items:
             type: string
     ReqUnlinkChildren:
       type: object
       properties:
         childSystemIds:
           type: array
+          description: List containing the IDs of the child systems to unlink from the parent system.
           minItems: 1
           items:
             $ref: '#/components/schemas/IdString'
  
     # -------------------------------------------------------------------------
     # --- Response objects ----------------------------------------------------
     # -------------------------------------------------------------------------
@@ -2734,27 +2756,35 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           type: object
         metadata:
           type: object
     RespBoolean:
       type: object
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/ResultBoolean'
         metadata:
           type: object
     ResultBoolean:
       type: object
       properties:
@@ -2765,14 +2795,18 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/ResultNameArray'
         metadata:
           type: object
     ResultNameArray:
       type: object
       properties:
@@ -2785,14 +2819,18 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/ResultChangeCount'
         metadata:
           type: object
     ResultChangeCount:
       type: object
       properties:
@@ -2804,14 +2842,18 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/ResultResourceUrl'
         metadata:
           type: object
     ResultResourceUrl:
       type: object
       properties:
@@ -2822,27 +2864,35 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/TapisSystem'
         metadata:
           type: object
     RespSystems:
       type: object
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           type: array
           items:
             $ref: '#/components/schemas/TapisSystem'
         metadata:
           type: object
           properties:
@@ -2863,14 +2913,18 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           type: array
           minItems: 1
           items:
             $ref: '#/components/schemas/SystemHistory'
         metadata:
           type: object
@@ -2879,40 +2933,52 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/Credential'
         metadata:
           type: object
     RespSchedulerProfile:
       type: object
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/SchedulerProfile'
         metadata:
           type: object
     RespSchedulerProfiles:
       type: object
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           type: array
           items:
             $ref: '#/components/schemas/SchedulerProfile'
         metadata:
           type: object
     RespGlobusAuthUrl:
@@ -2920,14 +2986,18 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/ResultGlobusAuthUrl'
         metadata:
           type: object
     ResultGlobusAuthUrl:
       type: object
       properties:
@@ -2940,14 +3010,18 @@
       properties:
         status:
           type: string
         message:
           type: string
         version:
           type: string
+        commit:
+          type: string
+        build:
+          type: string
         result:
           $ref: '#/components/schemas/ShareInfo'
         metadata:
           type: object
 
     # -------------------------------------------------------------------------
     # --- Enums ---------------------------------------------------------------
```

### Comparing `tapipy-1.4.0a4/tapipy/resources/openapi_v3-tenants.yml` & `tapipy-1.4.0a5/tapipy/resources/openapi_v3-tenants.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a4/tapipy/resources/openapi_v3-tokens.yml` & `tapipy-1.4.0a5/tapipy/resources/openapi_v3-tokens.yml`

 * *Files identical despite different names*

### Comparing `tapipy-1.4.0a4/tapipy/resources/openapi_v3-workflows.yml` & `tapipy-1.4.0a5/tapipy/resources/openapi_v3-workflows.yml`

 * *Files 0% similar despite different names*

```diff
@@ -2187,41 +2187,36 @@
           type: string
 
     Event:
       type: object
       properties:
         branch:
           type: string
-          nullable: true
           default: null
         commit:
-          nullable: true
           type: string
           default: null
         commit_sha:
           type: string
-          nullable: true
           default: null
         context_url:
           type: string
-          nullable: true
           default: null
         directives:
           type: string
         message:
           type: string
         pipeline:
           type: string
         source:
           type: string
         username:
           $ref: '#/components/schemas/Username'
         identity:
           type: string
-          nullable: true
           default: null
         uuid:
           type: string
           format: uuid
 
     # --- String types with constraints ------------------------------------
     ID:
```

### Comparing `tapipy-1.4.0a4/tapipy/resources/resource_etags.json` & `tapipy-1.4.0a5/tapipy/resources/resource_etags.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7333333333333333%*

 * *Differences: {"'apps'": '\'W/"69eef60649b3516d59d10d261ab02da39f9926c5"\'',*

 * * "'files'": '\'W/"ee9feff01143ad76c0cc8cfd66c4c2706e0226a8"\'',*

 * * "'notifications'": '\'W/"8a459ebc50eba937f09b4ecb16eacc93416138c4"\'',*

 * * "'pods'": '\'W/"da6d18aa800a7950aa7d49bce088a29ea99ad2d5"\'',*

 * * "'systems'": '\'W/"a0e719f43ffddc44bd8212ac0091ea2cd4fc689f"\'',*

 * * "'workflows'": '\'W/"fc3153b26218559770d10ed10e7b8743b9c430a8"\''}*

```diff
@@ -1,15 +1,17 @@
 {
     "actors": "W/\"790d47ac8c8c65e702080db8e564c154ee3ba420\"",
-    "apps": "W/\"0a4a20d1bc8b11ff2733248cfc30821ddd4324f7\"",
+    "apps": "W/\"69eef60649b3516d59d10d261ab02da39f9926c5\"",
     "authenticator": "W/\"16fca2e73ad502ffcc2da2c755df8d3abf680a6e\"",
+    "files": "W/\"ee9feff01143ad76c0cc8cfd66c4c2706e0226a8\"",
     "jobs": "W/\"eceba29d169471ccee3d1a1d0db8bff8374fffe2\"",
     "meta": "W/\"e49bc20f1b1e3296278db40fdd6b33d92c44beea\"",
-    "notifications": "W/\"897fb360129add26d02c77562f7ee168ce8f7625\"",
+    "notifications": "W/\"8a459ebc50eba937f09b4ecb16eacc93416138c4\"",
     "pgrest": "W/\"6494d146379036fdd95de0ed7da22d1bec1335cd\"",
-    "pods": "W/\"3a0278fd3115296c03324d28cd449ce8aa4d8793\"",
+    "pods": "W/\"da6d18aa800a7950aa7d49bce088a29ea99ad2d5\"",
     "sk": "W/\"1d60d95dc6576e129817e90c107bd4daf0200e4c\"",
     "streams": "W/\"d48bb1cdc3a01f8b4b42ecacc9f41585c29a660b\"",
-    "systems": "W/\"c0f9059da975bd80b9911958945521765ec020b8\"",
+    "systems": "W/\"a0e719f43ffddc44bd8212ac0091ea2cd4fc689f\"",
     "tenants": "W/\"19937e762737fba432a63c8f32e824c182d2e973\"",
-    "tokens": "W/\"8de22c7d82f2ba9906e937cb1da1610007319e45\""
+    "tokens": "W/\"8de22c7d82f2ba9906e937cb1da1610007319e45\"",
+    "workflows": "W/\"fc3153b26218559770d10ed10e7b8743b9c430a8\""
 }
```

### Comparing `tapipy-1.4.0a4/tapipy/tapis.py` & `tapipy-1.4.0a5/tapipy/tapis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,35 @@
+import time
 from asyncio.log import logger
 from base64 import b64encode
 from collections.abc import Sequence
 import datetime
 import importlib
 import json
 import jwt
 import os
 import requests
-from openapi_core import Spec
-from jsonschema_spec.handlers.file import BaseFilePathHandler
 import yaml
 import pickle
 import shutil
-import time
 import concurrent.futures
 import copy
 from typing import Dict, NewType, Mapping, Optional
 from atomicwrites import atomic_write
 
 from tapipy.util import dereference_spec
 import tapipy.errors
 from . import errors
-
 start_time = time.time()
 
 # Type declarations
 ResourceName = NewType('ResourceName', str)
 ResourceUrl = NewType('ResourceUrl', str)
 SpecPath = NewType('SpecPath', str)
-OpenApiSpec = NewType('OpenApiSpec', Spec)
 Resources = Dict[ResourceName, ResourceUrl]
-Specs = Dict[ResourceName, OpenApiSpec]
 ResourceInfo = Mapping[ResourceName, SpecPath]
 
 
 def _seq_but_not_str(obj: object) -> bool:
     """
     Determine if an object is a Sequence, i.e., has an iteratable type, but not a string, bytearray, etc.
     :param obj: Any python object.
@@ -129,15 +124,15 @@
         'apps': 'https://raw.githubusercontent.com/tapis-project/openapi-apps/dev/AppsAPI.yaml',
         'workflows': 'https://raw.githubusercontent.com/tapis-project/tapis-workflows/dev/src/api/specs/WorkflowsAPI.yaml',
         'notifications': 'https://raw.githubusercontent.com/tapis-project/openapi-notifications/dev/NotificationsAPI.yaml'
     }
 }
 
 
-def _get_specs(resources: Resources, spec_dir: str = None, download_latest_specs: bool = False) -> Specs:
+def _get_specs(resources: Resources, spec_dir: str = None, download_latest_specs: bool = False):
     """
     Gets specs requested in resources.
     Will download any spec that is not already downloaded.
     """
     spec_dir = get_spec_dir(spec_dir)
     # Download and save specs if neccessary
     download_and_pickle_spec_dicts(resources, spec_dir=spec_dir, download_latest_specs=download_latest_specs)
@@ -176,92 +171,89 @@
     # Set off some parallel processes cause it's quick.
     #POOL_SIZE = os.environ.get('POOL_SIZE', 16)
     #pool = multiprocessing.Pool(processes=POOL_SIZE)
     #pool.map(_thread_download_spec_dict, urls_to_download)
     #pool.close()
     #pool.join()
 
-from urllib.parse import urlparse
-def new_call(self, uri):
-    if hasattr(uri, 'read'):
-        return super(BaseFilePathHandler, self).__call__(uri)
-    
-    parsed_url = urlparse(uri)
-    if parsed_url.scheme not in self.allowed_schemes:
-        raise ValueError("Not allowed scheme")
-
-    return self._open(uri)
-
-BaseFilePathHandler.__call__ = new_call
-
 
 def _thread_download_spec_dict(resource_info: ResourceInfo) -> None:
     """
     Function that multiprocessing pool calls to download and store pickled
     spec dicts. Gets spec dict, if it's valid, stores it at 'spec_path',
     else it does nothing.
     """
     resource_name, resource_url, spec_path = resource_info
     # Attempt to get spec from url
     response = requests.get(resource_url)
     if response.status_code == 200:
         try:
-            # Directly creates spec from response. This validates spec as valid.
-            spec = Spec.from_file(response.content)
+            # Loads yaml into Python dictionary
+            spec_dict = yaml.load(response.content, Loader=yaml.FullLoader)
+        except Exception as e:
+            print(f'Got exception when attempting to load yaml for '
+                  f'"{resource_name}" resource; exception: {e}')
+            return
+        try:
+            # We import here as this takes a while to import
+            from openapi_core import create_spec
+            # Attempts to create spec from dict to ensure the spec is valid
+            spec = create_spec(spec_dict)
         except Exception as e:
             print(f'Got exception when test creating spec for "{resource_name}" '
                   f'resource; Spec probably not verifying; exception: {e}')
             return
         try:
             # Dereference spec so we have a dict we can pickle.
-            spec_dict = dereference_spec(spec)
+            deref_spec_dict = dereference_spec(spec)
         except Exception as e:
-            print(f'Got exception when derefrencing spec for "{resource_name}" '
+            print(f'Got exception when dereferencing spec for "{resource_name}" '
                   f'resource; exception: {e}')
             return
         try:
             # Pickles and saves the spec dict to the spec_path atomically
             with atomic_write(f'{spec_path}', overwrite=True, mode='wb') as spec_file:
-                pickle.dump(spec_dict, spec_file, protocol=4)
+                pickle.dump(deref_spec_dict, spec_file, protocol=4)
         except Exception as e:
             print(f'Got exception when attempting to pickle spec_dict for '
                   f'"{resource_name}" resource; exception: {e}')
             return
     else:
         raise KeyError(f'Error getting "{resource_name}" resource. URL: "{resource_url}".'
                        f'Did not get 200, got the following back:\n{response.text}')
 
 
-def unpickle_and_create_specs(resources: Resources, spec_dir: str) -> Specs:
+def unpickle_and_create_specs(resources: Resources, spec_dir: str):
     """
     Pickles loads a specifed spec_path and creates said spec.
     Can't be threaded, map doesn't allow spec object to be sent back.
     """
     specs = {}
-    dicts = {}
     # Get resource path to point the unpickling at.
     for resource_name, url in resources.items():
         if "local:" in url:
+            spec_path = url.replace('local:', '').strip()
             try:
-                spec_path = url.replace('local:', '').strip()
-                spec = Spec.from_file_path(spec_path)
-                spec_dict = dereference_spec(spec)
-                specs.update({resource_name: spec_dict})
-                dicts.update({resource_name: spec_dict})
+                # We import here as this takes a while to import
+                from openapi_core import create_spec
+                with open(spec_path, 'rb') as spec_file:
+                    spec_dict = yaml.load(spec_file, Loader=yaml.FullLoader)
+                spec = create_spec(spec_dict)
+                deref_spec_dict = dereference_spec(spec)
+                specs.update({resource_name: deref_spec_dict})
             except Exception as e:
                 print(f'Error reading local "{resource_name}" resource. '
                       f'Ensure path is absolute {spec_path}. e:{e}')
             continue
         _, _, spec_path = get_file_info_from_url(url, spec_dir)
         try:
             # Unpickle and create_spec
             with open(spec_path, 'rb') as spec_file:
                 spec_dict = pickle.load(spec_file)
             specs.update({resource_name: spec_dict})
-            dicts.update({resource_name: spec_dict})
         except Exception as e:
             print(f'Got exception trying to unpickle spec for '
                   f'spec_path: "{resource_name}"; exception: {e}')
             # Using resource name to look if the resource exists in the
             # tapipy prod resources. If it is found, we fall back and use that!
             # If it isn't we just skip it.
             print(f'Falling back to prod spec for "{resource_name}" resource')
@@ -269,20 +261,19 @@
                 url = RESOURCES['tapipy'][resource_name]
                 _, _, spec_path = get_file_info_from_url(url, spec_dir)
                 try:
                     # Unpickle and create_spec
                     with open(spec_path, 'rb') as spec_file:
                         spec = pickle.load(spec_file)
                     specs.update({resource_name: spec})
-                    dicts.update({resource_name: spec})
                 except Exception as e:
                     print('Error opening tapipy prod spec. This is bad.')
             else:
                 print(f'No "{resource_name}" spec was found to fallback on')
-    return specs, dicts
+    return specs, specs
 
 
 def update_spec_cache(resources: Resources = None, spec_dir: str = None) -> None:
     """
     Allows users to update specified specs in cache.
     If nothing specified, all urls in "RESOURCES" are updated
     in the Tapipy folder.
@@ -936,22 +927,22 @@
 
         # Here we create an attr on the object for each operationId in the spec. The attr is itself an
         # Operation object, defined below, with a special __call__ method.
         # Examples operationId's include "list_files", "upload_file", etc...
         for path_name, path_desc in self.resource_spec.items():
             # Each path_desc is an openapi_core.schema.paths.models.Path object
             # it has an operations object, which is a dictionary of operations associated with the path:
-            for op, op_desc in path_desc.items():
+            for op, op_desc in path_desc["operations"].items():
                 # each op_desc is an openapi_core.schema.operations.models.Operation object.
                 # the op_desc has a number of associated attributes, including operationId, parameters, etc.
                 # we create an Operation object for each one of these:
-                if not op_desc["operationId"]:
-                    print(f"invalid op_dec for {resource_name}; missing operationId. op_desc: {op_desc}")
+                if not op_desc["operation_id"]:
+                    print(f"invalid op_dec for {resource_name}; missing operation_id. op_desc: {op_desc}")
                     continue
-                setattr(self, op_desc["operationId"], Operation(self.resource_name, op_desc, path_name, op, self.tapis_client))
+                setattr(self, op_desc["operation_id"], Operation(self.resource_name, op_desc, path_name, op, self.tapis_client))
 
 
 class Operation(object):
     """
     Represents a single operation on an API resource defined by an OpenAPI spec file.
     Operation objects are in one-to-one correspondence with operationId's defined in the spec file.
     """
@@ -967,18 +958,18 @@
         self.resource_name = resource_name
         self.op_desc = op_desc
         self.path_name = path_name
         self.http_method = http_method
         self.tapis_client = tapis_client
 
         # derived attributes - for convenience
-        self.operation_id = op_desc["operationId"]
-        self.path_parameters = [p for p in op_desc.get('parameters', []) if p['in'] == 'path']
-        self.query_parameters = [p for p in op_desc.get('parameters', []) if p['in'] == 'query']
-        self.request_body = op_desc.get('requestBody', {})
+        self.operation_id = op_desc["operation_id"]
+        self.path_parameters = [p for _, p in op_desc['parameters'].items() if p['location'] == 'PATH']
+        self.query_parameters = [p for _, p in op_desc['parameters'].items() if p['location'] == 'QUERY']
+        self.request_body = op_desc['request_body'] or {}
 
     def __call__(self, **kwargs):
         """
         Turns the operation object into a callable. Arguments must be passed as kwargs, where the name of each kwarg
         corresponds to a "parameter" in the OpenApi definition. Here, parameter could be a path parameter, body
         parameter, or query parameter.
 
@@ -1110,25 +1101,25 @@
                 request_content_types = headers['Content-Type']
             else:
                 request_content_types = self.request_body['content'].keys()
 
             # Note: If multiple content types, we use first content type we have code for
             if 'application/json' in request_content_types:
                 headers['Content-Type'] = 'application/json'
-                required_fields = self.request_body['content']['application/json'].get('schema', {}).get('required', {})
+                required_fields = self.request_body['content']['application/json']['schema'].get('required', [])
 
                 data = {}
                 # if the request body has no defined properties, look for a single "request_body" parameter.
-                if self.request_body['content']['application/json'].get('schema', {}).get('properties', {}) == {}:
+                if self.request_body['content']['application/json']['schema']['properties'] == {}:
                     # choice of "request_body" is arbitrary, as the property name is not provided by the
                     # openapi spec in this case
                     data = kwargs.get('request_body', {})
                 else:
                     # otherwise, the request body has defined properties, so look for each one in the function kwargs
-                    for p_name, p_desc in self.request_body['content']['application/json'].get('schema', {}).get('properties', {}).items():
+                    for p_name, p_desc in self.request_body['content']['application/json']['schema']['properties'].items():
                         if p_name in kwargs:
                             data[p_name] = kwargs[p_name]
                         elif p_name in required_fields:
                             raise errors.InvalidInputError(msg=f'{p_name} is a required argument.')
                     # serialize data before passing it to the request
                 data = json.dumps(data)
             elif 'application/octet-stream' in request_content_types:
@@ -1141,24 +1132,24 @@
             elif 'multipart/form-data' in request_content_types:
                 # We DO NOT set multipart/form-data headers. The requests library will do header creation for us.
                 # multipart/form-data should use request.Request(files={"formpart1": "formdata1", "formpart2": "formdata2}, ...)
                 # With the files arg, requests will set the Content-Type, boundary and Content-Length headers for us.
                 # It doesn't seem to work if we set Content-Type ourselves.
                 # headers['Content-Type'] = 'multipart/form-data'
 
-                required_fields = self.request_body['content']['multipart/form-data'].get('schema', {}).get('required', {})
+                required_fields = self.request_body['content']['multipart/form-data']['schema'].get('required', [])
                 data = {}
                 # if the request body has no defined properties, look for a single "request_body" parameter.
-                if self.request_body['content']['multipart/form-data'].get('schema', {}).get('properties', {}) == {}:
+                if self.request_body['content']['multipart/form-data']['schema']['properties'] == {}:
                     # choice of "request_body" is arbitrary, as the property name is not provided by the
                     # openapi spec in this case
                     data['request_body'] = kwargs.get('request_body', {})
                 else:
                     # otherwise, the request body has defined properties, so look for each one in the function kwargs
-                    for p_name, p_desc in self.request_body['content']['multipart/form-data'].get('schema', {}).get('properties', {}).items():
+                    for p_name, p_desc in self.request_body['content']['multipart/form-data']['schema']['properties'].items():
                         if p_name in kwargs:
                             data[p_name] = kwargs[p_name]
                         elif p_name in required_fields:
                             raise errors.InvalidInputError(msg=f'{p_name} is a required argument.')
                 files = data
             else:
                 # We could default to providing message field
```

### Comparing `tapipy-1.4.0a4/tapipy/util.py` & `tapipy-1.4.0a5/tapipy/util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from enum import Enum
+
 class AttrDict(dict):
     def __getattr__(self, key):
         return self[key]
 
     def __setattr__(self, key, value):
         self[key] = value
 
@@ -41,41 +43,46 @@
     Returns:
     dict: The new dictionary containing the dereferenced schema.
     """
     # If new_spec is not provided, initialize it as an empty dictionary
     if new_spec is None:
         new_spec = {}
 
-    # Open the Spec object and store the result in spec_obj
-    with spec.open() as k:
-        spec_obj = k
-
-    # Iterate over all keys in spec_obj
-    for key, _ in spec_obj.items():
-        next_val = spec_obj[key]
-
-        # If the value at the current key is a dictionary, create a new dictionary in new_spec
-        # and recursively dereference the spec at the current key
-        if isinstance(next_val, dict):
+    if isinstance(spec, dict):
+        iter_spec = spec
+    elif hasattr(spec, "__dict__"):
+        iter_spec = vars(spec)
+    else:
+        iter_spec = spec
+
+    for key, val in iter_spec.items():
+        if key in  ["_resolver", "components"]:
+            continue
+
+        if isinstance(val, dict):
             new_spec[key] = {}
-            dereference_spec(spec / key, new_spec[key])
+            dereference_spec(val, new_spec[key])
 
         # If the value at the current key is a list, create a new list in new_spec
         # and iterate over each item in the list
-        elif isinstance(next_val, list):
+        elif isinstance(val, list):
             new_spec[key] = []
-            for i, item in enumerate(next_val):
+            for i, item in enumerate(val):
                 # If the item is a dictionary, append a new dictionary to the list in new_spec
                 # and recursively dereference the spec for the item
-                if isinstance(item, dict):
+                if hasattr(item, "__dict__"):
                     new_spec[key].append({})
-                    dereference_spec(spec / key / i, new_spec[key][i])
-                # If the item is not a dictionary, append it directly to the list in new_spec
+                    dereference_spec(val[i], new_spec[key][i])
                 else:
                     new_spec[key].append(item)
-        # If the value at the current key is neither a dictionary nor a list,
-        # copy it directly to new_spec
-        else:
-            new_spec[key] = spec_obj[key]
 
-    # Return the new dictionary containing the dereferenced schema
+        elif isinstance(val, Enum):
+            new_spec[key] = val.name
+            
+        elif hasattr(val, "__dict__"):
+            new_spec[key] = {}
+            dereference_spec(val, new_spec[key])
+
+        elif not hasattr(val, "__dict__"):
+            new_spec[key] = val
+
     return new_spec
```

### Comparing `tapipy-1.4.0a4/setup.py` & `tapipy-1.4.0a5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 install_requires = \
 ['PyJWT>=1.7.1',
  'atomicwrites>=1.4.0,<2.0.0',
  'certifi>=2020.11.8',
  'cloudpickle>=1.6.0',
  'cryptography>=3.3.2',
  'jsonschema>=3.2.0',
- 'openapi_core>=0.17,<0.18',
- 'openapi_spec_validator>=0.5.0,<0.6.0',
+ 'openapi_core>=0.12,<0.13',
+ 'openapi_spec_validator>=0.4.0,<0.5.0',
  'python_dateutil>=2.5.3,<3.0.0',
  'pyyaml>=5.4',
  'requests>=2.20.0,<3.0.0',
  'setuptools>=21.0.0',
  'six>=1.10,<2.0',
  'urllib3>=1.26.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'tapipy',
-    'version': '1.4.0a4',
+    'version': '1.4.0a5',
     'description': 'Python lib for interacting with an instance of the Tapis API Framework',
     'long_description': '# tapipy - Tapis V3 Python SDK\n\nPython library for interacting with an instance of the Tapis API Framework.\n\nThe library is automatically generated by referencing the OpenAPI spec files which  a `Tapis` object built from the OpenAPI spec files from TACC\'s Tapis services. With this functionality a user is able to authorize itself with the `Tapis` object and have a \'live\' library in order to interact with Tapis services.\n\n## Development\n\nThis project is under active development, exploring different approaches to SDK generation.\n\n## Installation\nTapipy is packaged on [pypi](https://pypi.org/project/tapipy/) and can be installed with pip.\n\n```\npip install tapipy\n```\n\n\n## Usage\nTapipy\'s Tapis object first must be initialized in order to be used.\nA basic example of logging in with a user account is below.\n\n```\n# Import the Tapis object\nfrom tapipy.tapis import Tapis\n\n# Log into you the Tapis service by providing user/pass and the base url of your tenant. For example, to interact with the tacc tenant --\nt = Tapis(base_url=\'https://tacc.tapis.io\',\n          username=\'myuser\',\n          password=\'mypass\')\n\t  \n# Get tokens that will be used for authentication function calls\nt.get_tokens()\n```\n\nNow you have a Tapis object that is authenticated and able to call Tapis service endpoints. It\'s useful to know that the Tapis object will automatically refresh it\'s token if it is deemed appropriate, so the object should stay in the good graces of Tapis indefinitely.\n\nNow in order to use the Tapis object you can reference the [Tapis Framework](https://tapis-project.github.io/live-docs/) to browse all functions. For example, if I wanted to use the SK service in order to check if a user has a specific role I would find the function on the site (which is just a better way to look at the json specs).\n\nWith the site I can see that I need to use my Tapis object, initialized as `t`, access `sk`, and then use the `hasRole` function with the required inputs as follows.\n```\nt.sk.hasRole(tenant=\'dev\', user=\'_testuser\', roleName=\'Do you have this role?\')\n```\n\n### Special Query Parameters and Headers\nFor the most part, arguments that can or should be passed to a Tapis endpoint are described in the OpenAPI \ndefinition files and recognized automatically by `tapipy`. However, due to limitations in what can be expressed\nin OpenAPI, there are some paramaters that are not defined in the definition files; for example, the search\nparameters for various endpoints.\n\nTo accommodate these cases, `tapipy` recognizes two special keyword arguments to all of its methods that\ncorrespond to Tapis API calls (i.e., all of its "operations"). They are:\n\n  * `_tapis_headers` -- dictionary-like object of header names (keys) and vales.\n  * `_tapis_query_parameters` -- dictionary-like object of query parameter names (keys) and values.\n\nUse the above two special arguments for passing headers (respectively, query parameters) that are not specified\nin the OpenAPI definition of an endpoint.\n\nFor example, I can issue a search using the following syntax:\n\n```\nt.jobs.getJobSearchList(limit=5, orderBy=\'lastUpdated(desc),name(asc)\', _tapis_query_parameters={\'key\': \'value\'})\n```\n\n# Development Docs\n## Running the tests\n\nTests resources are contained within the `test` directory. `Dockerfile-tests` is at root.\n1. Build the test docker image: `docker build -t tapis/tapipy-tests -f Dockerfile-tests .`\n2. Run these tests using the built docker image: `docker run -it --rm -e username=<dev_user> -e password=<dev_pass> tapis/tapipy-tests`\n\n\n## Important Parameters to Know\n\nThe `tapipy` package allows for spec file customization in Tapis object initialization:\n* resource_set: str \n\t* Determines which set of resource to use, master or dev, defaults to master.\n\t* Important to note that if a custom_spec_dictionary is used, it is appended to this resource_set.\n\t\t* For example, you would set master and then specify a custom specs that will be added on.\n* custom_spec_dict: {resource_name: str, resource_url: str}\n\t* Allows users to modify the base resource set urls.\n\t\t* e.g. I can specify actor as a resource name and change the url.\n\t* Also allows users to add new resources to the set.\n\t\t* e.g. I can add a new resource named "test" with a  custom url.\n\t\t* Important that know that any new specs will be downloaded and added to the cache\n\t\t\t* No need to specify download_latest_specs or update spec files.\n\t* ALLOWS LOCAL RESOURCES!\n\t\t* Specify an absolute path in the dict with `local:` prefixing it and tapipy will load in a local OpenAPI v3 yml spec file.\n\t\t* `custom_spec_dict={\'cactus\': \'local: /home/tapis/myfolder/cactusSpec.yml\'}`\n* download_latest_specs: bool\n\t* Allows users to re-download all specs regardless on if they already exist in the cache. Defaulted to False\n\t* This will happen every time the Tapis object is initialized, it\'s a tad slower, and can cause live updates to specs.\n\t\t* As such, be warned. There are functions to update spec files below.\n* spec_dir: str\n\t* Allows users to specify folder to save specs to. Defaults to none which uses Tapipy\'s package folder.\n\t* If you are updating specs it\'s wise to use a different folder in order to not modify the base specs.\n\nThe following is an example of some custom parameter setting. As you can see, the abaco resource will now use the spec at `URL#1`, overwriting the resource definition in the master resource set, it\'ll download it if it doesn\'t exist. The same for the longhorn resource. This means that the Tapis object will now have access to all specs in master like normal, but with a modified abaco and with a new longhorn resource. All of these are stored at the new spec_dir because I don\'t want to accidentally overwrite any base specs if I call `update_spec_cache()` later (talked about in the next section).\n```\nfrom tapipy.tapis import Tapis\n\nt = Tapis(base_url=\'https://admin.develop.tapis.io\',\n          tenant_id=\'admin\',\n          username=\'username\',\n          account_type=\'user\',\n          password=\'password\',\n          resource_set=\'admin\',\n          custom_spec_dict={\'abaco\': \'URL#1\',\n                            \'longhorn\': \'URL#2\'},\n                            \'cactus\': \'local: /home/tapis/myfolder/cactusSpec.yml\'},\n          spec_dir=\'/home/username/tapipy_specs\')\nt.get_tokens()\n```\n\n## Update Specs Files\n\nThe Tapipy package now uses a cache to organize spec dictionaries as pickled files and has the ability to accept custom spec files. By default Tapipy keeps a set of base spec files in the `%tapipy%/specs` folder. These specs are pre-pickled at package creation time.\n\nIn order to update all default spec files a user can use the `update_spec_cache()` function. Said function\'s definition is below. If no resources are provided the function will download all default spec urls in the RESOURCES object in `%tapipy%/tapipy/tapis.py` file.\n```\nResources = Dict[ResourceName, ResourceUrl]\nupdate_spec_cache(resources: Resources = None, spec_dir: str = None)\n```\nUsers are able to specify custom resources to download by providing their own resource dictionary. For example, providing `{\'actors\': \'URLToMyActorDictionary\'}` would update that spec.\n\nUsers can also specify here where to update the spec with the `spec_dir` variable.\n\nThe Tapis object itself also has a `update_spec_cache()` function that takes the Tapis parameters given at startup and updates the spec cache. Meaning that if the Tapis object was given a custom dictionary, the `update_spec_cache()` function would update it without the need for setting parameters.\n```\nt.update_spec_cache()\n```\n\n## Build instructions\n\nBuilding is done with poetry as follows:\n```\npip install poetry\npoetry install\n```\nThis installs `tapipy` to a virtual environment. Run a shell in this environment with:\n```\npoetry shell\n```\n\nTo install locally (not in a virtual environment):\n```\npip install poetry\npoetry build\ncd dists\npip install *.whl\n```\n\n## PyPi Push Instructions\n\n```\npoetry build\npoetry publish\n```\n\n## Archive Usage\nTODO - provide working examples, e.g., \n```\nimport tapipy\nt = tapipy.Tapis(base_url=\'http://localhost:5001\')\nreq = t.tokens.NewTokenRequest(token_type=\'service\', token_tenant_id=\'dev\', token_username=\'admin\')\nt.tokens.create_token(req)\n\nimport openapi_client\nconfiguration = openapi_client.Configuration()\nconfiguration.host = \'http://localhost:5001\'\napi_instance = openapi_client.TokensApi(openapi_client.ApiClient(configuration))\n\nnew_token = openapi_client.NewTokenRequest(token_type=\'service\', token_tenant_id=\'dev\', token_username=\'admin\')\n\nresp = api_instance.create_token(new_token)\njwt = resp.get(\'result\').get(\'access_token\').get(\'access_token\')\n```\n',
     'author': 'Joe Stubbs',
     'author_email': 'jstubbs@tacc.utexas.edu',
     'maintainer': 'Joe Stubbs',
     'maintainer_email': 'jstubbs@tacc.utexas.edu',
     'url': 'https://github.com/tapis-project/tapipy',
```

### Comparing `tapipy-1.4.0a4/PKG-INFO` & `tapipy-1.4.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapipy
-Version: 1.4.0a4
+Version: 1.4.0a5
 Summary: Python lib for interacting with an instance of the Tapis API Framework
 Home-page: https://github.com/tapis-project/tapipy
 License: BSD-4-Clause
 Author: Joe Stubbs
 Author-email: jstubbs@tacc.utexas.edu
 Maintainer: Joe Stubbs
 Maintainer-email: jstubbs@tacc.utexas.edu
@@ -18,16 +18,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyJWT (>=1.7.1)
 Requires-Dist: atomicwrites (>=1.4.0,<2.0.0)
 Requires-Dist: certifi (>=2020.11.8)
 Requires-Dist: cloudpickle (>=1.6.0)
 Requires-Dist: cryptography (>=3.3.2)
 Requires-Dist: jsonschema (>=3.2.0)
-Requires-Dist: openapi_core (>=0.17,<0.18)
-Requires-Dist: openapi_spec_validator (>=0.5.0,<0.6.0)
+Requires-Dist: openapi_core (>=0.12,<0.13)
+Requires-Dist: openapi_spec_validator (>=0.4.0,<0.5.0)
 Requires-Dist: python_dateutil (>=2.5.3,<3.0.0)
 Requires-Dist: pyyaml (>=5.4)
 Requires-Dist: requests (>=2.20.0,<3.0.0)
 Requires-Dist: setuptools (>=21.0.0)
 Requires-Dist: six (>=1.10,<2.0)
 Requires-Dist: urllib3 (>=1.26.5,<2.0.0)
 Project-URL: Repository, https://github.com/tapis-project/tapipy
```

