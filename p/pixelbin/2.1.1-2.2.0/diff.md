# Comparing `tmp/pixelbin-2.1.1.tar.gz` & `tmp/pixelbin-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelbin-2.1.1.tar", max compression
+gzip compressed data, was "pixelbin-2.2.0.tar", max compression
```

## Comparing `pixelbin-2.1.1.tar` & `pixelbin-2.2.0.tar`

### file list

```diff
@@ -1,65 +1,67 @@
--rw-r--r--   0        0        0     1065 2022-05-27 05:55:59.335216 pixelbin-2.1.1/LICENSE
--rw-r--r--   0        0        0     5229 2022-11-08 19:12:32.304049 pixelbin-2.1.1/README.md
--rw-r--r--   0        0        0    71822 2023-05-12 08:24:33.226873 pixelbin-2.1.1/documentation/platform/ASSETS.md
--rw-r--r--   0        0        0     3589 2022-11-08 19:12:32.304660 pixelbin-2.1.1/documentation/platform/ORGANIZATION.md
--rw-r--r--   0        0        0      176 2022-05-27 05:55:59.310022 pixelbin-2.1.1/documentation/platform/README.md
--rw-r--r--   0        0        0      167 2022-05-27 05:55:59.312424 pixelbin-2.1.1/pixelbin/__init__.py
--rw-r--r--   0        0        0        0 2022-05-27 06:01:25.401889 pixelbin-2.1.1/pixelbin/common/__init__.py
--rw-r--r--   0        0        0     3709 2023-05-12 08:24:33.227089 pixelbin-2.1.1/pixelbin/common/aiohttp_helper.py
--rw-r--r--   0        0        0      165 2022-05-27 06:01:25.402704 pixelbin-2.1.1/pixelbin/common/constants.py
--rw-r--r--   0        0        0      276 2022-05-27 05:55:59.314728 pixelbin-2.1.1/pixelbin/common/date_helper.py
--rw-r--r--   0        0        0     1241 2022-11-08 19:12:32.304888 pixelbin-2.1.1/pixelbin/common/exceptions.py
--rw-r--r--   0        0        0     2733 2022-05-27 06:01:25.403240 pixelbin-2.1.1/pixelbin/common/utils.py
--rw-r--r--   0        0        0      272 2022-05-27 06:01:25.403508 pixelbin-2.1.1/pixelbin/platform/OAuthClient.py
--rw-r--r--   0        0        0    57491 2023-02-03 06:42:04.215714 pixelbin-2.1.1/pixelbin/platform/PixelbinClient.py
--rw-r--r--   0        0        0     1164 2022-05-27 06:01:25.404202 pixelbin-2.1.1/pixelbin/platform/PixelbinConfig.py
--rw-r--r--   0        0        0     2289 2023-05-12 08:24:33.227557 pixelbin-2.1.1/pixelbin/platform/PlatformAPIClient.py
--rw-r--r--   0        0        0        0 2022-05-27 05:55:59.316752 pixelbin-2.1.1/pixelbin/platform/__init__.py
--rw-r--r--   0        0        0      318 2022-05-27 05:55:59.316973 pixelbin-2.1.1/pixelbin/platform/enums.py
--rw-r--r--   0        0        0      345 2023-02-03 06:42:04.215978 pixelbin-2.1.1/pixelbin/platform/models/AddCredentialsRequest.py
--rw-r--r--   0        0        0      297 2023-02-03 06:42:04.216164 pixelbin-2.1.1/pixelbin/platform/models/AddCredentialsResponse.py
--rw-r--r--   0        0        0      392 2023-02-03 06:42:04.216350 pixelbin-2.1.1/pixelbin/platform/models/AddPresetRequest.py
--rw-r--r--   0        0        0      446 2023-02-03 06:42:04.216479 pixelbin-2.1.1/pixelbin/platform/models/AddPresetResponse.py
--rw-r--r--   0        0        0      466 2022-11-08 19:12:32.305375 pixelbin-2.1.1/pixelbin/platform/models/AppOrgDetails.py
--rw-r--r--   0        0        0      650 2022-05-27 05:55:59.317908 pixelbin-2.1.1/pixelbin/platform/models/AppSchema.py
--rw-r--r--   0        0        0     2938 2023-02-03 06:42:04.216843 pixelbin-2.1.1/pixelbin/platform/models/AssetsValidator.py
--rw-r--r--   0        0        0      240 2022-05-27 05:55:59.318322 pixelbin-2.1.1/pixelbin/platform/models/BaseSchema.py
--rw-r--r--   0        0        0      331 2022-05-27 05:55:59.318534 pixelbin-2.1.1/pixelbin/platform/models/CreateFolderRequest.py
--rw-r--r--   0        0        0      630 2023-02-03 06:42:04.217084 pixelbin-2.1.1/pixelbin/platform/models/Credentials.py
--rw-r--r--   0        0        0      286 2023-02-03 06:42:04.217347 pixelbin-2.1.1/pixelbin/platform/models/CredentialsItem.py
--rw-r--r--   0        0        0      592 2023-02-03 06:42:04.217573 pixelbin-2.1.1/pixelbin/platform/models/DeleteCredentialsResponse.py
--rw-r--r--   0        0        0      321 2022-05-27 05:55:59.318746 pixelbin-2.1.1/pixelbin/platform/models/DeleteMultipleFilesRequest.py
--rw-r--r--   0        0        0      349 2022-05-27 05:55:59.318959 pixelbin-2.1.1/pixelbin/platform/models/Delimiter.py
--rw-r--r--   0        0        0      287 2022-05-27 05:55:59.319154 pixelbin-2.1.1/pixelbin/platform/models/ErrorSchema.py
--rw-r--r--   0        0        0      732 2022-05-27 05:55:59.319473 pixelbin-2.1.1/pixelbin/platform/models/FileUploadRequest.py
--rw-r--r--   0        0        0      826 2022-05-27 05:55:59.319760 pixelbin-2.1.1/pixelbin/platform/models/FilesResponse.py
--rw-r--r--   0        0        0      424 2022-05-27 05:55:59.319957 pixelbin-2.1.1/pixelbin/platform/models/FoldersResponse.py
--rw-r--r--   0        0        0      481 2023-02-03 06:42:04.217778 pixelbin-2.1.1/pixelbin/platform/models/GetAncestorsResponse.py
--rw-r--r--   0        0        0      384 2023-02-03 06:42:04.218175 pixelbin-2.1.1/pixelbin/platform/models/GetFilesWithConstraintsItem.py
--rw-r--r--   0        0        0      528 2023-02-03 06:42:04.218367 pixelbin-2.1.1/pixelbin/platform/models/GetFilesWithConstraintsRequest.py
--rw-r--r--   0        0        0      461 2023-02-03 06:42:04.218564 pixelbin-2.1.1/pixelbin/platform/models/GetPresetsResponse.py
--rw-r--r--   0        0        0      442 2022-05-27 05:55:59.320141 pixelbin-2.1.1/pixelbin/platform/models/ListFilesResponse.py
--rw-r--r--   0        0        0      590 2022-05-27 05:55:59.320346 pixelbin-2.1.1/pixelbin/platform/models/OrganizationDetailSchema.py
--rw-r--r--   0        0        0      270 2022-11-08 19:12:32.305605 pixelbin-2.1.1/pixelbin/platform/models/OrganizationValidator.py
--rw-r--r--   0        0        0      326 2022-05-27 05:55:59.320885 pixelbin-2.1.1/pixelbin/platform/models/PresignedUrl.py
--rw-r--r--   0        0        0      736 2022-05-27 05:55:59.321142 pixelbin-2.1.1/pixelbin/platform/models/SignedUploadRequest.py
--rw-r--r--   0        0        0      352 2022-05-27 05:55:59.321384 pixelbin-2.1.1/pixelbin/platform/models/SignedUploadResponse.py
--rw-r--r--   0        0        0      583 2022-05-27 05:55:59.321727 pixelbin-2.1.1/pixelbin/platform/models/TransformationModuleResponse.py
--rw-r--r--   0        0        0      474 2022-05-27 05:55:59.321995 pixelbin-2.1.1/pixelbin/platform/models/TransformationModulesResponse.py
--rw-r--r--   0        0        0      299 2023-02-03 06:42:04.218752 pixelbin-2.1.1/pixelbin/platform/models/UpdateCredentialsRequest.py
--rw-r--r--   0        0        0      553 2022-05-27 05:55:59.322258 pixelbin-2.1.1/pixelbin/platform/models/UpdateFileRequest.py
--rw-r--r--   0        0        0      294 2022-05-27 05:55:59.322486 pixelbin-2.1.1/pixelbin/platform/models/UpdateFolderRequest.py
--rw-r--r--   0        0        0      294 2023-02-03 06:42:04.219019 pixelbin-2.1.1/pixelbin/platform/models/UpdatePresetRequest.py
--rw-r--r--   0        0        0      774 2022-05-27 05:55:59.322832 pixelbin-2.1.1/pixelbin/platform/models/UploadResponse.py
--rw-r--r--   0        0        0      730 2022-05-27 05:55:59.323111 pixelbin-2.1.1/pixelbin/platform/models/UrlUploadRequest.py
--rw-r--r--   0        0        0     2248 2023-02-03 06:42:04.219260 pixelbin-2.1.1/pixelbin/platform/models/__init__.py
--rw-r--r--   0        0        0      542 2022-05-27 05:55:59.323718 pixelbin-2.1.1/pixelbin/platform/models/exploreFolderResponse.py
--rw-r--r--   0        0        0      598 2022-05-27 05:55:59.325079 pixelbin-2.1.1/pixelbin/platform/models/exploreItem.py
--rw-r--r--   0        0        0      440 2022-05-27 05:55:59.325358 pixelbin-2.1.1/pixelbin/platform/models/exploreResponse.py
--rw-r--r--   0        0        0      411 2022-05-27 05:55:59.325644 pixelbin-2.1.1/pixelbin/platform/models/folderItem.py
--rw-r--r--   0        0        0      466 2022-05-27 05:55:59.325929 pixelbin-2.1.1/pixelbin/platform/models/page.py
--rw-r--r--   0        0        0        0 2022-05-27 06:01:25.404488 pixelbin-2.1.1/pixelbin/utils/__init__.py
--rw-r--r--   0        0        0     8462 2022-11-08 19:12:32.306120 pixelbin-2.1.1/pixelbin/utils/url.py
--rw-r--r--   0        0        0      762 2023-05-12 08:24:33.228223 pixelbin-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     6269 2023-05-12 08:25:01.613765 pixelbin-2.1.1/setup.py
--rw-r--r--   0        0        0     6095 2023-05-12 08:25:01.614354 pixelbin-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-05-27 05:55:59.335216 pixelbin-2.2.0/LICENSE
+-rw-r--r--   0        0        0     5229 2022-11-08 19:12:32.304049 pixelbin-2.2.0/README.md
+-rw-r--r--   0        0        0    71892 2023-06-08 10:09:17.343564 pixelbin-2.2.0/documentation/platform/ASSETS.md
+-rw-r--r--   0        0        0     3589 2022-11-08 19:12:32.304660 pixelbin-2.2.0/documentation/platform/ORGANIZATION.md
+-rw-r--r--   0        0        0      247 2023-06-08 10:09:17.344691 pixelbin-2.2.0/documentation/platform/README.md
+-rw-r--r--   0        0        0      167 2022-05-27 05:55:59.312424 pixelbin-2.2.0/pixelbin/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-27 06:01:25.401889 pixelbin-2.2.0/pixelbin/common/__init__.py
+-rw-r--r--   0        0        0     3709 2023-05-12 08:24:33.227089 pixelbin-2.2.0/pixelbin/common/aiohttp_helper.py
+-rw-r--r--   0        0        0      165 2022-05-27 06:01:25.402704 pixelbin-2.2.0/pixelbin/common/constants.py
+-rw-r--r--   0        0        0      276 2022-05-27 05:55:59.314728 pixelbin-2.2.0/pixelbin/common/date_helper.py
+-rw-r--r--   0        0        0     1241 2022-11-08 19:12:32.304888 pixelbin-2.2.0/pixelbin/common/exceptions.py
+-rw-r--r--   0        0        0     2733 2022-05-27 06:01:25.403240 pixelbin-2.2.0/pixelbin/common/utils.py
+-rw-r--r--   0        0        0      272 2022-05-27 06:01:25.403508 pixelbin-2.2.0/pixelbin/platform/OAuthClient.py
+-rw-r--r--   0        0        0    59238 2023-06-08 10:09:17.345719 pixelbin-2.2.0/pixelbin/platform/PixelbinClient.py
+-rw-r--r--   0        0        0     1164 2022-05-27 06:01:25.404202 pixelbin-2.2.0/pixelbin/platform/PixelbinConfig.py
+-rw-r--r--   0        0        0     2289 2023-05-12 08:24:33.227557 pixelbin-2.2.0/pixelbin/platform/PlatformAPIClient.py
+-rw-r--r--   0        0        0        0 2022-05-27 05:55:59.316752 pixelbin-2.2.0/pixelbin/platform/__init__.py
+-rw-r--r--   0        0        0      319 2023-06-08 10:09:17.345977 pixelbin-2.2.0/pixelbin/platform/enums.py
+-rw-r--r--   0        0        0      345 2023-02-03 06:42:04.215978 pixelbin-2.2.0/pixelbin/platform/models/AddCredentialsRequest.py
+-rw-r--r--   0        0        0      297 2023-02-03 06:42:04.216164 pixelbin-2.2.0/pixelbin/platform/models/AddCredentialsResponse.py
+-rw-r--r--   0        0        0      392 2023-02-03 06:42:04.216350 pixelbin-2.2.0/pixelbin/platform/models/AddPresetRequest.py
+-rw-r--r--   0        0        0      446 2023-02-03 06:42:04.216479 pixelbin-2.2.0/pixelbin/platform/models/AddPresetResponse.py
+-rw-r--r--   0        0        0      466 2022-11-08 19:12:32.305375 pixelbin-2.2.0/pixelbin/platform/models/AppOrgDetails.py
+-rw-r--r--   0        0        0      650 2022-05-27 05:55:59.317908 pixelbin-2.2.0/pixelbin/platform/models/AppSchema.py
+-rw-r--r--   0        0        0     2938 2023-02-03 06:42:04.216843 pixelbin-2.2.0/pixelbin/platform/models/AssetsValidator.py
+-rw-r--r--   0        0        0      240 2022-05-27 05:55:59.318322 pixelbin-2.2.0/pixelbin/platform/models/BaseSchema.py
+-rw-r--r--   0        0        0      331 2022-05-27 05:55:59.318534 pixelbin-2.2.0/pixelbin/platform/models/CreateFolderRequest.py
+-rw-r--r--   0        0        0      630 2023-02-03 06:42:04.217084 pixelbin-2.2.0/pixelbin/platform/models/Credentials.py
+-rw-r--r--   0        0        0      286 2023-02-03 06:42:04.217347 pixelbin-2.2.0/pixelbin/platform/models/CredentialsItem.py
+-rw-r--r--   0        0        0      592 2023-02-03 06:42:04.217573 pixelbin-2.2.0/pixelbin/platform/models/DeleteCredentialsResponse.py
+-rw-r--r--   0        0        0      321 2022-05-27 05:55:59.318746 pixelbin-2.2.0/pixelbin/platform/models/DeleteMultipleFilesRequest.py
+-rw-r--r--   0        0        0      349 2022-05-27 05:55:59.318959 pixelbin-2.2.0/pixelbin/platform/models/Delimiter.py
+-rw-r--r--   0        0        0      287 2022-05-27 05:55:59.319154 pixelbin-2.2.0/pixelbin/platform/models/ErrorSchema.py
+-rw-r--r--   0        0        0      732 2022-05-27 05:55:59.319473 pixelbin-2.2.0/pixelbin/platform/models/FileUploadRequest.py
+-rw-r--r--   0        0        0      826 2022-05-27 05:55:59.319760 pixelbin-2.2.0/pixelbin/platform/models/FilesResponse.py
+-rw-r--r--   0        0        0      424 2022-05-27 05:55:59.319957 pixelbin-2.2.0/pixelbin/platform/models/FoldersResponse.py
+-rw-r--r--   0        0        0      481 2023-02-03 06:42:04.217778 pixelbin-2.2.0/pixelbin/platform/models/GetAncestorsResponse.py
+-rw-r--r--   0        0        0      384 2023-02-03 06:42:04.218175 pixelbin-2.2.0/pixelbin/platform/models/GetFilesWithConstraintsItem.py
+-rw-r--r--   0        0        0      528 2023-02-03 06:42:04.218367 pixelbin-2.2.0/pixelbin/platform/models/GetFilesWithConstraintsRequest.py
+-rw-r--r--   0        0        0      461 2023-02-03 06:42:04.218564 pixelbin-2.2.0/pixelbin/platform/models/GetPresetsResponse.py
+-rw-r--r--   0        0        0      318 2023-06-08 10:09:17.346152 pixelbin-2.2.0/pixelbin/platform/models/GetTransformationContextSuccessResponse.py
+-rw-r--r--   0        0        0      442 2022-05-27 05:55:59.320141 pixelbin-2.2.0/pixelbin/platform/models/ListFilesResponse.py
+-rw-r--r--   0        0        0      590 2022-05-27 05:55:59.320346 pixelbin-2.2.0/pixelbin/platform/models/OrganizationDetailSchema.py
+-rw-r--r--   0        0        0      270 2022-11-08 19:12:32.305605 pixelbin-2.2.0/pixelbin/platform/models/OrganizationValidator.py
+-rw-r--r--   0        0        0      326 2022-05-27 05:55:59.320885 pixelbin-2.2.0/pixelbin/platform/models/PresignedUrl.py
+-rw-r--r--   0        0        0      736 2022-05-27 05:55:59.321142 pixelbin-2.2.0/pixelbin/platform/models/SignedUploadRequest.py
+-rw-r--r--   0        0        0      352 2022-05-27 05:55:59.321384 pixelbin-2.2.0/pixelbin/platform/models/SignedUploadResponse.py
+-rw-r--r--   0        0        0      583 2022-05-27 05:55:59.321727 pixelbin-2.2.0/pixelbin/platform/models/TransformationModuleResponse.py
+-rw-r--r--   0        0        0      474 2022-05-27 05:55:59.321995 pixelbin-2.2.0/pixelbin/platform/models/TransformationModulesResponse.py
+-rw-r--r--   0        0        0      317 2023-06-08 10:09:17.346323 pixelbin-2.2.0/pixelbin/platform/models/TransformationValidator.py
+-rw-r--r--   0        0        0      299 2023-02-03 06:42:04.218752 pixelbin-2.2.0/pixelbin/platform/models/UpdateCredentialsRequest.py
+-rw-r--r--   0        0        0      553 2022-05-27 05:55:59.322258 pixelbin-2.2.0/pixelbin/platform/models/UpdateFileRequest.py
+-rw-r--r--   0        0        0      294 2022-05-27 05:55:59.322486 pixelbin-2.2.0/pixelbin/platform/models/UpdateFolderRequest.py
+-rw-r--r--   0        0        0      294 2023-02-03 06:42:04.219019 pixelbin-2.2.0/pixelbin/platform/models/UpdatePresetRequest.py
+-rw-r--r--   0        0        0      774 2022-05-27 05:55:59.322832 pixelbin-2.2.0/pixelbin/platform/models/UploadResponse.py
+-rw-r--r--   0        0        0      730 2022-05-27 05:55:59.323111 pixelbin-2.2.0/pixelbin/platform/models/UrlUploadRequest.py
+-rw-r--r--   0        0        0     2414 2023-06-08 10:09:17.347035 pixelbin-2.2.0/pixelbin/platform/models/__init__.py
+-rw-r--r--   0        0        0      542 2022-05-27 05:55:59.323718 pixelbin-2.2.0/pixelbin/platform/models/exploreFolderResponse.py
+-rw-r--r--   0        0        0      598 2022-05-27 05:55:59.325079 pixelbin-2.2.0/pixelbin/platform/models/exploreItem.py
+-rw-r--r--   0        0        0      440 2022-05-27 05:55:59.325358 pixelbin-2.2.0/pixelbin/platform/models/exploreResponse.py
+-rw-r--r--   0        0        0      411 2022-05-27 05:55:59.325644 pixelbin-2.2.0/pixelbin/platform/models/folderItem.py
+-rw-r--r--   0        0        0      466 2022-05-27 05:55:59.325929 pixelbin-2.2.0/pixelbin/platform/models/page.py
+-rw-r--r--   0        0        0        0 2022-05-27 06:01:25.404488 pixelbin-2.2.0/pixelbin/utils/__init__.py
+-rw-r--r--   0        0        0     8462 2022-11-08 19:12:32.306120 pixelbin-2.2.0/pixelbin/utils/url.py
+-rw-r--r--   0        0        0      762 2023-06-08 10:09:17.347394 pixelbin-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6269 2023-06-08 10:09:24.387891 pixelbin-2.2.0/setup.py
+-rw-r--r--   0        0        0     6095 2023-06-08 10:09:24.388509 pixelbin-2.2.0/PKG-INFO
```

### Comparing `pixelbin-2.1.1/LICENSE` & `pixelbin-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/README.md` & `pixelbin-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/documentation/platform/ASSETS.md` & `pixelbin-2.2.0/documentation/platform/ASSETS.md`

 * *Files 0% similar despite different names*

```diff
@@ -724,37 +724,39 @@
 
 | Argument | Type      | Required | Description                   |
 | -------- | --------- | -------- | ----------------------------- |
 | ids      | List[str] | yes      | Array of file \_ids to delete |
 
 _Returned Response:_
 
