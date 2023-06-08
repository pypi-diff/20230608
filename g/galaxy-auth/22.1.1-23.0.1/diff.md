# Comparing `tmp/galaxy-auth-22.1.1.tar.gz` & `tmp/galaxy-auth-23.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-auth-22.1.1.tar", last modified: Mon Aug 22 19:45:40 2022, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/auth/dist/.tmp-of_j90c6/galaxy-auth-23.0.1.tar", last modified: Thu Jun  8 17:43:01 2023, max compression
```

## Comparing `galaxy-auth-22.1.1.tar` & `galaxy-auth-23.0.1.tar`

### file list

```diff
@@ -1,41 +1,28 @@
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:40.112471 galaxy-auth-22.1.1/
--rw-r--r--   0 mvandenb   (501) staff       (20)      332 2022-08-22 19:45:28.000000 galaxy-auth-22.1.1/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)    11109 2021-09-10 08:52:38.000000 galaxy-auth-22.1.1/LICENSE
--rw-r--r--   0 mvandenb   (501) staff       (20)       28 2022-08-22 19:45:28.000000 galaxy-auth-22.1.1/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) staff       (20)     2954 2022-08-22 19:45:28.000000 galaxy-auth-22.1.1/Makefile
--rw-r--r--   0 mvandenb   (501) staff       (20)     1678 2022-08-22 19:45:40.112587 galaxy-auth-22.1.1/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      312 2022-03-24 19:47:11.000000 galaxy-auth-22.1.1/README.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)       89 2022-08-22 19:45:28.000000 galaxy-auth-22.1.1/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:40.105081 galaxy-auth-22.1.1/galaxy/
--rw-r--r--   0 mvandenb   (501) staff       (20)       91 2022-08-22 19:45:28.000000 galaxy-auth-22.1.1/galaxy/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:40.105803 galaxy-auth-22.1.1/galaxy/auth/
--rw-r--r--   0 mvandenb   (501) staff       (20)     5538 2022-08-22 19:45:27.000000 galaxy-auth-22.1.1/galaxy/auth/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:40.107483 galaxy-auth-22.1.1/galaxy/auth/providers/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1980 2022-08-22 19:45:27.000000 galaxy-auth-22.1.1/galaxy/auth/providers/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      768 2022-08-22 19:45:27.000000 galaxy-auth-22.1.1/galaxy/auth/providers/alwaysreject.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    10900 2022-08-22 19:45:27.000000 galaxy-auth-22.1.1/galaxy/auth/providers/ldap_ad.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      839 2022-08-22 19:45:27.000000 galaxy-auth-22.1.1/galaxy/auth/providers/localdb.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     7435 2022-08-22 19:45:27.000000 galaxy-auth-22.1.1/galaxy/auth/providers/pam_auth.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3392 2022-08-22 19:45:27.000000 galaxy-auth-22.1.1/galaxy/auth/util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      434 2022-08-22 19:45:29.000000 galaxy-auth-22.1.1/galaxy/project_galaxy_auth.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:40.110232 galaxy-auth-22.1.1/galaxy_auth.egg-info/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1678 2022-08-22 19:45:39.000000 galaxy-auth-22.1.1/galaxy_auth.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      792 2022-08-22 19:45:40.000000 galaxy-auth-22.1.1/galaxy_auth.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:39.000000 galaxy-auth-22.1.1/galaxy_auth.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       27 2022-08-22 19:45:39.000000 galaxy-auth-22.1.1/galaxy_auth.egg-info/entry_points.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:39.000000 galaxy-auth-22.1.1/galaxy_auth.egg-info/not-zip-safe
--rw-r--r--   0 mvandenb   (501) staff       (20)       12 2022-08-22 19:45:39.000000 galaxy-auth-22.1.1/galaxy_auth.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-08-22 19:45:39.000000 galaxy-auth-22.1.1/galaxy_auth.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       12 2022-08-22 19:45:28.000000 galaxy-auth-22.1.1/requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:40.111313 galaxy-auth-22.1.1/scripts/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1442 2022-08-22 19:45:28.000000 galaxy-auth-22.1.1/scripts/commit_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2166 2022-08-22 19:45:28.000000 galaxy-auth-22.1.1/scripts/new_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      804 2022-08-22 19:45:28.000000 galaxy-auth-22.1.1/scripts/print_version_for_release.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    33060 2022-08-22 19:45:40.120086 galaxy-auth-22.1.1/setup.cfg
--rw-r--r--   0 mvandenb   (501) staff       (20)     2788 2022-08-22 19:45:28.000000 galaxy-auth-22.1.1/setup.py
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-03-24 19:47:11.000000 galaxy-auth-22.1.1/test-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:40.111632 galaxy-auth-22.1.1/tests/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:11.000000 galaxy-auth-22.1.1/tests/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:40.112193 galaxy-auth-22.1.1/tests/auth/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:13.000000 galaxy-auth-22.1.1/tests/auth/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      845 2022-08-22 19:45:28.000000 galaxy-auth-22.1.1/tests/auth/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:01.000000 galaxy-auth-23.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 17:37:04.000000 galaxy-auth-23.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-08 17:37:03.000000 galaxy-auth-23.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 17:37:04.000000 galaxy-auth-23.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-08 17:43:01.000000 galaxy-auth-23.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-08 17:37:04.000000 galaxy-auth-23.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 17:37:04.000000 galaxy-auth-23.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:01.000000 galaxy-auth-23.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 17:37:04.000000 galaxy-auth-23.0.1/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:01.000000 galaxy-auth-23.0.1/galaxy/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-08 17:37:04.000000 galaxy-auth-23.0.1/galaxy/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:01.000000 galaxy-auth-23.0.1/galaxy/auth/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-08 17:37:04.000000 galaxy-auth-23.0.1/galaxy/auth/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-08 17:37:04.000000 galaxy-auth-23.0.1/galaxy/auth/providers/alwaysreject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18471 2023-06-08 17:37:04.000000 galaxy-auth-23.0.1/galaxy/auth/providers/ldap_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-08 17:37:04.000000 galaxy-auth-23.0.1/galaxy/auth/providers/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-06-08 17:37:04.000000 galaxy-auth-23.0.1/galaxy/auth/providers/pam_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-08 17:37:04.000000 galaxy-auth-23.0.1/galaxy/auth/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-auth-23.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:01.000000 galaxy-auth-23.0.1/galaxy_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-08 17:43:01.000000 galaxy-auth-23.0.1/galaxy_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-08 17:43:01.000000 galaxy-auth-23.0.1/galaxy_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:43:01.000000 galaxy-auth-23.0.1/galaxy_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 17:43:01.000000 galaxy-auth-23.0.1/galaxy_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:43:01.000000 galaxy-auth-23.0.1/galaxy_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 17:37:04.000000 galaxy-auth-23.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-08 17:43:01.000000 galaxy-auth-23.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:37:04.000000 galaxy-auth-23.0.1/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `galaxy-auth-22.1.1/LICENSE` & `galaxy-auth-23.0.1/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,61 @@
-Copyright (c) 2005-2016 Galaxy Contributors (see CONTRIBUTORS.md)
+Copyright (c) 2005-2022 Galaxy Contributors (see CONTRIBUTORS.md)
+
+Work contributed from 2021-04-07 onwards is licensed under the MIT License.
+Work contributed before this date is licensed under the Academic Free License
+version 3.0.
+See https://github.com/galaxyproject/galaxy/ for the contribution history.
+See below for the full text of both licenses.
+
+
+Some icons found in Galaxy are from the Silk Icons set, available under
+the Creative Commons Attribution 2.5 License, from:
+
+http://www.famfamfam.com/lab/icons/silk/
+
+
+Other images and documentation are licensed under the Creative Commons
+Attribution 3.0 (CC BY 3.0) License. See:
+
+http://creativecommons.org/licenses/by/3.0/
+
+
+--------------------------------------------------------------------------------
+
+
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+--------------------------------------------------------------------------------
+
+
+Academic Free License ("AFL") v. 3.0
+
+This Academic Free License (the "License") applies to any original work of
+authorship (the "Original Work") whose owner (the "Licensor") has placed the
+following licensing notice adjacent to the copyright notice for the Original
+Work:
 
 Licensed under the Academic Free License version 3.0
 
  1) Grant of Copyright License. Licensor grants You a worldwide, royalty-free, 
     non-exclusive, sublicensable license, for the duration of the copyright, to 
     do the following:
 
@@ -169,18 +222,7 @@
     replace the notice specified in the first paragraph above with the 
     notice "Licensed under <insert your license name here>" or with a notice 
     of your own that is not confusingly similar to the notice in this 
     License; and (iii) You may not claim that your original works are open 
     source software unless your Modified License has been approved by Open 
     Source Initiative (OSI) and You comply with its license review and 
     certification process.
-
-
-Some icons found in Galaxy are from the Silk Icons set, available under
-the Creative Commons Attribution 2.5 License, from:
-
-http://www.famfamfam.com/lab/icons/silk/
-
-
-Other images and documentation are licensed under the Creative Commons Attribution 3.0 (CC BY 3.0) License.   See 
-
-http://creativecommons.org/licenses/by/3.0/
```

