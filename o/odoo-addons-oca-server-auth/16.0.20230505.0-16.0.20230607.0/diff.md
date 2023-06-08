# Comparing `tmp/odoo_addons_oca_server_auth-16.0.20230505.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_server_auth-16.0.20230607.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1400 bytes, number of entries: 4
--rw-r--r--  2.0 unx      608 b- defN 23-May-06 07:03 odoo_addons_oca_server_auth-16.0.20230505.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-06 07:03 odoo_addons_oca_server_auth-16.0.20230505.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-06 07:03 odoo_addons_oca_server_auth-16.0.20230505.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      416 b- defN 23-May-06 07:03 odoo_addons_oca_server_auth-16.0.20230505.0.dist-info/RECORD
-4 files, 1117 bytes uncompressed, 578 bytes compressed:  48.3%
+Zip file size: 1409 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      725 b- defN 23-Jun-08 05:17 odoo_addons_oca_server_auth-16.0.20230607.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 05:17 odoo_addons_oca_server_auth-16.0.20230607.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-08 05:17 odoo_addons_oca_server_auth-16.0.20230607.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      416 b- defN 23-Jun-08 05:17 odoo_addons_oca_server_auth-16.0.20230607.0.dist-info/RECORD
+4 files, 1234 bytes uncompressed, 587 bytes compressed:  52.4%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_server_auth-16.0.20230505.0.dist-info/METADATA
+Filename: odoo_addons_oca_server_auth-16.0.20230607.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_server_auth-16.0.20230505.0.dist-info/WHEEL
+Filename: odoo_addons_oca_server_auth-16.0.20230607.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_server_auth-16.0.20230505.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_server_auth-16.0.20230607.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_server_auth-16.0.20230505.0.dist-info/RECORD
+Filename: odoo_addons_oca_server_auth-16.0.20230607.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_server_auth-16.0.20230505.0.dist-info/METADATA` & `odoo_addons_oca_server_auth-16.0.20230607.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-server-auth
-Version: 16.0.20230505.0
+Version: 16.0.20230607.0
 Summary: Meta package for oca-server-auth Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-auth-admin-passkey (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-auth-api-key (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-auth-jwt (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-auth-jwt-demo (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-auth-ldaps (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-auth-oidc (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-auth-saml (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

