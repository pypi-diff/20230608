# Comparing `tmp/pasqal-cloud-0.2.6.tar.gz` & `tmp/pasqal-cloud-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal-cloud-0.2.6.tar", last modified: Fri Jun  2 14:10:18 2023, max compression
+gzip compressed data, was "pasqal-cloud-0.2.7.tar", last modified: Thu Jun  8 09:25:09 2023, max compression
```

## Comparing `pasqal-cloud-0.2.6.tar` & `pasqal-cloud-0.2.7.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.066529 pasqal-cloud-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-06-02 14:10:18.066529 pasqal-cloud-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/pasqal_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/pasqal_cloud/device/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/pasqal_cloud/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/device/configuration/emu_tn.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/device/emulator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/pasqal_cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pasqal_cloud/utils/strenum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/pasqal_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-06-02 14:10:18.000000 pasqal-cloud-0.2.6/pasqal_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-02 14:10:18.000000 pasqal-cloud-0.2.6/pasqal_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:10:18.000000 pasqal-cloud-0.2.6/pasqal_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-02 14:10:18.000000 pasqal-cloud-0.2.6/pasqal_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 14:10:18.000000 pasqal-cloud-0.2.6/pasqal_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.062529 pasqal-cloud-0.2.6/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-02 14:10:18.066529 pasqal-cloud-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.066529 pasqal-cloud-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_cloud_sdk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_device_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:18.066529 pasqal-cloud-0.2.6/tests/test_doubles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_doubles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_doubles/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-02 14:10:06.000000 pasqal-cloud-0.2.6/tests/test_project_renaming_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.791922 pasqal-cloud-0.2.7/pasqal_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/pasqal_cloud/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/pasqal_cloud/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/pasqal_cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pasqal_cloud/utils/strenum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/pasqal_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-06-08 09:25:09.000000 pasqal-cloud-0.2.7/pasqal_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-08 09:25:09.000000 pasqal-cloud-0.2.7/pasqal_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:25:09.000000 pasqal-cloud-0.2.7/pasqal_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-08 09:25:09.000000 pasqal-cloud-0.2.7/pasqal_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 09:25:09.000000 pasqal-cloud-0.2.7/pasqal_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_cloud_sdk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:25:09.795922 pasqal-cloud-0.2.7/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_doubles/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-08 09:24:59.000000 pasqal-cloud-0.2.7/tests/test_project_renaming_compatibility.py
```

### Comparing `pasqal-cloud-0.2.6/LICENSE` & `pasqal-cloud-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.6/PKG-INFO` & `pasqal-cloud-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.2.6
+Version: 0.2.7
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -174,25 +174,22 @@
 
 The method returns a dict object mapping a device type to a serialized device specs. These specs can be used
 to instantiate a `Device` instance in the `Pulser` library.
 
 
 ### Target different API endpoints
 
-This is intended to the package developers.
+This is intended to the package developers or users which were given access to non-prod 
+environments of the PASQAL cloud platform.
 
-If you want to redefine the APIs used by the SDK, please, do the following.
+To target a specific environment (`prod`, `preprod` or `dev`), instantiate the SDK class using 
+`PASQAL_ENDPOINTS['env']` for the parameter `endpoints` and `AUTH0_CONFIG['env']` for 
+`auth0` with env being the environment you want to target.
 
+Example:
 ```python
-from pasqal_cloud import SDK, Endpoints, Auth0COnf
+from pasqal_cloud import SDK
 
-endpoints = Endpoints(core = "my_new_core_endpoint")
-auth0 = Auth0Conf(
-    domain="new_domain",
-    public_client_id="public_id",
-    audience="new_audience"
-)
-sdk = SDK(..., endpoints=endpoints, auth0=auth0)
+sdk = SDK(..., endpoints=PASQAL_ENDPOINTS['preprod'], auth0=AUTH_CONFIG['preprod'])
 ```
 
-This enables you to target backend services running locally on your machine, or other environment like preprod or dev.
-
+By default, the targeted environment for `endpoints` and `auth0` is `prod`.
```

### Comparing `pasqal-cloud-0.2.6/README.md` & `pasqal-cloud-0.2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -159,25 +159,22 @@
 
 The method returns a dict object mapping a device type to a serialized device specs. These specs can be used
 to instantiate a `Device` instance in the `Pulser` library.
 
 
 ### Target different API endpoints
 
