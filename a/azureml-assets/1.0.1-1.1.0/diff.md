# Comparing `tmp/azureml-assets-1.0.1.tar.gz` & `tmp/azureml-assets-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azureml-assets-1.0.1.tar", last modified: Thu May 18 14:11:33 2023, max compression
+gzip compressed data, was "azureml-assets-1.1.0.tar", last modified: Thu Jun  8 19:23:09 2023, max compression
```

## Comparing `azureml-assets-1.0.1.tar` & `azureml-assets-1.1.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:11:33.481663 azureml-assets-1.0.1/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-05-18 14:11:33.481663 azureml-assets-1.0.1/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:11:33.473663 azureml-assets-1.0.1/azureml/
--rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:11:33.477663 azureml-assets-1.0.1/azureml/assets/
--rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3788 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/asset_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    36250 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4737 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/copy_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:11:33.477663 azureml-assets-1.0.1/azureml/assets/environment/
--rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/environment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15375 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/environment/build.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4773 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/environment/pin_image_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/environment/pin_package_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/environment/pin_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/extract_tagged_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:11:33.477663 azureml-assets-1.0.1/azureml/assets/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/model/mlflow_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/model/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/tag_released_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10152 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/update_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/update_spec.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:11:33.477663 azureml-assets-1.0.1/azureml/assets/util/
--rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/util/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/util/template.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15565 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/util/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15082 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/azureml/assets/validate_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-18 14:11:33.481663 azureml-assets-1.0.1/azureml_assets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-05-18 14:11:33.000000 azureml-assets-1.0.1/azureml_assets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      943 2023-05-18 14:11:33.000000 azureml-assets-1.0.1/azureml_assets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-18 14:11:33.000000 azureml-assets-1.0.1/azureml_assets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-05-18 14:11:33.000000 azureml-assets-1.0.1/azureml_assets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-05-18 14:11:33.000000 azureml-assets-1.0.1/azureml_assets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-18 14:11:33.481663 azureml-assets-1.0.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1221 2023-05-18 14:10:48.000000 azureml-assets-1.0.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 19:23:09.772192 azureml-assets-1.1.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-06-08 19:23:09.772192 azureml-assets-1.1.0/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 19:23:09.764191 azureml-assets-1.1.0/azureml/
+-rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 19:23:09.764191 azureml-assets-1.1.0/azureml/assets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      669 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4119 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/asset_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    36250 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4737 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/copy_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8088 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/deployment_config.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 19:23:09.768191 azureml-assets-1.1.0/azureml/assets/environment/
+-rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/environment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15375 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/environment/build.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6517 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/environment/pin_image_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/environment/pin_package_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/environment/pin_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/extract_tagged_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 19:23:09.768191 azureml-assets-1.1.0/azureml/assets/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/model/mlflow_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/model/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/tag_released_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10380 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/update_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/update_spec.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 19:23:09.772192 azureml-assets-1.1.0/azureml/assets/util/
+-rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/util/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/util/template.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15565 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/util/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15082 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/azureml/assets/validate_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 19:23:09.772192 azureml-assets-1.1.0/azureml_assets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-06-08 19:23:09.000000 azureml-assets-1.1.0/azureml_assets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      979 2023-06-08 19:23:09.000000 azureml-assets-1.1.0/azureml_assets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-08 19:23:09.000000 azureml-assets-1.1.0/azureml_assets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-06-08 19:23:09.000000 azureml-assets-1.1.0/azureml_assets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-06-08 19:23:09.000000 azureml-assets-1.1.0/azureml_assets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-08 19:23:09.772192 azureml-assets-1.1.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-06-08 19:22:30.000000 azureml-assets-1.1.0/setup.py
```

### Comparing `azureml-assets-1.0.1/PKG-INFO` & `azureml-assets-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.0.1
+Version: 1.1.0
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.0.1/azureml/assets/__init__.py` & `azureml-assets-1.1.0/azureml/assets/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     EnvironmentConfig,
     Os,
     PathType,
     PublishLocation,
     PublishVisibility,
     Spec,
 )
+from .deployment_config import (
+    DeploymentConfig,
+)
 from .update_assets import (
     pin_env_files,
     release_tag_exists,
     update_asset,
     update_assets,
 )
 from .update_spec import create_template_data, update as update_spec