### Comparing `galaxy-auth-22.1.1/PKG-INFO` & `galaxy-auth-23.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,65 @@
 Metadata-Version: 2.1
 Name: galaxy-auth
-Version: 22.1.1
-Summary: Galaxy Auth Framework and Implementations
+Version: 23.0.1
+Summary: Galaxy auth framework and implementations
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
-Keywords: galaxy
-Platform: UNKNOWN
+Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Testing
 Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: https://badge.fury.io/py/galaxy-auth.svg
    :target: https://pypi.org/project/galaxy-auth/
 
 
 
 Overview
 --------
 
 The Galaxy_ auth framework and default plugins.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
-
-
-
 History
 -------
 
 .. to_doc
 
----------------------
-20.9.1.dev0
----------------------
-
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
+No recorded changes since last release
 
----------------------
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.05 branch of Galaxy.
-
-
```

### Comparing `galaxy-auth-22.1.1/galaxy/auth/__init__.py` & `galaxy-auth-23.0.1/galaxy/auth/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,132 +1,130 @@
 """
 Contains implementations of the authentication logic.
 """
 import logging
 
-from galaxy.auth.util import get_authenticators, parse_auth_results
+from galaxy.auth.util import (
+    get_authenticators,
+    parse_auth_results,
+)
 from galaxy.exceptions import Conflict
 from galaxy.util import string_as_bool
 
 log = logging.getLogger(__name__)
 
 
 class AuthManager:
