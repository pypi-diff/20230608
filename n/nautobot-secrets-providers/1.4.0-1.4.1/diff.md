# Comparing `tmp/nautobot_secrets_providers-1.4.0.tar.gz` & `tmp/nautobot_secrets_providers-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_secrets_providers-1.4.0.tar", max compression
+gzip compressed data, was "nautobot_secrets_providers-1.4.1.tar", max compression
```

## Comparing `nautobot_secrets_providers-1.4.0.tar` & `nautobot_secrets_providers-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      591 2023-04-19 20:54:25.659742 nautobot_secrets_providers-1.4.0/LICENSE
--rw-r--r--   0        0        0    28981 2023-04-19 20:54:25.659742 nautobot_secrets_providers-1.4.0/README.md
--rw-r--r--   0        0        0     1194 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/migrations/__init__.py
--rw-r--r--   0        0        0      690 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/__init__.py
--rw-r--r--   0        0        0     7245 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/aws.py
--rw-r--r--   0        0        0      800 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/choices.py
--rw-r--r--   0        0        0     9512 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/delinea.py
--rw-r--r--   0        0        0     9120 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/hashicorp.py
--rw-r--r--   0        0        0      758 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/secrets.py
--rw-r--r--   0        0        0     3452 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/templates/nautobot_secrets_providers/home.html
--rw-r--r--   0        0        0       56 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/tests/__init__.py
--rw-r--r--   0        0        0     2086 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/tests/nautobot_config.py
--rw-r--r--   0        0        0      621 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/tests/test_basic.py
--rw-r--r--   0        0        0    26973 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/tests/test_providers.py
--rw-r--r--   0        0        0      281 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/urls.py
--rw-r--r--   0        0        0      534 2023-04-19 20:54:25.663742 nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/views.py
--rw-r--r--   0        0        0     3105 2023-04-19 20:54:35.383724 nautobot_secrets_providers-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    30235 1970-01-01 00:00:00.000000 nautobot_secrets_providers-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-06-08 16:22:15.947508 nautobot_secrets_providers-1.4.1/LICENSE
+-rw-r--r--   0        0        0    28981 2023-06-08 16:22:15.947508 nautobot_secrets_providers-1.4.1/README.md
+-rw-r--r--   0        0        0     1194 2023-06-08 16:22:15.951508 nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:22:15.951508 nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/migrations/__init__.py
+-rw-r--r--   0        0        0      690 2023-06-08 16:22:15.951508 nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/providers/__init__.py
+-rw-r--r--   0        0        0     7245 2023-06-08 16:22:15.951508 nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/providers/aws.py
+-rw-r--r--   0        0        0      800 2023-06-08 16:22:15.951508 nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/providers/choices.py
+-rw-r--r--   0        0        0     9512 2023-06-08 16:22:15.951508 nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/providers/delinea.py
+-rw-r--r--   0        0        0     9179 2023-06-08 16:22:15.951508 nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/providers/hashicorp.py
+-rw-r--r--   0        0        0      758 2023-06-08 16:22:15.951508 nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/secrets.py
+-rw-r--r--   0        0        0     3452 2023-06-08 16:22:15.951508 nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/templates/nautobot_secrets_providers/home.html
+-rw-r--r--   0        0        0       56 2023-06-08 16:22:15.951508 nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/tests/__init__.py
+-rw-r--r--   0        0        0     2086 2023-06-08 16:22:15.951508 nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/tests/nautobot_config.py
+-rw-r--r--   0        0        0      621 2023-06-08 16:22:15.951508 nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/tests/test_basic.py
+-rw-r--r--   0        0        0    26973 2023-06-08 16:22:15.951508 nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/tests/test_providers.py
+-rw-r--r--   0        0        0      281 2023-06-08 16:22:15.951508 nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/urls.py
+-rw-r--r--   0        0        0      534 2023-06-08 16:22:15.951508 nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/views.py
+-rw-r--r--   0        0        0     3105 2023-06-08 16:22:29.235402 nautobot_secrets_providers-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    30235 1970-01-01 00:00:00.000000 nautobot_secrets_providers-1.4.1/PKG-INFO
```

### Comparing `nautobot_secrets_providers-1.4.0/LICENSE` & `nautobot_secrets_providers-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_secrets_providers-1.4.0/README.md` & `nautobot_secrets_providers-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/__init__.py` & `nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/__init__.py` & `nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/aws.py` & `nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/providers/aws.py`

 * *Files identical despite different names*

### Comparing `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/choices.py` & `nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/providers/choices.py`

 * *Files identical despite different names*

### Comparing `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/delinea.py` & `nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/providers/delinea.py`

 * *Files identical despite different names*

### Comparing `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/providers/hashicorp.py` & `nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/providers/hashicorp.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,19 +147,20 @@
                 elif auth_method == "kubernetes":
                     with open(k8s_token_path, "r", encoding="utf-8") as token_file:
                         jwt = token_file.read()
                     client.auth.kubernetes.login(role=vault_settings["role_name"], jwt=jwt, **login_kwargs)
                 elif auth_method == "aws":
                     session = boto3.Session()
                     aws_creds = session.get_credentials()
+                    aws_region = session.region_name or "us-east-1"
                     client.auth.aws.iam_login(
                         access_key=aws_creds.access_key,
                         secret_key=aws_creds.secret_key,
                         session_token=aws_creds.token,
-                        region=session.region_name,
+                        region=aws_region,
                         role=vault_settings.get("role_name", None),
                         **login_kwargs,
                     )
         except hvac.exceptions.InvalidRequest as err:
             raise exceptions.SecretProviderError(
                 secret, cls, f"HashiCorp Vault Login failed (auth_method: {auth_method}). Error: {err}"
             ) from err
```

### Comparing `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/secrets.py` & `nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/secrets.py`

 * *Files identical despite different names*

### Comparing `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/templates/nautobot_secrets_providers/home.html` & `nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/templates/nautobot_secrets_providers/home.html`

 * *Files identical despite different names*

### Comparing `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/tests/nautobot_config.py` & `nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/tests/nautobot_config.py`

 * *Files identical despite different names*

### Comparing `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/tests/test_basic.py` & `nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/tests/test_providers.py` & `nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `nautobot_secrets_providers-1.4.0/nautobot_secrets_providers/views.py` & `nautobot_secrets_providers-1.4.1/nautobot_secrets_providers/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_secrets_providers-1.4.0/pyproject.toml` & `nautobot_secrets_providers-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-secrets-providers"
-version = "v1.4.0"
+version = "v1.4.1"
 description = "Nautobot Secrets Providers Plugin."
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-secrets-providers"
 repository = "https://github.com/nautobot/nautobot-plugin-secrets-providers"
 keywords = ["nautobot", "nautobot-plugin"]
```

### Comparing `nautobot_secrets_providers-1.4.0/PKG-INFO` & `nautobot_secrets_providers-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-secrets-providers
-Version: 1.4.0
+Version: 1.4.1
 Summary: Nautobot Secrets Providers Plugin.
 Home-page: https://github.com/nautobot/nautobot-plugin-secrets-providers
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: opensource@networktocode.com
 Requires-Python: >=3.7,<4.0
```