-This is intended to the package developers.
+This is intended to the package developers or users which were given access to non-prod 
+environments of the PASQAL cloud platform.
 
-If you want to redefine the APIs used by the SDK, please, do the following.
+To target a specific environment (`prod`, `preprod` or `dev`), instantiate the SDK class using 
+`PASQAL_ENDPOINTS['env']` for the parameter `endpoints` and `AUTH0_CONFIG['env']` for 
+`auth0` with env being the environment you want to target.
 
+Example:
 ```python
-from pasqal_cloud import SDK, Endpoints, Auth0COnf
+from pasqal_cloud import SDK
 
-endpoints = Endpoints(core = "my_new_core_endpoint")
-auth0 = Auth0Conf(
-    domain="new_domain",
-    public_client_id="public_id",
-    audience="new_audience"
-)
-sdk = SDK(..., endpoints=endpoints, auth0=auth0)
+sdk = SDK(..., endpoints=PASQAL_ENDPOINTS['preprod'], auth0=AUTH_CONFIG['preprod'])
 ```
 
-This enables you to target backend services running locally on your machine, or other environment like preprod or dev.
-
+By default, the targeted environment for `endpoints` and `auth0` is `prod`.
```

### Comparing `pasqal-cloud-0.2.6/pasqal_cloud/__init__.py` & `pasqal-cloud-0.2.7/pasqal_cloud/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,47 +17,64 @@
 from warnings import warn
 
 from pasqal_cloud.authentication import TokenProvider
 from pasqal_cloud.batch import Batch, RESULT_POLLING_INTERVAL
 from pasqal_cloud.client import Client
 from pasqal_cloud.device import BaseConfig
 from pasqal_cloud.device import EmulatorType
-from pasqal_cloud.endpoints import Auth0Conf, Endpoints
+from pasqal_cloud.endpoints import Auth0Conf, Endpoints, PASQAL_ENDPOINTS, AUTH0_CONFIG
 from pasqal_cloud.job import Job
 
 
 class SDK:
     _client: Client
 
     def __init__(
         self,
         username: Optional[str] = None,
         password: Optional[str] = None,
         token_provider: Optional[TokenProvider] = None,
         endpoints: Optional[Endpoints] = None,
         auth0: Optional[Auth0Conf] = None,
         webhook: Optional[str] = None,
-        group_id: Optional[str] = None,
-        project_id: Optional[str] = None
+        project_id: Optional[str] = None,
+        group_id: Optional[str] = None,  # deprecated
     ):
-        """This class provides helper methods to call the PASQAL Cloud endpoints.
+        """
+        This class provides helper methods to call the PASQAL Cloud endpoints.
 
         To authenticate to PASQAL Cloud, you have to provide either an
         email/password combination or a TokenProvider instance.
         You may omit the password, you will then be prompted to enter one.
+
+        Args:
+            username: email of the user to login as.
+            password: password of the user to login as.
+            token_provider: The token provider is an alternative log-in method not for human users.
+            webhook: Webhook where the job results are automatically sent to.
+            endpoints: Endpoints targeted of the public apis.
+            auth0: Auth0Config object to define the auth0 tenant to target.
+            project_id: ID of the owner project of the batch.
+            group_id (deprecated): Use project_id instead.
         """
 
         # Ticket (#622), to be removed, used to avoid a breaking change during the group to project renaming
         if not project_id:
             if not group_id:
-                raise TypeError("Either a group_id or project_id has to be given as argument")
-            warn('The parameter group_id is deprecated, from now use project_id instead',
-                 DeprecationWarning,
-                 stacklevel=2
-                 )
+                raise TypeError(
+                    "Either a 'group_id' or 'project_id' has to be given as argument"
+                )
+            warn(
+                (
+                    "The parameter 'group_id' is deprecated, from now on use"
+                    " 'project_id' instead"
+                ),
+                DeprecationWarning,
+                stacklevel=2,
+            )
             project_id = group_id
 
         self._client = Client(
             project_id=project_id,
             username=username,
             password=password,
             token_provider=token_provider,
@@ -121,17 +138,15 @@
                 time.sleep(RESULT_POLLING_INTERVAL)
                 batch_rsp, jobs_rsp = self._client._get_batch(batch_id)
 
             if fetch_results:
                 batch_rsp, jobs_rsp = self._client._get_batch(
                     batch_id, fetch_results=True
                 )
-        batch = Batch(**batch_rsp, _client=self._client)
-        for job_rsp in jobs_rsp:
-            batch.jobs[job_rsp["id"]] = Job(**job_rsp, _client=self._client)
+        batch = Batch(**batch_rsp, jobs=jobs_rsp, _client=self._client)
 
         self.batches[batch.id] = batch
         return batch
 
     def get_batch(self, id: str, fetch_results: bool = False) -> Batch:
         """Retrieve a batch's data and all its jobs.
 
