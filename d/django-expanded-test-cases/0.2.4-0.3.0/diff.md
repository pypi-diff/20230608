# Comparing `tmp/django-expanded-test-cases-0.2.4.tar.gz` & `tmp/django-expanded-test-cases-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-expanded-test-cases-0.2.4.tar", last modified: Tue May 23 03:26:21 2023, max compression
+gzip compressed data, was "django-expanded-test-cases-0.3.0.tar", last modified: Thu Jun  8 07:14:47 2023, max compression
```

## Comparing `django-expanded-test-cases-0.2.4.tar` & `django-expanded-test-cases-0.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1074 2022-06-02 21:49:59.000000 django-expanded-test-cases-0.2.4/LICENSE
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       91 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/MANIFEST.in
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5168 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/PKG-INFO
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/django_expanded_test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      181 2022-06-02 21:49:59.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7303 2023-05-23 03:17:15.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/constants.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/django_expanded_test_cases/mixins/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      325 2022-10-11 03:11:48.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/mixins/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    35675 2023-05-23 03:17:15.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/mixins/core_mixin.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    29221 2023-04-11 22:52:56.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/mixins/response_mixin.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.047754 django-expanded-test-cases-0.2.4/django_expanded_test_cases/templates/
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/django_expanded_test_cases/templates/django_expanded_test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      528 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/templates/django_expanded_test_cases/index.html
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1376 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    16682 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/base_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    55191 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/integration_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7790 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/live_server_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1093 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_urls.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5168 2023-05-23 03:26:21.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/PKG-INFO
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1116 2023-05-23 03:26:21.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/SOURCES.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        1 2023-05-23 03:26:21.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/dependency_links.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      112 2023-05-23 03:26:21.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/requires.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       33 2023-05-23 03:26:21.000000 django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/top_level.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1781 2023-05-23 03:23:42.000000 django-expanded-test-cases-0.2.4/pyproject.toml
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2335 2023-04-11 23:02:41.000000 django-expanded-test-cases-0.2.4/readme.md
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1192 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/setup.cfg
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/tests/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-05-23 23:45:09.000000 django-expanded-test-cases-0.2.4/tests/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      198 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.4/tests/apps.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      360 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.4/tests/asgi.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3527 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/tests/settings.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 03:26:21.051754 django-expanded-test-cases-0.2.4/tests/test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-06-02 21:49:59.000000 django-expanded-test-cases-0.2.4/tests/test_cases/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    96771 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/tests/test_cases/test_base_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   269449 2023-04-11 23:12:20.000000 django-expanded-test-cases-0.2.4/tests/test_cases/test_integration_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2230 2023-02-17 03:47:57.000000 django-expanded-test-cases-0.2.4/tests/test_cases/test_live_server_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      316 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/tests/urls.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3964 2023-03-05 08:40:41.000000 django-expanded-test-cases-0.2.4/tests/views.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.733480 django-expanded-test-cases-0.3.0/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1074 2023-05-23 04:12:24.000000 django-expanded-test-cases-0.3.0/LICENSE
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       91 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/MANIFEST.in
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5168 2023-06-08 07:14:47.733480 django-expanded-test-cases-0.3.0/PKG-INFO
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.729480 django-expanded-test-cases-0.3.0/django_expanded_test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      181 2023-05-23 04:12:47.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     8697 2023-06-08 01:04:49.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/constants.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.729480 django-expanded-test-cases-0.3.0/django_expanded_test_cases/mixins/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      325 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/mixins/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    37346 2023-06-08 04:10:33.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/mixins/core_mixin.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    29317 2023-06-08 03:30:55.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/mixins/response_mixin.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.729480 django-expanded-test-cases-0.3.0/django_expanded_test_cases/templates/
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.729480 django-expanded-test-cases-0.3.0/django_expanded_test_cases/templates/django_expanded_test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      528 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/templates/django_expanded_test_cases/index.html
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.733480 django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1376 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    16682 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/base_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    56799 2023-06-08 05:09:20.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/integration_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7790 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/live_server_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1093 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_urls.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.729480 django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5168 2023-06-08 07:14:47.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/PKG-INFO
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1116 2023-06-08 07:14:47.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/SOURCES.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        1 2023-06-08 07:14:47.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/dependency_links.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      112 2023-06-08 07:14:47.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/requires.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       33 2023-06-08 07:14:47.000000 django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/top_level.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1781 2023-06-08 07:13:39.000000 django-expanded-test-cases-0.3.0/pyproject.toml
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2335 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/readme.md
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1192 2023-06-08 07:14:47.733480 django-expanded-test-cases-0.3.0/setup.cfg
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.733480 django-expanded-test-cases-0.3.0/tests/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-05-23 23:45:09.000000 django-expanded-test-cases-0.3.0/tests/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      198 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/tests/apps.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      360 2023-05-23 04:25:19.000000 django-expanded-test-cases-0.3.0/tests/asgi.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3527 2023-05-23 04:25:20.000000 django-expanded-test-cases-0.3.0/tests/settings.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-08 07:14:47.733480 django-expanded-test-cases-0.3.0/tests/test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2023-05-23 04:12:47.000000 django-expanded-test-cases-0.3.0/tests/test_cases/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    96771 2023-05-23 04:25:20.000000 django-expanded-test-cases-0.3.0/tests/test_cases/test_base_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   300247 2023-06-08 06:24:32.000000 django-expanded-test-cases-0.3.0/tests/test_cases/test_integration_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2230 2023-05-23 04:25:20.000000 django-expanded-test-cases-0.3.0/tests/test_cases/test_live_server_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      316 2023-05-23 04:25:20.000000 django-expanded-test-cases-0.3.0/tests/urls.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3964 2023-05-23 04:25:20.000000 django-expanded-test-cases-0.3.0/tests/views.py
```

### Comparing `django-expanded-test-cases-0.2.4/LICENSE` & `django-expanded-test-cases-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.4/PKG-INFO` & `django-expanded-test-cases-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-expanded-test-cases
-Version: 0.2.4
+Version: 0.3.0
 Summary: Expands the existing Django TestCase class with extra functionality.
 Home-page: https://github.com/brodriguez8774/django-expanded-test-cases
 Author: Brandon Rodriguez
 Author-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 Maintainer-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 License: MIT License
```

### Comparing `django-expanded-test-cases-0.2.4/django_expanded_test_cases/constants.py` & `django-expanded-test-cases-0.3.0/django_expanded_test_cases/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -137,55 +137,83 @@
 ETC_MATCH_ALL_CONTEXT_MESSAGES = bool(getattr(
     settings,
     'DJANGO_EXPANDED_TESTCASES_MATCH_ALL_CONTEXT_MESSAGES',
     False,
 ))
 
 
+# Controls if test-users should be automatically generated or not.
+ETC_AUTO_GENERATE_USERS = bool(getattr(
+    settings,
+    'DJANGO_EXPANDED_TESTCASES_AUTO_GENERATE_USERS',
+    True,
+))
+# Controls what level of strictness UnitTest requests have for users.
+ETC_REQUEST_USER_STRICTNESS = str(getattr(
+    settings,
+    'DJANGO_EXPANDED_TESTCASES_REQUEST_USER_STRICTNESS',
+    'anonymous',
+)).strip().lower()
 # Allows incorporating package with non-standard user identifiers.
 # Such as the common case of using a user email as an identifier, instead of a username.
-ETC_USER_MODEL_IDENTIFIER = getattr(
+ETC_USER_MODEL_IDENTIFIER = str(getattr(
     settings,
     'DJANGO_EXPANDED_TESTCASES_USER_MODEL_IDENTIFIER',
     'username',
-)
+))
+# The identifier used for the auto-generated "superuser" user.
 ETC_DEFAULT_SUPER_USER_IDENTIFIER = getattr(
     settings,
     'DJANGO_EXPANDED_TESTCASES_DEFAULT_SUPER_USER_IDENTIFIER',
     None,
 )
+# The identifier used for the auto-generated "admin" user.
 ETC_DEFAULT_ADMIN_USER_IDENTIFIER = getattr(
     settings,
     'DJANGO_EXPANDED_TESTCASES_DEFAULT_ADMIN_USER_IDENTIFIER',
     None,
 )
+# The identifier used for the auto-generated "standard" user.
 ETC_DEFAULT_STANDARD_USER_IDENTIFIER = getattr(
     settings,
     'DJANGO_EXPANDED_TESTCASES_DEFAULT_STANDARD_USER_IDENTIFIER',
     None,
 )
+# The identifier used for the auto-generated "inactive" user.
 ETC_DEFAULT_INACTIVE_USER_IDENTIFIER = getattr(
     settings,
     'DJANGO_EXPANDED_TESTCASES_DEFAULT_INACTIVE_USER_IDENTIFIER',
     None,
 )