-
     def __init__(self, config):
         self.redact_username_in_logs = config.redact_username_in_logs
-        self.authenticators = get_authenticators(config.auth_config_file, config.is_set('auth_config_file'))
+        self.authenticators = get_authenticators(config.auth_config_file, config.is_set("auth_config_file"))
 
-    def check_registration_allowed(self, email, username, password):
+    def check_registration_allowed(self, email, username, password, request):
         """Checks if the provided email/username is allowed to register."""
-        message = ''
-        status = 'done'
+        message = ""
+        status = "done"
         for provider, options in self.active_authenticators(email, username, password):
             allow_reg = _get_allow_register(options)
-            if allow_reg == 'challenge':
-                auth_results = provider.authenticate(email, username, password, options)
+            if allow_reg == "challenge":
+                auth_results = provider.authenticate(email, username, password, options, request)
                 if auth_results[0] is True:
                     break
                 if auth_results[0] is None:
-                    message = 'Invalid email address/username or password.'
-                    status = 'error'
+                    message = "Invalid email address/username or password."
+                    status = "error"
                     break
             elif allow_reg is True:
                 break
             elif allow_reg is False:
-                message = 'Account registration not required for your account.  Please simply login.'
-                status = 'error'
+                message = "Account registration not required for your account.  Please simply login."
+                status = "error"
                 break
         return message, status
 
     def check_auto_registration(self, trans, login, password, no_password_check=False):
         """
         Checks the username/email & password using auth providers in order.
         If a match is found, returns the 'auto-register' option for that provider.
         """
-        if '@' in login:
+        if "@" in login:
             email = login
             username = None
         else:
             email = None
             username = login