```

### Comparing `azureml-assets-1.0.1/azureml/assets/asset_utils.py` & `azureml-assets-1.1.0/azureml/assets/asset_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,38 +37,44 @@
     # Set variables
     logger.set_output(ASSET_COUNT, len(asset_list))
 
 
 def delete_assets(args: argparse.Namespace):
     """Delete assets that are not in the retention file.
 
+    NOTE: This is generally meant to be run against the release branch, where there's
+    no risk of deleting shared files like component source code.
+
     Args:
         args (argparse.Namespace): Args from argparse.
     """
     # Read retention file
     with open(args.retention_file) as f:
         retention_list = f.read().splitlines()
         print(f"Read {len(retention_list)} asset(s) from retention file")
 
     # Find assets under input dir
     asset_count = 0
     deleted_count = 0
     for asset_config in util.find_assets(args.input_dirs, args.asset_config_filename):
         asset_count += 1
         if asset_config.partial_name not in retention_list:
+            # Get common directory, in case asset config file isn't at the root
+            common_dir, _ = util.find_common_directory(asset_config.release_paths)
+
             # Delete asset
             if args.dry_run:
-                logger.print(f"Would delete {asset_config.partial_name}")
+                logger.print(f"Would delete {asset_config.partial_name} from {common_dir}")
             else:
                 try:
-                    logger.print(f"Deleting {asset_config.partial_name}")
-                    shutil.rmtree(asset_config.file_path)
+                    logger.print(f"Deleting {asset_config.partial_name} from {common_dir}")
+                    shutil.rmtree(common_dir)
                     deleted_count += 1
                 except Exception as e:
-                    logger.log_warning(f"Failed to delete {asset_config.partial_name}: {e}")
+                    logger.log_warning(f"Failed to delete {common_dir}: {e}")
 
     # Set variables
     logger.set_output(ASSET_COUNT, asset_count)
     logger.set_output(DELETED_COUNT, deleted_count)
 
 
 if __name__ == '__main__':
```

### Comparing `azureml-assets-1.0.1/azureml/assets/config.py` & `azureml-assets-1.1.0/azureml/assets/config.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.1/azureml/assets/copy_assets.py` & `azureml-assets-1.1.0/azureml/assets/copy_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.1/azureml/assets/environment/build.py` & `azureml-assets-1.1.0/azureml/assets/environment/build.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.1/azureml/assets/environment/pin_image_versions.py` & `azureml-assets-1.1.0/azureml/assets/environment/pin_image_versions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,100 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 
+"""Pin image versions in a Dockerfile."""
+
 import argparse
 import json
 import re
 import urllib.parse
 from pathlib import Path
-from typing import List, Tuple
+from typing import List, Tuple, Union
+from http.client import HTTPResponse
 from urllib.request import Request, urlopen
 
 from azureml.assets.util import logger
 
+from tenacity import retry, stop_after_attempt, wait_fixed, retry_if_not_exception_type, retry_if_not_exception_message
+from urllib.error import HTTPError
+
 LATEST_TAG = "latest"
 # Handles registry/image_name:{{latest-image-tag}} and registry/image_name:{{latest-image-tag:regex}}
 LATEST_IMAGE_TAG = re.compile(r"([^\"'\s]+):\{\{latest-image-tag(?::(.+))?\}\}")
 
 
-def get_latest_tag_or_digest(image: str, tags: List[str]) -> Tuple[str, str]:
+@retry(stop=stop_after_attempt(3), wait=wait_fixed(5),
+       retry=(retry_if_not_exception_type(HTTPError) & retry_if_not_exception_message(match=r".*404.*")))
+def _urlopen_with_retries(request: Union[Request, str]) -> HTTPResponse:
+    """Execute urlopen with retries.
+
+    Args:
+        request (Union[Request, str]): Request to execute, or URL to open.
+
+    Returns:
+        HTTPResponse: Response from urlopen.
+    """
+    return urlopen(request)
+
+
+def _get_latest_tag_or_digest(image: str, tags: List[str]) -> Tuple[str, str]:
+    """Get latest tag or digest for an image.
+
+    Args:
+        image (str): Full image name, including hostname of the container registry.
+        tags (List[str]): List of tags for the image.
+
+    Returns:
+        Tuple[str, str]: Latest tag and digest, or (None, digest) if latest is not found.
+    """
     (hostname, repo) = image.split("/", 1)
 
     # Find another tag corresponding to latest
     latest_tag = None
     latest_digest = None
     for tag in tags:
         # Retrieve digest
         encoded_tag = urllib.parse.quote(tag, safe="")
         request = Request(f"https://{hostname}/v2/{repo}/manifests/{encoded_tag}",
                           method="HEAD",
                           headers={'Accept': "application/vnd.docker.distribution.manifest.v2+json"})