@@ -140,17 +155,15 @@
             fetch_results: whether to download job results
 
         Returns:
             Batch: the batch stored in the PCS database.
         """
 
         batch_rsp, jobs_rsp = self._client._get_batch(id, fetch_results=fetch_results)
-        batch = Batch(**batch_rsp, _client=self._client)
-        for job_rsp in jobs_rsp:
-            batch.jobs[job_rsp["id"]] = Job(**job_rsp, _client=self._client)
+        batch = Batch(**batch_rsp, jobs=jobs_rsp, _client=self._client)
         self.batches[batch.id] = batch
         return batch
 
     def cancel_batch(self, id: str) -> Batch:
         """Cancel the given batch on the PCS
 
         Args:
```

### Comparing `pasqal-cloud-0.2.6/pasqal_cloud/_version.py` & `pasqal-cloud-0.2.7/pasqal_cloud/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
```

### Comparing `pasqal-cloud-0.2.6/pasqal_cloud/authentication.py` & `pasqal-cloud-0.2.7/pasqal_cloud/authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 class ExpiringTokenProvider(TokenProvider, ABC):
     """TokenProvider class which caches a token up to its expiry date.
 
     This is an abstract class. Create your custom TokenProvider by inheriting from
     this class and defining your own `_query_token` method. See Auth0TokenProvider for
     an implementation example.
     """
+
     __token_cache: Optional[tuple[datetime, str]] = None
     expiry_window: timedelta = timedelta(minutes=1.0)
 
     @abstractmethod
     def _query_token(self) -> dict[str, Any]:
         """Return a dictionnary mapping the key 'access_token' to the token value.
 
@@ -114,14 +115,15 @@
             # The token is not in a format that could be parsed as a JWT
             pass
         return None
 
 
 class Auth0TokenProvider(ExpiringTokenProvider):
     """ExpiringTokenProvider implementation which fetches a token from auth0."""
+
     def __init__(self, username: str, password: str, auth0: Auth0Conf):
         """Initializes the token provider with user credentials and
         an auth0 configuration object
 
         Args:
             username: name of the user to log in as
             password: password of the user to log in as
```

### Comparing `pasqal-cloud-0.2.6/pasqal_cloud/batch.py` & `pasqal-cloud-0.2.7/pasqal_cloud/batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import time
-from dataclasses import dataclass, field
 from typing import Any, Dict, Optional, Type, Union
-from warnings import warn
+
+from pydantic import BaseModel, Extra, root_validator, validator
 
 from pasqal_cloud.client import Client
-from pasqal_cloud.job import Job
-from pasqal_cloud.device.configuration import BaseConfig, EmuTNConfig, EmuFreeConfig
 from pasqal_cloud.device import EmulatorType
+from pasqal_cloud.device.configuration import (
+    BaseConfig,
+    EmuFreeConfig,
+    EmuTNConfig,
+)
+from pasqal_cloud.job import Job
 
 RESULT_POLLING_INTERVAL = 2  # seconds
 
 
-@dataclass
-class Batch:
-    """Class for batch data.
+class Batch(BaseModel):
+    """Class to load batch data return by the API.
 
     A batch groups up several jobs with the same sequence. When a batch is assigned to
     a QPU, all its jobs are ran sequentially and no other batch can be assigned to the
     device until all its jobs are done and declared complete.
 
     Attributes:
         - complete: Whether the batch has been declared as complete.
@@ -47,38 +50,53 @@
     updated_at: str
     device_type: str
     project_id: str
     id: str
     user_id: int
     priority: int
     status: str
-    webhook: str
+    webhook: Optional[str]
     _client: Client
     sequence_builder: str
-    start_datetime: Optional[str] = None
-    end_datetime: Optional[str] = None
-    device_status: Optional[str] = None
-    jobs: Dict[str, Job] = field(default_factory=dict)
+    start_datetime: Optional[str]
+    end_datetime: Optional[str]
+    device_status: Optional[str]
+    jobs: Dict[str, Job] = {}
     jobs_count: int = 0