-[FilesResponse](#filesresponse)
+[List[FilesResponse]](#filesresponse)
 
 Success
 
 <details>
 <summary><i>&nbsp; Example:</i></summary>
 
 ```json
-{
-    "_id": "dummy-uuid",
-    "name": "asset",
-    "path": "dir",
-    "fileId": "dir/asset",
-    "format": "jpeg",
-    "size": 1000,
-    "access": "private",
-    "isActive": true,
-    "tags": ["tag1", "tag2"],
-    "metadata": {
-        "key": "value"
-    },
-    "url": "https://domain.com/filename.jpeg"
-}
+[
+    {
+        "_id": "dummy-uuid",
+        "name": "asset",
+        "path": "dir",
+        "fileId": "dir/asset",
+        "format": "jpeg",
+        "size": 1000,
+        "access": "private",
+        "isActive": true,
+        "tags": ["tag1", "tag2"],
+        "metadata": {
+            "key": "value"
+        },
+        "url": "https://domain.com/filename.jpeg"
+    }
+]
 ```
 
 </details>
 
 ### createFolder
 
 **Summary**: Create folder
```

### Comparing `pixelbin-2.1.1/documentation/platform/ORGANIZATION.md` & `pixelbin-2.2.0/documentation/platform/ORGANIZATION.md`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/common/aiohttp_helper.py` & `pixelbin-2.2.0/pixelbin/common/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/common/exceptions.py` & `pixelbin-2.2.0/pixelbin/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/common/utils.py` & `pixelbin-2.2.0/pixelbin/common/utils.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/PixelbinClient.py` & `pixelbin-2.2.0/pixelbin/platform/PixelbinClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,33 @@
 
 
 from .enums import AccessEnum
 
 
 
 
+
 from .models.AssetsValidator import AssetsValidator
 from .models.OrganizationValidator import OrganizationValidator
+from .models.TransformationValidator import TransformationValidator
 
 
 class PixelbinClient:
     """PixelbinClient is wrapper class for hitting pixelbin apis"""
 
     def __init__(self, config: PixelbinConfig):
         """
         summary: create instance of PixelbinClient
         
         :param - config : instances of PixelbinConfig : Type - PixelbinConfig
         """
         self.config = config
         self.assets = Assets(config)
         self.organization = Organization(config)
+        self.transformation = Transformation(config)
         
     
 
 
 
 class Assets:
     def __init__(self, config):
@@ -2072,7 +2075,79 @@
         return asyncio.get_event_loop().run_until_complete(
             self.getAppOrgDetailsAsync()
         )
 
     
     
 
+
+
+class Transformation:
+    def __init__(self, config):
+        self.config = config
+    
+    
+    
+    
+
+    
+    async def getTransformationContextAsync(
+        self, 
+        
+        url:str=None
+        ) -> dict:   
+        """
+        summary: Get transformation context
+        description: Get transformation context
+        :param - url : CDN URL with transformation.: Type - str 
+        
+        """
+
+        payload = {}
+        
+        if url is not None:
+            payload["url"] = url
+        
+
+        # Parameter validation
+        schema = TransformationValidator.getTransformationContext()
+        schema.dump(schema.load(payload))
+
+        
+
+        query_params = {}
+        
+        if url:
+            query_params['url'] = url
+        
+
+        response = await APIClient.execute(
+            conf=self.config,
+            method="get",
+            url=f"/service/platform/transformation/context",
+            query=query_params,
+            body=None,
+            contentType=""
+            )
+        if response["status_code"] != 200:
+            raise PixelbinServerResponseError(str(response["content"]))
+        return ujson.loads(response["content"])
+
+    def getTransformationContext(
+        self, 
+        
+        url:str=None
+        ):   
+        """
+        summary: Get transformation context
+        description: Get transformation context
+        :param - url : CDN URL with transformation.: Type - str 
+        
+        """
+        return asyncio.get_event_loop().run_until_complete(
+            self.getTransformationContextAsync(
+                url=url)
+        )
+
+    
+    
+
```

### Comparing `pixelbin-2.1.1/pixelbin/platform/PixelbinConfig.py` & `pixelbin-2.2.0/pixelbin/platform/PixelbinConfig.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/PlatformAPIClient.py` & `pixelbin-2.2.0/pixelbin/platform/PlatformAPIClient.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/AppSchema.py` & `pixelbin-2.2.0/pixelbin/platform/models/AppSchema.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/AssetsValidator.py` & `pixelbin-2.2.0/pixelbin/platform/models/AssetsValidator.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/Credentials.py` & `pixelbin-2.2.0/pixelbin/platform/models/Credentials.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/DeleteCredentialsResponse.py` & `pixelbin-2.2.0/pixelbin/platform/models/DeleteCredentialsResponse.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/FileUploadRequest.py` & `pixelbin-2.2.0/pixelbin/platform/models/FileUploadRequest.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/FilesResponse.py` & `pixelbin-2.2.0/pixelbin/platform/models/FilesResponse.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/GetFilesWithConstraintsRequest.py` & `pixelbin-2.2.0/pixelbin/platform/models/GetFilesWithConstraintsRequest.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/OrganizationDetailSchema.py` & `pixelbin-2.2.0/pixelbin/platform/models/OrganizationDetailSchema.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/SignedUploadRequest.py` & `pixelbin-2.2.0/pixelbin/platform/models/SignedUploadRequest.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/TransformationModuleResponse.py` & `pixelbin-2.2.0/pixelbin/platform/models/TransformationModuleResponse.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/UpdateFileRequest.py` & `pixelbin-2.2.0/pixelbin/platform/models/UpdateFileRequest.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/UploadResponse.py` & `pixelbin-2.2.0/pixelbin/platform/models/UploadResponse.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/UrlUploadRequest.py` & `pixelbin-2.2.0/pixelbin/platform/models/UrlUploadRequest.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/__init__.py` & `pixelbin-2.2.0/pixelbin/platform/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,12 +77,18 @@
 from .AppSchema import AppSchema
     
 from .AppOrgDetails import AppOrgDetails
     
 from .ErrorSchema import ErrorSchema
     
 
+    
+from .GetTransformationContextSuccessResponse import GetTransformationContextSuccessResponse
+    
+
 
 from .AssetsValidator import AssetsValidator
 
 from .OrganizationValidator import OrganizationValidator
 
+from .TransformationValidator import TransformationValidator
+
```

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/exploreFolderResponse.py` & `pixelbin-2.2.0/pixelbin/platform/models/exploreFolderResponse.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/platform/models/exploreItem.py` & `pixelbin-2.2.0/pixelbin/platform/models/exploreItem.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pixelbin/utils/url.py` & `pixelbin-2.2.0/pixelbin/utils/url.py`

 * *Files identical despite different names*

### Comparing `pixelbin-2.1.1/pyproject.toml` & `pixelbin-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pixelbin"
-version = "2.1.1"
+version = "2.2.0"
 description = "Pixelbin SDK for Python"
 authors = ["Pixelbin <dev@pixelbin.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pixelbin-dev/pixelbin-python-sdk"
 repository = "https://github.com/pixelbin-dev/pixelbin-python-sdk"
 keywords = ["Pixelbin"]
```

### Comparing `pixelbin-2.1.1/setup.py` & `pixelbin-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'marshmallow>=3.15.0,<4.0.0',
  'pytest>=7.2.2,<8.0.0',
  'pytz>=2022.1,<2023.0',
  'ujson>=5.2.0,<6.0.0']
 
 setup_kwargs = {
     'name': 'pixelbin',
-    'version': '2.1.1',
+    'version': '2.2.0',
     'description': 'Pixelbin SDK for Python',
     'long_description': '# Pixelbin Backend SDK for Python\n\nPixelbin Backend SDK for python helps you integrate the core Pixelbin features with your application.\n\n## Getting Started\n\nGetting started with Pixelbin Backend SDK for Python\n\n### Installation\n\n```\npip install pixelbin\n```\n\n---\n\n### Usage\n\n#### Quick Example\n\n```python\nimport asyncio\n\nfrom pixelbin import PixelbinClient, PixelbinConfig\n\n# create client with your API_TOKEN\nconfig = PixelbinConfig({\n    "domain": "https://api.pixelbin.io",\n    "apiSecret": "API_TOKEN",\n})\n\n# Create a pixelbin instance\npixelbin:PixelbinClient = PixelbinClient(config=config)\n\n# Sync method call\ntry:\n    result = pixelbin.assets.listFiles()\n    print(result)\nexcept Exception as e:\n    print(e)\n\n# Async method call\ntry:\n    result = asyncio.get_event_loop().run_until_complete(pixelbin.assets.listFilesAsync())\n    print(result)\nexcept Exception as e:\n    print(e)\n```\n\n## Utilities\n\nPixelbin provides url utilities to construct and deconstruct Pixelbin urls.\n\n### url_to_obj\n\nDeconstruct a pixelbin url\n\n| parameter            | description          | example                                                                                               |\n| -------------------- | -------------------- | ----------------------------------------------------------------------------------------------------- |\n| pixelbinUrl (string) | A valid pixelbin url | `https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg` |\n\n**Returns**:\n\n| property                | description                            | example                    |\n| ----------------------- | -------------------------------------- | -------------------------- |\n| cloudName (string)      | The cloudname extracted from the url   | `your-cloud-name`          |\n| zone (string)           | 6 character zone slug                  | `z-slug`                   |\n| version (string)        | cdn api version                        | `v2`                       |\n| options (object)        | optional query parameters              |                            |\n| transformations (array) | Extracted transformations from the url |                            |\n| filePath                | Path to the file on Pixelbin storage   | `/path/to/image.jpeg`      |\n| baseUrl (string)        | Base url                               | `https://cdn.pixelbin.io/` |\n\nExample:\n\n```python\nfrom pixelbin.utils.url import url_to_obj\n\npixelbinUrl = "https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg?dpr=2.0&f_auto=True"\nobj = url_to_obj(pixelbinUrl)\n# obj\n# {\n#     "cloudName": "your-cloud-name",\n#     "zone": "z-slug",\n#     "version": "v2",\n#     "options": {\n#         "dpr": 2.0,\n#         "f_auto": True,\n#     },\n#     "transformations": [\n#         {\n#             "plugin": "t",\n#             "name": "resize",\n#             "values": [\n#                 {\n#                     "key": "h",\n#                     "value": "100"\n#                 },\n#                 {\n#                     "key": "w",\n#                     "value": "200"\n#                 }\n#             ]\n#         },\n#         {\n#             "plugin": "t",\n#             "name": "flip",\n#         }\n#     ],\n#     "filePath": "path/to/image.jpeg",\n#     "baseUrl": "https://cdn.pixelbin.io"\n# }\n```\n\n### obj_to_url\n\nConverts the extracted url obj to a Pixelbin url.\n\n| property                | description                            | example                    |\n| ----------------------- | -------------------------------------- | -------------------------- |\n| cloudName (string)      | The cloudname extracted from the url   | `your-cloud-name`          |\n| zone (string)           | 6 character zone slug                  | `z-slug`                   |\n| version (string)        | cdn api version                        | `v2`                       |\n| options (object)        | optional query parameters              |                            |\n| transformations (array) | Extracted transformations from the url |                            |\n| filePath                | Path to the file on Pixelbin storage   | `/path/to/image.jpeg`      |\n| baseUrl (string)        | Base url                               | `https://cdn.pixelbin.io/` |\n\n```python\nfrom pixelbin.utils.url import obj_to_url\n\nobj = {\n    cloudName: "your-cloud-name",\n    zone: "z-slug",\n    version: "v2",\n    options: {\n        dpr: 2.0,\n        f_auto: True,\n    },\n    transformations: [\n        {\n            plugin: "t",\n            name: "resize",\n            values: [\n                {\n                    key: "h",\n                    value: "100",\n                },\n                {\n                    key: "w",\n                    value: "200",\n                },\n            ],\n        },\n        {\n            plugin: "t",\n            name: "flip",\n        },\n    ],\n    filePath: "path/to/image.jpeg",\n    baseUrl: "https://cdn.pixelbin.io",\n}\nurl = obj_to_url(obj) # obj is as shown above\n# url\n# https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg?dpr=2.0&f_auto=True\n```\n\n## Documentation\n\n-   [API docs](documentation/platform/README.md)\n',
     'author': 'Pixelbin',
     'author_email': 'dev@pixelbin.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/pixelbin-dev/pixelbin-python-sdk',
```

### Comparing `pixelbin-2.1.1/PKG-INFO` & `pixelbin-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelbin
-Version: 2.1.1
+Version: 2.2.0
 Summary: Pixelbin SDK for Python
 Home-page: https://github.com/pixelbin-dev/pixelbin-python-sdk
 License: MIT
 Keywords: Pixelbin
 Author: Pixelbin
 Author-email: dev@pixelbin.io
 Requires-Python: >=3.8,<4.0
```