-        auth_return = {
-            "auto_reg": False,
-            "email": "",
-            "username": ""
-        }
+        auth_return = {"auto_reg": False, "email": "", "username": ""}
         for provider, options in self.active_authenticators(email, username, password):
             if provider is None:
                 log.debug(f"Unable to find module: {options}")
             else:
-                options['no_password_check'] = no_password_check
-                auth_results = provider.authenticate(email, username, password, options)
+                options["no_password_check"] = no_password_check
+                auth_results = provider.authenticate(email, username, password, options, trans.request)
                 if auth_results[0] is True:
                     try:
                         auth_return = parse_auth_results(trans, auth_results, options)
                     except Conflict as conflict:
                         log.exception(conflict)
                         raise
                     return auth_return
                 elif auth_results[0] is None:
                     log.debug("Login: '%s', stopping due to failed non-continue", login)
                     break  # end authentication (skip rest)
         return auth_return
 
-    def check_password(self, user, password):
+    def check_password(self, user, password, request):
         """Checks the username/email and password using auth providers."""
         for provider, options in self.active_authenticators(user.email, user.username, password):
             if provider is None:
                 log.debug(f"Unable to find module: {options}")
             else:
-                auth_result = provider.authenticate_user(user, password, options)
+                auth_result = provider.authenticate_user(user, password, options, request)
                 if auth_result is True:
                     return True  # accept user
                 elif auth_result is None:
                     break  # end authentication (skip rest)
         return False
 
-    def check_change_password(self, user, current_password):
+    def check_change_password(self, user, current_password, request):
         """Checks that auth provider allows password changes and current_password
         matches.
         """
         for provider, options in self.active_authenticators(user.email, user.username, current_password):
             if provider is None:
                 log.debug(f"Unable to find module: {options}")
             else:
-                auth_result = provider.authenticate_user(user, current_password, options)
+                auth_result = provider.authenticate_user(user, current_password, options, request)
                 if auth_result is True:
                     if string_as_bool(options.get("allow-password-change", False)):
                         return
                     else:
-                        return 'Password change not supported.'
+                        return "Password change not supported."
                 elif auth_result is None:
                     break  # end authentication (skip rest)
-        return 'Invalid current password.'
+        return "Invalid current password."
 
     def active_authenticators(self, email, username, password):
         """Yields AuthProvider instances for the provided configfile that match the
         filters.
         """
         try:
             for authenticator in self.authenticators:
                 filter_template = authenticator.filter_template
                 if filter_template:
                     filter_str = filter_template.format(email=email, username=username, password=password)
-                    passed_filter = eval(filter_str, {"__builtins__": None}, {'str': str})
+                    passed_filter = eval(filter_str, {"__builtins__": None}, {"str": str})
                     if not passed_filter:
                         continue  # skip to next
                 options = authenticator.options
-                options['redact_username_in_logs'] = self.redact_username_in_logs
+                options["redact_username_in_logs"] = self.redact_username_in_logs
                 yield authenticator.plugin, options
         except Exception:
             log.exception("Active Authenticators Failure")
             raise
 
 
 def _get_allow_register(d):
-    s = d.get('allow-register', True)
+    s = d.get("allow-register", True)
     lower_s = str(s).lower()
-    if lower_s == 'challenge':
+    if lower_s == "challenge":
         return lower_s
     else:
         return string_as_bool(s)
```

### Comparing `galaxy-auth-22.1.1/galaxy/auth/providers/__init__.py` & `galaxy-auth-23.0.1/galaxy/auth/providers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,53 +5,70 @@
 """
 import abc
 
 
 class AuthProvider(metaclass=abc.ABCMeta):
     """A base class for all Auth Providers."""
 
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def plugin_type(self):
-        """ Short string providing labelling this plugin """
+        """Short string providing labelling this plugin"""
 
     @abc.abstractmethod
-    def authenticate(self, email, username, password, options):
+    def authenticate(self, email, username, password, options, request):
         """
         Check that the user credentials are correct.
 