-    jobs_count_per_status: Dict[str, int] = field(default_factory=dict)
-    configuration: Optional[Union[BaseConfig, dict]] = None
-    # Ticket (#622)
-    group_id: Optional[str] = None
-
-    def __post_init__(self) -> None:
-        """Post init method to convert the configuration to a BaseConfig object."""
-        if not isinstance(self.configuration, dict):
-            return
+    jobs_count_per_status: Dict[str, int] = {}
+    configuration: Union[BaseConfig, Dict[str, Any], None] = None
+
+    class Config:
+        extra = Extra.allow
+        arbitrary_types_allowed = True
+
+    @validator("configuration", pre=True)
+    def _load_configuration(
+        cls,
+        configuration: Union[Dict[str, Any], BaseConfig, None],
+        values: Dict[str, Any],
+    ) -> Optional[BaseConfig]:
+        if not isinstance(configuration, dict):
+            return configuration
         conf_class: Type[BaseConfig] = BaseConfig
-        if self.device_type == EmulatorType.EMU_TN.value:
+        if values["device_type"] == EmulatorType.EMU_TN.value:
             conf_class = EmuTNConfig
-        elif self.device_type == EmulatorType.EMU_FREE.value:
+        elif values["device_type"] == EmulatorType.EMU_FREE.value:
             conf_class = EmuFreeConfig
 