-ETC_DEFAULT_USER_PASSWORD = getattr(
+# The default password used for auto-generated users.
+ETC_DEFAULT_USER_PASSWORD = str(getattr(
     settings,
     'DJANGO_EXPANDED_TESTCASES_DEFAULT_PASSWORD',
     'password',
-)
+))
+# Indicates if auto-generated users should get pretend "real" first/last name values.
 ETC_GENERATE_USERS_WITH_REAL_NAMES = bool(getattr(
     settings,
     'DJANGO_EXPANDED_TESTCASES_GENERATE_USERS_WITH_REAL_NAMES',
     False,
 ))
 
 
 # region User Identifiers
 
+# Validate ETC_REQUEST_USER_STRICTNESS setting.
+if ETC_REQUEST_USER_STRICTNESS not in ['anonymous', 'relaxed', 'strict']:
+    raise ValueError(
+        'Invalid value provided for EXPANDED_TEST_CASES_REQUEST_USER_STRICTNESS setting. '
+        'Must be one of: ["anonymous", "relaxed", "strict"].'
+    )
+# Validate combination of ETC_REQUEST_USER_STRICTNESS and ETC_AUTO_GENERATE_USERS settings.
+elif ETC_REQUEST_USER_STRICTNESS == 'relaxed' and not ETC_AUTO_GENERATE_USERS:
+    raise ValueError('When ETC_REQUEST_USER_STRICTNESS is set to "relaxed", ETC_AUTO_GENERATE_USERS must be True.')
+
 # Set default identifier value, based on either provided value or common user identifier types.
 default_superuser_identifier = None
 default_admin_identifier = None
 default_inactive_identifier = None
 default_user_identifier = None
 
 if ETC_USER_MODEL_IDENTIFIER == 'username':
```

### Comparing `django-expanded-test-cases-0.2.4/django_expanded_test_cases/mixins/core_mixin.py` & `django-expanded-test-cases-0.3.0/django_expanded_test_cases/mixins/core_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # Third-Party Imports.
 from django.contrib.auth import get_user_model
 from django.utils.http import urlencode
 
 # Internal Imports.
 from django_expanded_test_cases.constants import (
     ETC_DEBUG_PRINT,
+    ETC_AUTO_GENERATE_USERS,
+    ETC_REQUEST_USER_STRICTNESS,
     ETC_USER_MODEL_IDENTIFIER,
     ETC_DEFAULT_SUPER_USER_IDENTIFIER,
     ETC_DEFAULT_ADMIN_USER_IDENTIFIER,
     ETC_DEFAULT_STANDARD_USER_IDENTIFIER,
     ETC_DEFAULT_INACTIVE_USER_IDENTIFIER,
     ETC_DEFAULT_USER_PASSWORD,
     ETC_GENERATE_USERS_WITH_REAL_NAMES,
@@ -98,14 +100,35 @@
 
         However, since this is not inheriting from a given TestCase, calling the literal function
         here would override instead.
 
         :param extra_usergen_kwargs: Optional extra kwargs to pass into the get_user_model().objects.create_user()
                                      function.
         """
+        if ETC_AUTO_GENERATE_USERS:
+            # Run logic to auto-generate test users. Setting is on by default.
+            if extra_usergen_kwargs is None:
+                extra_usergen_kwargs = {}
+            elif not isinstance(extra_usergen_kwargs, dict):
+                raise ValueError(
+                    'The extra_usergen_kwargs value must be a dictionary of additional args used in the '
+                    'get_user_model().objects.create_user() function.'
+                )
+
+            cls._auto_generate_test_users(extra_usergen_kwargs=extra_usergen_kwargs)
+
+    @classmethod
+    def _auto_generate_test_users(cls, extra_usergen_kwargs=None):
+        """Logic to automatically generate test users.
+
+        Only run if DJANGO_EXPANDED_TESTCASES_AUTO_GENERATE_USERS setting is true.
+        """
+        # Django imports here to avoid situational "Apps aren't loaded yet" error.
+        from django.contrib.auth.models import AnonymousUser
+
         if extra_usergen_kwargs is None:
             extra_usergen_kwargs = {}
         elif not isinstance(extra_usergen_kwargs, dict):
             raise ValueError(
                 'The extra_usergen_kwargs value must be a dictionary of additional args used in the '
                 'get_user_model().objects.create_user() function.'
             )
@@ -192,16 +215,32 @@
             cls.test_user.last_name = 'UserLast'
             cls.test_user.name = 'StandardUserName'
         if ETC_USER_MODEL_IDENTIFIER.lower() != 'email':
             cls.test_user.email = 'user@example.com'
         cls.test_user.save()
         cls.test_user = cls.get_user(cls, ETC_DEFAULT_STANDARD_USER_IDENTIFIER)
 
-        # Default user to run tests with is above "test_user".
-        cls.user = cls.test_user
+        # Set actual default "class user" for tests based on settings.
+        if ETC_REQUEST_USER_STRICTNESS == 'anonymous':
+            # Default user to run tests with an anonymous user.
+            cls.user = AnonymousUser()
+
+        elif ETC_REQUEST_USER_STRICTNESS == 'relaxed':
+            # Default user to run tests with above "test_user".
+            cls.user = cls.test_user
+
+        elif ETC_REQUEST_USER_STRICTNESS == 'strict':
+            # No default user to run tests with.
+            cls.user = None
+
+        else:
+            raise ValueError(
+                'Invalid value provided for EXPANDED_TEST_CASES_REQUEST_USER_STRICTNESS setting. '
+                'Must be one of: ["anonymous", "relaxed", "strict"].'
+            )
 
     def sub_test(self):
         """
         Acts as the equivalent of the UnitTesting "subtTest()" function.
 
         However, since this is not inheriting from a given TestCase, calling the literal function
         here would override instead.
```

### Comparing `django-expanded-test-cases-0.2.4/django_expanded_test_cases/mixins/response_mixin.py` & `django-expanded-test-cases-0.3.0/django_expanded_test_cases/mixins/response_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,15 @@
             style=OUTPUT_EMPHASIS,
         )
 
         # Only proceed if we got a proper user model.
         if isinstance(user, get_user_model()):
 
             # General user information.