+        Besides checking password, it is possible to perform custom checks
+        like filtering client remote IP address using the request argument. We can
+        get the remote IP address of the client using request.remote_addr and
+        check if the IP is in whitelisted IPs and deny the authentication if
+        it is not.
+
         NOTE: Used within auto-registration to check it is ok to register this
         user.
 
         :param  email: the user's email address
         :type   email: str
         :param  username: the user's username
         :type   username: str
         :param  password: the plain text password they typed
         :type   password: str
         :param  options: options provided in auth_config_file
         :type   options: dict
+        :param  request: HTTP request object
+        :type   request: GalaxyWebTransaction.request
         :returns:   True: accept user, False: reject user and None: reject user
             and don't try any other providers.  str, str are the email and
             username to register with if accepting. The optional dict may
             contain other attributes, e.g. roles to assign when autoregistering.
         :rtype:     (bool, str, str) or (bool, str, str, dict)
         """
 
     @abc.abstractmethod
-    def authenticate_user(self, user, password, options):
+    def authenticate_user(self, user, password, options, request):
         """
         Same as authenticate() method, except an User object is provided instead
         of a username.
 
+        Besides checking password, it is possible to perform custom checks
+        like filtering client remote IP address using the request argument. We can
+        get the remote IP address of the client using request.remote_addr and
+        check if the IP is in whitelisted IPs and deny the authentication if
+        it is not.
+
         NOTE: used on normal login to check authentication and update user
         details if required.
 
         :param  user: the user to authenticate
         :type   user: galaxy.model.User
         :param  password: the plain text password they typed
         :type   password: str
         :param  options: options provided in auth_config_file
         :type   options: dict
+        :param  request: HTTP request object
+        :type   request: GalaxyWebTransaction.request
         :returns:   True: accept user, False: reject user and None: reject user
             and don't try any other providers
         :rtype:     bool
         """
```

### Comparing `galaxy-auth-22.1.1/galaxy/auth/providers/alwaysreject.py` & `galaxy-auth-23.0.1/galaxy/auth/providers/alwaysreject.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """
 Created on 16/07/2014
 
 @author: Andrew Robinson
 """
 import logging
 
-from ..providers import AuthProvider
+from . import AuthProvider
 
 log = logging.getLogger(__name__)
 
 
 class AlwaysReject(AuthProvider):
     """A simple authenticator that just accepts users (does not care about their
     password).
     """
-    plugin_type = 'alwaysreject'
 
-    def authenticate(self, email, username, password, options):
+    plugin_type = "alwaysreject"
+
+    def authenticate(self, email, username, password, options, request):
         """
         See abstract method documentation.
         """
-        return (None, '', '')
+        return (None, "", "")
 
-    def authenticate_user(self, user, password, options):
+    def authenticate_user(self, user, password, options, request):
         """
         See abstract method documentation.
         """
         log.debug(f"User: {user.id if options['redact_username_in_logs'] else user.email}, ALWAYSREJECT: None")
         return None
 
 
-__all__ = ('AlwaysReject', )
+__all__ = ("AlwaysReject",)
```

### Comparing `galaxy-auth-22.1.1/galaxy/auth/providers/localdb.py` & `galaxy-auth-23.0.1/galaxy/auth/providers/localdb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """
 Created on 16/07/2014
 
 @author: Andrew Robinson
 """
 import logging
 
-from ..providers import AuthProvider
+from . import AuthProvider
 
 log = logging.getLogger(__name__)
 
 
 class LocalDB(AuthProvider):
     """Authenticate users against the local Galaxy database (as per usual)."""
-    plugin_type = 'localdb'
 
-    def authenticate(self, email, username, password, options):
+    plugin_type = "localdb"
+
+    def authenticate(self, email, username, password, options, request):
         """
         See abstract method documentation.
         """
-        return (False, '', '')  # it can never auto-create based of localdb (chicken-egg)
+        return (False, "", "")  # it can never auto-create based of localdb (chicken-egg)
 
-    def authenticate_user(self, user, password, options):
+    def authenticate_user(self, user, password, options, request):
         """
         See abstract method documentation.
         """
         user_ok = user.check_password(password)
         log.debug(f"User: {user.id if options['redact_username_in_logs'] else user.email}, LOCALDB: {user_ok}")
         return user_ok
 
 
-__all__ = ('LocalDB', )
+__all__ = ("LocalDB",)
```

### Comparing `galaxy-auth-22.1.1/galaxy/auth/providers/pam_auth.py` & `galaxy-auth-23.0.1/galaxy/auth/providers/pam_auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 Author Peter van Heusden (pvh@sanbi.ac.za)
 """
 import logging
 import shlex
 
 from galaxy.util import (
     commands,
-    string_as_bool
+    string_as_bool,
 )