-        self.configuration = conf_class.from_dict(self.configuration)
+        return conf_class.from_dict(configuration)
+
+    @root_validator(pre=True)
+    def _build_job_dict(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+        jobs = values.get("jobs", [])
+        job_dict = {}
+        for job in jobs:
+            job_dict[job["id"]] = {**job, "_client": values["_client"]}
+        values["jobs"] = job_dict
+        return values
 
     def add_job(
         self,
         runs: int = 100,
         variables: Optional[Dict[str, Any]] = None,
         wait: bool = False,
     ) -> Job:
```

### Comparing `pasqal-cloud-0.2.6/pasqal_cloud/client.py` & `pasqal-cloud-0.2.7/pasqal_cloud/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def __init__(
         self,
         project_id: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
         token_provider: Optional[TokenProvider] = None,
         endpoints: Optional[Endpoints] = None,
-        auth0: Optional[Auth0Conf] = None
+        auth0: Optional[Auth0Conf] = None,
     ):
         if not username and not token_provider:
             raise ValueError(
                 "At least a username or TokenProvider object should be provided."
             )
         if token_provider is not None:
             self._check_token_provider(token_provider)
```

### Comparing `pasqal-cloud-0.2.6/pasqal_cloud/device/configuration/base_config.py` & `pasqal-cloud-0.2.7/pasqal_cloud/device/configuration/base_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import asdict, dataclass, fields
-from typing import Any, Optional
+from typing import Any, Dict, Optional
 
 
 class InvalidConfiguration(Exception):
     pass
 
 
 INVALID_KEY_ERROR_MSG = "Invalid key {} in Configuration.extra_config. Attempted to override a default field."
@@ -22,15 +22,15 @@
     The extra configuration parameters are stored in the `extra_config` field.
     This field is a dictionary that can be used to store any extra configuration
     parameters. The `extra_config` field is not part of the configuration
     dictionary returned by the `to_dict` method. Instead, the extra configuration
     parameters are added to the configuration dictionary.
     """
 
-    extra_config: Optional[dict[str, Any]] = None
+    extra_config: Optional[Dict[str, Any]] = None
 
     def to_dict(self) -> dict[str, Any]:
         """Converts the configuration to a dictionary.
 
         The extra configuration parameters are added to the configuration
         dictionary.
```

### Comparing `pasqal-cloud-0.2.6/pasqal_cloud/device/configuration/emu_tn.py` & `pasqal-cloud-0.2.7/pasqal_cloud/device/configuration/emu_tn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 
-from pasqal_cloud.device.configuration.base_config import BaseConfig, InvalidConfiguration
+from pasqal_cloud.device.configuration.base_config import (
+    BaseConfig,
+    InvalidConfiguration,
+)
 
 DT_VALUE_NOT_VALID = "dt must be larger than 0. Not {}."
 PRECISION_NOT_VALID = "Precision {} not valid. Must be one of 'low', 'normal', 'high'"
 MAX_BOND_DIM_NOT_VALID = "Max bond dimension {} must be larger than 0. Not {}."
 
 
 @dataclass
```

### Comparing `pasqal-cloud-0.2.6/pasqal_cloud/errors.py` & `pasqal-cloud-0.2.7/pasqal_cloud/errors.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.6/pasqal_cloud/job.py` & `pasqal-cloud-0.2.7/pasqal_cloud/job.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from dataclasses import dataclass
 from typing import Any, Dict, List, Optional
-from warnings import warn
+
+from pydantic import BaseModel, Extra
 
 from pasqal_cloud.client import Client
 
 
-@dataclass
-class Job:
+class Job(BaseModel):
     """Class for job data.
 
     Attributes:
         - runs: Number of times the job should be run.
         - batch_id: ID of the batch which the job belongs to.
         - id: Unique identifier for the job.
         - project_id: ID of the project which the users scheduling the job belong to.
@@ -31,20 +30,24 @@
     batch_id: str
     id: str
     project_id: str
     status: str
     _client: Client
     created_at: str
     updated_at: str
-    errors: List[str]
+    errors: Optional[List[str]] = None
     start_timestamp: Optional[str] = None
     end_timestamp: Optional[str] = None
     result: Optional[Dict[str, Any]] = None
     variables: Optional[Dict[str, Any]] = None
     # Ticket (#622)
     group_id: Optional[str] = None
 
+    class Config:
+        extra = Extra.allow
+        arbitrary_types_allowed = True
+
     def cancel(self) -> Dict[str, Any]:
         """Cancel the current job on the PCS."""
         job_rsp = self._client._cancel_job(self.id)
         self.status = job_rsp.get("status", "CANCELED")
         return job_rsp
```

### Comparing `pasqal-cloud-0.2.6/pasqal_cloud/utils/jsend.py` & `pasqal-cloud-0.2.7/pasqal_cloud/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.6/pasqal_cloud.egg-info/PKG-INFO` & `pasqal-cloud-0.2.7/pasqal_cloud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.2.6
+Version: 0.2.7
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -174,25 +174,22 @@
 
 The method returns a dict object mapping a device type to a serialized device specs. These specs can be used
 to instantiate a `Device` instance in the `Pulser` library.
 
 
 ### Target different API endpoints
 
-This is intended to the package developers.
+This is intended to the package developers or users which were given access to non-prod 
+environments of the PASQAL cloud platform.
 
-If you want to redefine the APIs used by the SDK, please, do the following.
+To target a specific environment (`prod`, `preprod` or `dev`), instantiate the SDK class using 
+`PASQAL_ENDPOINTS['env']` for the parameter `endpoints` and `AUTH0_CONFIG['env']` for 
+`auth0` with env being the environment you want to target.
 
+Example:
 ```python
-from pasqal_cloud import SDK, Endpoints, Auth0COnf
+from pasqal_cloud import SDK
 
-endpoints = Endpoints(core = "my_new_core_endpoint")
-auth0 = Auth0Conf(
-    domain="new_domain",
-    public_client_id="public_id",
-    audience="new_audience"
-)
-sdk = SDK(..., endpoints=endpoints, auth0=auth0)
+sdk = SDK(..., endpoints=PASQAL_ENDPOINTS['preprod'], auth0=AUTH_CONFIG['preprod'])
 ```
 
-This enables you to target backend services running locally on your machine, or other environment like preprod or dev.
-
+By default, the targeted environment for `endpoints` and `auth0` is `prod`.
```

### Comparing `pasqal-cloud-0.2.6/pasqal_cloud.egg-info/SOURCES.txt` & `pasqal-cloud-0.2.7/pasqal_cloud.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -35,10 +35,11 @@
 tests/__init__.py
 tests/conftest.py
 tests/test_batch.py
 tests/test_client.py
 tests/test_cloud_sdk_import.py
 tests/test_config.py
 tests/test_device_specs.py
+tests/test_job.py
 tests/test_project_renaming_compatibility.py
 tests/test_doubles/__init__.py
 tests/test_doubles/authentication.py
```

### Comparing `pasqal-cloud-0.2.6/sdk/setup.py` & `pasqal-cloud-0.2.7/sdk/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.6/setup.py` & `pasqal-cloud-0.2.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,18 +36,19 @@
         "Programming Language :: Python :: 3",
     ],
     url="https://github.com/pasqal-io/pasqal-cloud",
     install_requires=[
         "auth0-python >= 3.23.1, <4.0.0 ",
         "requests>=2.25.1, <3.0.0",
         "pyjwt[crypto]>=2.5.0, <3.0.0",
+        "pydantic>=1.10",
     ],
     extras_require={
         "dev": {
-            "black==20.8b1",
+            "black==22.3.0",
             "flake8==3.9.0",
             "flake8-import-order==0.18.1",
             "mypy==0.982",
             "pytest==6.2.5",
             "pytest-cov==2.11.1",
             "types-requests==2.25.1",
             "requests-mock==1.9.3",
```

### Comparing `pasqal-cloud-0.2.6/tests/conftest.py` & `pasqal-cloud-0.2.7/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         "status": "PENDING",
         "webhook": "https://example.com/webhook",
         "_client": pasqal_client_mock,
         "sequence_builder": "pulser",
         "start_datetime": "2023-01-01T00:00:00.000Z",
         "end_datetime": None,
         "device_status": "available",
-        "jobs": {}
+        "jobs": {},
     }
     return Batch(**batch_data)
 
 
 @pytest.fixture
 def job(pasqal_client_mock):
     job_data = {
@@ -97,14 +97,10 @@
         "id": "00000000-0000-0000-0000-000000022010",
         "project_id": "00000000-0000-0000-0000-000000000001",
         "status": "PENDING",
         "_client": pasqal_client_mock,
         "created_at": "2022-12-31T23:59:59.999Z",
         "updated_at": "2023-01-01T00:00:00.000Z",
         "errors": [],
-        "variables": {
-            "param1": 1,
-            "param2": 2,
-            "param3": 3
-        }
+        "variables": {"param1": 1, "param2": 2, "param3": 3},
     }
     return Job(**job_data)
```

### Comparing `pasqal-cloud-0.2.6/tests/test_batch.py` & `pasqal-cloud-0.2.7/tests/test_batch.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,57 +70,53 @@
         for job_id, job in batch.jobs.items():
             assert self.job_id == job_id
             assert job.result == self.job_result
         assert request_mock.last_request.method == "GET"
 
     def test_get_batch(self, batch):
         batch_requested = self.sdk.get_batch(batch.id)
-        assert (
-            batch_requested.id == self.batch_id
-        )
+        assert batch_requested.id == self.batch_id
 
     def test_cancel_batch_self(self, request_mock, batch):
         batch.cancel()
-        assert batch.status == 'CANCELED'
+        assert batch.status == "CANCELED"
         assert request_mock.last_request.method == "PUT"
         assert (
             request_mock.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/batches/{self.batch_id}/cancel"
         )
 
     def test_cancel_batch_sdk(self, request_mock):
         client_rsp = self.sdk.cancel_batch(self.batch_id)
         assert type(client_rsp) == Batch
-        assert client_rsp.status == 'CANCELED'
+        assert client_rsp.status == "CANCELED"
         assert request_mock.last_request.method == "PUT"
         assert (
-                request_mock.last_request.url
-                == f"{self.sdk._client.endpoints.core}/api/v1/batches/{self.batch_id}/cancel"
+            request_mock.last_request.url
+            == f"{self.sdk._client.endpoints.core}/api/v1/batches/{self.batch_id}/cancel"
         )
 
     def test_get_job(self, job):
         job_requested = self.sdk.get_job(job.id)
         print(self.sdk)
-        assert (
-            job_requested.id == job.id
-        )
+        assert job_requested.id == job.id
 
     def test_cancel_job_self(self, request_mock, job):
         job.cancel()
-        assert job.status == 'CANCELED'
+        assert job.status == "CANCELED"
         assert request_mock.last_request.method == "PUT"
         assert (
             request_mock.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}/cancel"
         )
 
     def test_cancel_job_sdk(self, request_mock):
         client_rsp = self.sdk.cancel_job(self.job_id)
         assert type(client_rsp) == Job
-        assert client_rsp.status == 'CANCELED'
+        assert client_rsp.status == "CANCELED"
         assert request_mock.last_request.method == "PUT"
         assert (
             request_mock.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}/cancel"
         )
 
     @pytest.mark.skip(reason="Not enabled during Iroise MVP")
@@ -201,7 +197,23 @@
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
             jobs=[job],
             emulator=emulator,
             configuration=configuration,
         )
         assert batch.configuration == expected
+
+    def test_batch_instantiation_with_extra_field(self, batch):
+        """Instantiating a batch with an extra field should not raise an error.
+
+        This enables us to add new fields in the API response on the batches endpoint
+        without breaking compatibility for users with old versions of the SDK where
+        the field is not present in the Batch class.
+        """
+        batch_dict = batch.dict()  # Batch data expected by the SDK
+        # We add an extra field to mimick the API exposing new values to the user
+        batch_dict["new_field"] = "any_value"
+
+        new_batch = Batch(**batch_dict)  # this should raise no error
+        assert (
+            new_batch.new_field == "any_value"
+        )  # The new value should be stored regardless
```

### Comparing `pasqal-cloud-0.2.6/tests/test_client.py` & `pasqal-cloud-0.2.7/tests/test_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from unittest.mock import patch
 
 import pytest
 from auth0.v3.exceptions import Auth0Error  # type: ignore
 
-from pasqal_cloud import Auth0Conf, Endpoints, SDK
+from pasqal_cloud import Auth0Conf, Endpoints, SDK, AUTH0_CONFIG, PASQAL_ENDPOINTS
 from pasqal_cloud.authentication import TokenProvider
 from tests.test_doubles.authentication import (
     FakeAuth0AuthenticationFailure,
     FakeAuth0AuthenticationSuccess,
 )
 
 
-@patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
-class TestAuthSuccess:
+class TestSDKCommonAttributes:
     project_id = "random_project_id"
     username = "random_username"
     password = "random_password"
     new_core_endpoint = "random_endpoint"
+    no_username = ""
+    no_password = ""
+
 
+@patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
+class TestAuthSuccess(TestSDKCommonAttributes):
     @patch("pasqal_cloud.client.getpass")
     def test_module_getpass_success(self, getpass):
         getpass.return_value = self.password
         SDK(project_id=self.project_id, username=self.username)
         getpass.assert_called_once()
 
     def test_authentication_success(self):
@@ -31,67 +35,69 @@
         SDK(
             project_id=self.project_id,
             token_provider=FakeAuth0AuthenticationSuccess("username", "password", None),
         )
 
     def test_custom_token_provider(self):
         """Test that the custom provider suggested in the readme is working"""
+
         class CustomTokenProvider(TokenProvider):
             def get_token(self):
-                return "your-token" # Replace this value with your token
+                return "your-token"  # Replace this value with your token
+
         SDK(token_provider=CustomTokenProvider(), project_id="project_id")
 
+    @pytest.mark.filterwarnings(
+        "ignore:The parameters 'endpoints' and 'auth0' are deprecated, from now use"
+        " 'env' instead"
+    )
     def test_correct_endpoints(self):
         sdk = SDK(
             project_id=self.project_id,
             username=self.username,
             password=self.password,
             endpoints=Endpoints(core=self.new_core_endpoint),
         )
         assert sdk._client.endpoints.core == self.new_core_endpoint
 
+    @pytest.mark.filterwarnings(
+        "ignore:The parameters 'endpoints' and 'auth0' are deprecated, from now use"
+        " 'env' instead"
+    )
     def test_correct_new_auth0(self):
         new_auth0 = Auth0Conf(domain="new_domain")
         SDK(
             project_id=self.project_id,
             username=self.username,
             password=self.password,
             auth0=new_auth0,
         )
 
 
 @patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationFailure)
-class TestAuthFailure:
-    project_id = "random_project_id"
-    username = "random_username"
-    no_username = ""
-    password = "random_password"
-    no_password = ""
-
+class TestAuthFailure(TestSDKCommonAttributes):
     @patch("pasqal_cloud.client.getpass")
     def test_module_getpass_bad_password(self, getpass):
         getpass.return_value = self.password
 
         with pytest.raises(Auth0Error):
             SDK(project_id=self.project_id, username=self.username)
 
         getpass.assert_called_once()
 
     def test_module_bad_password(self):
         with pytest.raises(Auth0Error):
-            SDK(project_id=self.project_id, username=self.username, password=self.password)
-
+            SDK(
+                project_id=self.project_id,
+                username=self.username,
+                password=self.password,
+            )
 
-class TestAuthInvalidClient:
-    project_id = "random_project_id"
-    username = "random_username"
-    no_username = ""
-    password = "random_password"
-    no_password = ""
 
+class TestAuthInvalidClient(TestSDKCommonAttributes):
     def test_module_no_user_with_password(self):
         with pytest.raises(ValueError):
             SDK(
                 project_id=self.project_id,
                 username=self.no_username,
                 password=self.password,
             )
@@ -128,18 +134,43 @@
                 auth0="",
             )
 
     def test_authentication_no_credentials_provided(self):
         with pytest.raises(ValueError):
             SDK(project_id=self.project_id)
 
+    @pytest.mark.filterwarnings(
+        "ignore:The parameters 'endpoints' and 'auth0' are deprecated, from now use"
+        " 'env' instead"
+    )
     def test_bad_endpoints(self):
         with pytest.raises(TypeError):
             SDK(
                 project_id=self.project_id,
                 username=self.username,
                 password=self.password,
                 endpoints={
                     "core": "",
                     "account": "",
                 },
             )
+
+
+@patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
+class TestEnvSDK(TestSDKCommonAttributes):
+    @pytest.mark.parametrize(
+        "env, core_endpoint_expected",
+        [
+            ("prod", "https://apis.pasqal.cloud/core-fast"),
+            ("preprod", "https://apis.preprod.pasqal.cloud/core-fast"),
+            ("dev", "https://apis.dev.pasqal.cloud/core-fast"),
+        ],
+    )
+    def test_select_env(self, env, core_endpoint_expected):
+        sdk = SDK(
+            project_id=self.project_id,
+            username=self.username,
+            password=self.password,
+            auth0=AUTH0_CONFIG[env],
+            endpoints=PASQAL_ENDPOINTS[env],
+        )
+        assert sdk._client.endpoints.core == core_endpoint_expected
```

### Comparing `pasqal-cloud-0.2.6/tests/test_cloud_sdk_import.py` & `pasqal-cloud-0.2.7/tests/test_cloud_sdk_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 with the former folder called `sdk`.
 """
 
 
 def test_verify_import_sdk_is_module():
     with pytest.warns(DeprecationWarning):
         import sdk
+
         assert inspect.ismodule(sdk)
 
 
 def test_verify_import_classes_from_sdk():
     with pytest.warns(DeprecationWarning):
         from sdk import SDK
         from sdk import Batch
```

### Comparing `pasqal-cloud-0.2.6/tests/test_config.py` & `pasqal-cloud-0.2.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.6/tests/test_device_specs.py` & `pasqal-cloud-0.2.7/tests/test_device_specs.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.6/tests/test_doubles/authentication.py` & `pasqal-cloud-0.2.7/tests/test_doubles/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.6/tests/test_project_renaming_compatibility.py` & `pasqal-cloud-0.2.7/tests/test_project_renaming_compatibility.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from unittest.mock import patch
-from uuid import uuid4
 
 import pytest
 
 from pasqal_cloud import SDK
 from tests.test_doubles.authentication import FakeAuth0AuthenticationSuccess
 
 
@@ -15,19 +14,32 @@
 @patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
 class TestInitSDKWithGroupId:
     project_id = "random_project_id"
     group_id = "random_group_id"
     username = "random_username"
     password = "random_password"
 
-    @pytest.mark.filterwarnings("ignore:The parameter group_id is deprecated, from now use project_id instead")
+    @pytest.mark.filterwarnings(
+        "ignore:The parameter 'group_id' is deprecated, from now on use 'project_id'"
+        " instead"
+    )
     def test_client_group_parameter(self):
-        sdk = SDK(group_id=self.group_id, username=self.username, password=self.password)
+        sdk = SDK(
+            group_id=self.group_id, username=self.username, password=self.password
+        )
         assert sdk._client.project_id == self.group_id
 
     def test_client_project_and_group_given(self):
-        sdk = SDK(project_id=self.project_id, group_id=self.group_id, username=self.username, password=self.password)
+        sdk = SDK(
+            project_id=self.project_id,
+            group_id=self.group_id,
+            username=self.username,
+            password=self.password,
+        )
         assert sdk._client.project_id == self.project_id
 
     def test_client_group_and_project_arguments_not_given(self):
-        with pytest.raises(TypeError, match=r"Either a group_id or project_id has to be given as argument"):
+        with pytest.raises(
+            TypeError,
+            match=r"Either a 'group_id' or 'project_id' has to be given as argument",
+        ):
             SDK(username=self.username, password=self.password)
```