+
         try:
-            response = urlopen(request)
+            response = _urlopen_with_retries(request)
         except Exception as e:
             raise Exception(f"Failed to retrieve manifest for {repo}:{tag}: {e}")
+
         digest = response.info()['Docker-Content-Digest']
 
         if tag == LATEST_TAG:
             # Store latest digest for comparison
             latest_digest = digest
         elif digest == latest_digest:
             # Found matching digest
             latest_tag = tag
             break
 
     return latest_tag, latest_digest
 
 
-def get_latest_image_suffix(image: str, regex: re.Pattern = None) -> str:
+def _get_latest_image_suffix(image: str, regex: re.Pattern = None) -> str:
+    """Get suffix to use for latest image tag or digest.
+
+    Args:
+        image (str): Full image name, including hostname of the container registry.
+        regex (re.Pattern): Regex to use to filter tags.
+
+    Returns:
+        str: Suffix as :tag or @digest.
+    """
     (hostname, repo) = image.split("/", 1)
 
     # Retrieve tags
     try:
-        response = urlopen(f"https://{hostname}/v2/{repo}/tags/list")
+        response = _urlopen_with_retries(f"https://{hostname}/v2/{repo}/tags/list")
     except Exception as e:
         raise Exception(f"Failed to retrieve tags for {repo}: {e}")
     tags = json.loads(response.read().decode("utf-8")).get("tags", [])
 
     # Filter tags and sort in descending order because this should be faster
     tags_sorted = sorted([t for t in tags if t != LATEST_TAG and
                          (regex is None or regex.search(t) is not None)], reverse=True)
@@ -71,45 +111,59 @@
         if LATEST_TAG not in tags:
             raise Exception(f"{image} does not have a {LATEST_TAG} tag")
 
         # Insert latest at the beginning to ensure we get its digest first
         tags_sorted.insert(0, LATEST_TAG)
 
         # Find another tag corresponding to latest, or default to digest
-        latest_tag, latest_digest = get_latest_tag_or_digest(image, tags)
+        latest_tag, latest_digest = _get_latest_tag_or_digest(image, tags)
 
     # Return tag or digest
     if latest_tag is not None:
         return f":{latest_tag}"
     else:
         logger.log_warning(f"Using digest for {image} because a non-{LATEST_TAG} was not found")
         return f"@{latest_digest}"
 
 
 def pin_images(contents: str) -> str:
+    """Pin images in a Dockerfile.
+
+    Args:
+        contents (str): Contents of a Dockerfile.
+
+    Returns:
+        str: Contents of the Dockerfile with images pinned to latest versions.
+    """
     # Process MCR template tags
     while True:
         match = LATEST_IMAGE_TAG.search(contents)
         if not match:
             break
         repo = match.group(1)
         regex = match.group(2)
         message = f"Finding latest image tag/digest for {repo}"
         if regex is not None:
             message += f" matching {regex}"
             regex = re.compile(regex)
         logger.log_debug(message)
-        suffix = get_latest_image_suffix(repo, regex)
+        suffix = _get_latest_image_suffix(repo, regex)
         logger.log_debug(f"Latest image reference is {repo}{suffix}")
         contents = contents[:match.start()] + f"{repo}{suffix}" + contents[match.end():]
 
     return contents
 
 
 def transform_file(input_file: Path, output_file: Path = None):
+    """Transform a file.
+
+    Args:
+        input_file (Path): File to transform.
+        output_file (Path): File to which output will be written. Defaults to the input file.
+    """
     # Read file
     with open(input_file) as f:
         contents = f.read()
 
     # Transform
     contents = pin_images(contents)