-from ..providers import AuthProvider
+from . import AuthProvider
 
 log = logging.getLogger(__name__)
 
 """
 This module provides an AuthProvider for PAM (pluggable authentication module) authentication.
 PAM is the Pluggable Authentication Module system (http://www.linux-pam.org/)
 It relies on python-pam (https://pypi.python.org/pypi/python-pam)
@@ -51,105 +51,112 @@
           <pam-service>ssh</pam-service>
   </options>
 </authenticator>
 """
 
 
 class PAM(AuthProvider):
+    plugin_type = "PAM"
 
-    plugin_type = 'PAM'
-
-    def authenticate(self, email, username, password, options):
+    def authenticate(self, email, username, password, options, request):
         pam_username = None
         auto_register_username = None
         auto_register_email = None
         force_fail = False
-        if not options['redact_username_in_logs']:
-            log.debug(f"use username: {options.get('login-use-username')} use email {options.get('login-use-email', False)} email {email} username {username}")
+        if not options["redact_username_in_logs"]:
+            log.debug(
+                f"use username: {options.get('login-use-username')} use email {options.get('login-use-email', False)} email {email} username {username}"
+            )
         # check email based login first because if email exists in Galaxy DB
         # we will be given the "public name" as username
-        if string_as_bool(options.get('login-use-email', False)) and email is not None:
-            if '@' in email:
-                (email_user, email_domain) = email.split('@')
+        if string_as_bool(options.get("login-use-email", False)) and email is not None:
+            if "@" in email:
+                (email_user, email_domain) = email.split("@")
                 pam_username = email_user
-                if email_domain == options.get('maildomain', None):
+                if email_domain == options.get("maildomain", None):
                     auto_register_email = email
                     if username is not None:
                         auto_register_username = username
                     else:
                         auto_register_username = email_user
                 else:
-                    log.debug('PAM authenticate: warning: email does not match configured PAM maildomain')
+                    log.debug("PAM authenticate: warning: email does not match configured PAM maildomain")
                     # no need to fail: if auto-register is not enabled, this
                     # might still be a valid user
             else:
-                log.debug('PAM authenticate: email must be used to login, but no valid email found')
+                log.debug("PAM authenticate: email must be used to login, but no valid email found")
                 force_fail = True
-        elif string_as_bool(options.get('login-use-username', False)):
+        elif string_as_bool(options.get("login-use-username", False)):
             # if we get here via authenticate_user then
             # user will be "public name" and
             # email address will be as per registered user
             if username is not None:
                 pam_username = username
                 if email is not None:
                     auto_register_email = email
-                elif options.get('maildomain', None) is not None:
+                elif options.get("maildomain", None) is not None:
                     # we can register a user with this username and mail domain
                     # if auto registration is enabled
                     auto_register_email = f"{username}@{options['maildomain']}"
                 auto_register_username = username
             else:
-                log.debug('PAM authenticate: username login selected but no username provided')
+                log.debug("PAM authenticate: username login selected but no username provided")
                 force_fail = True
         else:
-            log.debug('PAM authenticate: could not find username for PAM')
+            log.debug("PAM authenticate: could not find username for PAM")
             force_fail = True
 
         if force_fail:
-            return None, '', ''
+            return None, "", ""
 
-        pam_service = options.get('pam-service', 'galaxy')
-        use_helper = string_as_bool(options.get('use-external-helper', False))
+        pam_service = options.get("pam-service", "galaxy")
+        use_helper = string_as_bool(options.get("use-external-helper", False))
         log.debug(f"PAM auth: will use external helper: {use_helper}")
         authenticated = False
         if use_helper:
-            authentication_helper = options.get('authentication-helper-script', '/bin/false').strip()
+            authentication_helper = options.get("authentication-helper-script", "/bin/false").strip()
             log.debug(f"PAM auth: external helper script: {authentication_helper}")
-            if not authentication_helper.startswith('/'):
+            if not authentication_helper.startswith("/"):
                 # don't accept relative path
                 authenticated = False
             else:
-                auth_cmd = shlex.split(f'/usr/bin/sudo -n {authentication_helper}')
+                auth_cmd = shlex.split(f"/usr/bin/sudo -n {authentication_helper}")
                 log.debug(f"PAM auth: external helper cmd: {auth_cmd}")
-                message = f'{pam_service}\n{pam_username}\n{password}\n'
+                message = f"{pam_service}\n{pam_username}\n{password}\n"
                 try:
                     output = commands.execute(auth_cmd, input=message)
                 except commands.CommandLineException as e:
-                    if e.stderr != '':
-                        log.debug(f"PAM auth: external authentication script had errors: status {e.returncode} error {e.stderr}")
+                    if e.stderr != "":
+                        log.debug(
+                            f"PAM auth: external authentication script had errors: status {e.returncode} error {e.stderr}"
+                        )
                     output = e.stdout
-                if output.strip() == 'True':
+                if output.strip() == "True":
                     authenticated = True
                 else:
                     authenticated = False
         else:
             try:
                 import pam
             except ImportError:
-                log.debug('PAM authenticate: could not load pam module, PAM authentication disabled')
-                return None, '', ''
+                log.debug("PAM authenticate: could not load pam module, PAM authentication disabled")
+                return None, "", ""
 
             p_auth = pam.pam()
             authenticated = p_auth.authenticate(pam_username, password, service=pam_service)
 
         if authenticated:
-            log.debug(f"PAM authentication successful for {'redacted' if options['redact_username_in_logs'] else pam_username}")
+            log.debug(
+                f"PAM authentication successful for {'redacted' if options['redact_username_in_logs'] else pam_username}"
+            )
             return True, auto_register_email, auto_register_username
         else:
-            log.debug(f"PAM authentication failed for {'redacted' if options['redact_username_in_logs'] else pam_username}")
-            return False, '', ''
+            log.debug(
+                f"PAM authentication failed for {'redacted' if options['redact_username_in_logs'] else pam_username}"
+            )
+            return False, "", ""
 
-    def authenticate_user(self, user, password, options):
-        return self.authenticate(user.email, user.username, password, options)[0]
+    def authenticate_user(self, user, password, options, request):
+        return self.authenticate(user.email, user.username, password, options, request)[0]
 
 
-__all__ = ('PAM', )
+__all__ = ("PAM",)
```

### Comparing `galaxy-auth-22.1.1/galaxy/auth/util.py` & `galaxy-auth-23.0.1/galaxy/auth/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,61 +8,62 @@
 from galaxy.util import (
     parse_xml,
     parse_xml_string,
     plugin_config,
     string_as_bool,
 )
 
-
 log = logging.getLogger(__name__)
 
 AUTH_CONF_XML = """<?xml version="1.0"?>
 <auth>
     <authenticator>
         <type>localdb</type>
         <options>
             <allow-password-change>true</allow-password-change>
         </options>
     </authenticator>
 </auth>
 """
 
-Authenticator = namedtuple('Authenticator', ['plugin', 'filter_template', 'options'])
+Authenticator = namedtuple("Authenticator", ["plugin", "filter_template", "options"])
 
 
 def get_authenticators(auth_config_file, auth_config_file_set):
-    __plugins_dict = plugin_config.plugins_dict(galaxy.auth.providers, 'plugin_type')
+    __plugins_dict = plugin_config.plugins_dict(galaxy.auth.providers, "plugin_type")
     # parse XML
     try:
         ct = parse_xml(auth_config_file)
         conf_root = ct.getroot()
     except OSError as exc:
         if exc.errno == errno.ENOENT and not auth_config_file_set:
             conf_root = parse_xml_string(AUTH_CONF_XML)
         else:
             raise
 
     authenticators = []
     # process authenticators
     for auth_elem in conf_root:
-        type_elem_text = auth_elem.find('type').text
+        type_elem_text = auth_elem.find("type").text
         plugin_class = __plugins_dict.get(type_elem_text)
         if not plugin_class:
-            raise Exception(f"Authenticator type '{type_elem_text}' not recognized, should be one of {', '.join(__plugins_dict)}")
+            raise Exception(
+                f"Authenticator type '{type_elem_text}' not recognized, should be one of {', '.join(__plugins_dict)}"
+            )
         plugin = plugin_class()
 
         # check filterelem
-        filter_elem = auth_elem.find('filter')
+        filter_elem = auth_elem.find("filter")
         if filter_elem is not None:
             filter_template = str(filter_elem.text)
         else:
             filter_template = None
 
         # extract options
-        options_elem = auth_elem.find('options')
+        options_elem = auth_elem.find("options")
         options = {}
         if options_elem is not None:
             for opt in options_elem:
                 options[opt.tag] = opt.text
         authenticator = Authenticator(
             plugin=plugin,
             filter_template=filter_template,
@@ -73,28 +74,36 @@
 
 
 def parse_auth_results(trans, auth_results, options):
     auth_return = {}
     auth_result, auto_email, auto_username = auth_results[:3]
     auto_username = str(auto_username).lower()
     # make username unique
-    if validate_publicname(trans, auto_username) != '':
-        i = 1
-        while i <= 10:  # stop after 10 tries
-            if validate_publicname(trans, "%s-%i" % (auto_username, i)) == '':
-                auto_username = "%s-%i" % (auto_username, i)
-                break
-            i += 1
+    max_retries = int(options.get("max-retries", "10"))
+    try_number = 0
+    while try_number <= max_retries:
+        if try_number == 0:
+            test_name = auto_username
+        else:
+            test_name = f"{auto_username}-{try_number}"
+        validate_result = validate_publicname(trans, test_name)
+        if validate_result == "":
+            auto_username = test_name
+            break
         else:
-            raise Conflict("Cannot make unique username")
+            log.debug(f"Invalid username '{auto_username}': {validate_result}")
+        try_number += 1
+    else:
+        raise Conflict("Cannot make unique username")
     log.debug(f"Email: {auto_email}, auto-register with username: {auto_username}")
-    auth_return["auto_reg"] = string_as_bool(options.get('auto-register', False))
+    auth_return["auto_reg"] = string_as_bool(options.get("auto-register", False))
     auth_return["email"] = auto_email
     auth_return["username"] = auto_username
-    auth_return["auto_create_roles"] = string_as_bool(options.get('auto-create-roles', False))
-    auth_return["auto_create_groups"] = string_as_bool(options.get('auto-create-groups', False))
+    auth_return["auto_create_roles"] = string_as_bool(options.get("auto-create-roles", False))
+    auth_return["auto_create_groups"] = string_as_bool(options.get("auto-create-groups", False))
     auth_return["auto_assign_roles_to_groups_only"] = string_as_bool(
-        options.get('auto-assign-roles-to-groups-only', False))
+        options.get("auto-assign-roles-to-groups-only", False)
+    )
 
     if len(auth_results) == 4:
         auth_return["attributes"] = auth_results[3]
     return auth_return
```

### Comparing `galaxy-auth-22.1.1/galaxy_auth.egg-info/PKG-INFO` & `galaxy-auth-23.0.1/galaxy_auth.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,65 @@
 Metadata-Version: 2.1
 Name: galaxy-auth
-Version: 22.1.1
-Summary: Galaxy Auth Framework and Implementations
+Version: 23.0.1
+Summary: Galaxy auth framework and implementations
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
-Keywords: galaxy
-Platform: UNKNOWN
+Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Testing
 Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: https://badge.fury.io/py/galaxy-auth.svg
    :target: https://pypi.org/project/galaxy-auth/
 
 
 
 Overview
 --------
 
 The Galaxy_ auth framework and default plugins.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
-
-
-
 History
 -------
 
 .. to_doc
 
----------------------
-20.9.1.dev0
----------------------
-
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
+No recorded changes since last release
 
----------------------
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.05 branch of Galaxy.
-
-
```

