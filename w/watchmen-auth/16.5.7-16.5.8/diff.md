# Comparing `tmp/watchmen_auth-16.5.7.tar.gz` & `tmp/watchmen_auth-16.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_auth-16.5.7.tar", max compression
+gzip compressed data, was "watchmen_auth-16.5.8.tar", max compression
```

## Comparing `watchmen_auth-16.5.7.tar` & `watchmen_auth-16.5.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-06-07 11:34:15.599986 watchmen_auth-16.5.7/LICENSE
--rw-r--r--   0        0        0      418 2023-06-07 11:34:15.603986 watchmen_auth-16.5.7/pyproject.toml
--rw-r--r--   0        0        0      362 2023-06-07 11:34:15.603986 watchmen_auth-16.5.7/src/watchmen_auth/__init__.py
--rw-r--r--   0        0        0      755 2023-06-07 11:34:15.603986 watchmen_auth-16.5.7/src/watchmen_auth/auth_helper.py
--rw-r--r--   0        0        0     1569 2023-06-07 11:34:15.603986 watchmen_auth-16.5.7/src/watchmen_auth/authentication.py
--rw-r--r--   0        0        0     1212 2023-06-07 11:34:15.603986 watchmen_auth-16.5.7/src/watchmen_auth/authorization.py
--rw-r--r--   0        0        0      742 2023-06-07 11:34:15.603986 watchmen_auth-16.5.7/src/watchmen_auth/fake_principal_service.py
--rw-r--r--   0        0        0      816 2023-06-07 11:34:15.603986 watchmen_auth-16.5.7/src/watchmen_auth/principal_service.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 watchmen_auth-16.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.183630 watchmen_auth-16.5.8/LICENSE
+-rw-r--r--   0        0        0      418 2023-06-08 03:33:39.183630 watchmen_auth-16.5.8/pyproject.toml
+-rw-r--r--   0        0        0      362 2023-06-08 03:33:39.183630 watchmen_auth-16.5.8/src/watchmen_auth/__init__.py
+-rw-r--r--   0        0        0      755 2023-06-08 03:33:39.183630 watchmen_auth-16.5.8/src/watchmen_auth/auth_helper.py
+-rw-r--r--   0        0        0     1569 2023-06-08 03:33:39.183630 watchmen_auth-16.5.8/src/watchmen_auth/authentication.py
+-rw-r--r--   0        0        0     1212 2023-06-08 03:33:39.183630 watchmen_auth-16.5.8/src/watchmen_auth/authorization.py
+-rw-r--r--   0        0        0      742 2023-06-08 03:33:39.183630 watchmen_auth-16.5.8/src/watchmen_auth/fake_principal_service.py
+-rw-r--r--   0        0        0      816 2023-06-08 03:33:39.183630 watchmen_auth-16.5.8/src/watchmen_auth/principal_service.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 watchmen_auth-16.5.8/PKG-INFO
```

### Comparing `watchmen_auth-16.5.7/LICENSE` & `watchmen_auth-16.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.5.7/src/watchmen_auth/auth_helper.py` & `watchmen_auth-16.5.8/src/watchmen_auth/auth_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.5.7/src/watchmen_auth/authentication.py` & `watchmen_auth-16.5.8/src/watchmen_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.5.7/src/watchmen_auth/authorization.py` & `watchmen_auth-16.5.8/src/watchmen_auth/authorization.py`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.5.7/src/watchmen_auth/fake_principal_service.py` & `watchmen_auth-16.5.8/src/watchmen_auth/fake_principal_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_auth-16.5.7/src/watchmen_auth/principal_service.py` & `watchmen_auth-16.5.8/src/watchmen_auth/principal_service.py`

 * *Files identical despite different names*