+            self._debug_print('    * pk: "{0}"'.format(user.pk), fore=RESPONSE_DEBUG_USER_INFO)
             self._debug_print('    * Username: "{0}"'.format(user.username), fore=RESPONSE_DEBUG_USER_INFO)
             self._debug_print('    * First: "{0}"'.format(user.first_name), fore=RESPONSE_DEBUG_USER_INFO)
             self._debug_print('    * Last: "{0}"'.format(user.last_name), fore=RESPONSE_DEBUG_USER_INFO)
             self._debug_print('    * Email: "{0}"'.format(user.email), fore=RESPONSE_DEBUG_USER_INFO)
 
             # User auth data.
             self._debug_print(
```

### Comparing `django-expanded-test-cases-0.2.4/django_expanded_test_cases/templates/django_expanded_test_cases/index.html` & `django-expanded-test-cases-0.3.0/django_expanded_test_cases/templates/django_expanded_test_cases/index.html`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/__init__.py` & `django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/base_test_case.py` & `django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/base_test_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/integration_test_case.py` & `django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/integration_test_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 """
 
 # System Imports.
 import logging, re, textwrap
 
 # Third-Party Imports.
 from django.conf import settings
+from django.core.exceptions import ValidationError
 from django.http.response import HttpResponseBase
 from django.urls import reverse
 from django.urls.exceptions import NoReverseMatch
 
 # Internal Imports.
 from .base_test_case import BaseTestCase
 from django_expanded_test_cases.constants import (
     ETC_ALLOW_MESSAGE_PARTIALS,
+    ETC_REQUEST_USER_STRICTNESS,
     ETC_DEFAULT_STANDARD_USER_IDENTIFIER,
     RESPONSE_DEBUG_URL,
     OUTPUT_EMPHASIS,
     VOID_ELEMENT_LIST,
 )
 from django_expanded_test_cases.mixins import ResponseTestCaseMixin
 
@@ -42,15 +44,15 @@
 
     def assertResponse(
         self,
         url, *args,
         get=True, data=None,
         expected_redirect_url=None, expected_status=200,
         expected_title=None, expected_header=None, expected_messages=None, expected_content=None,
-        auto_login=True, user=ETC_DEFAULT_STANDARD_USER_IDENTIFIER, user_permissions=None, user_groups=None,
+        auto_login=True, user=None, user_permissions=None, user_groups=None,
         ignore_content_ordering=False, content_starts_after=None, content_ends_before=None,
         **kwargs,
     ):
         """Verifies the view response object at given URL matches provided parameters.
 
         At minimum, gets a response object from parsing provided url, then asserts the status code matches.
         Optionally also allows testing:
@@ -80,17 +82,16 @@
         """
         # Django imports here to avoid situational "Apps aren't loaded yet" error.
         from django.contrib.auth.models import AnonymousUser
 
         # Reset client "user login" state for new response generation.
         self.client.logout()
 
-        # Handle if auto login is set to False.
-        if auto_login is False:
-            user = AnonymousUser()
+        # Handle getting user.
+        user = self._get_default_request_user(user, auto_login)
 
         # Run logic to get corresponding response object.
         response = self._get_page_response(
             url,
             *args,
             get=get,
             data=data,
@@ -174,15 +175,15 @@
 
     def assertGetResponse(
         self,
         url, *args,
         data=None,
         expected_redirect_url=None, expected_status=200,
         expected_title=None, expected_header=None, expected_messages=None, expected_content=None,
-        auto_login=True, user=ETC_DEFAULT_STANDARD_USER_IDENTIFIER, user_permissions=None, user_groups=None,
+        auto_login=True, user=None, user_permissions=None, user_groups=None,
         ignore_content_ordering=False, content_starts_after=None, content_ends_before=None,
         **kwargs,
     ):
         """Verifies a GET response was found at given URL, and matches provided parameters."""
 
         # Call base function to handle actual logic.
         return self.assertResponse(
@@ -208,15 +209,15 @@
 
     def assertPostResponse(
         self,
         url, *args,
         data=None,
         expected_redirect_url=None, expected_status=200,
         expected_title=None, expected_header=None, expected_messages=None, expected_content=None,
-        auto_login=True, user=ETC_DEFAULT_STANDARD_USER_IDENTIFIER, user_permissions=None, user_groups=None,
+        auto_login=True, user=None, user_permissions=None, user_groups=None,
         ignore_content_ordering=False, content_starts_after=None, content_ends_before=None,
         **kwargs,
     ):
         """Verifies a GET response was found at given URL, and matches provided parameters."""
 
         # Handle mutable data defaults.
         data = data or {}
@@ -721,71 +722,118 @@
         # Run full assertPageContent() to make sure we're thorough (unsure of if this part is needed?).
         return self.assertPageContent(truncated_content, expected_content, debug_output=debug_output)
 
     # endregion Custom Assertions
 
     # region Helper Functions
 
+    def _get_default_request_user(self, user, auto_login):
+        """
+        # We first prioritize a direct value passed into this function (if not the default).
+        # Then we prioritize a user saved to the class "self.user" variable (if not the default).
+        :param user:
+        :param auto_login:
+        :return:
+        """
+        # Django imports here to avoid situational "Apps aren't loaded yet" error.
+        from django.contrib.auth.models import AnonymousUser
+
+        print('\n\n\n\n')
+        print('User: {0}'.format(user))
+
+        # If user is None, attempt to fallback to class-user.
+        if user is None:
+            class_user = getattr(self, 'user', None)
+            if class_user != AnonymousUser and class_user != AnonymousUser():
+                user = class_user
+
+        print('User: {0}'.format(user))
+
+        # Proceed if user still None.
+        if user is None:
+            # Handle if default mode is "anonymous" and no user provided.
+            if ETC_REQUEST_USER_STRICTNESS == 'anonymous':
+                print('Strictness: Anonymous')
+                user = AnonymousUser()
+
+            # Handle if default mode is "relaxed" and no user provided.
+            elif ETC_REQUEST_USER_STRICTNESS == 'relaxed':
+                print('Strictness: Relaxed')
+                user = ETC_DEFAULT_STANDARD_USER_IDENTIFIER
+
+            # Handle if default mode is "strict" and no user provided.
+            elif ETC_REQUEST_USER_STRICTNESS == 'strict':
+                # Handle for logging in a user.
+                print('Strictness: Strict')
+                if auto_login:
+                    raise ValidationError(
+                        'ETC_REQUEST_USER_STRICTNESS is set to "strict" but auto_login is True and no user was provided. '
+                        'Please either set auto_login to False OR explicitly provide a user to authenticate with.'
+                    )
+
+            else:
+                raise ValueError(
+                    'Invalid value provided for EXPANDED_TEST_CASES_REQUEST_USER_STRICTNESS setting. '
+                    'Must be one of: ["anonymous", "relaxed", "strict"].'
+                )
+
+        print('User: {0}'.format(user))
+
+        # Use anonymous user if not set to auto-login.
+        if not auto_login:
+            user = AnonymousUser()
+
+        print('User: {0}'.format(user))
+
+        print('\n\n\n\n')
+
+        # Return calculated user.
+        return user
+
     def _get_page_response(
         self,
         url,
         *args,
         get=True, data=None,
-        auto_login=True, user=ETC_DEFAULT_STANDARD_USER_IDENTIFIER, user_permissions=None, user_groups=None,
+        auto_login=True, user=None, user_permissions=None, user_groups=None,
         **kwargs,
     ):
         """Helper function for assertResponse().
 
         Fully parses provided user url, and returns corresponding response object.
 
         :param url: Url to get response object from.
         :param get: Bool indicating if response is GET or POST. Defaults to GET.
         :param data: Optional dict of items to pass into response generation.
         :param auto_login: Bool indicating if User should be "logged in" to client or not.
         :param user_permissions: Set of Django Permissions to give to test user before accessing page.
         :param user_groups: Set of Django PermissionGroups to give to test user before accessing page.
         :return: Django response object for provided url.
         """
-        # Django imports here to avoid situational "Apps aren't loaded yet" error.
-        from django.contrib.auth.models import AnonymousUser
-
         # Handle mutable data defaults.
         data = data or {}
 
         # Validate data types.
         if not isinstance(data, dict):
             raise TypeError('Provided "data" arg must be a dict, for passing into POST requests.')
 
-        # Handle for logging in a user.
-        if auto_login:
-            # Determine which user to pass in.
-            # We first prioritize a direct value passed into this function (if not the default).
-            # Then we prioritize a user saved to the class "self.user" variable (if not the default).
-            # Finally, if neither is set, then we fall back to the default. Note that the default
-            # should be the same for both those values. So there should never be a case where defaults conflict.
-            chosen_user = self.user
-            if user != ETC_DEFAULT_STANDARD_USER_IDENTIFIER:
-                # Provided function user is non-default. Use this for login.
-                chosen_user = user
-            elif self.user.username != ETC_DEFAULT_STANDARD_USER_IDENTIFIER:
-                # Provided class variable user is non-default. Use this for login.
-                chosen_user = self.user
-            user = self._get_login_user(
-                chosen_user,
-                *args,
-                url=url,
-                get=get,
-                data=data,
-                auto_login=auto_login,
-                user_permissions=user_permissions,
-                user_groups=user_groups,
-                **kwargs,
-            )
-        if not auto_login or not hasattr(user, 'is_active') or not user.is_active:
-            user = AnonymousUser()
+        # Handle getting user.
+        user = self._get_default_request_user(user, auto_login)
+
+        user = self._get_login_user(
+            user,
+            *args,
+            url=url,
+            get=get,
+            data=data,
+            auto_login=auto_login,
+            user_permissions=user_permissions,
+            user_groups=user_groups,
+            **kwargs,
+        )
 
         # Preprocess all potential url values.
         url = str(url).strip()
         current_site = '127.0.0.1'
         url_args = ()
         url_kwargs = {}
 
@@ -870,15 +918,27 @@
         :param user: User to manipulate.
         :param auto_login: Bool indicating if User should be "logged in" to client or not.
         :param user_permissions: Django Permissions to give to User.
         :param user_groups: Django Groups to give to User.
         :return: Updated User object.
         """
         # Django imports here to avoid situational "Apps aren't loaded yet" error.
-        from django.contrib.auth.models import Group, Permission
+        from django.contrib.auth.models import AnonymousUser, Group, Permission
+
+        # If not an anonymous user, attempt to get corresponding actual user object.
+        if not isinstance(user, AnonymousUser):
+            user = self.get_user(user)
+
+        # Use anonymous user if either not set to auto-login, or provided user is inactive.
+        if not auto_login or not hasattr(user, 'is_active') or not user.is_active:
+            user = AnonymousUser()
+
+        # If user is provided and is anonymous user object, then skip attempting any other login logic.
+        if isinstance(user, AnonymousUser):
+            return user
 
         # Handle mutable data defaults.
         user_permissions = user_permissions or []
         user_groups = user_groups or []
 
         # Handle possible types for Permissions.
         if isinstance(user_permissions, list) or isinstance(user_permissions, tuple):
@@ -906,32 +966,28 @@
             # Invalid/unknown type. Raise error.
             raise TypeError('Provided Django Groups must be either a str, array, or model format.')
 
         # Add all Groups to provided user.
         for group in user_groups:
             user = self.add_user_group(group, user=user)
 
-        # Ensure by this point that we have a proper instance of the User object.
-        # If no Permissions or Groups were set, we might still have a Str or something.
-        user = self.get_user(user)
-
         # Optional hook to run additional authentication logic/setup on User.
         # For example, if project has 2-Factor setup that needs to be run.
         user = self._get_login_user__extra_user_auth_setup(
             user,
             *args,
             auto_login=True,
             user_permissions=None,
             user_groups=None,
             **kwargs,
         )
 
         # Ensure by this point that we have a proper instance of the User object.
-        # If no Permissions or Groups were set, OR if wonky logic was used in extra_auth_setup,
-        # we might still have a Str or something.
+        # Accounts for if wonky logic was used in extra_auth_setup, which is defined by the project importing
+        # this package, so we have no control over.
         user = self.get_user(user)
 
         # Handle logging in with user.
         # This forces all response objects to act like this user is logged in for all page accesses.
         # Otherwise, it will act like an anonymous user is navigating the site.
         if auto_login:
             self.client.force_login(user)
@@ -1130,15 +1186,15 @@
 
     def _assertResponse__pre_builtin_tests(
         self,
         url, *args,
         get=True, data=None,
         expected_redirect_url=None, expected_status=200,
         expected_title=None, expected_header=None, expected_messages=None, expected_content=None,
-        auto_login=True, user='test_user', user_permissions=None, user_groups=None,
+        auto_login=True, user=None, user_permissions=None, user_groups=None,
         ignore_content_ordering=False, content_starts_after=None, content_ends_before=None,
         **kwargs,
     ):
         """Hook function to allow injecting code prior to running any of the built-in assertResponse() tests.
 
         For maximum usability, this function receives all args/kwargs provided to the default assertResponse()
         function.
@@ -1149,15 +1205,15 @@
 
     def _assertResponse__post_builtin_tests(
         self,
         url, *args,
         get=True, data=None,
         expected_redirect_url=None, expected_status=200,
         expected_title=None, expected_header=None, expected_messages=None, expected_content=None,
-        auto_login=True, user='test_user', user_permissions=None, user_groups=None,
+        auto_login=True, user=None, user_permissions=None, user_groups=None,
         ignore_content_ordering=False, content_starts_after=None, content_ends_before=None,
         **kwargs,
     ):
         """Hook function to allow injecting code after running all of the built-in assertResponse() tests.
 
         For maximum usability, this function receives all args/kwargs provided to the default assertResponse()
         function.
```

### Comparing `django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_cases/live_server_test_case.py` & `django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_cases/live_server_test_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.4/django_expanded_test_cases/test_urls.py` & `django-expanded-test-cases-0.3.0/django_expanded_test_cases/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/PKG-INFO` & `django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-expanded-test-cases
-Version: 0.2.4
+Version: 0.3.0
 Summary: Expands the existing Django TestCase class with extra functionality.
 Home-page: https://github.com/brodriguez8774/django-expanded-test-cases
 Author: Brandon Rodriguez
 Author-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 Maintainer-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 License: MIT License
```

### Comparing `django-expanded-test-cases-0.2.4/django_expanded_test_cases.egg-info/SOURCES.txt` & `django-expanded-test-cases-0.3.0/django_expanded_test_cases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.4/pyproject.toml` & `django-expanded-test-cases-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=40.8.0', 'wheel']
 build-backend = 'setuptools.build_meta:__legacy__'
 
 [project]
 name = "django-expanded-test-cases"
-version = "0.2.4"
+version = "0.3.0"
 description = "Expands the existing Django TestCase class with extra functionality."
 readme = "readme.md"
 authors = [
     { name = "Brandon Rodriguez", email = "brodriguez8774@gmail.com" },
 ]
 maintainers = [
     { name = "Brandon Rodriguez", email = "brodriguez8774@gmail.com" },
```

### Comparing `django-expanded-test-cases-0.2.4/readme.md` & `django-expanded-test-cases-0.3.0/readme.md`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.4/setup.cfg` & `django-expanded-test-cases-0.3.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-expanded-test-cases
-version = 0.2.4
+version = 0.3.0
 description = Expands the existing Django TestCase class with extra functionality.
 long_description = file: readme.md
 url = https://github.com/brodriguez8774/django-expanded-test-cases
 author = Brandon Rodriguez
 author_email = brodriguez8774@gmail.com
 license = MIT License
 classifiers =
```

### Comparing `django-expanded-test-cases-0.2.4/tests/settings.py` & `django-expanded-test-cases-0.3.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.4/tests/test_cases/test_base_case.py` & `django-expanded-test-cases-0.3.0/tests/test_cases/test_base_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.4/tests/test_cases/test_integration_case.py` & `django-expanded-test-cases-0.3.0/tests/test_cases/test_integration_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,206 +6,24 @@
 import logging
 from unittest.mock import patch
 
 # Third-Party Imports.
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import AnonymousUser, Group, Permission
 from django.contrib.contenttypes.models import ContentType
+from django.core.exceptions import ValidationError
 from django.http import HttpResponse
 
 # Internal Imports.
 from django_expanded_test_cases import IntegrationTestCase
 
 
-class IntegrationClassTest(IntegrationTestCase):
+class IntegrationClassTest__Base():
     """Tests for IntegrationTestCase class."""
 
-    @classmethod
-    def setUpClass(cls):
-        # Run parent setup logic.
-        super().setUpClass()
-
-        cls.test_superuser.first_name = 'TestFirst'
-        cls.test_superuser.last_name = 'TestLast'
-        cls.test_superuser.save()
-
-    # region Response Tests
-
-    def test__assertGetResponse__with_login(self):
-        """Verifies that expected user is logged in during assertGetResponse."""
-
-        with self.subTest('Check login using default user'):
-            response = self.assertGetResponse('django_expanded_test_cases:index')
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
-            self.assertEqual(self.test_user, response.wsgi_request.user)
-            self.assertEqual(self.test_user, response.context['user'])
-            self.assertEqual(self.test_user, response.user)
-
-        with self.subTest('Check login using super user - Provided as arg'):
-            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_superuser')
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(self.test_superuser.pk, int(self.client.session['_auth_user_id']))
-            self.assertEqual(self.test_superuser, response.wsgi_request.user)
-            self.assertEqual(self.test_superuser, response.context['user'])
-            self.assertEqual(self.test_superuser, response.user)
-
-        with self.subTest('Check login using admin user - Provided as arg'):
-            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_admin')
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(self.test_admin.pk, int(self.client.session['_auth_user_id']))
-            self.assertEqual(self.test_admin, response.wsgi_request.user)
-            self.assertEqual(self.test_admin, response.context['user'])
-            self.assertEqual(self.test_admin, response.user)
-
-        with self.subTest('Check login using inactive user - Provided as arg'):
-
-            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_inactive')
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(self.test_inactive_user.pk, int(self.client.session['_auth_user_id']))
-            self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
-            self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
-            self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
-            self.assertTrue(isinstance(response.user, AnonymousUser))
-            self.assertFalse(isinstance(response.user, get_user_model()))
-
-        with self.subTest('Check login using standard user - Provided as arg'):
-            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_user')
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
-            self.assertEqual(self.test_user, response.wsgi_request.user)
-            self.assertEqual(self.test_user, response.context['user'])
-            self.assertEqual(self.test_user, response.user)
-
-        with self.subTest('Check login using custom new user - Provided as arg'):
-            new_user = self.get_user('new_user')
-            response = self.assertGetResponse('django_expanded_test_cases:index', user=new_user)
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
-            self.assertEqual(new_user, response.wsgi_request.user)
-            self.assertEqual(new_user, response.context['user'])
-            self.assertEqual(new_user, response.user)
-
-        with self.subTest('Check login using super user - Provided as class variable'):
-            self.user = self.get_user('test_superuser')
-            response = self.assertGetResponse('django_expanded_test_cases:index')
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(self.test_superuser.pk, int(self.client.session['_auth_user_id']))
-            self.assertEqual(self.test_superuser, response.wsgi_request.user)
-            self.assertEqual(self.test_superuser, response.context['user'])
-            self.assertEqual(self.test_superuser, response.user)
-
-        with self.subTest('Check login using admin user - Provided as class variable'):
-            self.user = self.get_user('test_admin')
-            response = self.assertGetResponse('django_expanded_test_cases:index')
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(self.test_admin.pk, int(self.client.session['_auth_user_id']))
-            self.assertEqual(self.test_admin, response.wsgi_request.user)
-            self.assertEqual(self.test_admin, response.context['user'])
-            self.assertEqual(self.test_admin, response.user)
-
-        with self.subTest('Check login using inactive user - Provided as class variable'):
-            self.user = self.get_user('test_inactive')
-            response = self.assertGetResponse('django_expanded_test_cases:index')
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(self.test_inactive_user.pk, int(self.client.session['_auth_user_id']))
-            self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
-            self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
-            self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
-            self.assertTrue(isinstance(response.user, AnonymousUser))
-            self.assertFalse(isinstance(response.user, get_user_model()))
-
-        with self.subTest('Check login using standard user - Provided as class variable'):
-            self.user = self.get_user('test_user')
-            response = self.assertGetResponse('django_expanded_test_cases:index')
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
-            self.assertEqual(self.test_user, response.wsgi_request.user)
-            self.assertEqual(self.test_user, response.context['user'])
-            self.assertEqual(self.test_user, response.user)
-
-        with self.subTest('Check login using custom new user - Provided as class variable'):
-            self.user = self.get_user('new_user')
-            response = self.assertGetResponse('django_expanded_test_cases:index')
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
-            self.assertEqual(new_user, response.wsgi_request.user)
-            self.assertEqual(new_user, response.context['user'])
-            self.assertEqual(new_user, response.user)
-
-        with self.subTest('Check login using super user - Provided with conflicting values (function value should win)'):
-            self.user = self.get_user('new_user')
-            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_superuser')
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(self.test_superuser.pk, int(self.client.session['_auth_user_id']))
-            self.assertEqual(self.test_superuser, response.wsgi_request.user)
-            self.assertEqual(self.test_superuser, response.context['user'])
-            self.assertEqual(self.test_superuser, response.user)
-
-        with self.subTest('Check login using admin user - Provided with conflicting values (function value should win)'):
-            self.user = self.get_user('test_superuser')
-            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_admin')
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(self.test_admin.pk, int(self.client.session['_auth_user_id']))
-            self.assertEqual(self.test_admin, response.wsgi_request.user)
-            self.assertEqual(self.test_admin, response.context['user'])
-            self.assertEqual(self.test_admin, response.user)
-
-        with self.subTest('Check login using inactive user - Provided with conflicting values (function value should win)'):
-            self.user = self.get_user('test_admin')
-            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_inactive')
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(self.test_inactive_user.pk, int(self.client.session['_auth_user_id']))
-            self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
-            self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
-            self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
-            self.assertTrue(isinstance(response.user, AnonymousUser))
-            self.assertFalse(isinstance(response.user, get_user_model()))
-
-        with self.subTest('Check login using standard user - Provided with conflicting values (class value should win)'):
-            # This is the exception, because "test_user" technically IS the "default" user.
-            # Thus, providing this for the function value when a class value is also provided will result
-            # in the class value being used instead.
-            self.user = self.get_user('test_inactive')
-            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_user')
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(self.test_inactive_user.pk, int(self.client.session['_auth_user_id']))
-            self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
-            self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
-            self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
-            self.assertTrue(isinstance(response.user, AnonymousUser))
-            self.assertFalse(isinstance(response.user, get_user_model()))
-
-        with self.subTest('Check login using custom new user - Provided with conflicting values (function value should win)'):
-            self.user = self.get_user('test_user')
-            response = self.assertGetResponse('django_expanded_test_cases:index', user='new_user')
-
-            # Various checks, of different ways to ensure expected user is logged in.
-            self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
-            self.assertEqual(new_user, response.wsgi_request.user)
-            self.assertEqual(new_user, response.context['user'])
-            self.assertEqual(new_user, response.user)
-
-    # endregion Response Tests
-
     # region Assertion Tests
 
     # region Response Assertion Tests
 
     def test__assertResponse__url(self):
         """
         Tests URL value returned response object in assertResponse() function.
@@ -362,75 +180,14 @@
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('django_expanded_test_cases:index', expected_redirect_url='django_expanded_test_cases:index')
             self.assertEqual(str(err.exception), exception_msg)
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('django_expanded_test_cases:login', expected_redirect_url='django_expanded_test_cases:index')
             self.assertEqual(str(err.exception), exception_msg)
 
-    def test__assertResponse__user(self):
-        """
-        Tests "user" functionality of assertResponse() function.
-        """
-        with self.subTest('With login as test user'):
-            response = self.assertResponse('')
-            self.assertEqual(response.user, self.test_user)
-            self.assertEqual(str(self.test_user.pk), self.client.session['_auth_user_id'])
-            response = self.assertResponse('', user=self.test_user)
-            self.assertEqual(response.user, self.test_user)
-            self.assertEqual(str(self.test_user.pk), self.client.session['_auth_user_id'])
-            response = self.assertResponse('', user='test_user')
-            self.assertEqual(response.user, self.test_user)
-            self.assertEqual(str(self.test_user.pk), self.client.session['_auth_user_id'])
-
-        with self.subTest('With login as admin user'):
-            response = self.assertResponse('', user=self.test_admin)
-            self.assertEqual(response.user, self.test_admin)
-            self.assertEqual(str(self.test_admin.pk), self.client.session['_auth_user_id'])
-            response = self.assertResponse('', user='test_admin')
-            self.assertEqual(response.user, self.test_admin)
-            self.assertEqual(str(self.test_admin.pk), self.client.session['_auth_user_id'])
-
-        with self.subTest('With login as superuser'):
-            response = self.assertResponse('', user=self.test_superuser)
-            self.assertEqual(response.user, self.test_superuser)
-            self.assertEqual(str(self.test_superuser.pk), self.client.session['_auth_user_id'])
-            response = self.assertResponse('', user='test_superuser')
-            self.assertEqual(response.user, self.test_superuser)
-            self.assertEqual(str(self.test_superuser.pk), self.client.session['_auth_user_id'])
-
-        with self.subTest('Without login, but test user passed'):
-            # Basically, passing a user should not really do anything here.
-            response = self.assertResponse('', auto_login=False)
-            self.assertEqual(response.user, AnonymousUser())
-            self.assertNotIn('_auth_user_id', self.client.session.keys())
-            response = self.assertResponse('', user=self.test_user, auto_login=False)
-            self.assertEqual(response.user, AnonymousUser())
-            self.assertNotIn('_auth_user_id', self.client.session.keys())
-            response = self.assertResponse('', user='test_user', auto_login=False)
-            self.assertEqual(response.user, AnonymousUser())
-            self.assertNotIn('_auth_user_id', self.client.session.keys())
-
-        with self.subTest('Without login, but admin user passed'):
-            # Basically, passing a user should not really do anything here.
-            response = self.assertResponse('', user=self.test_admin, auto_login=False)
-            self.assertEqual(response.user, AnonymousUser())
-            self.assertNotIn('_auth_user_id', self.client.session.keys())
-            response = self.assertResponse('', user='test_admin', auto_login=False)
-            self.assertEqual(response.user, AnonymousUser())
-            self.assertNotIn('_auth_user_id', self.client.session.keys())
-
-        with self.subTest('Without login, but superuser passed'):
-            # Basically, passing a user should not really do anything here.
-            response = self.assertResponse('', user=self.test_superuser, auto_login=False)
-            self.assertEqual(response.user, AnonymousUser())
-            self.assertNotIn('_auth_user_id', self.client.session.keys())
-            response = self.assertResponse('', user='test_superuser', auto_login=False)
-            self.assertEqual(response.user, AnonymousUser())
-            self.assertNotIn('_auth_user_id', self.client.session.keys())
-
     def test__assertResponse__status_code(self):
         """
         Tests "status_code" functionality of assertResponse() function.
         """
         exception_msg = '{0} != {1} : Expected status code (after potential redirects) of "{1}". Actual code was "{0}".'
 
         with self.subTest('With status_code=200 - Basic view'):
@@ -3136,43 +2893,43 @@
 
         with self.subTest('No login as test user'):
             # Verify no user is logged in.
             self.assertNotIn('_auth_user_id', self.client.session.keys())
 
             # Run _get_login_user() function. Should not log in provided user.
             return_val = self._get_login_user('test_user', auto_login=False)
-            self.assertEqual(return_val, self.test_user)
+            self.assertEqual(return_val, AnonymousUser())
 
             # Verify user is still not logged in.
             self.assertNotIn('_auth_user_id', self.client.session.keys())
 
         # Reset login state.
         self.client.logout()
 
         with self.subTest('No login as test admin'):
             # Verify no user is logged in.
             self.assertNotIn('_auth_user_id', self.client.session.keys())
 
             # Run _get_login_user() function. Should not log in provided user.
             return_val = self._get_login_user('test_admin', auto_login=False)
-            self.assertEqual(return_val, self.test_admin)
+            self.assertEqual(return_val, AnonymousUser())
 
             # Verify user is still not logged in.
             self.assertNotIn('_auth_user_id', self.client.session.keys())
 
         # Reset login state.
         self.client.logout()
 
         with self.subTest('No login as test superuser'):
             # Verify no user is logged in.
             self.assertNotIn('_auth_user_id', self.client.session.keys())
 
             # Run _get_login_user() function. Should not log in provided user.
             return_val = self._get_login_user('test_superuser', auto_login=False)
-            self.assertEqual(return_val, self.test_superuser)
+            self.assertEqual(return_val, AnonymousUser())
 
             # Verify user is still not logged in.
             self.assertNotIn('_auth_user_id', self.client.session.keys())
 
     def test___get_login_user__set_permissions(self):
         """"""
         # Generate dummy content_type.
@@ -5456,7 +5213,772 @@
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_link_text(response, 'test_link_text')
             self.assertText(str(err.exception), err_msg)
 
     # endregion Helper Function Tests
+
+
+class IntegrationClassTest__StrictnessOfAnonymous(IntegrationTestCase):
+    """Tests for IntegrationTestCase class, specifically with user strictness set to "anonymous"."""
+
+    @classmethod
+    @patch('django_expanded_test_cases.test_cases.integration_test_case.ETC_REQUEST_USER_STRICTNESS', 'anonymous')
+    def setUpClass(cls):
+        # Run parent setup logic.
+        super().setUpClass()
+
+        cls.test_superuser.first_name = 'TestFirst'
+        cls.test_superuser.last_name = 'TestLast'
+        cls.test_superuser.save()
+
+    @patch('django_expanded_test_cases.test_cases.integration_test_case.ETC_REQUEST_USER_STRICTNESS', 'anonymous')
+    def test__assertGetResponse__with_login(self):
+        """Verifies that expected user is logged in during assertGetResponse."""
+
+        with self.subTest('Check login using default user'):
+            # Default user should be Anonymous, and no actual user is logged in unless explicitly provided.
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            self.assertEqual(AnonymousUser(), response.wsgi_request.user)
+            self.assertEqual(AnonymousUser(), response.context['user'])
+            self.assertEqual(AnonymousUser(), response.user)
+
+        with self.subTest('Check login using super user - Provided as arg'):
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_superuser')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_superuser.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_superuser, response.wsgi_request.user)
+            self.assertEqual(self.test_superuser, response.context['user'])
+            self.assertEqual(self.test_superuser, response.user)
+
+        with self.subTest('Check login using admin user - Provided as arg'):
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_admin')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_admin.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_admin, response.wsgi_request.user)
+            self.assertEqual(self.test_admin, response.context['user'])
+            self.assertEqual(self.test_admin, response.user)
+
+        with self.subTest('Check login using inactive user - Provided as arg'):
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_inactive')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
+            self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
+            self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
+            self.assertTrue(isinstance(response.user, AnonymousUser))
+            self.assertFalse(isinstance(response.user, get_user_model()))
+
+        with self.subTest('Check login using standard user - Provided as arg'):
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_user')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_user, response.wsgi_request.user)
+            self.assertEqual(self.test_user, response.context['user'])
+            self.assertEqual(self.test_user, response.user)
+
+        with self.subTest('Check login using custom new user - Provided as arg'):
+            new_user = self.get_user('new_user')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user=new_user)
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(new_user, response.wsgi_request.user)
+            self.assertEqual(new_user, response.context['user'])
+            self.assertEqual(new_user, response.user)
+
+        with self.subTest('Check login using super user - Provided as class variable'):
+            self.user = self.get_user('test_superuser')
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_superuser.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_superuser, response.wsgi_request.user)
+            self.assertEqual(self.test_superuser, response.context['user'])
+            self.assertEqual(self.test_superuser, response.user)
+
+        with self.subTest('Check login using admin user - Provided as class variable'):
+            self.user = self.get_user('test_admin')
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_admin.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_admin, response.wsgi_request.user)
+            self.assertEqual(self.test_admin, response.context['user'])
+            self.assertEqual(self.test_admin, response.user)
+
+        with self.subTest('Check login using inactive user - Provided as class variable'):
+            self.user = self.get_user('test_inactive')
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
+            self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
+            self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
+            self.assertTrue(isinstance(response.user, AnonymousUser))
+            self.assertFalse(isinstance(response.user, get_user_model()))
+
+        with self.subTest('Check login using standard user - Provided as class variable'):
+            self.user = self.get_user('test_user')
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_user, response.wsgi_request.user)
+            self.assertEqual(self.test_user, response.context['user'])
+            self.assertEqual(self.test_user, response.user)
+
+        with self.subTest('Check login using custom new user - Provided as class variable'):
+            self.user = self.get_user('new_user')
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(new_user, response.wsgi_request.user)
+            self.assertEqual(new_user, response.context['user'])
+            self.assertEqual(new_user, response.user)
+
+        with self.subTest(
+            'Check login using super user - Provided with conflicting values (function value should win)'):
+            self.user = self.get_user('new_user')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_superuser')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_superuser.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_superuser, response.wsgi_request.user)
+            self.assertEqual(self.test_superuser, response.context['user'])
+            self.assertEqual(self.test_superuser, response.user)
+
+        with self.subTest(
+            'Check login using admin user - Provided with conflicting values (function value should win)'):
+            self.user = self.get_user('test_superuser')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_admin')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_admin.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_admin, response.wsgi_request.user)
+            self.assertEqual(self.test_admin, response.context['user'])
+            self.assertEqual(self.test_admin, response.user)
+
+        with self.subTest(
+            'Check login using inactive user - Provided with conflicting values (function value should win)'):
+            self.user = self.get_user('test_admin')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_inactive')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
+            self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
+            self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
+            self.assertTrue(isinstance(response.user, AnonymousUser))
+            self.assertFalse(isinstance(response.user, get_user_model()))
+
+        with self.subTest(
+            'Check login using standard user - Provided with conflicting values (function value should win)'):
+            self.user = self.get_user('test_inactive')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_user')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_user, response.wsgi_request.user)
+            self.assertEqual(self.test_user, response.context['user'])
+            self.assertEqual(self.test_user, response.user)
+
+        with self.subTest(
+            'Check login using custom new user - Provided with conflicting values (function value should win)'):
+            self.user = self.get_user('test_user')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='new_user')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(new_user, response.wsgi_request.user)
+            self.assertEqual(new_user, response.context['user'])
+            self.assertEqual(new_user, response.user)
+
+    @patch('django_expanded_test_cases.test_cases.integration_test_case.ETC_REQUEST_USER_STRICTNESS', 'anonymous')
+    def test__assertResponse__user(self):
+        """
+        Tests "user" functionality of assertResponse() function.
+        """
+        with self.subTest('Without providing a login user'):
+            response = self.assertResponse('')
+            self.assertEqual(response.user, AnonymousUser())
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+
+        with self.subTest('With login as test user'):
+            response = self.assertResponse('', user=self.test_user)
+            self.assertEqual(response.user, self.test_user)
+            self.assertEqual(str(self.test_user.pk), self.client.session['_auth_user_id'])
+            response = self.assertResponse('', user='test_user')
+            self.assertEqual(response.user, self.test_user)
+            self.assertEqual(str(self.test_user.pk), self.client.session['_auth_user_id'])
+
+        with self.subTest('With login as admin user'):
+            response = self.assertResponse('', user=self.test_admin)
+            self.assertEqual(response.user, self.test_admin)
+            self.assertEqual(str(self.test_admin.pk), self.client.session['_auth_user_id'])
+            response = self.assertResponse('', user='test_admin')
+            self.assertEqual(response.user, self.test_admin)
+            self.assertEqual(str(self.test_admin.pk), self.client.session['_auth_user_id'])
+
+        with self.subTest('With login as superuser'):
+            response = self.assertResponse('', user=self.test_superuser)
+            self.assertEqual(response.user, self.test_superuser)
+            self.assertEqual(str(self.test_superuser.pk), self.client.session['_auth_user_id'])
+            response = self.assertResponse('', user='test_superuser')
+            self.assertEqual(response.user, self.test_superuser)
+            self.assertEqual(str(self.test_superuser.pk), self.client.session['_auth_user_id'])
+
+        with self.subTest('Without login, but test user passed'):
+            # Basically, passing a user should not really do anything here.
+            response = self.assertResponse('', user=self.test_user, auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            response = self.assertResponse('', user='test_user', auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+
+        with self.subTest('Without login, but admin user passed'):
+            # Basically, passing a user should not really do anything here.
+            response = self.assertResponse('', user=self.test_admin, auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            response = self.assertResponse('', user='test_admin', auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+
+        with self.subTest('Without login, but superuser passed'):
+            # Basically, passing a user should not really do anything here.
+            response = self.assertResponse('', user=self.test_superuser, auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            response = self.assertResponse('', user='test_superuser', auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+
+
+class IntegrationClassTest__StrictnessOfRelaxed(IntegrationTestCase):
+    """Tests for IntegrationTestCase class, specifically with user strictness set to "relaxed"."""
+
+    @classmethod
+    @patch('django_expanded_test_cases.test_cases.integration_test_case.ETC_REQUEST_USER_STRICTNESS', 'relaxed')
+    def setUpClass(cls):
+        # Run parent setup logic.
+        super().setUpClass()
+
+        cls.test_superuser.first_name = 'TestFirst'
+        cls.test_superuser.last_name = 'TestLast'
+        cls.test_superuser.save()
+
+    @patch('django_expanded_test_cases.test_cases.integration_test_case.ETC_REQUEST_USER_STRICTNESS', 'relaxed')
+    def test__assertGetResponse__with_login(self):
+        """Verifies that expected user is logged in during assertGetResponse."""
+
+        with self.subTest('Check login using default user'):
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_user, response.wsgi_request.user)
+            self.assertEqual(self.test_user, response.context['user'])
+            self.assertEqual(self.test_user, response.user)
+
+        with self.subTest('Check login using super user - Provided as arg'):
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_superuser')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_superuser.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_superuser, response.wsgi_request.user)
+            self.assertEqual(self.test_superuser, response.context['user'])
+            self.assertEqual(self.test_superuser, response.user)
+
+        with self.subTest('Check login using admin user - Provided as arg'):
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_admin')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_admin.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_admin, response.wsgi_request.user)
+            self.assertEqual(self.test_admin, response.context['user'])
+            self.assertEqual(self.test_admin, response.user)
+
+        with self.subTest('Check login using inactive user - Provided as arg'):
+
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_inactive')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
+            self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
+            self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
+            self.assertTrue(isinstance(response.user, AnonymousUser))
+            self.assertFalse(isinstance(response.user, get_user_model()))
+
+        with self.subTest('Check login using standard user - Provided as arg'):
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_user')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_user, response.wsgi_request.user)
+            self.assertEqual(self.test_user, response.context['user'])
+            self.assertEqual(self.test_user, response.user)
+
+        with self.subTest('Check login using custom new user - Provided as arg'):
+            new_user = self.get_user('new_user')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user=new_user)
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(new_user, response.wsgi_request.user)
+            self.assertEqual(new_user, response.context['user'])
+            self.assertEqual(new_user, response.user)
+
+        with self.subTest('Check login using super user - Provided as class variable'):
+            self.user = self.get_user('test_superuser')
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_superuser.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_superuser, response.wsgi_request.user)
+            self.assertEqual(self.test_superuser, response.context['user'])
+            self.assertEqual(self.test_superuser, response.user)
+
+        with self.subTest('Check login using admin user - Provided as class variable'):
+            self.user = self.get_user('test_admin')
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_admin.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_admin, response.wsgi_request.user)
+            self.assertEqual(self.test_admin, response.context['user'])
+            self.assertEqual(self.test_admin, response.user)
+
+        with self.subTest('Check login using inactive user - Provided as class variable'):
+            self.user = self.get_user('test_inactive')
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
+            self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
+            self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
+            self.assertTrue(isinstance(response.user, AnonymousUser))
+            self.assertFalse(isinstance(response.user, get_user_model()))
+
+        with self.subTest('Check login using standard user - Provided as class variable'):
+            self.user = self.get_user('test_user')
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_user, response.wsgi_request.user)
+            self.assertEqual(self.test_user, response.context['user'])
+            self.assertEqual(self.test_user, response.user)
+
+        with self.subTest('Check login using custom new user - Provided as class variable'):
+            self.user = self.get_user('new_user')
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(new_user, response.wsgi_request.user)
+            self.assertEqual(new_user, response.context['user'])
+            self.assertEqual(new_user, response.user)
+
+        with self.subTest('Check login using super user - Provided with conflicting values (function value should win)'):
+            self.user = self.get_user('new_user')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_superuser')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_superuser.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_superuser, response.wsgi_request.user)
+            self.assertEqual(self.test_superuser, response.context['user'])
+            self.assertEqual(self.test_superuser, response.user)
+
+        with self.subTest('Check login using admin user - Provided with conflicting values (function value should win)'):
+            self.user = self.get_user('test_superuser')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_admin')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_admin.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_admin, response.wsgi_request.user)
+            self.assertEqual(self.test_admin, response.context['user'])
+            self.assertEqual(self.test_admin, response.user)
+
+        with self.subTest('Check login using inactive user - Provided with conflicting values (function value should win)'):
+            self.user = self.get_user('test_admin')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_inactive')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
+            self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
+            self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
+            self.assertTrue(isinstance(response.user, AnonymousUser))
+            self.assertFalse(isinstance(response.user, get_user_model()))
+
+        with self.subTest('Check login using standard user - Provided with conflicting values (function value should win)'):
+            self.user = self.get_user('test_inactive')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_user')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_user, response.wsgi_request.user)
+            self.assertEqual(self.test_user, response.context['user'])
+            self.assertEqual(self.test_user, response.user)
+
+        with self.subTest('Check login using custom new user - Provided with conflicting values (function value should win)'):
+            self.user = self.get_user('test_user')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='new_user')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(new_user, response.wsgi_request.user)
+            self.assertEqual(new_user, response.context['user'])
+            self.assertEqual(new_user, response.user)
+
+    @patch('django_expanded_test_cases.test_cases.integration_test_case.ETC_REQUEST_USER_STRICTNESS', 'relaxed')
+    def test__assertResponse__user(self):
+        """
+        Tests "user" functionality of assertResponse() function.
+        """
+        with self.subTest('With login as test user'):
+            response = self.assertResponse('')
+            self.assertEqual(response.user, self.test_user)
+            self.assertEqual(str(self.test_user.pk), self.client.session['_auth_user_id'])
+            response = self.assertResponse('', user=self.test_user)
+            self.assertEqual(response.user, self.test_user)
+            self.assertEqual(str(self.test_user.pk), self.client.session['_auth_user_id'])
+            response = self.assertResponse('', user='test_user')
+            self.assertEqual(response.user, self.test_user)
+            self.assertEqual(str(self.test_user.pk), self.client.session['_auth_user_id'])
+
+        with self.subTest('With login as admin user'):
+            response = self.assertResponse('', user=self.test_admin)
+            self.assertEqual(response.user, self.test_admin)
+            self.assertEqual(str(self.test_admin.pk), self.client.session['_auth_user_id'])
+            response = self.assertResponse('', user='test_admin')
+            self.assertEqual(response.user, self.test_admin)
+            self.assertEqual(str(self.test_admin.pk), self.client.session['_auth_user_id'])
+
+        with self.subTest('With login as superuser'):
+            response = self.assertResponse('', user=self.test_superuser)
+            self.assertEqual(response.user, self.test_superuser)
+            self.assertEqual(str(self.test_superuser.pk), self.client.session['_auth_user_id'])
+            response = self.assertResponse('', user='test_superuser')
+            self.assertEqual(response.user, self.test_superuser)
+            self.assertEqual(str(self.test_superuser.pk), self.client.session['_auth_user_id'])
+
+        with self.subTest('Without login, but test user passed'):
+            # Basically, passing a user should not really do anything here.
+            response = self.assertResponse('', auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            self.assertNotIn('_auth_user_id', self.client.session.keys())
+            response = self.assertResponse('', user=self.test_user, auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            self.assertNotIn('_auth_user_id', self.client.session.keys())
+            response = self.assertResponse('', user='test_user', auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            self.assertNotIn('_auth_user_id', self.client.session.keys())
+
+        with self.subTest('Without login, but admin user passed'):
+            # Basically, passing a user should not really do anything here.
+            response = self.assertResponse('', user=self.test_admin, auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            self.assertNotIn('_auth_user_id', self.client.session.keys())
+            response = self.assertResponse('', user='test_admin', auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            self.assertNotIn('_auth_user_id', self.client.session.keys())
+
+        with self.subTest('Without login, but superuser passed'):
+            # Basically, passing a user should not really do anything here.
+            response = self.assertResponse('', user=self.test_superuser, auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            self.assertNotIn('_auth_user_id', self.client.session.keys())
+            response = self.assertResponse('', user='test_superuser', auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            self.assertNotIn('_auth_user_id', self.client.session.keys())
+
+
+class IntegrationClassTest__StrictnessOfStrict(IntegrationTestCase):
+    """Tests for IntegrationTestCase class, specifically with user strictness set to "strict"."""
+
+    @classmethod
+    @patch('django_expanded_test_cases.test_cases.integration_test_case.ETC_REQUEST_USER_STRICTNESS', 'strict')
+    def setUpClass(cls):
+        # Run parent setup logic.
+        super().setUpClass()
+
+        cls.test_superuser.first_name = 'TestFirst'
+        cls.test_superuser.last_name = 'TestLast'
+        cls.test_superuser.save()
+
+    @patch('django_expanded_test_cases.test_cases.integration_test_case.ETC_REQUEST_USER_STRICTNESS', 'strict')
+    def test__assertGetResponse__with_login(self):
+        """Verifies that expected user is logged in during assertGetResponse."""
+
+        with self.subTest('Check login using default user'):
+            # No default user provided. Should error.
+            with self.assertRaises(ValidationError):
+                self.assertGetResponse('django_expanded_test_cases:index')
+
+        with self.subTest('Check login using super user - Provided as arg'):
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_superuser')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_superuser.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_superuser, response.wsgi_request.user)
+            self.assertEqual(self.test_superuser, response.context['user'])
+            self.assertEqual(self.test_superuser, response.user)
+
+        with self.subTest('Check login using admin user - Provided as arg'):
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_admin')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_admin.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_admin, response.wsgi_request.user)
+            self.assertEqual(self.test_admin, response.context['user'])
+            self.assertEqual(self.test_admin, response.user)
+
+        with self.subTest('Check login using inactive user - Provided as arg'):
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_inactive')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
+            self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
+            self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
+            self.assertTrue(isinstance(response.user, AnonymousUser))
+            self.assertFalse(isinstance(response.user, get_user_model()))
+
+        with self.subTest('Check login using standard user - Provided as arg'):
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_user')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_user, response.wsgi_request.user)
+            self.assertEqual(self.test_user, response.context['user'])
+            self.assertEqual(self.test_user, response.user)
+
+        with self.subTest('Check login using custom new user - Provided as arg'):
+            new_user = self.get_user('new_user')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user=new_user)
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(new_user, response.wsgi_request.user)
+            self.assertEqual(new_user, response.context['user'])
+            self.assertEqual(new_user, response.user)
+
+        with self.subTest('Check login using super user - Provided as class variable'):
+            self.user = self.get_user('test_superuser')
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_superuser.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_superuser, response.wsgi_request.user)
+            self.assertEqual(self.test_superuser, response.context['user'])
+            self.assertEqual(self.test_superuser, response.user)
+
+        with self.subTest('Check login using admin user - Provided as class variable'):
+            self.user = self.get_user('test_admin')
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_admin.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_admin, response.wsgi_request.user)
+            self.assertEqual(self.test_admin, response.context['user'])
+            self.assertEqual(self.test_admin, response.user)
+
+        with self.subTest('Check login using inactive user - Provided as class variable'):
+            self.user = self.get_user('test_inactive')
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
+            self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
+            self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
+            self.assertTrue(isinstance(response.user, AnonymousUser))
+            self.assertFalse(isinstance(response.user, get_user_model()))
+
+        with self.subTest('Check login using standard user - Provided as class variable'):
+            self.user = self.get_user('test_user')
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_user, response.wsgi_request.user)
+            self.assertEqual(self.test_user, response.context['user'])
+            self.assertEqual(self.test_user, response.user)
+
+        with self.subTest('Check login using custom new user - Provided as class variable'):
+            self.user = self.get_user('new_user')
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(new_user, response.wsgi_request.user)
+            self.assertEqual(new_user, response.context['user'])
+            self.assertEqual(new_user, response.user)
+
+        with self.subTest('Check login using super user - Provided with conflicting values (function value should win)'):
+            self.user = self.get_user('new_user')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_superuser')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_superuser.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_superuser, response.wsgi_request.user)
+            self.assertEqual(self.test_superuser, response.context['user'])
+            self.assertEqual(self.test_superuser, response.user)
+
+        with self.subTest('Check login using admin user - Provided with conflicting values (function value should win)'):
+            self.user = self.get_user('test_superuser')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_admin')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_admin.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_admin, response.wsgi_request.user)
+            self.assertEqual(self.test_admin, response.context['user'])
+            self.assertEqual(self.test_admin, response.user)
+
+        with self.subTest('Check login using inactive user - Provided with conflicting values (function value should win)'):
+            self.user = self.get_user('test_admin')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_inactive')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            self.assertTrue(isinstance(response.wsgi_request.user, AnonymousUser))
+            self.assertFalse(isinstance(response.wsgi_request.user, get_user_model()))
+            self.assertNotEqual(self.test_inactive_user, response.wsgi_request.user)
+            self.assertTrue(isinstance(response.user, AnonymousUser))
+            self.assertFalse(isinstance(response.user, get_user_model()))
+
+        with self.subTest('Check login using standard user - Provided with conflicting values (function value should win)'):
+            self.user = self.get_user('test_inactive')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='test_user')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(self.test_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(self.test_user, response.wsgi_request.user)
+            self.assertEqual(self.test_user, response.context['user'])
+            self.assertEqual(self.test_user, response.user)
+
+        with self.subTest('Check login using custom new user - Provided with conflicting values (function value should win)'):
+            self.user = self.get_user('test_user')
+            response = self.assertGetResponse('django_expanded_test_cases:index', user='new_user')
+
+            # Various checks, of different ways to ensure expected user is logged in.
+            self.assertEqual(new_user.pk, int(self.client.session['_auth_user_id']))
+            self.assertEqual(new_user, response.wsgi_request.user)
+            self.assertEqual(new_user, response.context['user'])
+            self.assertEqual(new_user, response.user)
+
+    @patch('django_expanded_test_cases.test_cases.integration_test_case.ETC_REQUEST_USER_STRICTNESS', 'strict')
+    def test__assertResponse__user(self):
+        """
+        Tests "user" functionality of assertResponse() function.
+        """
+        with self.subTest('Without providing a login user'):
+            # No default user provided. Should error.
+            with self.assertRaises(ValidationError):
+                self.assertResponse('')
+
+        with self.subTest('With login as test user'):
+            response = self.assertResponse('', user=self.test_user)
+            self.assertEqual(response.user, self.test_user)
+            self.assertEqual(str(self.test_user.pk), self.client.session['_auth_user_id'])
+            response = self.assertResponse('', user='test_user')
+            self.assertEqual(response.user, self.test_user)
+            self.assertEqual(str(self.test_user.pk), self.client.session['_auth_user_id'])
+
+        with self.subTest('With login as admin user'):
+            response = self.assertResponse('', user=self.test_admin)
+            self.assertEqual(response.user, self.test_admin)
+            self.assertEqual(str(self.test_admin.pk), self.client.session['_auth_user_id'])
+            response = self.assertResponse('', user='test_admin')
+            self.assertEqual(response.user, self.test_admin)
+            self.assertEqual(str(self.test_admin.pk), self.client.session['_auth_user_id'])
+
+        with self.subTest('With login as superuser'):
+            response = self.assertResponse('', user=self.test_superuser)
+            self.assertEqual(response.user, self.test_superuser)
+            self.assertEqual(str(self.test_superuser.pk), self.client.session['_auth_user_id'])
+            response = self.assertResponse('', user='test_superuser')
+            self.assertEqual(response.user, self.test_superuser)
+            self.assertEqual(str(self.test_superuser.pk), self.client.session['_auth_user_id'])
+
+        with self.subTest('Without login, but test user passed'):
+            # Basically, passing a user should not really do anything here.
+            response = self.assertResponse('', user=self.test_user, auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            response = self.assertResponse('', user='test_user', auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+
+        with self.subTest('Without login, but admin user passed'):
+            # Basically, passing a user should not really do anything here.
+            response = self.assertResponse('', user=self.test_admin, auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            response = self.assertResponse('', user='test_admin', auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+
+        with self.subTest('Without login, but superuser passed'):
+            # Basically, passing a user should not really do anything here.
+            response = self.assertResponse('', user=self.test_superuser, auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+            response = self.assertResponse('', user='test_superuser', auto_login=False)
+            self.assertEqual(response.user, AnonymousUser())
+            with self.assertRaises(KeyError):
+                self.client.session['_auth_user_id']
+
+
+class IntegrationClassTest__NoAutoGeneratedUser(IntegrationTestCase):
+    """Tests for IntegrationTestCase class, specifically with no auto-generated users."""
+
+    @classmethod
+    @patch('django_expanded_test_cases.mixins.core_mixin.ETC_AUTO_GENERATE_USERS', False)
+    def setUpClass(cls):
+        # Run parent setup logic.
+        super().setUpClass()
+
+    @patch('django_expanded_test_cases.mixins.core_mixin.ETC_AUTO_GENERATE_USERS', False)
+    def test__class_users(self):
+        # Since no users were auto-generated, all of these class attributes should come back as None.
+        self.assertFalse(hasattr(self, 'test_superuser'))
+        self.assertFalse(hasattr(self, 'test_admin_user'))
+        self.assertFalse(hasattr(self, 'test_user'))
+        self.assertFalse(hasattr(self, 'test_inactive_user'))
```

### Comparing `django-expanded-test-cases-0.2.4/tests/test_cases/test_live_server_case.py` & `django-expanded-test-cases-0.3.0/tests/test_cases/test_live_server_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.2.4/tests/views.py` & `django-expanded-test-cases-0.3.0/tests/views.py`

 * *Files identical despite different names*