```

### Comparing `azureml-assets-1.0.1/azureml/assets/environment/pin_package_versions.py` & `azureml-assets-1.1.0/azureml/assets/environment/pin_package_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.1/azureml/assets/environment/pin_versions.py` & `azureml-assets-1.1.0/azureml/assets/environment/pin_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.1/azureml/assets/extract_tagged_assets.py` & `azureml-assets-1.1.0/azureml/assets/extract_tagged_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.1/azureml/assets/model/mlflow_utils.py` & `azureml-assets-1.1.0/azureml/assets/model/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.1/azureml/assets/model/utils.py` & `azureml-assets-1.1.0/azureml/assets/model/utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.1/azureml/assets/tag_released_assets.py` & `azureml-assets-1.1.0/azureml/assets/tag_released_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.1/azureml/assets/update_assets.py` & `azureml-assets-1.1.0/azureml/assets/update_assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,16 +99,20 @@
     auto_version = asset_config.auto_version
     release_version = None
     check_contents = False
     pending_release = False
 
     # Check existing release dir
     if release_dir.exists():
-        release_asset_config = util.find_assets(input_dirs=release_dir,
-                                                asset_config_filename=asset_config.file_name)[0]
+        release_asset_configs = util.find_assets(input_dirs=release_dir,
+                                                 asset_config_filename=asset_config.file_name)
+        if not release_asset_configs:
+            logger.log_error(f"Release directory {release_dir} exists, but it's missing an asset config file")
+            exit(1)
+        release_asset_config = release_asset_configs[0]
         release_version = release_asset_config.version
         check_contents = True
 
         # See if the asset version is unreleased
         pending_release = not release_tag_exists(release_asset_config, release_directory_root)
         if pending_release and not auto_version and main_version != release_version and skip_unreleased:
             # Skip the unreleased asset version
```

### Comparing `azureml-assets-1.0.1/azureml/assets/update_spec.py` & `azureml-assets-1.1.0/azureml/assets/update_spec.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.1/azureml/assets/util/__init__.py` & `azureml-assets-1.1.0/azureml/assets/util/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.1/azureml/assets/util/logger.py` & `azureml-assets-1.1.0/azureml/assets/util/logger.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.1/azureml/assets/util/template.py` & `azureml-assets-1.1.0/azureml/assets/util/template.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.1/azureml/assets/util/util.py` & `azureml-assets-1.1.0/azureml/assets/util/util.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.1/azureml/assets/validate_assets.py` & `azureml-assets-1.1.0/azureml/assets/validate_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.0.1/azureml_assets.egg-info/PKG-INFO` & `azureml-assets-1.1.0/azureml_assets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.0.1
+Version: 1.1.0
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.0.1/azureml_assets.egg-info/SOURCES.txt` & `azureml-assets-1.1.0/azureml_assets.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 setup.py
 azureml/__init__.py
 azureml/assets/__init__.py
 azureml/assets/asset_utils.py
 azureml/assets/config.py
 azureml/assets/copy_assets.py
+azureml/assets/deployment_config.py
 azureml/assets/extract_tagged_assets.py
 azureml/assets/tag_released_assets.py
 azureml/assets/update_assets.py
 azureml/assets/update_spec.py
 azureml/assets/validate_assets.py
 azureml/assets/environment/__init__.py
 azureml/assets/environment/build.py
```

### Comparing `azureml-assets-1.0.1/setup.py` & `azureml-assets-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 
 """Set up azureml-assets package."""
 
 from setuptools import setup, find_packages
 
 setup(
    name="azureml-assets",
-   version="1.0.1",
+   version="1.1.0",
    description="Utilities for publishing assets to Azure Machine Learning system registries.",
    author="Microsoft Corp",
    packages=find_packages(),
    install_requires=[
       "GitPython>=3.1",
       "ruamel.yaml==0.17.21",
       "pip>=21",
+      "marshmallow>=3.19",
+      "tenacity>=8.2.2",
    ],
    python_requires=">=3.8,<4.0",
    license="MIT",
    classifiers=[
       "Development Status :: 5 - Production/Stable",
       "Intended Audience :: Developers",
       "Topic :: Software Development :: Build Tools",
```

