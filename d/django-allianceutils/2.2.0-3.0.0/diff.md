# Comparing `tmp/django-allianceutils-2.2.0.tar.gz` & `tmp/django_allianceutils-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-allianceutils-2.2.0.tar", max compression
+gzip compressed data, was "django_allianceutils-3.0.0.tar", max compression
```

## Comparing `django-allianceutils-2.2.0.tar` & `django_allianceutils-3.0.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0     2325 2022-03-28 00:32:33.115624 django-allianceutils-2.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1541 2021-01-26 21:26:44.937248 django-allianceutils-2.2.0/LICENSE
--rw-r--r--   0        0        0    36849 2021-12-16 08:21:35.329736 django-allianceutils-2.2.0/README.md
--rw-r--r--   0        0        0      418 2022-03-28 00:32:39.769775 django-allianceutils-2.2.0/allianceutils/__init__.py
--rw-r--r--   0        0        0       22 2021-03-25 03:28:54.795488 django-allianceutils-2.2.0/allianceutils/api/__init__.py
--rw-r--r--   0        0        0     3223 2021-03-25 03:28:54.795707 django-allianceutils-2.2.0/allianceutils/api/mixins.py
--rw-r--r--   0        0        0     4407 2021-03-25 03:28:54.795929 django-allianceutils-2.2.0/allianceutils/api/parsers.py
--rw-r--r--   0        0        0     7935 2021-12-16 08:21:35.330332 django-allianceutils-2.2.0/allianceutils/api/permissions.py
--rw-r--r--   0        0        0      568 2021-03-25 03:28:54.796128 django-allianceutils-2.2.0/allianceutils/api/renderers.py
--rw-r--r--   0        0        0      192 2020-03-16 00:53:11.409068 django-allianceutils-2.2.0/allianceutils/apps.py
--rw-r--r--   0        0        0        0 2021-01-26 21:23:34.993918 django-allianceutils-2.2.0/allianceutils/auth/__init__.py
--rw-r--r--   0        0        0     2277 2021-12-16 08:21:35.330609 django-allianceutils-2.2.0/allianceutils/auth/backends.py
--rw-r--r--   0        0        0    12299 2021-12-16 08:21:35.330890 django-allianceutils-2.2.0/allianceutils/auth/models.py
--rwxr-xr-x   0        0        0      590 2020-03-16 00:53:11.410494 django-allianceutils-2.2.0/allianceutils/bin/internaldeps.sh
--rw-r--r--   0        0        0    17294 2022-03-28 00:23:15.657007 django-allianceutils-2.2.0/allianceutils/checks.py
--rw-r--r--   0        0        0     2089 2021-02-23 01:51:58.449400 django-allianceutils-2.2.0/allianceutils/decorators.py
--rw-r--r--   0        0        0     1144 2021-12-16 08:21:35.331612 django-allianceutils-2.2.0/allianceutils/filters.py
--rw-r--r--   0        0        0        0 2020-03-16 00:53:11.411040 django-allianceutils-2.2.0/allianceutils/management/__init__.py
--rw-r--r--   0        0        0        0 2020-03-16 00:53:11.411159 django-allianceutils-2.2.0/allianceutils/management/commands/__init__.py
--rw-r--r--   0        0        0     1759 2021-12-16 08:21:35.331990 django-allianceutils-2.2.0/allianceutils/management/commands/base.py
--rw-r--r--   0        0        0     6206 2021-01-26 21:26:44.938773 django-allianceutils-2.2.0/allianceutils/management/commands/document_reverse_accessors.py
--rw-r--r--   0        0        0     1547 2020-03-16 00:53:11.411790 django-allianceutils-2.2.0/allianceutils/management/commands/print_logging.py
--rw-r--r--   0        0        0      234 2020-03-16 00:53:11.412072 django-allianceutils-2.2.0/allianceutils/middleware/__init__.py
--rw-r--r--   0        0        0     1898 2021-12-16 08:21:35.332305 django-allianceutils-2.2.0/allianceutils/middleware/current_user.py
--rw-r--r--   0        0        0     1216 2020-03-16 00:53:11.412294 django-allianceutils-2.2.0/allianceutils/middleware/http_auth.py
--rw-r--r--   0        0        0     3378 2021-01-26 21:26:44.939135 django-allianceutils-2.2.0/allianceutils/middleware/query_count.py
--rw-r--r--   0        0        0     1028 2021-01-26 21:26:44.939348 django-allianceutils-2.2.0/allianceutils/migrations.py
--rw-r--r--   0        0        0     8680 2021-12-16 08:21:35.332574 django-allianceutils-2.2.0/allianceutils/models.py
--rw-r--r--   0        0        0     1325 2021-12-16 08:21:35.332796 django-allianceutils-2.2.0/allianceutils/rules.py
--rw-r--r--   0        0        0        0 2020-03-16 00:53:11.413094 django-allianceutils-2.2.0/allianceutils/serializers/__init__.py
--rw-r--r--   0        0        0      560 2020-03-16 00:53:11.413216 django-allianceutils-2.2.0/allianceutils/serializers/json_ordered.py
--rw-r--r--   0        0        0        0 2020-03-16 00:53:11.413950 django-allianceutils-2.2.0/allianceutils/templatetags/__init__.py
--rw-r--r--   0        0        0     1957 2020-03-16 00:53:11.414071 django-allianceutils-2.2.0/allianceutils/templatetags/alliance_webpack.py
--rw-r--r--   0        0        0     1345 2021-12-16 08:21:35.333166 django-allianceutils-2.2.0/allianceutils/templatetags/default_value.py
--rw-r--r--   0        0        0     2073 2021-12-16 08:21:35.333450 django-allianceutils-2.2.0/allianceutils/util/__init__.py
--rw-r--r--   0        0        0     8216 2021-03-25 10:17:24.367010 django-allianceutils-2.2.0/allianceutils/util/camel_case.py
--rw-r--r--   0        0        0     1238 2021-01-26 21:26:44.939791 django-allianceutils-2.2.0/allianceutils/util/date.py
--rw-r--r--   0        0        0      968 2021-12-16 08:21:35.333699 django-allianceutils-2.2.0/allianceutils/util/get_firstparty_apps.py
--rw-r--r--   0        0        0        0 2020-03-16 00:53:11.415065 django-allianceutils-2.2.0/allianceutils/views/__init__.py
--rw-r--r--   0        0        0      872 2020-03-16 00:53:11.415195 django-allianceutils-2.2.0/allianceutils/views/decorators.py
--rw-r--r--   0        0        0     7092 2021-06-11 05:03:32.421912 django-allianceutils-2.2.0/allianceutils/webpack.py
--rw-r--r--   0        0        0     1737 2022-03-28 00:32:40.577285 django-allianceutils-2.2.0/pyproject.toml
--rw-r--r--   0        0        0    38971 2022-03-28 00:32:44.684311 django-allianceutils-2.2.0/setup.py
--rw-r--r--   0        0        0    37870 2022-03-28 00:32:44.687882 django-allianceutils-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3628 2023-06-08 00:59:23.897567 django_allianceutils-3.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1541 2020-09-13 18:13:00.145577 django_allianceutils-3.0.0/LICENSE
+-rw-r--r--   0        0        0    38610 2023-06-08 00:58:48.623754 django_allianceutils-3.0.0/README.md
+-rw-r--r--   0        0        0     5972 2023-06-08 00:59:36.341485 django_allianceutils-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1000 2023-06-08 00:59:35.523430 django_allianceutils-3.0.0/src/allianceutils/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-05 01:24:04.281525 django_allianceutils-3.0.0/src/allianceutils/api/__init__.py
+-rw-r--r--   0        0        0     4154 2023-06-05 01:24:04.281720 django_allianceutils-3.0.0/src/allianceutils/api/mixins.py
+-rw-r--r--   0        0        0     4380 2023-06-05 01:24:04.281911 django_allianceutils-3.0.0/src/allianceutils/api/parsers.py
+-rw-r--r--   0        0        0     7935 2023-06-05 01:24:04.282167 django_allianceutils-3.0.0/src/allianceutils/api/permissions.py
+-rw-r--r--   0        0        0      568 2023-06-05 01:24:04.282357 django_allianceutils-3.0.0/src/allianceutils/api/renderers.py
+-rw-r--r--   0        0        0      192 2023-06-05 01:24:04.282852 django_allianceutils-3.0.0/src/allianceutils/apps.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:24:04.282975 django_allianceutils-3.0.0/src/allianceutils/auth/__init__.py
+-rw-r--r--   0        0        0     2056 2023-06-05 01:24:04.283129 django_allianceutils-3.0.0/src/allianceutils/auth/backends.py
+-rw-r--r--   0        0        0    13890 2023-06-08 00:58:45.062512 django_allianceutils-3.0.0/src/allianceutils/auth/models.py
+-rwxr-xr-x   0        0        0      590 2023-06-05 01:24:04.283948 django_allianceutils-3.0.0/src/allianceutils/bin/internaldeps.sh
+-rw-r--r--   0        0        0    15004 2023-06-05 01:24:04.284300 django_allianceutils-3.0.0/src/allianceutils/checks.py
+-rw-r--r--   0        0        0     3118 2023-06-08 00:58:45.063255 django_allianceutils-3.0.0/src/allianceutils/decorators.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:24:04.284626 django_allianceutils-3.0.0/src/allianceutils/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:24:04.284767 django_allianceutils-3.0.0/src/allianceutils/management/commands/__init__.py
+-rw-r--r--   0        0        0     1829 2023-06-05 01:24:04.284986 django_allianceutils-3.0.0/src/allianceutils/management/commands/base.py
+-rw-r--r--   0        0        0     6991 2023-06-05 01:24:04.285225 django_allianceutils-3.0.0/src/allianceutils/management/commands/document_reverse_accessors.py
+-rw-r--r--   0        0        0     1600 2023-06-05 01:24:04.285405 django_allianceutils-3.0.0/src/allianceutils/management/commands/print_logging.py
+-rw-r--r--   0        0        0      234 2023-06-05 01:24:04.285610 django_allianceutils-3.0.0/src/allianceutils/middleware/__init__.py
+-rw-r--r--   0        0        0     1899 2023-06-05 01:24:04.285819 django_allianceutils-3.0.0/src/allianceutils/middleware/current_user.py
+-rw-r--r--   0        0        0     1216 2023-06-05 01:24:04.285981 django_allianceutils-3.0.0/src/allianceutils/middleware/http_auth.py
+-rw-r--r--   0        0        0     2643 2023-06-05 01:24:04.286203 django_allianceutils-3.0.0/src/allianceutils/middleware/query_count.py
+-rw-r--r--   0        0        0     1705 2023-06-05 01:24:04.286378 django_allianceutils-3.0.0/src/allianceutils/migrations.py
+-rw-r--r--   0        0        0    11164 2023-06-05 01:24:04.286743 django_allianceutils-3.0.0/src/allianceutils/models.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:58:45.063336 django_allianceutils-3.0.0/src/allianceutils/py.typed
+-rw-r--r--   0        0        0     1325 2023-06-05 01:24:04.286949 django_allianceutils-3.0.0/src/allianceutils/rules.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:24:04.287065 django_allianceutils-3.0.0/src/allianceutils/serializers/__init__.py
+-rw-r--r--   0        0        0      640 2023-06-05 01:24:04.287268 django_allianceutils-3.0.0/src/allianceutils/serializers/json_ordered.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:24:04.287375 django_allianceutils-3.0.0/src/allianceutils/templatetags/__init__.py
+-rw-r--r--   0        0        0     2054 2023-06-05 01:24:04.287568 django_allianceutils-3.0.0/src/allianceutils/templatetags/alliance_webpack.py
+-rw-r--r--   0        0        0     1345 2023-06-05 01:24:04.287736 django_allianceutils-3.0.0/src/allianceutils/templatetags/default_value.py
+-rw-r--r--   0        0        0     2217 2023-06-05 01:24:04.287963 django_allianceutils-3.0.0/src/allianceutils/util/__init__.py
+-rw-r--r--   0        0        0     9530 2023-06-05 01:24:04.288588 django_allianceutils-3.0.0/src/allianceutils/util/camel_case.py
+-rw-r--r--   0        0        0     1238 2023-06-05 01:24:04.288782 django_allianceutils-3.0.0/src/allianceutils/util/date.py
+-rw-r--r--   0        0        0     1278 2023-06-08 00:33:28.380905 django_allianceutils-3.0.0/src/allianceutils/util/get_firstparty_apps.py
+-rw-r--r--   0        0        0        0 2023-06-05 01:24:04.289603 django_allianceutils-3.0.0/src/allianceutils/views/__init__.py
+-rw-r--r--   0        0        0      788 2023-06-05 01:24:04.289806 django_allianceutils-3.0.0/src/allianceutils/views/decorators.py
+-rw-r--r--   0        0        0     7186 2023-06-05 01:24:04.290003 django_allianceutils-3.0.0/src/allianceutils/webpack.py
+-rw-r--r--   0        0        0    40536 1970-01-01 00:00:00.000000 django_allianceutils-3.0.0/PKG-INFO
```

### Comparing `django-allianceutils-2.2.0/LICENSE` & `django_allianceutils-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-allianceutils-2.2.0/README.md` & `django_allianceutils-3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 A collection of utilities for django projects from [Alliance Software](https://www.alliancesoftware.com.au/).
 
 * [Installation](#installation)
 * [Usage](#usage)
     * [API](#api)
     * [Auth](#auth)
     * [Decorators](#decorators)
-    * [Filters](#filters)
     * [Management](#management)
         * [Commands](#commands)
         * [Checks](#checks)
     * [Middleware](#middleware)
     * [Migrations](#migrations)
     * [Models](#models)
     * [Rules](#rules)
@@ -24,17 +23,17 @@
 
 ## Installation
 
 `pip install django-allianceutils`
 
 ## System Requirements
 
-* Tested with django 2.2 and 3.2
+* Tested with django 3.2 and 4.2
   * Pull requests accepted for other versions, but at minimum we test against current LTS versions
-* Python >=3.6 (no python 3.5 support)
+* Python >=3.8
 
 ## Usage
 
 ### API
 
 #### Mixins
 
@@ -226,24 +225,25 @@
     * Replaces the built-in django [ModelBackend](https://docs.djangoproject.com/en/stable/ref/contrib/auth/#django.contrib.auth.backends.ModelBackend)
     * Provides django model-based authentication
     * Removes the default authorization (permissions checks) except for checking `is_superuser` 
 
 #### ProfileModelBackend
 
 * Backends for use with [GenericUserProfile](#GenericUserProfile); see code examples there
-* `allianceutils.auth.backends.ProfileModelBackendMixin` - in combo with [AuthenticationMiddleware](https://docs.djangoproject.com/en/stable/ref/middleware/#django.contrib.auth.middleware.AuthenticationMiddleware) will set user profiles on `request.user`  
-    * ~`allianceutils.auth.backends.ProfileModelBackend`~ - convenience class combined with case insensitive username & default django permissions backend
-        * this depended on [`authtools`](https://django-authtools.readthedocs.io/en/latest/) which appears to have been
-          abandoned and does not work with django >= 3.
-          If using django 3 then we recommended that you create your own backend in your app:
-          ```python
-            class ProfileModelBackend(ProfileModelBackendMixin, MinimalModelBackend):
-                # you'll need to implement case insensitivity either here or in the User Model  
-                pass
-          ```
+* `allianceutils.auth.backends.ProfileModelBackendMixin` - in combo with [AuthenticationMiddleware](https://docs.djangoproject.com/en/stable/ref/middleware/#django.contrib.auth.middleware.AuthenticationMiddleware) will set user profiles on `request.user`
+  * If you want  
+      * ~`allianceutils.auth.backends.ProfileModelBackend`~ - convenience class combined with case insensitive username & default django permissions backend
+          * this depended on [`authtools`](https://django-authtools.readthedocs.io/en/latest/) which appears to have been
+            abandoned and does not work with django >= 3.
+            If using django 3 then we recommended that you create your own backend in your app:
+            ```python
+              class ProfileModelBackend(ProfileModelBackendMixin, MinimalModelBackend):
+                  # you'll need to implement case insensitivity either here or in the User Model  
+                  pass
+            ```
 
 ### Decorators
 
 #### gzip_page_ajax
 
 * Smarter version of django's [gzip_page](https://docs.djangoproject.com/en/stable/topics/http/decorators/#django.views.decorators.gzip.gzip_page):
     * If settings.DEBUG not set, will always gzip
@@ -262,17 +262,20 @@
     return django.http.JsonResponse(data) 
 
 ```
 
 #### method_cache
 
 * Caches the results of a method on the object instance
+* There is no thread synchronization so in some circumstances the method may be called multiple times if multiple threads share the object 
 * Only works for regular object methods with no arguments other than `self`.
     * Does not support `@classmethod` or `@staticmethod`
-    * If you want more powerful caching behaviour then you can wrap `cachetools` (examples [here](https://github.com/tkem/cachetools/issues/107))
+    * If you want more powerful caching behaviour then you can
+      * use [`methodtools`](https://pypi.org/project/methodtools/)
+      * wrap `cachetools` (examples [here](https://github.com/tkem/cachetools/issues/107#issuecomment-436274285))
 * Similar to [`@cached_property`](https://docs.python.org/3/library/functools.html#functools.cached_property) except that it works on methods instead of properties
 * Differs from [`@lru_cache()`](https://docs.python.org/3/library/functools.html#functools.lru_cache) in that
     * `lru_cache` uses a single cache for each decorated function
     * `lru_cache` will block garbage collection of values in the cache 
     * A `cache_clear()` method is attached to the function but unlike `lru_cache` it is scoped to an object instance   
 
 Usage
@@ -286,30 +289,14 @@
         return super().get_object()
 
 obj = MyViewSet()
 obj.get_object() is obj.get_object()
 obj.get_object.cache_clear()   
 ```
 
-### Filters
-
-#### MultipleFieldCharFilter
-
-Search for a string across multiple fields. Requires `django_filters`.
-
-* Usage 
-
-```python
-from allianceutils.filters import MultipleFieldCharFilter
-
-# ...
-# In your filter set (see django_filters for documentation)
-customer = MultipleFieldCharFilter(names=('customer__first_name', 'customer__last_name'), lookup_expr='icontains')
-```
-
 ### Management
 
 #### Commands
 
 ##### OptionalAppCommand
 
 * A utility class that extends `django.core.management.base.BaseCommand` and adds optional argument(s) for django apps
@@ -458,17 +445,19 @@
     * Uses the `warnings` module to raise a warning; by default this is suppressed by django
         * To ensure `QueryCountWarning` is never suppressed  
 
 ```python
 warnings.simplefilter('always', allianceutils.middleware.QueryCountWarning)
 ```
 
-* To increase the query count limit for a given request, you can increase `request.QUERY_COUNT_WARNING_THRESHOLD`
-    * Rather than hardcode a new limit, you should increment the existing value
-    * If `request.QUERY_COUNT_WARNING_THRESHOLD` is falsy then checks are disabled for this request 
+* To increase the query count limit for one request, you can call `QueryCountMiddleware.increase_threshold(request, increment)` 
+* To set the query count limit for one request you can call `QueryCountMiddleware.set_threshold(request, threshold)`
+  * Rather than hardcode a new limit, `increase_threshold()` is generally preferable
+  * This can be useful to disable checks entirely (pass `0` as the new limit)
+
 
 ```python
 def my_view(request, *args, **kwargs):
     request.QUERY_COUNT_WARNING_THRESHOLD += 10
     ...
 
 ```
@@ -530,18 +519,15 @@
     
     # these are the tables that should be select_related()/prefetch_related()
     # to minimise queries
     related_profile_tables = [
         'customerprofile',
         'adminprofile',
     ]
-
-    def natural_key(self):
-        return (self.email,)
-        
+    
     # the default implementation will iterate through the related profile tables
     # and return the first profile it can find. If you have custom logic for
     # choosing the profile for a user then you can do that here
     #
     # You would normally not access this directly but instead use the`.profile`
     # property that caches the return value of `get_profile()` and works
     # correctly for both user and profile records  
@@ -913,14 +899,22 @@
 
 ## Changelog
 
 See [CHANGELOG.md](CHANGELOG.md)
 
 ## Development
 
+* To create a clean local environment
+  * `python3 -m venv venv && source venv/bin/activate && pip install --upgrade pip` 
+  * `poetry install --no-root --sync --only=main --extras=""`
+  * Note that due to [a poetry bug](https://github.com/python-poetry/poetry/issues/7364) extras are currently not removed
+  * This will install the latest django version; if you want to test a specific django version you need to `pip install` it manually 
+* Dev dependencies
+  * `poetry install --no-root --sync --with=dev --extras "extras mysql postgres"`
+
 ### Release Process
 
 #### Poetry Config
 * Add test repository
     * `poetry config repositories.testpypi https://test.pypi.org/legacy/`
     * Generate an account API token at https://test.pypi.org/manage/account/token/
     * `poetry config pypi-token.testpypi ${TOKEN}`
@@ -939,7 +933,37 @@
         * `git push --tags`
     * To publish to test.pypi.org
         * `poetry publish --repository testpypi`
     * To publish to pypi.org
         * `poetry publish`
 
 
+### Testing
+* To run test cases
+  * The django settings module is `test_allianceutils/settings.py`
+    * The following env vars are optional but you may want to set them if the default don't match your local setup: 
+      * `DB_NAME`
+      * `DB_HOST`
+      * `DB_PORT`
+      * `DB_USER`
+      * `DB_PASSWORD`
+* [tox](https://tox.wiki/en/latest/)
+  * used to run tests against different django/python/database versions
+  * `tox` to run all tests. Will require that you have a postgres & mysql server running.
+    * `tox -f django42` will run the subset of tests that cover django 4.2. Check `tox.ini` for the list of tested environments. 
+* When you push to github a [github Actions](https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python) workflow will be triggered (see `.github/workflows/django.yml`)  
+
+
+
+TODO:
+- [x] mypy checks all pass
+- [x] github actions pass
+- [] stricter mypy settings?
+- [] flake8, black, isort
+- [x] can cachetools replace @method_cache?
+  - No; can use methodtools but is another dependency. just documented the alternative 
+- [x] Use collections.abc:
+  - no, doesn't work with 3.8
+- [x] Use | instead of Optional, Union
+  - no, doesn't work with 3.8
+- [] Remove legacy build settings (poetry shouldn't need setup.cfg, MANIFEST.in so can we remove them?)
+
```

### Comparing `django-allianceutils-2.2.0/allianceutils/api/mixins.py` & `django_allianceutils-3.0.0/src/allianceutils/api/mixins.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,31 @@
+from __future__ import annotations
+
 from typing import Collection
+from typing import Protocol
+from typing import TYPE_CHECKING
+
+from django.db.models import Field as ModelField
+from django.db.models.options import Options
+from rest_framework.fields import Field
+from rest_framework.serializers import ModelSerializer
+
+if TYPE_CHECKING:
+    # ModelSerializer.Meta is only available in DRF stubs
+    class DRFSerializerProtocol(Protocol):
+        Meta: ModelSerializer.Meta
+        fields: dict[str, Field]
+
+        # this is provided by SerializerOptInFieldsMixin
+        def get_pinned_fields(self: DRFSerializerProtocol) -> Collection[str]:
+            ...
+
+else:
+    class DRFSerializerProtocol:
+        pass
 
 
 class SerializerOptInFieldsMixin:
     """
     Regulates fields exposed by default & as requested based on query parameters or context.
 
     Pass 'include_fields' / 'opt_in_fields' thru query params or context to use.
@@ -16,31 +39,35 @@
     1. By default, all "fields" defined in serializer, minus those listed in "opt_in_fields" would be returned.
     2. If "include_fields" is supplied, only fields requested this way would be returned.
     3. If "opt_in_fields" is supplied, fields requested this way PLUS fields from #1 or #2 would be returned.
 
     Pinned fields are always returned. (currently pk only if pk exists)
     """
 
-    def get_pinned_fields(self) -> Collection[str]:
+    def get_pinned_fields(self: DRFSerializerProtocol) -> Collection[str]:
         """
         Get by-default pinned fields. Pinned fields are fields always returned regardless of include_fields inclusions.
         Override on serializer to customize.
 
         Currently, the only pinned field is pk of model (with ModelSerializer).
 
         :return: [] - a list of pinned fields.
         """
 
         try:
-            return [self.Meta.model._meta.pk.name]
+            model = self.Meta.model
+            meta: Options = model._meta  # type:ignore[attr-defined]  # _meta is not included in stubs
+            assert meta.pk is not None
+            pk: ModelField = meta.pk
+            return [pk.name]
         except AttributeError:
             pass
         return []
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self: DRFSerializerProtocol, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         if not hasattr(self, "context"):
             # serializer invoked without context - inspection?
             return
 
         pinned_fields = self.get_pinned_fields()
@@ -56,15 +83,15 @@
             or ("include_fields" in self.context and self.context["include_fields"])
             or set(self.Meta.fields).difference(set(fields_to_exclude))
         )
 
         if isinstance(fields_to_include, str):
             fields_to_include = [fields_to_include]
 
-        fields_to_include_list = []
+        fields_to_include_list: list[str] = []
         for f in fields_to_include:
             if f.find(",") != -1:
                 fields_to_include_list += f.split(",")
             else:
                 fields_to_include_list.append(f)
 
         opt_in_fields_to_include = (
```

### Comparing `django-allianceutils-2.2.0/allianceutils/api/parsers.py` & `django_allianceutils-3.0.0/src/allianceutils/api/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,12 +114,11 @@
                     if type(v) == str and v.startswith("____ATTACHED_FILE_ID_"):
                         final_v = data_and_files.files.get(v)
                     else:
                         final_v = v
                     transformed_values.append((k, final_v))
                 return dict(transformed_values)
 
-            json_data = json.loads(
-                data_and_files.data.get("jsonData"), object_pairs_hook=hook
-            )
+            json_data_str = data_and_files.data["jsonData"]
+            json_data = json.loads(json_data_str, object_pairs_hook=hook)
             return self.underscoreize(json_data)
-        return super().parse(stream, media_type, parser_context)
+        return data_and_files
```

### Comparing `django-allianceutils-2.2.0/allianceutils/api/permissions.py` & `django_allianceutils-3.0.0/src/allianceutils/api/permissions.py`

 * *Files identical despite different names*

### Comparing `django-allianceutils-2.2.0/allianceutils/api/renderers.py` & `django_allianceutils-3.0.0/src/allianceutils/api/renderers.py`

 * *Files identical despite different names*

### Comparing `django-allianceutils-2.2.0/allianceutils/auth/backends.py` & `django_allianceutils-3.0.0/src/allianceutils/auth/backends.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,49 @@
+from __future__ import annotations
+
+from typing import cast
 from typing import Optional
+from typing import Protocol
 
 from django.contrib.auth import get_user_model
 from django.contrib.auth.backends import ModelBackend
 from django.db.models import Model
 
+from allianceutils.auth.models import GenericUserProfile
+
 
-def resolve_rule_name(module, entity, action, is_global) -> str:
+def resolve_perm_name(module, entity, action, is_global) -> str:
     """
     Used by csv_permissions to calculate rule names for each row
     """
     return f"{module}.{entity}_{action}"
 
 
 UserModel = get_user_model()
 
 
+class _BaseUserModelBackend(Protocol):
+    def get_user(self, user_id):
+        ...
+
+    def user_can_authenticate(self, user: Model):
+        ...
+
+
+class _BaseUserModel(Protocol):
+    is_superuser: bool
+
+
 class ProfileModelBackendMixin:
     """
     Backend that provides authentication using User.profiles & get_profile().
     Will fall back to default get_user() behaviour if no profiles manager available
     """
 
-    def get_user(self, user_id):
+    def get_user(self: _BaseUserModelBackend, user_id) -> GenericUserProfile | None:
         try:
             manager = UserModel.profiles
         except AttributeError:
             return super().get_user(user_id)
 
         try:
             user = manager.get(pk=user_id)
@@ -44,31 +62,14 @@
     want to exclude entirely
     """
 
     authenticate = ModelBackend.authenticate
     get_user = ModelBackend.get_user
     user_can_authenticate = ModelBackend.user_can_authenticate
 
-    def has_perm(self, user: Model, perm: str, obj: Optional[Model] = None) -> bool:
+    def has_perm(self, user: _BaseUserModel, perm: str, obj: Optional[Model] = None) -> bool:
         """
         We defer to other backends for the real logic
         """
         if user.is_superuser:
             return True
-        return False
-
-
-try:
-    from authtools.backends import CaseInsensitiveUsernameFieldBackendMixin
-except ImportError:
-    # no authtools present
-    #
-    # we could just remove CaseInsensitiveUsernameFieldBackendMixin from ProfileModelBackend but that
-    # would mean devs who do an upgrade without reading the release notes would not notice that behaviour
-    # had changed and would get unexpected silent failures. Is safer to remove this to force them to
-    # deal with the issue
-    pass
-else:
-    class ProfileModelBackend(
-        ProfileModelBackendMixin, CaseInsensitiveUsernameFieldBackendMixin, MinimalModelBackend
-    ):
-        pass
+        return False
```

### Comparing `django-allianceutils-2.2.0/allianceutils/auth/models.py` & `django_allianceutils-3.0.0/src/allianceutils/auth/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,40 @@
+from __future__ import annotations
+
+from typing import cast
 from typing import Iterable
-from typing import Optional
 from typing import Type
-from typing import Union
+from typing import TYPE_CHECKING
+from typing import TypeVar
 
 from django.contrib.auth.models import BaseUserManager
 from django.contrib.auth.models import UserManager
 from django.core import checks
 from django.core.exceptions import ValidationError
-from django.db.models import Manager
+from django.db.models import EmailField
+from django.db.models import Field
 from django.db.models import Model
 from django.db.models import QuerySet
 from django.db.models.query import ModelIterable
+from typing_extensions import Self
 
+from allianceutils import ModelProtocol
 from allianceutils.checks import ID_ERROR_PROFILE_RELATED_TABLES
 
+_ModelT = TypeVar("_ModelT", bound=Model, covariant=True)
+
 
 class GenericUserProfileIterable(ModelIterable):
     """
     The iterator that transforms user records into profiles
     """
-    def __iter__(self) -> Iterable[Model]:
+
+    queryset: GenericUserProfileQuerySet  # this is coupled to this QuerySet
+
+    def __iter__(self) -> Iterable[GenericUserProfile | _ModelT]:  # type:ignore[override]  # specialised return
         if self.queryset._do_iterate_profiles:
             for user in super().__iter__():
                 yield user.profile
         else:
             yield from super().__iter__()
 
 
@@ -35,32 +46,32 @@
     def __init__(self, *args, **kwargs):
         # We can't pass through _do_iterate_profiles as a constructor argument because QuerySet creation is hardcoded
         # in multiple places in BaseManager [eg _clone()]
         super().__init__(*args, **kwargs)
         self._do_iterate_profiles = False
         self._iterable_class = GenericUserProfileIterable
 
-    def profiles(self) -> QuerySet:
+    def profiles(self) -> Self:
         """
         Return a queryset that when iterated will yield User profiles instead of User records
         """
         qs = self.all()
         qs._do_iterate_profiles = True
         qs._validate_iterator()
         return qs
 
-    def values(self, *args, **kwargs) -> QuerySet:
+    def values(self, *args, **kwargs) -> Self:
         # We want to fail early if needed rather than when the iterator is created (easier to debug)
-        qs = super().values(*args, **kwargs)
+        qs = cast(Self, super().values(*args, **kwargs))
         qs._validate_iterator()
         return qs
 
-    def values_list(self, *args, **kwargs) -> QuerySet:
+    def values_list(self, *args, **kwargs) -> Self:
         # We want to fail early if needed rather than when the iterator is created (easier to debug)
-        qs = super().values_list(*args, **kwargs)
+        qs = cast(Self, super().values_list(*args, **kwargs))
         qs._validate_iterator()
         return qs
 
     def _validate_iterator(self):
         """
         We shouldn't use values() and values_list() in conjunction with profiles()
 
@@ -72,34 +83,37 @@
         This is not a hard restriction and is only intended to catch developer mistakes; this constraint may
         be relaxed in future when the need arises.
         """
         if self._do_iterate_profiles and not issubclass(self._iterable_class, GenericUserProfileIterable):
             raise ValueError('Bad _iterable_class. (Trying to use values()/values_list() with profiles()? This has not been implemented yet)')
 
     def _clone(self, **kwargs):
-        qs = super()._clone(**kwargs)
+        qs = super()._clone(**kwargs)  # type:ignore[misc]  # not in django stubs
         qs._do_iterate_profiles = self._do_iterate_profiles
         return qs
 
-    def _get_related_profile_tables(self):
+    def _get_related_profile_tables(self) -> list[str]:
+        """
+        See GenericUserProfile.related_profile_tables
+        """
         if _is_profile(self.model):
             return []
         else:
             return self.model.related_profile_tables
 
-    def select_related_profiles(self) -> QuerySet:
+    def select_related_profiles(self) -> Self:
         """
         Adds relevant select_related() joins so that user_to_profile() doesn't trigger extra queries
         """
         if _is_profile(self.model):
             # is already a profile table so no need to do any joins
             return self._clone()
         return self.select_related(*self.model.related_profile_tables)
 
-    def prefetch_related_profiles(self) -> QuerySet:
+    def prefetch_related_profiles(self) -> Self:
         """
         Adds relevant select_related() joins so that user_to_profile() doesn't trigger extra queries
         """
         if _is_profile(self.model):
             # is already a profile table so no need to do any joins
             return self._clone()
         return self.prefetch_related(*self.model.related_profile_tables)
@@ -130,20 +144,30 @@
     # print('validating %s.%s' % (app_name, model_name))
     if not getattr(model, 'related_profile_tables', None):
         msg = f'A model with a GenericUserProfileManagerMixin ({model.__name__}.{manager_name}) ' \
               'is missing a related_profile_tables definition'
         raise NotImplementedError(msg)
 
 
+_ManagerQuerySet = TypeVar("_ManagerQuerySet", covariant=True)
+
+
 class GenericUserProfileManagerMixin(BaseUserManager):
     """
     Manager mixin that provides for iteration over user profiles.
     Is assumed to be a manager for a GenericUserProfile
     """
-    _queryset_class = GenericUserProfileQuerySet
+
+    # if you change this you may also want to narrow the types of some methods;
+    # I can't find a way to explain to mypy that this can be overridden
+    _queryset_class: type[GenericUserProfileQuerySet] = GenericUserProfileQuerySet
+    _auto_select_related_profiles: bool
+    _auto_prefetch_related_profiles: bool
+
+    model: type[GenericUserProfile] # type:ignore[assignment] # narrow from parent definition
 
     def __init__(self, select_related_profiles=False, prefetch_related_profiles=False, *args, **kwargs):
         """
         Constructor; allows you to create a manager that will iterate over profiles by default
 
         :param select_related_profiles: If set, will automatically call select_related_profiles() and profiles() on every queryset
         :param prefetch_related_profiles: If set, will automatically prefetch_related_profiles() and profiles() on every queryset
@@ -153,27 +177,27 @@
 
         if self._auto_select_related_profiles and self._auto_prefetch_related_profiles:
             # If you do this you probably messed up (is redundant and inefficient)
             raise ValueError('Both prefetching and selecting related entities is usually a mistake')
 
         super().__init__(*args, **kwargs)
 
-    def get_queryset(self) -> QuerySet:
+    def get_queryset(self) -> GenericUserProfileQuerySet:
         qs = super().get_queryset()
         if not isinstance(qs, GenericUserProfileQuerySet):
             raise TypeError('GenericUserProfileManagerMixin QuerySet does not inherit GenericUserProfileQuerySet')
         if self._auto_select_related_profiles:
             qs = qs.select_related_profiles()
         if self._auto_prefetch_related_profiles:
             qs = qs.prefetch_related_profiles()
         if self._auto_prefetch_related_profiles or self._auto_select_related_profiles:
             qs = qs.profiles()
         return qs
 
-    def contribute_to_class(self, model: Model, name):
+    def contribute_to_class(self, model: type[Model], name):
         # Do some extra sanity checks on the model
         #
         # We could extend the underlying queryset class and mix in GenericUserProfileQuerySet automatically here
         # but that involves extra hidden magic which is anti-pythonic
 
         # If get_queryset() does something other than instantiating _queryset_class then this may be a false positive
         # but that's a case we haven't had to handle yet
@@ -182,52 +206,62 @@
 
         super(GenericUserProfileManagerMixin, self).contribute_to_class(model, name)
 
     def check(self, **kwargs):
         errors = super().check(**kwargs)
 
         model = self.model
-        if getattr(model, 'related_profile_tables') is None:
+        if not hasattr(model, 'related_profile_tables'):
             errors.append(checks.Error(
                 f"Model '{model._meta.label}' does not define related_profile_tables",
                 hint=f"Manager '{self.name}' needs related_profile_tables",
                 obj=self.model,
                 id=ID_ERROR_PROFILE_RELATED_TABLES,
             ))
 
         return errors
 
-    def profiles(self) -> QuerySet:
+    def profiles(self) -> GenericUserProfileQuerySet:
         return self.get_queryset().profiles()
 
     # TODO: It would be nice to be able to do something like:
     #   SomeModel.objects.select_related('user__profile')
     # and have the '__profile' transformed into the relevant select_related() based on model.related_profile_tables
     # unfortunately the code to do the joins is baked into SQLCompiler.get_related_selections() and is not really
     # extensible without being very invasive
     #
     # Instead we have to call select_related_profiles on an unrelated queryset with a prefix
 
-    def select_related_profiles(self, queryset: Optional[Union[QuerySet, Manager]]=None, prefix: str='') -> QuerySet:
+    def select_related_profiles(
+        self,
+        queryset: GenericUserProfileQuerySet | GenericUserProfileManagerMixin | None = None,
+        prefix: str = ""
+    ) -> GenericUserProfileQuerySet:
         if bool(queryset) != bool(prefix):
             raise ValueError('Either none or both of queryset and prefix must be specified')
 
-        if not queryset and not prefix:
+        if queryset is None:
             return self.get_queryset().select_related_profiles()
         else:
-            return queryset.select_related(*[prefix + '__' + profile for profile in self.model.related_profile_tables])
+            filters = [prefix + '__' + profile for profile in self.model.related_profile_tables]
+            return cast(GenericUserProfileQuerySet, queryset.select_related(*filters))
 
-    def prefetch_related_profiles(self, queryset: Optional[Union[QuerySet, Manager]]=None, prefix: str='') -> QuerySet:
+    def prefetch_related_profiles(
+        self,
+        queryset: GenericUserProfileQuerySet | GenericUserProfileManagerMixin | None = None,
+        prefix: str = ""
+    ) -> GenericUserProfileQuerySet:
         if bool(queryset) != bool(prefix):
             raise ValueError('Either none or both of queryset and prefix must be specified')
 
-        if not queryset and not prefix:
+        if queryset is None:
             return self.get_queryset().prefetch_related_profiles()
         else:
-            return queryset.prefetch_related(*[prefix + '__' + profile for profile in self.model.related_profile_tables])
+            filters = [prefix + '__' + profile for profile in self.model.related_profile_tables]
+            return cast(GenericUserProfileQuerySet, queryset.prefetch_related(*filters))
 
 
 class GenericUserProfileManager(GenericUserProfileManagerMixin, UserManager):
     """
     Default User Profile Manager using django.contrib.auth.models.UserManager
     """
     pass
@@ -237,32 +271,24 @@
     """
     A User model that provides iteration over user profiles (if available)
     You should override related_profile_tables
     """
     objects = GenericUserProfileManager()
     profiles = GenericUserProfileManager(select_related_profiles=True)
 
+    # This should be overridden to include a list of the FKs to the tables
+    # to join to in order to fetch profiles [will be passed to select_related()]
+    related_profile_tables: list[str]
+
     class Meta:
         abstract = True
 
-    @classmethod
-    def normalize_email(cls, email: str) -> str:
-        return email.lower()
-
-    def clean(self):
-        if self.__class__._base_manager.filter(email=self.normalize_email(self.email)).exclude(pk=self.pk).exists():
-            raise ValidationError({'email': 'Sorry, this email address is not available.'})
-
-    def save(self, *args, **kwargs):
-        self.email = self.normalize_email(self.email)
-        return super().save(*args, **kwargs)
-
-    def get_profile(self) -> Model:
+    def get_profile(self) -> Self:
         # We're already a profile
-        if _is_profile(self):
+        if _is_profile(type(self)):
             return self
 
         # try each FK reference one at a time; this will be inefficient if
         # select_related_profiles() or prefetch_related_profiles() haven't been called
         for profile_model in self.related_profile_tables:
             try:
                 return getattr(self, profile_model)
@@ -273,27 +299,35 @@
         return self
 
     class _CachedProfileDescriptor:
         """
         Evaluates and caches the result of get_profile()
         Caches the result on all records in the multi-table inheritance chain
         """
-        def __get__(self, obj, cls=None) -> Optional[Model]:
+        def __get__(
+            self,
+            obj: GenericUserProfile | None,
+            cls: type[GenericUserProfile] | None = None
+        ) -> Self | GenericUserProfile:
             if obj is None:
+                # class invocation
                 return self
 
             user_profile = obj.get_profile()
 
             # cache the result on all records in the multi-table inheritance chain
-            record = user_profile
+            record: GenericUserProfile | None = user_profile
             while isinstance(record, Model):
                 record.__dict__['profile'] = user_profile
 
                 # note that record.pk will always return the underlying pk id, not the user_ptr record
-                record = getattr(record, record._meta.pk.name)
+                # so we have to access it via the pk field's name and not the 'pk' alias
+                pk = cast(Field, record._meta.pk)
+                record = getattr(record, pk.name)
 
             return user_profile
 
-    profile = _CachedProfileDescriptor()
-
-    # This should be overridden to include a list of the tables to join to [will be passed to select_related()]
-    related_profile_tables = None
+    # This isn't strictly the correct type; because this is a descriptor if you access this as a class property
+    # (ie ClassName.profile) then you'll get the descriptor itself rather than the profile.
+    # The overwhelming majority of the time you'll be accessing this via an instance (my_obj.profile) and want the
+    # GenericUserProfile instance, so we type it for convenience rather than 100% accuracy
+    profile: Self = cast(Self, _CachedProfileDescriptor())
```

### Comparing `django-allianceutils-2.2.0/allianceutils/bin/internaldeps.sh` & `django_allianceutils-3.0.0/src/allianceutils/bin/internaldeps.sh`

 * *Files identical despite different names*

### Comparing `django-allianceutils-2.2.0/allianceutils/checks.py` & `django_allianceutils-3.0.0/src/allianceutils/checks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from __future__ import annotations
+
 import ast
 from collections import defaultdict
 import inspect
 from pathlib import Path
 import re
 import subprocess
-from typing import Dict
+from typing import cast
+from typing import Collection
 from typing import Iterable
 from typing import List
 from typing import Mapping
 from typing import Optional
 from typing import Type
 from typing import Union
 
@@ -27,171 +30,158 @@
 from allianceutils.util import get_firstparty_apps
 from allianceutils.util import underscore_to_camel
 
 # W001 not used
 # W002 not used
 # W003 not used
 ID_ERROR_PROFILE_RELATED_TABLES = 'allianceutils.E001'
-ID_ERROR_DB_CONSTRAINTS = 'allianceutils.E002'
+#ID_ERROR_DB_CONSTRAINTS = 'allianceutils.E002'
 ID_ERROR_ADMINS = 'allianceutils.E003'
 ID_WARNING_TRAILING_SLASH = 'allianceutils.W004'
 #ID_WARNING_AUTODUMP_MISSING = 'allianceutils.W005'
 #ID_WARNING_AUTODUMP_PROXY = 'allianceutils.W006'
 ID_WARNING_GIT = 'allianceutils.W007'
 ID_WARNING_GIT_HOOKS = 'allianceutils.W008'
 ID_ERROR_GIT_HOOKS = 'allianceutils.E008'
 ID_ERROR_EXPLICIT_TABLE_NAME = 'allianceutils.E009'
 ID_ERROR_EXPLICIT_TABLE_NAME_LOWERCASE = 'allianceutils.E010'
 ID_INFO_EXPLICIT_TABLE_NAME_LOWERCASE = 'allianceutils.I010'
 ID_ERROR_FIELD_NAME_NOT_CAMEL_FRIENDLY = 'allianceutils.E011'
 
-try:
-    Pattern = re.Pattern
-except AttributeError:
-    # Until python 3.7 re.Pattern was not exposed (was only present internally as _pattern_type)
-    Pattern = object
-
 
 def find_candidate_models(
     app_configs: Optional[Iterable[AppConfig]],
-    ignore_labels: Iterable[Union[str, Pattern]] = None
-) -> Dict[str, Type[Model]]:
+    ignore_labels: Optional[Iterable[Union[str, re.Pattern]]] = None
+) -> dict[str, Type[Model]]:
     """
     Given a list of labels to ignore, return models whose app_label or label is NOT in ignore_labels.
     :return: dict which is a mapping of candidate models in the format of { model_label: Model }
     """
     if app_configs is None:
         app_configs = get_firstparty_apps()
 
     if ignore_labels is None:
         ignore_labels = []
 
     def should_ignore(label: str) -> bool:
+        assert ignore_labels is not None
         return (
             # string match
             any(s == label for s in ignore_labels) or
             # regex pattern match
             any(p.match(label) for p in ignore_labels if hasattr(p, "match"))
         )
 
-    candidate_models: Dict[str, Type[Model]] = {}
+    candidate_models: dict[str, Type[Model]] = {}
 
     for app_config in app_configs:
         candidate_models.update({
             model._meta.label: model
             for model
             in app_config.get_models()
             if not should_ignore(model._meta.app_label) and not should_ignore(model._meta.label)
         })
 
     return candidate_models
 
 
 class CheckUrlTrailingSlash:
     expect_trailing_slash: bool
-    ignore_attrs: Mapping[str, Iterable[str]]
+    ignore_attrs: dict[str, Collection[str]]
 
-    def __init__(self, expect_trailing_slash: bool, ignore_attrs: Mapping[str, Iterable[str]] = {}):
+    def __init__(self, expect_trailing_slash: bool, ignore_attrs: Mapping[str, Collection[str]] = {}):
         self.expect_trailing_slash = expect_trailing_slash
-        self.ignore_attrs = ignore_attrs
+        self.ignore_attrs = dict(ignore_attrs.items())
 
-    def __call__(self, app_configs: Iterable[AppConfig], **kwargs) -> List[CheckMessage]:
+    def __call__(self, app_configs: Iterable[AppConfig], **kwargs) -> list[CheckMessage]:
         # We ignore app_configs; so does django core check_url_settings()
         # Consider where ROOT_URLCONF points app A urlpatterns which include() app B urlpatterns
         # which define a URL to view in app C -- which app was the one that owned the URL?
-        _ignore_attrs = {
+        _ignore_attrs: dict[str, Collection[str]] = {
             '_regex': [
                 '^$',
             ],
             'lookup_str': [
                 'django.views.static.serve',
             ],
             'app_name': [
                 'admin',
                 'djdt',
             ],
         }
         _ignore_attrs.update(self.ignore_attrs)
 
-        def check_resolver(resolver: URLResolver, depth: int = 0) -> List[CheckMessage]:
+        def check_resolver(resolver: URLResolver, depth: int = 0) -> list[CheckMessage]:
             messages = []
             for url_pattern in resolver.url_patterns:
 
-                # look
                 if any(
-                        getattr(url_pattern, attr, None) in vals or getattr(getattr(url_pattern, 'pattern', {}), attr, None) in vals
-                        for attr, vals
-                        in _ignore_attrs.items()):
+                    getattr(url_pattern, attr, None) in vals
+                        or getattr(getattr(url_pattern, 'pattern', {}), attr, None) in vals
+                    for attr, vals
+                    in _ignore_attrs.items()
+                ):
                     continue
 
-                try:
-                    # django 2.0+ simplified urls (stilluses a regex underneath)
-                    regex_pattern = url_pattern.pattern.regex.pattern
-                except AttributeError:
-                    # django <2.0 regex patterns
-                    regex_pattern = url_pattern.regex.pattern
+                regex_pattern = url_pattern.pattern.regex.pattern
 
                 if regex_pattern == r'^\Z' or regex_pattern == '^$':
                     # empty patterns are a special case; they may be nested inside an
                     # include(), if that's the case then we don't really care whether
                     # they do or don't have a slash
                     continue
 
-                if hasattr(url_pattern, 'url_patterns'):
+                if isinstance(url_pattern, URLResolver):
                     # is a resolver, not a pattern: recurse
                     messages.extend(check_resolver(url_pattern, depth+1))
                 elif (regex_pattern.endswith('/$') or regex_pattern.endswith(r'/\Z')) != self.expect_trailing_slash:
-                    try:
-                        # django 2.0+ simplified urls
-                        description = url_pattern.pattern.describe()
-                    except AttributeError:
-                        # django <2.0 regex urls
-                        description = url_pattern.describe()
-
+                    description = url_pattern.pattern.describe()
                     messages.append(
                         Warning(
                             f'The URL pattern {description} is inconsistent with expect_trailing_slash',
                             obj=url_pattern,
                             id=ID_WARNING_TRAILING_SLASH,
                         )
                     )
 
             return messages
 
         return check_resolver(get_resolver())
 
 
 class CheckGitHooks:
-    git_path: Optional[Union[str, Path]] = None
+    git_path: Path
 
     def __init__(self, git_path: Optional[Union[str, Path]] = None):
-        self.git_path = Path(git_path) or get_default_git_path()
+        self.git_path = Path(git_path) if git_path is not None else get_default_git_path()
 
     def __call__(self, app_configs: Iterable[AppConfig], **kwargs):
         return _check_git_hooks(app_configs, self.git_path, **kwargs)
 
 
-def get_default_git_path() -> str:
-    return Path(settings.PROJECT_DIR, '.git')
+def get_default_git_path() -> Path:
+    assert hasattr(settings, "PROJECT_DIR")
+    project_dir = settings.PROJECT_DIR  # type:ignore[misc]  # we already checked that this is present
+    return Path(project_dir, '.git')
 
 
-def check_git_hooks(app_configs: Iterable[AppConfig], **kwargs) -> List[CheckMessage]:
+def check_git_hooks(app_configs: Iterable[AppConfig], **kwargs) -> list[CheckMessage]:
     return _check_git_hooks(app_configs, git_path=get_default_git_path(), **kwargs)
 
 
-def _check_git_hooks(app_configs: Iterable[AppConfig], git_path: Path, **kwargs) -> List[CheckMessage]:
+def _check_git_hooks(app_configs: Iterable[AppConfig], git_path: Path, **kwargs) -> list[CheckMessage]:
 
     # handle the case where .git is a file rather than a directory
     try:
         with git_path.open() as f:
             git_path = Path(f.readline())
     except OSError:
         pass
 
-    messages = []
+    messages: list[CheckMessage] = []
 
     if not git_path.exists():
         if settings.DEBUG:
             # If in dev mode then there should be a .git dir
             messages.append(
                 Warning(
                     "DEBUG is true but can't find a .git dir; are you trying to use DEBUG in production?",
@@ -211,15 +201,17 @@
             ["git", "config", "core.hooksPath"],
             capture_output=True,
             cwd=git_path,
         )
         if not git_config_result.returncode:
             git_hooks_path = Path(git_config_result.stdout.decode('utf-8').strip('\n'))
             if not git_hooks_path.is_absolute():
-                git_hooks_path = Path(settings.PROJECT_DIR) / git_hooks_path
+                assert hasattr(settings, "PROJECT_DIR")
+                project_dir = settings.PROJECT_DIR  # type:ignore[misc]  # we already checked that this is present
+                git_hooks_path = Path(project_dir, git_hooks_path)
 
         precommit = git_hooks_path / 'pre-commit'
 
         found_installed_hooks = False
         if git_hooks_path.is_symlink():
             found_installed_hooks = True
         else:
@@ -244,84 +236,35 @@
                     id=warning_id,
                 )
             )
 
     return messages
 
 
-def check_admins(app_configs: Iterable[AppConfig], **kwargs) -> List[CheckMessage]:
-    messages = []
-    if not settings.AUTOMATED_TESTS and not settings.DEBUG:
+def check_admins(app_configs: Iterable[AppConfig] | None, **kwargs) -> list[CheckMessage]:
+    messages: list[CheckMessage] = []
+    if not getattr(settings, "AUTOMATED_TESTS", False) and not settings.DEBUG:
         if len(settings.ADMINS) == 0:
             messages.append(
                 Error(
                     "settings.ADMINS should not be empty",
                     obj='settings',
                     id=ID_ERROR_ADMINS,
                 )
             )
     return messages
 
 
-def check_db_constraints(app_configs: Iterable[AppConfig], **kwargs) -> List[CheckMessage]:
-    """
-    If using django-db-constraints, constraint identifiers can be supplied
-    that are longer than the max identifier length for Postgres
-    (63 bytes, see https://stackoverflow.com/a/8218026/6653190) or MySQL
-    (64 BMP unicode characters, see https://dev.mysql.com/doc/refman/8.0/en/identifiers.html).
-    Check that any such constraints are globally unique when truncated to the smaller (Postgres) limit.
-    """
-    if app_configs is None:
-        app_configs = apps.app_configs
-    else:
-        app_configs = {app_config.label: app_config for app_config in app_configs}
-
-    NAMEDATALEN = 63
-
-    def _truncate_constraint_name(_name):
-        return _name.encode('utf-8')[:NAMEDATALEN]
-
-    known_constraints = defaultdict(list)
-    for app_config in app_configs.values():
-        for model in app_config.get_models():
-            # native django constraints
-            if hasattr(model._meta, 'constraints'):
-                for constraint in model._meta.constraints:
-                    known_constraints[_truncate_constraint_name(constraint.name)].append((model, constraint.name))
-            # constraints from the django-db-constraints package
-            if hasattr(model._meta, 'db_constraints'):
-                for constraint_name in model._meta.db_constraints.keys():
-                    known_constraints[_truncate_constraint_name(constraint_name)].append((model, constraint_name))
-
-    messages = []
-    for truncated_name, model_constraints in known_constraints.items():
-        if len(model_constraints) == 1:
-            continue
-        _models = [f'{model._meta.app_label}.{model.__name__}' for model, _ in model_constraints]
-        models_string = ', '.join(_models)
-        for _model, constraint_name in model_constraints:
-            messages.append(
-                Error(
-                    f'{_model._meta.label} constraint {constraint_name} is not unique',
-                    hint='Constraint truncates to ' + truncated_name.decode('utf-8', 'replace'),
-                    obj=models_string,
-                    id=ID_ERROR_DB_CONSTRAINTS,
-                )
-            )
-
-    return messages
-
-
-def _check_explicit_table_names_on_model(model: Type[Model], enforce_lowercase: bool) -> List[CheckMessage]:
+def _check_explicit_table_names_on_model(model: Type[Model], enforce_lowercase: bool) -> list[CheckMessage]:
     """
     Use an ast to check if a model has the db_table meta option set.
     This is done this way because a model instance's db_table is always
     populated even if with that of the default.
     """
-    messages = []
+    messages: list[CheckMessage] = []
     found = None
     try:
         source = inspect.getsource(model)
     except OSError:
         # if a model class is dynamically created then we can't inspect the source code
         # (eg this happens with audit models)
         message = f"Can't get source for {model.__name__}"
@@ -334,28 +277,27 @@
         ))
         return messages
     tree = ast.parse(source)
     for node in ast.walk(tree):
         if isinstance(node, ast.ClassDef) and node.name == 'Meta':
             for sub_node in node.body:
                 if isinstance(sub_node, ast.Assign):
-                    if sub_node.targets[0].id == 'db_table':
-                        # in python <=3.7 it will be an ast.Str
-                        # in python >=3.8 it will be an ast.Constant
-                        if isinstance(sub_node.value, (ast.Constant, ast.Str)):
+                    first_target = sub_node.targets[0]
+                    if first_target.id == 'db_table':  # type:ignore[attr-defined] # isn't present in type defs
+                        if isinstance(sub_node.value, ast.Constant):
                             found = sub_node.value.s
                         else:
                             # If it's an expression then we don't know what it's going to evaluate it
                             # so we're just going to assume it's ok
                             found = True
                         break
 
                     # Skip for unmanaged models
                     elif (
-                        sub_node.targets[0].id == 'managed'
+                        first_target.id == 'managed'  # type:ignore[attr-defined] # isn't present in type defs
                         and isinstance(sub_node.value, (ast.Constant))
                         and sub_node.value.s == False
                     ):
                         found = True
                         break
     if not found:
         messages.append(
@@ -385,26 +327,26 @@
 
 
 class CheckExplicitTableNames:
     """
     A check for models with missing or invalid db_table settings
     """
 
-    ignore_labels: Iterable[str]
+    ignore_labels: Iterable[Union[str, re.Pattern]]
     enforce_lowercase: bool
 
-    def __init__(self, ignore_labels: Iterable[Union[str, Pattern]] = DEFAULT_TABLE_NAME_CHECK_IGNORE, enforce_lowercase: bool = True):
+    def __init__(self, ignore_labels: Iterable[Union[str, re.Pattern]] = DEFAULT_TABLE_NAME_CHECK_IGNORE, enforce_lowercase: bool = True):
         """
         ignore_labels: ignore apps or models matching supplied labels
         enforce_lowercase: applies rule E010 which enforces table name to be all lowercase; defaults to True
         """
         self.ignore_labels = ignore_labels
         self.enforce_lowercase = enforce_lowercase
 
-    def __call__(self, app_configs: Iterable[AppConfig], **kwargs) -> List[CheckMessage]:
+    def __call__(self, app_configs: Iterable[AppConfig], **kwargs) -> list[CheckMessage]:
         """
         Warn when models don't have Meta's db_table_name set in apps that require it.
         """
         candidate_models = find_candidate_models(app_configs, self.ignore_labels)
 
         messages = []
         for model in candidate_models.values():
@@ -421,25 +363,25 @@
     def __call__(self, app_configs: Iterable[AppConfig], ** kwargs):
         candidate_models = find_candidate_models(app_configs, self.ignore_labels)
         errors = []
         for model in candidate_models.values():
             errors += self._check_field_names_on_model(model)
         return errors
 
-    def _check_field_names_on_model(self, model: Type[Model]) -> List[CheckMessage]:
+    def _check_field_names_on_model(self, model: Type[Model]) -> list[CheckMessage]:
         """
         check whether field names on model are legit
 
         currently contains only one check:
         1. checks whether field name contains any number preceded by an underscore. the underscore will be lost when
            camelized then de-camelized again. Since camelize is performed automatically to/from frontend it leads to bugs.
 
         """
 
-        messages = []
+        messages: list[CheckMessage] = []
 
         for field in model._meta.fields:
             if camel_to_underscore(underscore_to_camel(field.name)) != field.name:
                 hint = None
                 if re.search(r'_[0-9]', field.name):
                     hint = f'Underscore before a number in {model._meta.label}.{field.name}'
                 messages.append(
```

### Comparing `django-allianceutils-2.2.0/allianceutils/management/commands/base.py` & `django_allianceutils-3.0.0/src/allianceutils/management/commands/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Iterable
+
 from django.apps import AppConfig
 from django.apps import apps
 from django.core.management.base import BaseCommand
 from django.core.management.base import CommandError
 
 from allianceutils.util.get_firstparty_apps import get_firstparty_apps
 
@@ -13,14 +15,15 @@
     supplied it attempts to find all local apps by using isort's method
     of determining if a module is first party or not.
     """
     def add_arguments(self, parser):
         parser.add_argument('args', metavar='app_label', nargs='*')
 
     def handle(self, *app_labels, **options):
+        app_configs: Iterable[AppConfig]
         if len(app_labels) > 0:
             try:
                 app_configs = [
                     apps.get_app_config(app_label)
                     for app_label in app_labels
                 ]
             except (LookupError, ImportError) as e:
```

### Comparing `django-allianceutils-2.2.0/allianceutils/management/commands/document_reverse_accessors.py` & `django_allianceutils-3.0.0/src/allianceutils/management/commands/document_reverse_accessors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+from __future__ import annotations
+
 import ast
 import difflib
 import inspect
 from itertools import groupby
 import re
+from typing import Callable
+from typing import cast
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Type
 
 from django.db.models import Field
 from django.db.models import Model
@@ -31,50 +35,53 @@
         output = self.generate_comments(source_file_model_fields)
 
         if options['preview']:
             self.preview_output(output)
         else:
             self.apply_output(output)
 
-    def determine_fields_by_model_by_file(self, models: Iterable[Type[Model]]) -> Dict[str, Dict[Model, Field]]:
+    def determine_fields_by_model_by_file(self, models: Iterable[type[Model]]) -> Dict[str, Dict[type[Model], list[ForeignObjectRel]]]:
         """
         Takes a list of models and returns the models & fields for each source file
         :param: models[] - look up the source file & fields for these models
         :returns: { source_file: { Model: [ Field ] } }
         """
         related_fields = [
             field
             for model in models
-            for field in model._meta.related_objects
+            for field in model._meta.related_objects  # type:ignore[attr-defined] # related_object exists
         ]
 
+
         model_fields = {
             model: list(model_fields)
             for model, model_fields
             in groupby(sorted(related_fields, key=lambda f: f.model.__name__), key=lambda f: f.model)
         }
 
-        source_file_models = {
+        get_model_source = cast(Callable[[type], str], inspect.getsourcefile)
+        models_sorted_by_source = sorted(model_fields.keys(), key=get_model_source)
+        source_file_models: dict[str, list[type[Model]]] = {
             source_file: list(models)
             for source_file, models
-            in groupby(sorted(model_fields.keys(), key=inspect.getsourcefile), key=inspect.getsourcefile)
+            in groupby(models_sorted_by_source, key=get_model_source)
         }
 
         source_file_model_fields = {
             source_file: {
                 model: model_fields[model]
                 for model
-                in source_file_models[source_file]
+                in models
             }
-            for source_file
-            in source_file_models.keys()
+            for source_file, models
+            in source_file_models.items()
         }
         return source_file_model_fields
 
-    def generate_comments(self, fields_by_model_by_source_file: Dict[str, Dict[Model, Field]]) -> Dict[str, List[str]]:
+    def generate_comments(self, fields_by_model_by_source_file: Dict[str, Dict[type[Model], list[ForeignObjectRel]]]) -> Dict[str, List[str]]:
         """
         takes in a dict of fields in the format returned by determine_fields_by_model_by_file
         spits out { source_file: [ lines_with_comments ] }, where lines_with_comments are consisted of
         original code (without any reverse accessor comments) + added reverse accessor comments.
         """
         output = {}
         for source_file, fields_by_model in fields_by_model_by_source_file.items():
@@ -83,32 +90,47 @@
                     line
                     for line
                     in source_code.readlines()
                     if not re.match(self.COMMENT_REGEX, line)
                 ]
                 patches = {}
                 tree = ast.parse(''.join(source_lines))
-                fields_by_model_names = dict([(model.__name__, model) for model in fields_by_model])
+                fields_by_model_names = {
+                    model.__name__: model
+                    for model
+                    in fields_by_model
+                }
 
                 for node in ast.walk(tree):
                     if isinstance(node, ast.ClassDef) and node.name in fields_by_model_names:
                         model = fields_by_model_names[node.name]
                         field_names = [field.name for field in model._meta.fields]
-                        ast_fields = dict([(_assign.targets[0].id, _assign.lineno) for _assign in node.body if isinstance(_assign, ast.Assign)])
-                        actual_fields = set(ast_fields.keys()).intersection(set(field_names)) # do an intersection here - both ast_fields and model def fields contains some passive unwanted ones
+                        ast_fields = {
+                            _assign.targets[0].id: _assign.lineno  # type:ignore[attr-defined]  # id does exist
+                            for _assign
+                            in node.body
+                            if isinstance(_assign, ast.Assign)
+                        }
+                        # do an intersection here: both ast_fields and model def fields contains some passive
+                        # unwanted ones
+                        actual_fields = set(ast_fields.keys()).intersection(set(field_names))
                         if actual_fields:
                             inject_location = max([ast_fields[field] for field in actual_fields])
                         else:
-                            # this model contains no active field definition at this moment; insert comments at beginning of class def
+                            # this model contains no active field definition at this moment; insert comments
+                            # at beginning of class def
                             inject_location = node.lineno
 
                         patches[inject_location] = [
                             self.create_comment(field)
                             for field
-                            in sorted(fields_by_model[model], key=lambda f: f.get_accessor_name())
+                            in sorted(
+                                fields_by_model[model],
+                                key=lambda f: cast(str, f.get_accessor_name())  # will always have a name
+                            )
                         ]
 
                 # mash em up
                 offset = 0
                 for lineno, lines in sorted(patches.items()):
                     if source_lines[lineno+offset].strip() == '' :
                         source_lines[lineno+offset+1:lineno+offset+1] = lines
```

### Comparing `django-allianceutils-2.2.0/allianceutils/management/commands/print_logging.py` & `django_allianceutils-3.0.0/src/allianceutils/management/commands/print_logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,11 +39,11 @@
             logging.getLogger('werkzeug')
         except ImportError:
             pass
 
         # logging_tree always goes to stdout; need to capture it and redirect to django management stdout
         orig_stdout = sys.stdout
         try:
-            sys.stdout = self.stdout
+            sys.stdout = self.stdout  # type:ignore[assignment] # we're changing the type
             logging_tree.printout()
         finally:
             sys.stdout = orig_stdout
```

### Comparing `django-allianceutils-2.2.0/allianceutils/middleware/current_user.py` & `django_allianceutils-3.0.0/src/allianceutils/middleware/current_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import threading
 
 from django.utils.deprecation import MiddlewareMixin
 
 GLOBAL_USER = threading.local()
 
+
 class CurrentUserMiddleware(MiddlewareMixin):
 
     def __init__(self, get_response=None):
         self.get_response = get_response
 
     """
     Middleware to enable accessing the currently logged-in user without
```

### Comparing `django-allianceutils-2.2.0/allianceutils/middleware/http_auth.py` & `django_allianceutils-3.0.0/src/allianceutils/middleware/http_auth.py`

 * *Files identical despite different names*

### Comparing `django-allianceutils-2.2.0/allianceutils/models.py` & `django_allianceutils-3.0.0/src/allianceutils/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,42 @@
+from __future__ import annotations
+
 from typing import Callable
+from typing import cast
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import TYPE_CHECKING
 from typing import Union
 
 from django.contrib.auth.models import Group
 from django.contrib.auth.models import Permission
 from django.core.exceptions import NON_FIELD_ERRORS
 from django.core.exceptions import ValidationError
 from django.db import IntegrityError
 from django.db.models import Manager
 from django.db.models import Model
 from django.db.models import QuerySet
+from django.utils.functional import Promise
+from typing_extensions import TypeAlias
 
 
-def combine_querysets_as_manager(*queryset_classes: List[QuerySet]) -> Manager:
+def combine_querysets_as_manager(*queryset_classes: type[QuerySet]) -> Manager:
     """
     Replacement for django_permanent.managers.MultiPassThroughManager which no longer works in django 1.8
 
     Returns a new Manager instance that passes through calls to multiple underlying queryset_classes via inheritance
 
     :param queryset_classes: Queryset cla
     :return: class
     """
-    name = "".join([cls.__name__ for cls in queryset_classes])
-    return type(name, queryset_classes, {}).as_manager()
+    names = [cls.__name__ for cls in queryset_classes]
+    name = "".join(names)
+    combined_querysets: type[QuerySet] = type(name, queryset_classes, {})
+    return combined_querysets.as_manager()
 
 
 class NoDeleteQuerySet(QuerySet):
     def delete(self, force: bool=False):
         raise IntegrityError(f"Instances of model '{self.__class__.__name__}' are marked as undeletable")
 
 
@@ -53,59 +61,97 @@
 
     class Meta:
         abstract = True
 
 
 # -------------------------------------------------------------------------------------------------------------------
 
-# We need a placeholder to indicate that a ValidationError actually has no error; we use this
-class _NO_VALIDATION_ERROR:
-    pass
+# we don't want to rely on django_stubs_ext being present at runtime
+if TYPE_CHECKING:
+    from django_stubs_ext import StrOrPromise
+else:
+    StrOrPromise: TypeAlias = str
+
+ErrorListT: TypeAlias = List[Union[ValidationError, StrOrPromise, None]]
+ErrorDictT: TypeAlias = Dict[str, Union[ErrorListT, StrOrPromise]]
+
+# this is the type that a normal ValidationError accepts
+ErrorT: TypeAlias = Union[StrOrPromise, ValidationError, ErrorDictT, ErrorListT]
+
+# ExtendedValidationError also accept None
+ExtendedErrorT: TypeAlias = Union[ErrorT, None]
 
 
 class _ExtendedValidationError(ValidationError):
     """
     Extended version of ValidationError for use with raise_validation_errors()
 
-    Internal behaviour is slightly different in that it may contain no errors at all
+    A normal ValidationError contains one (and only one) of:
+        - a single message (str or Promise)
+            - self.message - the message
+            - self.error_list - [self]
+        - a list of ValidationError
+            - self.error_list
+        - a dict mapping field names to lists of ValidationError
+            - self.error_dict
+
+    It can't contain a combination of error_list and error_dict
+
+    An ExtendedValidationError is extended so that
+        - you can pass None to the constructor (to indicate no errors)
+            - internally None is simply translated to []
+        - ValidationErrors can be merged with other ValidationErrors
     """
 
-    ErrorType = Union[str, ValidationError]
-
-    def add_error(self, field: Optional[str], error: Union[ErrorType, List[ErrorType], Dict[str, List[ErrorType]]]):
+    def __init__(self, message: ExtendedErrorT, *args, **kwargs):
+        if message is None:
+            message = []
+        super().__init__(message, *args, *kwargs)
+
+    def add_error(
+        self,
+        field: str | None,
+        error: ExtendedErrorT,
+    ):
         """
         This has the same behaviour as BaseForm.add_error()
         """
+        if error is None:
+            return
+
         if not isinstance(error, ValidationError):
             # Normalize to ValidationError and let its constructor
             # do the hard work of making sense of the input.
             error = _ExtendedValidationError(error)
 
         if hasattr(error, 'error_dict'):
             if field is not None:
                 raise TypeError(
                     "The argument `field` must be `None` when the `error` "
                     "argument contains errors for multiple fields."
                 )
 
         if field is not None:
-            error = _ExtendedValidationError({field: error})
+            if not isinstance(error, list):
+                error = _ExtendedValidationError({field: [error]})
+            else:
+                error = _ExtendedValidationError({field: error})
 
         self.merge(error)
 
     def merge(self, error: ValidationError):
         """
         Merge another ValidationError into this one
         """
 
         # we need to copy self in order to avoid recursive self-references
         self_copy = _ExtendedValidationError(self)
         new_ve = self_copy.merged(error)
 
-        # now copy the details from the new ValidationError into this one
+        # now replace our internal state with that from the new ValidationError
         self.__dict__.clear()
         self.__dict__.update(new_ve.__dict__)
 
     def merged(self, errors: ValidationError) -> ValidationError:
         """
         Return a new ValidationError that is a merge of `self` and `errors`
         """
@@ -115,56 +161,67 @@
             # this does a little unbound function magic to treat it as though
             # it were an _ExtendedValidationError
             return _ExtendedValidationError._is_empty(ve)
 
         # A ValidationError could be in any of the following forms:
         # [1] dict: self.error_dict exists
         # [2] list: self.error_list exists but self.message doesn't
-        # [3] scalar: self.message is a single message
+        # [3] scalar: self.message is a single message & self.error_list == [self]
 
         # list of validation errors to merge
         to_merge = [self, errors]
 
         # we need to promote one or more both to a dict-type ValidationError
         if any(hasattr(ve, 'error_dict') for ve in to_merge):
-            to_merge_dicts = []
+            to_merge_dicts: list[ErrorDictT] = []
             for ve in to_merge:
                 if not hasattr(ve, 'error_dict'):
-                    ve_list = [x for x in ve.error_list if not is_empty(x)]
+                    ve_list: ErrorListT = [x for x in ve.error_list if not is_empty(x)]
                     if ve_list:
                         to_merge_dicts.append({NON_FIELD_ERRORS: ve_list})
                 else:
-                    to_merge_dicts.append(ve.error_dict)
+                    # cast() needed because list is invariant
+                    # https://mypy.readthedocs.io/en/stable/common_issues.html#variance
+                    error_dict: ErrorDictT = cast(ErrorDictT, ve.error_dict)
+                    to_merge_dicts.append(error_dict)
 
-            merged_dict = {}
+            merged_dict: ErrorDictT = {}
             for to_merge_dict in to_merge_dicts:
                 for key, value in to_merge_dict.items():
                     merged_dict.setdefault(key, [])
-                    merged_dict[key].extend(value.copy())
+                    error_list = cast(list, merged_dict[key])
+                    copied_value: ErrorT
+                    # there's an assumption here that a promise is only wrapping a str and
+                    # not a mutable structure like a dict or list
+                    if isinstance(value, (str, Promise)):
+                        copied_value = value
+                    else:
+                        copied_value = value.copy() # cast(ErrorListT | ErrorDictT, value).copy()
+                    error_list.extend(copied_value)
 
             new_ve = _ExtendedValidationError(merged_dict)
         else:
             codes = []
             params = []
             to_merge_messages = []
-            to_merge_lists = []
+            to_merge_lists: ErrorListT = []
             for ve in to_merge:
                 if hasattr(ve, 'message'):
                     # ve might be a ValidationError instead of an _ExtendedValidationError
                     if not is_empty(ve):
                         to_merge_messages.append(ve.message)
                         to_merge_lists.extend(ve.error_list)
                         codes.append(ve.code)
                         params.append(ve.params)
                 else:
                     to_merge_lists.extend(ve.error_list)
 
             if len(to_merge_lists) == 0:
-                # all _NO_VALIDATION_ERROR
-                new_ve = _ExtendedValidationError(_NO_VALIDATION_ERROR)
+                # no validation errors
+                new_ve = _ExtendedValidationError(None)
             elif len(to_merge_lists) == 1 and len(to_merge_messages) == 1:
                 # was just a single ValidationError with a simple message
                 new_ve = _ExtendedValidationError(to_merge_messages[0], code=codes[0], params=params[0])
             else:
                 new_ve = _ExtendedValidationError(to_merge_lists)
 
         return new_ve
@@ -176,27 +233,31 @@
         The following are not considered errors:
         - a named field whose errors consist of an empty list
         - a non-truthy value in a list of errors
         - a ValidationError that is just an empty message
 
         For example, the following are considered empty validation errors:
 
-        ValidationError(None)
-        ValidationError('')
-        ValidationError([''])
-        ValidationError({})
-        ValidationError({'my_field': []})
+        ExtendedValidationError(None)
+        ExtendedValidationError('')
+        ExtendedValidationError([''])
+        ExtendedValidationError({})
+        ExtendedValidationError({'my_field': []})
 
         The following *will* be considered validation errors:
-        ValidationError({'my_field': ['']})
-        ValidationError({'my_field': [None]})
-        ValidationError('foo')
-        ValidationError(['foo'])
+        ExtendedValidationError({'my_field': ['']})
+        ExtendedValidationError({'my_field': [None]})
+        ExtendedValidationError('foo')
+        ExtendedValidationError(['foo'])
         """
-        return getattr(self, 'message', None) == _NO_VALIDATION_ERROR
+        return (
+            getattr(self, 'message', None) is None and
+            len(getattr(self, "error_list", [])) == 0 and
+            len(getattr(self, "message_dict", {})) == 0
+        )
 
     def capture_validation_error(self) -> '_ExtendedValidationErrorCaptureContext':
         return _ExtendedValidationErrorCaptureContext(self)
 
 
 class _ExtendedValidationErrorCaptureContext:
     def __init__(self, ve: _ExtendedValidationError):
@@ -217,15 +278,15 @@
             raise TypeError('raise_validation_errors func is not callable')
         self.func = func
 
     def __enter__(self) -> _ExtendedValidationError:
         try:
             if self.func is not None:
                 self.func()
-            self.ve = _ExtendedValidationError(_NO_VALIDATION_ERROR)
+            self.ve = _ExtendedValidationError(None)
         except ValidationError as ve:
             self.ve = _ExtendedValidationError(ve)
 
         return self.ve
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if exc_type is None:
```

### Comparing `django-allianceutils-2.2.0/allianceutils/rules.py` & `django_allianceutils-3.0.0/src/allianceutils/rules.py`

 * *Files identical despite different names*

### Comparing `django-allianceutils-2.2.0/allianceutils/templatetags/alliance_webpack.py` & `django_allianceutils-3.0.0/src/allianceutils/templatetags/alliance_webpack.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,10 +30,11 @@
           <script type="text/javascript" src="http://whatever/app.bundle.js?806fc65dbad8a4dbb1cc" crossorigin></script>
         
         {% render_entry_point 'app' 'css' %}
           <link type="text/css" href="http://whatever/common.bundle.css?e2b781da02d36dad3aff" rel="stylesheet"></link>
           <link type="text/css" href="http://whatever/app.bundle.css?e2b781da02d36dad3aff" rel="stylesheet"></link>
 
     """
-    loader = WebpackEntryPointLoader(settings.WEBPACK_LOADER[config])
+    webpack_settings: dict = settings.WEBPACK_LOADER[config]  # type:ignore[misc]  # we've added a new settings
+    loader = WebpackEntryPointLoader(webpack_settings)
     tags = get_chunk_tags(loader.get_chunks_for_entry_point(entry_point_name, resource_type), attrs)
     return mark_safe('\n'.join(tags))
```

#### html2text {}

```diff
@@ -9,10 +9,11 @@
 config. :param resource_type: Currently supports 'js' or 'css' :param attrs:
 Optional attributes to pass through to the underlying HTML tag (eg.
 'crossorigin') :param config: Config identifier to use. Maps to a key in
 WEBPACK_LOADER settings. Example: {% render_entry_point 'app' 'js'
 attrs="crossorigin" %}
  {% render_entry_point 'app' 'css' %}
 
- """ loader = WebpackEntryPointLoader(settings.WEBPACK_LOADER[config]) tags =
-get_chunk_tags(loader.get_chunks_for_entry_point(entry_point_name,
-resource_type), attrs) return mark_safe('\n'.join(tags))
+ """ webpack_settings: dict = settings.WEBPACK_LOADER[config] # type:ignore
+[misc] # we've added a new settings loader = WebpackEntryPointLoader
+(webpack_settings) tags = get_chunk_tags(loader.get_chunks_for_entry_point
+(entry_point_name, resource_type), attrs) return mark_safe('\n'.join(tags))
```

### Comparing `django-allianceutils-2.2.0/allianceutils/templatetags/default_value.py` & `django_allianceutils-3.0.0/src/allianceutils/templatetags/default_value.py`

 * *Files identical despite different names*

### Comparing `django-allianceutils-2.2.0/allianceutils/util/__init__.py` & `django_allianceutils-3.0.0/src/allianceutils/util/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pathlib import Path
 from typing import Callable
 from typing import Iterable
 from typing import Tuple
 from typing import Union
 
 from django.conf import settings
@@ -40,25 +42,26 @@
                 raise
 
 
 def add_autoreload_extra_files(extra_files: Iterable[Union[str, Path]]):
     if not settings.DEBUG:
         return
 
+    is_running_from_reloader: Callable[[], bool] | None
     try:
        from werkzeug.serving import is_running_from_reloader
     except ImportError:
         is_running_from_reloader = None
 
     if is_running_from_reloader and is_running_from_reloader():
         # we're running from the main runserver_plus process
         if not hasattr(settings, 'RUNSERVER_PLUS_EXTRA_FILES'):
             settings.RUNSERVER_PLUS_EXTRA_FILES = []
 
-        settings.RUNSERVER_PLUS_EXTRA_FILES += extra_files
+        settings.RUNSERVER_PLUS_EXTRA_FILES += extra_files  # type:ignore[misc]  # we're adding a new property
 
     else:
         # either:
         #  - we're using the runserver (django) server
         #  - we're running from a child runserver_plus thread. If this is the case
         #    then the django autoreload signal will do nothing: working as intended
```

### Comparing `django-allianceutils-2.2.0/allianceutils/util/camel_case.py` & `django_allianceutils-3.0.0/src/allianceutils/util/camel_case.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,68 @@
 # Inspired by https://github.com/vbabiy/djangorestframework-camel-case
 # (but apart from 2 regexes, completely rewritten in order to add `ignore` parameters)
+from __future__ import annotations
+
 from collections import OrderedDict
-from collections.abc import Mapping
 import re
 from typing import Any
 from typing import Callable
+from typing import cast
 from typing import Dict
 from typing import Iterable
+from typing import Literal
+from typing import Mapping
 from typing import Sequence
 from typing import Tuple
+from typing import TypeVar
+from typing import Union
 
 from django.core.files import File
 from django.utils.functional import Promise
+from typing_extensions import TypeAlias
 
 _first_cap_re = re.compile('(.)([A-Z][a-z]+)')
 _all_cap_re = re.compile('([a-z0-9])([A-Z])')
 _re_underscore = re.compile(r'(?!^)(?<!_)_([^_])')
 
-_empty_dict = {} # we use this a lot in here
+"""
+a sequence of fields to ignore when camelizing
+# see camelize()/underscorize() 
+"""
+IgnoreSpecifier = Iterable[str]
+
+# Internal structure: see _create_ignore_lookup() for usage
+# Exposed only for typing purposes; treat this as an opaque type
+IgnoreDict: TypeAlias = Dict[Union[str, None], Union["IgnoreDict", Literal[True]]]
+
+_empty_dict: IgnoreDict = {} # we use this a lot in here
+
 
+# a generic type that can be camelized/underscorized
+CamelizeT = TypeVar('CamelizeT')
 
-def _debug_lookup(ignore_tree: Dict, indent: int=0) -> str:
+
+def _debug_lookup(ignore_tree: IgnoreDict, indent: int = 0) -> list[str]:
     """
-    Format a tree processed by _transform_ignore() into something human-readable (for debugging)
-    :param ignore_tree:
-    :return:
+    Format a tree processed by _transform_ignore() into something human-readable (for debugging/testing purposes)
     """
     x = []
-    for sort_key, key in sorted([(key or '', key) for key in ignore_tree.keys()]):
-        if key is None: continue
-        line = ' ' * 4 * indent + str(key) + ('!' if ignore_tree[key].get(None) is True else '')
+    for sort_key, key, children in sorted([(key or '', key, val) for key, val in ignore_tree.items()]):
+        if key is None:
+            continue
+        assert children is not True  # only None key should have a children value of True
+
+        line = ' ' * 4 * indent + str(key) + ('!' if None in children else '')
         x.append(line)
-        if isinstance(ignore_tree[key], Mapping):
-            x += _debug_lookup(ignore_tree[key], indent + 1)
-    if indent == 0:
-        return '\n'.join(x)
-    else:
-        return x
+        if isinstance(children, Mapping):
+            x += _debug_lookup(children, indent + 1)
+    return x
 
 
-def _create_ignore_lookup(ignore: Sequence[str]) -> Dict:
+def _create_ignore_lookup(ignore: IgnoreSpecifier) -> IgnoreDict:
     """
     Transforms a list of field-paths-to-ignore of the following form:
     [
         'a.b',
         'a.b.c',
         'a.*.d',
         'e.*.f',
@@ -84,58 +103,65 @@
         - * is a wildcard indicator
     TODO: In future if we allow pre-split paths then we might relax some of these constraints
 
     :param ignore: list of field paths to ignore
     :return: See above
     """
 
-    def process_path(parts: Sequence[str], candidates: Sequence[Dict]):
+    def process_path(parts: Sequence[str], candidates: list[IgnoreDict]):
         """
-        Breadth-first transform of the tree; will add `parts` to the sub-tree(s) specified by `candidates`
+        Breadth-first transform of the tree; will merge `parts` into the sub-tree(s) specified by `candidates`
 
         :param parts: list of field path parts (ie already split on '.') relative to candidates
         :param candidates: list of current candidate sub-trees to process
         """
         while len(parts):
             part = parts[0]
             assert part != ''
 
-            new_candidates = []
+            new_candidates: list[IgnoreDict] = []
 
             for candidate in candidates:
                 if part not in candidate:
                     candidate[part] = {}
 
                 if len(parts) > 1:
                     if part == '*':
                         # all candidates
-                        new_candidates += candidate.values()
+                        new_candidates.extend(cast(Iterable[IgnoreDict], candidate.values()))
                     else:
-                        new_candidates.append(candidate[part])
+                        new_candidate = cast(IgnoreDict, candidate[part])
+                        assert candidate[part] is not True
+                        new_candidates.append(new_candidate)
                 else:
                     # current element is a terminal
-                    candidate[part][None] = True
+                    cast(IgnoreDict, candidate[part])[None] = True
 
             candidates = new_candidates
             parts = parts[1:]
 
-    ignore = [x.split('.') for x in ignore]
+    ignore_parts = [x.split('.') for x in ignore]
     # We need to process the wildcard parts last, so sort according to wildcard positions
-    ignore = [(tuple(part == '*' for part in path), path) for path in ignore]
-    ignore.sort(key=lambda x: x[0])
-    ignore = [x[1] for x in ignore]
+    ignore_parts_keyed = [(tuple(part == '*' for part in path), path) for path in ignore_parts]
+    ignore_parts_keyed.sort(key=lambda x: x[0])
+    ignore_parts = [x[1] for x in ignore_parts_keyed]
 
     # Now do the processing
-    data = {}
-    for parts in ignore:
+    data: IgnoreDict = {}
+    for parts in ignore_parts:
         process_path(parts, [data])
     return data
 
 
-def _transform_key_val(key, value, transform_key: Callable, ignore_lookup: Dict) -> Tuple[Any, Any]:
+def _transform_key_val(
+    key: str | Promise,
+    value: CamelizeT,
+    transform_key: Callable,
+    ignore_lookup: Dict
+) -> Tuple[str, CamelizeT]:
     """
     Transform a particular key/value pair
     - Will rename the key if it's not in the ignore_lookup
     - Will recursively transform the value
 
     :param key: key name
     :param value: data value
@@ -153,18 +179,19 @@
         ignore_lookup = ignore_lookup['*']
     else:
         ignore_lookup = _empty_dict
 
     if not (ignore_lookup.get(None, False) is True):
         key = transform_key(key)
 
+    assert not isinstance(key, Promise)
     return key, _transform_data(value, transform_key, ignore_lookup)
 
 
-def _transform_data(data, transform_key: Callable, ignore_lookup: Dict):
+def _transform_data(data: CamelizeT, transform_key: Callable, ignore_lookup: Dict) -> CamelizeT:
 
     # Mapping (dict) -- transform keys
     if isinstance(data, Mapping):
         cls = OrderedDict if isinstance(data, OrderedDict) else dict
         return cls(
             _transform_key_val(key, value, transform_key, ignore_lookup)
             for (key, value) in data.items()
@@ -176,18 +203,21 @@
     # containing File objects for any file fields.
     # At least for now we don't support numeric indices in ignores, so '*' is the only ignore lookup index
     # that can match a list/iterable
     # `Promise` is included here as django uses that as the base for proxy class created in lazy functions, eg.
     # gettext_lazy. Without this they are treated as an iterable.
     if isinstance(data, Iterable) and not isinstance(data, (str, bytes, File, Promise)):
         ignore_lookup = ignore_lookup.get('*', _empty_dict)
-        return [_transform_data(x, transform_key, ignore_lookup) for x in data]
+        transformed = [_transform_data(x, transform_key, ignore_lookup) for x in data]
+        # this cast is not strictly true, but for our purposes an iterable => list might as well be the same type
+        return cast(CamelizeT, transformed)
 
     # is a string/scalar/noniterable; return as-is
-    return data
+    # the cast is because mypy incorrectly thinks the type could have changed
+    return cast(CamelizeT, data)
 
 
 def underscore_to_camel(key: str) -> str:
     """
     Turn underscores into camel case
 
     Double underscores will be left alone
@@ -202,15 +232,15 @@
             key
         )
     except TypeError:
         # Not a string... ignore
         return key
 
 
-def camelize(data: Any, ignore: Sequence[str]=[]) -> Any:
+def camelize(data: CamelizeT, ignore: IgnoreSpecifier = []) -> CamelizeT:
     """
     Recursively turn underscore-cased keys into camel-cased keys
 
     :param data:
     :param ignore: list of key paths to ignore; see `_creat_ignore_lookup`
     :return: structure with keys turned into camelcase
     """
@@ -228,15 +258,15 @@
         s1 = _first_cap_re.sub(r'\1_\2', key)
         return _all_cap_re.sub(r'\1_\2', s1).lower()
     except TypeError:
         # Not a string... ignore
         return key
 
 
-def underscoreize(data: Any, ignore: Sequence[str]=[]) -> Any:
+def underscoreize(data: CamelizeT, ignore: IgnoreSpecifier = []) -> CamelizeT:
     """
     Recursively turn camelcase keys into underscored keys
 
     :param data:
     :param ignore: list of key paths to ignore; see `_create_ignore_lookup`
     :return: structure with keys turned into camelcase
     """
```

### Comparing `django-allianceutils-2.2.0/allianceutils/util/date.py` & `django_allianceutils-3.0.0/src/allianceutils/util/date.py`

 * *Files identical despite different names*

### Comparing `django-allianceutils-2.2.0/allianceutils/util/get_firstparty_apps.py` & `django_allianceutils-3.0.0/src/allianceutils/util/get_firstparty_apps.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,37 @@
+from __future__ import annotations
+
 import os
-import sys
+from typing import Iterable
 
 from django.apps import AppConfig
 from django.apps import apps
-from isort.api import Config
-from isort.api import place_module
 
 # we don't use __main__.__file__ because debugging in an IDE (eg pycharm) __main__ may be the IDE's setup script
 # os.getcwd() should be safe since django's manage.py insists on running in the django root
-isort_config = Config(settings_path=os.getcwd())
+#
+# take a copy of the current working directory asap in case something else changes it
+_root_path = os.getcwd()
 
 
-def is_firstparty_app(app_config: AppConfig):
+def is_firstparty_app(app_config: AppConfig) -> bool:
     """
     Use isort's way of determining whether an app is "first party" or otherwise
     """
+    # import isort here so that it's not a hard dependency
+    from isort.api import Config
+    from isort.api import place_module
+
+    isort_config = Config(settings_path=_root_path)
+
+    assert app_config.module is not None
     module_name = app_config.module.__name__
     return place_module(module_name, config=isort_config) == 'FIRSTPARTY'
        # this shouldn't be needed anymore now that we specify the isort config:
        # or app_config.__module__ == 'allianceutils.apps'
 
 
-def get_firstparty_apps():
+def get_firstparty_apps() -> Iterable[AppConfig]:
     """
     Return all installed first party apps in an iterator
     """
     return filter(is_firstparty_app, apps.get_app_configs())
```

### Comparing `django-allianceutils-2.2.0/allianceutils/views/decorators.py` & `django_allianceutils-3.0.0/src/allianceutils/views/decorators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from functools import wraps
 
 from django.conf import settings
-from django.utils.decorators import available_attrs
 from django.views.decorators.gzip import gzip_page
 
 
 def gzip_page_ajax(func):
     """
     Smarter version of django's gzip_page:
     - If settings.DEBUG not set, will always gzip
@@ -13,13 +12,13 @@
     This allows you to use django-debug-toolbar in DEBUG mode (if you gzip a response then the debug toolbar middleware won't run)
     """
     gzipped_func = gzip_page(func)
 
     if not settings.DEBUG:
         return gzipped_func
 
-    @wraps(func, assigned=available_attrs(func))
+    @wraps(func)
     def conditional_gzip_func(request, *args, **kwargs):
         if request.is_ajax():
             return gzipped_func(request, *args, **kwargs)
         return func(request, *args, **kwargs)
     return conditional_gzip_func
```

### Comparing `django-allianceutils-2.2.0/allianceutils/webpack.py` & `django_allianceutils-3.0.0/src/allianceutils/webpack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import json
 import logging
 import time
 from typing import Dict
+from typing import Generator
+from typing import Iterable
 from typing import Optional
 from typing import Sequence
 from urllib.parse import ParseResult
 from urllib.parse import quote
 from urllib.parse import urljoin
 from urllib.parse import urlparse
 
@@ -15,15 +17,15 @@
 logger = logging.Logger('webpack')
 
 # Number of seconds before warning about slow build
 # Helps catch broken dev servers and confusing devs about why requests are loading
 WEBPACK_DEV_LOADING_TIME_WARNING_DELAY = 20
 
 
-def get_chunk_tags(chunks: Dict, attrs: str):
+def get_chunk_tags(chunks: Iterable[Dict], attrs: str):
     """
     Get tags for
     :param chunks:
     :param attrs:
     :return:
     """
     tags = []
@@ -154,28 +156,28 @@
         if self.config['INCLUDE_QUERY_HASH'] and chunk.get('contentHash'):
             query = f'?{chunk["contentHash"]}'
         path = f'{public_path}{name}{query}'
         if self.config['BASE_URL']:
             return urljoin(self.config['BASE_URL'], path)
         return path
 
-    def filter_chunks(self, public_path: str, chunks: Sequence[Dict], required_resource_type:str) -> Sequence[Dict]:
+    def filter_chunks(self, public_path: str, chunks: Sequence[Dict], required_resource_type:str) -> Generator[dict, None, None]:
         if required_resource_type not in self.extensions_by_resource_type:
             valid_resource_types = ', '.join(self.extensions_by_resource_type.keys())
             raise ValueError(f'Invalid chunk type {required_resource_type}. Must be one of: {valid_resource_types}')
         for chunk in chunks:
             resource_type = self.get_resource_type(chunk)
             if required_resource_type == resource_type:
                 yield {
                     'url': self.get_chunk_url(public_path, chunk),
                     'resource_type': resource_type,
                     **chunk,
                 }
 
-    def get_chunks_for_entry_point(self, entry_point_name:str, resource_type:str) -> Sequence[Dict]:
+    def get_chunks_for_entry_point(self, entry_point_name:str, resource_type:str) ->  Generator[dict, None, None]:
         stats = self.load_stats()
         if stats['status'] == 'compiling':
             logger.warning('Webpack is compiling... web requests will wait until this resolves before loading')
             start = time.time()
             warning_logged = False
             while stats['status'] == 'compiling':
                 time.sleep(0.1)
```

### Comparing `django-allianceutils-2.2.0/setup.py` & `django_allianceutils-3.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,1013 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-allianceutils
+Version: 3.0.0
+Summary: Alliance Software common utilities for Django
+Home-page: https://github.com/AllianceSoftware/django-allianceutils/
+License: BSD-2-Clause
+Keywords: django,alliance,alliancesoftware
+Author: Alliance Software
+Author-email: support@alliancesoftware.com.au
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Typing :: Typed
+Provides-Extra: extras
+Provides-Extra: mysql
+Provides-Extra: postgres
+Requires-Dist: Django (>=3.2)
+Requires-Dist: django-filter ; extra == "extras"
+Requires-Dist: django-storages ; extra == "extras"
+Requires-Dist: djangorestframework ; extra == "extras"
+Requires-Dist: isort (>=5) ; extra == "extras"
+Requires-Dist: logging_tree ; extra == "extras"
+Requires-Dist: mysqlclient ; extra == "mysql"
+Requires-Dist: psycopg2 ; extra == "postgres"
+Requires-Dist: rules ; extra == "extras"
+Requires-Dist: typing_extensions (>=4.5.0,<5.0.0)
+Project-URL: Documentation, https://github.com/AllianceSoftware/django-allianceutils/blob/master/README.md
+Project-URL: Repository, https://github.com/AllianceSoftware/django-allianceutils/
+Project-URL: issues, https://github.com/AllianceSoftware/django-allianceutils/issues
+Description-Content-Type: text/markdown
 
-packages = \
-['allianceutils',
- 'allianceutils.api',
- 'allianceutils.auth',
- 'allianceutils.management',
- 'allianceutils.management.commands',
- 'allianceutils.middleware',
- 'allianceutils.serializers',
- 'allianceutils.templatetags',
- 'allianceutils.util',
- 'allianceutils.views']
-
-package_data = \
-{'': ['*'], 'allianceutils': ['bin/*']}
-
-install_requires = \
-['Django>=2.2', 'isort>=4']
-
-setup_kwargs = {
-    'name': 'django-allianceutils',
-    'version': '2.2.0',
-    'description': 'Alliance Software common utilities for Django',
-    'long_description': '# Alliance Utils\n\n![CI Tests](https://github.com/AllianceSoftware/django-allianceutils/workflows/Django%20CI/badge.svg)\n\nA collection of utilities for django projects from [Alliance Software](https://www.alliancesoftware.com.au/).\n\n* [Installation](#installation)\n* [Usage](#usage)\n    * [API](#api)\n    * [Auth](#auth)\n    * [Decorators](#decorators)\n    * [Filters](#filters)\n    * [Management](#management)\n        * [Commands](#commands)\n        * [Checks](#checks)\n    * [Middleware](#middleware)\n    * [Migrations](#migrations)\n    * [Models](#models)\n    * [Rules](#rules)\n    * [Serializers](#serializers)\n    * [Template Tags](#template-tags)\n    * [Util](#util)\n* [Changelog](#changelog)\n\n## Installation\n\n`pip install django-allianceutils`\n\n## System Requirements\n\n* Tested with django 2.2 and 3.2\n  * Pull requests accepted for other versions, but at minimum we test against current LTS versions\n* Python >=3.6 (no python 3.5 support)\n\n## Usage\n\n### API\n\n#### Mixins\n\n##### SerializerOptInFieldsMixin\n\nRegulates fields exposed on a Serializer by default & as requested based on query parameters or context.\n\n* Pass \'include_fields\' / \'opt_in_fields\' thru query params or context to use.\n* multiple fields can either be separated by comma\n  eg, `/?include_fields=first_name,email&opt_in_fields=gait_recognition_prediction`\n* or passed in the traditional list fashion\n  eg, `/?include_fields=first_name&include_fields=email&opt_in_fields=gait_recognition_prediction`\n* or mixed eg, `/?include_fields=first_name,email&include_fields=boo`\n* By default, all "fields" defined in serializer, minus those listed in "opt_in_fields" would be returned.\n* If "include_fields" is supplied, only fields requested this way would be returned.\n* If "opt_in_fields" is supplied, fields requested this way PLUS fields from #1 or #2 would be returned.\n* Pinned fields are always returned (defaults to primary key)\n\nUsage:\n\n```python\nclass UserSerializer(SerializerOptInFieldsMixin, ModelSerializer):\n    class Meta:\n        model = User\n        fields = (\n            "id",\n            "first_name",\n            "last_name",\n            "email",\n            "region",\n            "activated_at",\n            "is_staff",\n        )\n        # These fields only returned if explicitly requested\n        opt_in_only_fields = ["activated_at", "is_staff"]\n```\n\n#### Permissions\n\n##### register_custom_permissions\n\n* Creates permissions that have no model by linking them to an empty content type\n* Django creates permissions as part of\n  the [`post_migrate` signal](https://docs.djangoproject.com/en/stable/ref/signals/#post-migrate)\n\nUsage\n\n```py\ndef on_post_migrate(sender, **kwargs):\n    register_custom_permissions("myapp", ("my_perm", "My Permission"))\n```\n\n##### SimpleDjangoObjectPermissions\n\nPermission class for Django Rest Framework that adds support for object level permissions.\n\nDiffers from just DRF\'s [DjangoObjectPermissions](https://www.django-rest-framework.org/api-guide/permissions/#object-level-permissions) because it\n* does not require a queryset\n* uses the same permission for every request http method and ViewSet method \n\nNotes\n* The default django permissions system will [always return False](https://docs.djangoproject.com/en/stable/topics/auth/customizing/#handling-object-permissions) if given an object; you must be using another permissions backend\n* As per [DRF documentation](http://www.django-rest-framework.org/api-guide/permissions/#object-level-permissions): get_object() is only required if you want to implement object-level permissions\n* **WARNING** If you override `get_object()` then you need to *manually* invoke `self.check_object_permissions(self.request, obj)`\n* Will attempt to check permission both globally and on a per-object basis but considers it an error if the check returns True for both\n*   \n\nUsage\n* See [DRF permissions policy](https://www.django-rest-framework.org/api-guide/permissions/#setting-the-permission-policy) for details on apply Permissions policies globally\n\n* To apply to a specific view you need to set `permission_required`\n```python\nclass MyAPIView(SimpleDjangoObjectPermissions, APIView):\n        permission_required = \'my_module.my_permission\'\n        permission_classes = [allianceutils.api.permissions.SimpleDjangoObjectPermissions] \n```\n\nIf you have no object level permissions (eg. from rules) then it will just do a static permission check.\n\n##### GenericDjangoViewsetPermissions\n\n* Map viewset actions to Django permissions.\n  * The model used for permission is extracted from the ViewSet\n    * If you implement `get_permission_model` on the ViewSet that will be used\n    * Otherwise it will call `get_queryset` on the ViewSet and extract the model from the returned queryset \n * To alter this behaviour extends `GenericDjangoViewsetPermissions` and implement `get_model` \n* Usage example:\n```\nclass MyViewSet(GenericDjangoViewsetPermissions, viewsets.ModelViewSet):\n    queryset = MyModel.objects.all()\n    serializer_class = MySerializer\n```\n* `GenericDjangoViewsetPermissions.default_actions_to_perms_map` defines the default set of permissions. These can be extended or overridden using `actions_to_perms_map`:\n```\nclass MyViewSet(GenericDjangoViewsetPermissions, viewsets.ModelViewSet):\n\n    # ...\n\n    actions_to_perms_map = {\n        \'create\': []\n    }\n```\n* No permissions will be required for the create action, but permissions for other actions will remain unchanged.\n* By default permissions checks are passed the relevant model instance for per-object permission checks\n    * This assumes that your backend doesn\'t ignore the model object (default django permissions simply ignore any object passed to a permissions check)\n    * Since there is no model object, functions decorated with `@list_route` will pass `None` as the permissions check object\n\n#### Parsers\n\n##### CamelCaseJSONParser\n\nParser that recursively turns camelcase keys into underscored keys for JSON data.\nThis can be set globally on the [DEFAULT_PARSER_CLASSES](https://www.django-rest-framework.org/api-guide/settings/#default_parser_classes)\nsetting or on a ViewSet on the `parser_classes` property.\n\n##### CamelCaseMultiPartJSONParser\n\nParser that recursively turns camelcase keys into underscored keys for JSON data and handles file uploads.\nThis parser supports receiving JSON data where a field value anywhere in the structure can be a file.\nThis is achieved on the frontend by converting a structure like:\n\n```js\n{\n    name: \'Test\',\n    photo: File,\n}\n```\n\nAnd converting it to\n\n```js\n{\n    name: \'Test\',\n    photo: \'____ATTACHED_FILE_ID_1\',\n}\n```\n\nThis is then set on a field `jsonData` and the file is set on `____ATTACHED_FILE_ID_1` and submitted\nas multipart.\nThis parser then handles parsing the JSON data into a dict and setting each attached file on the\ncorrect key in the dict.\nNote that this works with nested data (ie. any File anywhere in a nested JSON structure is supported).\nTo activate this behaviour the `X-MultiPart-JSON` header must be set to \'1\' or \'true\'. If this header\nis not set it falls back to the default behaviour of MultiPartParser\nThis can be set globally on the [DEFAULT_PARSER_CLASSES](https://www.django-rest-framework.org/api-guide/settings/#default_parser_classes)\nsetting or on a ViewSet on the `parser_classes` property.\nExample frontend code to activate:\n```js\nlet fileCount = 0;\nconst files = {};\nconst replacer = (key, value) => {\n    if (value instanceof File) {\n        const id = `____ATTACHED_FILE_ID_${fileCount++}`;\n        files[id] = value;\n        return id;\n    }\n    return value;\n};\nconst stringifiedData = JSON.stringify(data, replacer);\nconst body = new FormData();\nconst body.append(\'jsonData\', stringifiedData);\nfor (const [fileKey, file] of Object.entries(files)) {\n    body.append(fileKey, file);\n}\n// eg. using a presto Endpoint\nawait myEndpoint.execute({\n    body,\n    headers: {\n        // Remove default content type from endpoint (eg. json)\n        \'Content-Type\': undefined,\n        \'X-MultiPart-JSON\': true,\n    },\n});\n```\n\n#### Renderers\n\n##### CamelCaseJSONRenderer\n\nRenderer that recursively turns underscore-cased keys into camel-cased keys.\nThis can be set globally on the [DEFAULT_RENDERER_CLASSES](https://www.django-rest-framework.org/api-guide/settings/#default_renderer_classes)\nsetting or on a ViewSet on the `renderer_classes` property.\n\n### Auth\n\n#### MinimalModelBackend\n\n* `allianceutils.auth.backends.MinimalModelBackend`\n    * Replaces the built-in django [ModelBackend](https://docs.djangoproject.com/en/stable/ref/contrib/auth/#django.contrib.auth.backends.ModelBackend)\n    * Provides django model-based authentication\n    * Removes the default authorization (permissions checks) except for checking `is_superuser` \n\n#### ProfileModelBackend\n\n* Backends for use with [GenericUserProfile](#GenericUserProfile); see code examples there\n* `allianceutils.auth.backends.ProfileModelBackendMixin` - in combo with [AuthenticationMiddleware](https://docs.djangoproject.com/en/stable/ref/middleware/#django.contrib.auth.middleware.AuthenticationMiddleware) will set user profiles on `request.user`  \n    * ~`allianceutils.auth.backends.ProfileModelBackend`~ - convenience class combined with case insensitive username & default django permissions backend\n        * this depended on [`authtools`](https://django-authtools.readthedocs.io/en/latest/) which appears to have been\n          abandoned and does not work with django >= 3.\n          If using django 3 then we recommended that you create your own backend in your app:\n          ```python\n            class ProfileModelBackend(ProfileModelBackendMixin, MinimalModelBackend):\n                # you\'ll need to implement case insensitivity either here or in the User Model  \n                pass\n          ```\n\n### Decorators\n\n#### gzip_page_ajax\n\n* Smarter version of django\'s [gzip_page](https://docs.djangoproject.com/en/stable/topics/http/decorators/#django.views.decorators.gzip.gzip_page):\n    * If settings.DEBUG not set, will always gzip\n    * If settings.DEBUG set, will gzip only if request is an ajax request\n* This allows you to use django-debug-toolbar in DEBUG mode (if you gzip a response then the debug toolbar middleware won\'t run)\n\nExample\n\n```\n\n@allianceutils.views.decorators.gzip_page_ajax\ndef my_view(request: HttpRequest) -> httpResponse:\n    data = {\n        "message": "Hello World",\n    }\n    return django.http.JsonResponse(data) \n\n```\n\n#### method_cache\n\n* Caches the results of a method on the object instance\n* Only works for regular object methods with no arguments other than `self`.\n    * Does not support `@classmethod` or `@staticmethod`\n    * If you want more powerful caching behaviour then you can wrap `cachetools` (examples [here](https://github.com/tkem/cachetools/issues/107))\n* Similar to [`@cached_property`](https://docs.python.org/3/library/functools.html#functools.cached_property) except that it works on methods instead of properties\n* Differs from [`@lru_cache()`](https://docs.python.org/3/library/functools.html#functools.lru_cache) in that\n    * `lru_cache` uses a single cache for each decorated function\n    * `lru_cache` will block garbage collection of values in the cache \n    * A `cache_clear()` method is attached to the function but unlike `lru_cache` it is scoped to an object instance   \n\nUsage\n```python\nclass MyViewSet(ViewSet):\n\n    # ...\n\n    @method_cache\n    def get_object(self):\n        return super().get_object()\n\nobj = MyViewSet()\nobj.get_object() is obj.get_object()\nobj.get_object.cache_clear()   \n```\n\n### Filters\n\n#### MultipleFieldCharFilter\n\nSearch for a string across multiple fields. Requires `django_filters`.\n\n* Usage \n\n```python\nfrom allianceutils.filters import MultipleFieldCharFilter\n\n# ...\n# In your filter set (see django_filters for documentation)\ncustomer = MultipleFieldCharFilter(names=(\'customer__first_name\', \'customer__last_name\'), lookup_expr=\'icontains\')\n```\n\n### Management\n\n#### Commands\n\n##### OptionalAppCommand\n\n* A utility class that extends `django.core.management.base.BaseCommand` and adds optional argument(s) for django apps\n* If app names are passed on the command line `handle_app_config()` will be called with the `AppConfig` for each app otherwise it will be called with every first-party app (as determined by `isort`)\n\n\nExample:\n\n```\nclass Command(allianceutils.management.commands.base.OptionalAppCommand):\n    def add_arguments(self, parser):\n        super().add_arguments(parser)\n        parser.add_argument(\'--type\', choices=(\'name\', \'label\'), default=\'name\')\n\n    def handle_app_config(self, app_config: AppConfig, **options):\n        if options[\'type\'] == \'name\':\n            print(f"Called with {app_config.name}")\n        if options[\'type\'] == \'label\':\n            print(f"Called with {app_config.label}")\n```  \n\n##### print_logging\n\n* Displays the current logging configuration in a hierarchical fashion\n* Requires [`logging_tree`](https://pypi.python.org/pypi/logging_tree) to be installed\n\n#### Checks\n\n* Checks with no configuration are functions that can be passed directly to [register](https://docs.djangoproject.com/en/3.1/topics/checks/)\n* Checks that expect parameters are classes that need to be instantiated\n\nSetting up django hooks:\n\n```python\nfrom django.apps import AppConfig\nfrom django.core.checks import register\nfrom django.core.checks import Tags\n\nfrom allianceutils.checks import check_admins\nfrom allianceutils.checks import check_db_constraints\nfrom allianceutils.checks import CheckExplicitTableNames\nfrom allianceutils.checks import check_git_hooks\nfrom allianceutils.checks import CheckReversibleFieldNames\nfrom allianceutils.checks import CheckUrlTrailingSlash\n\nclass MyAppConfig(AppConfig):\n    # ...\n\n    def ready(self):\n        register(check=check_admins, tags=Tags.admin, deploy=True)\n        register(check=check_db_constraints, tags=Tags.database)\n        register(check=CheckExplicitTableNames(), tags=Tags.models)\n        register(check=check_git_hooks, tags=Tags.admin)\n        register(check=CheckReversibleFieldNames(), tags=Tags.models)\n        register(check=CheckUrlTrailingSlash(expect_trailing_slash=True), tags=Tags.url)        \n```\n\n##### CheckUrlTrailingSlash\n\n* Checks that your URLs are consistent with the `settings.APPEND_SLASH`  \n* Arguments:\n    * `ignore_attrs` - skip checks on url patterns where an attribute of the pattern matches something in here (see example above)\n        * Most relevant attributes of a `RegexURLResolver`:\n            * `_regex` - string used for regex matching. Defaults to `[r\'^$\']`\n            * `app_name` - app name (only works for `include()` patterns). Defaults to `[\'djdt\']` (django debug toolbar)\n            * `namespace` - pattern defines a namespace\n            * `lookup_str` - string defining view to use. Defaults to `[\'django.views.static.serve\']`\n        * Note that if you skip a resolver it will also skip checks on everything inside that resolver\n* Note: If using Django REST Framework\'s [`DefaultRouter`](http://www.django-rest-framework.org/api-guide/routers/#defaultrouter) then you need to turn off `include_format_suffixes`:\n\n```\nrouter = routers.DefaultRouter(trailing_slash=True)\nrouter.include_format_suffixes = False\nrouter.register(r\'myurl\', MyViewSet)\nurlpatterns += router.urls\n```\n\n\n##### check\\_admins\n\n* Checks that `settings.ADMINS` has been properly set in settings files.\n\n##### check\\_git\\_hooks\n\n* Checks that git hookshave been set up, one of:\n  * `.git/hooks` directory has been symlinked to the project\'s `git-hooks`\n  * [`husky`](https://github.com/typicode/husky) hooks have been installed \n* \n\n##### check\\_db\\_constraints\n\n* Checks that all models that specify `db_constraints` in their Meta will generate unique constraint names when truncated by the database.\n\n##### CheckExplicitTableNames\n\n* Checks that all first-party models have `db_table` explicitly defined on their Meta class, and the table name is in lowercase\n* Arguments:\n    * `enforce_lowercase` - check that there are no uppercase characters in the table name\n    * `ignore_labels` - if an app label (eg `silk`) or app_label + model labels (eg `silk.request`)\n        matches something in `ignore_labels` then it will be ignored.\n        * `allianceutils.checks.DEFAULT_TABLE_NAME_CHECK_IGNORE` contains a default list of apps/models to ignore\n        * Can be either a `str` or a regex (anything that contains a `.match()` method) \n\n##### CheckReversibleFieldNames\n\n* Checks that all models have fields names that are reversible with `underscorize`/`camelize`/`camel_to_underscore`/`underscore_to_camel`\n* Arguments:\n    * `ignore_labels` - ignore these apps/models: see `CheckExplicitTableNames`\n\n### Middleware\n\n#### HttpAuthMiddleware\n\n* Middleware to enable basic http auth to block unwanted traffic from search engines and random visitors\n    * Intended to be used on dev / staging servers\n    * Is not a full authorization system: is a single hardcoded username/password and should be used on top of a proper authorization system\n\n* Setup\n    * Add `allianceutils.middleware.HttpAuthMiddleware` to `MIDDLEWARE`.\n    * Add `HTTP_AUTH_USERNAME` and `HTTP_AUTH_PASSWORD` to appropriate setting file, e.g. `settings/production_staging.py`\n        * Remember that you shouldn\'t be hardcoding credentials in code: read content from env vars or file\n\n#### CurrentUserMiddleware\n\n* Middleware to enable accessing the currently logged-in user without a request object.\n    * Assumes that `threading.local` is not shared between requests (an assumption also made by django internationalisation) \n\n* Setup\n    * Add `allianceutils.middleware.CurrentUserMiddleware` to `MIDDLEWARE`.\n\n* Usage\n\n```python\nfrom allianceutils.middleware import CurrentUserMiddleware\n\nuser = CurrentUserMiddleware.get_user()\n```\n\n#### QueryCountMiddleware\n\n* Warns if query count reaches a given threshold\n    * Threshold can be changed by setting `settings.QUERY_COUNT_WARNING_THRESHOLD`\n\n* Usage\n    * Add `allianceutils.middleware.CurrentUserMiddleware` to `MIDDLEWARE`.\n    * Uses the `warnings` module to raise a warning; by default this is suppressed by django\n        * To ensure `QueryCountWarning` is never suppressed  \n\n```python\nwarnings.simplefilter(\'always\', allianceutils.middleware.QueryCountWarning)\n```\n\n* To increase the query count limit for a given request, you can increase `request.QUERY_COUNT_WARNING_THRESHOLD`\n    * Rather than hardcode a new limit, you should increment the existing value\n    * If `request.QUERY_COUNT_WARNING_THRESHOLD` is falsy then checks are disabled for this request \n\n```python\ndef my_view(request, *args, **kwargs):\n    request.QUERY_COUNT_WARNING_THRESHOLD += 10\n    ...\n\n```\n \n\n### Migrations\n\n#### Run SQL function\n* Wrapper to `RunSQL` that reads SQL from a file instead of inline in python\n* The reason you would do this as an external file & function is so that squashed migrations don\'t become unwieldy (django will inline and strip whitespace in the SQL)\n\nUsage:\n```python\nclass Migration(migrations.Migration):\n    # ...\n    operations = [\n        allianceutils.migrations.RunSQLFromFile(\'my_app\', \'0001_intial.sql\'),\n    ]\n```\n\n### Models\n\n#### Utility functions / classes\n\n##### combine_querysets_as_manager\n* `allianceutils.models.combine_querysets_as_manager(Iterable[Queryset]) -> Manager`\n* Replacement for django_permanent.managers.MultiPassThroughManager which no longer works in django 1.8\n* Returns a new Manager instance that passes through calls to multiple underlying queryset_classes via inheritance\n\n##### NoDeleteModel\n\n* A model that blocks deletes in django\n    * Can still be deleted with manual queries\n* Read django docs about [manager inheritance](https://docs.djangoproject.com/en/stable/topics/db/managers/#custom-managers-and-model-inheritance)\n    * If you wish add your own manager, you need to combine the querysets:\n\n```python\nclass MyModel(NoDeleteModel):\n        objects = combine_querysets_as_manager(NoDeleteQuerySet, MyQuerySet)\n```  \n\n#### GenericUserProfile\nAllows you to iterate over a `User` table and have it return a corresponding `Profile` record without generating extra queries\n\nMinimal example:\n\n```python\n# ------------------------------------------------------------------\n# base User model \n\n# If you\'re using django auth instead of authtools, you can just use\n# GenericUserProfileManager instead of having to make your own manager class\nclass UserManager(GenericUserProfileManagerMixin, authtools.models.UserManager):\n    pass\n\nclass User(GenericUserProfile, authtools.models.AbstractEmailUser):\n    objects = UserManager()\n    profiles = UserManager(select_related_profiles=True)\n    \n    # these are the tables that should be select_related()/prefetch_related()\n    # to minimise queries\n    related_profile_tables = [\n        \'customerprofile\',\n        \'adminprofile\',\n    ]\n\n    def natural_key(self):\n        return (self.email,)\n        \n    # the default implementation will iterate through the related profile tables\n    # and return the first profile it can find. If you have custom logic for\n    # choosing the profile for a user then you can do that here\n    #\n    # You would normally not access this directly but instead use the`.profile`\n    # property that caches the return value of `get_profile()` and works\n    # correctly for both user and profile records  \n    def get_profile(self) -> Model:\n        # custom logic\n        if datetime.now() > datetime.date(2000,1,1):\n            return self\n        return super().get_profile()\n\n\n# ------------------------------------------------------------------\n# Custom user profiles\nclass CustomerProfile(User):\n    customer_details = models.CharField(max_length=191)\n\n\nclass AdminProfile(User):\n    admin_details = models.CharField(max_length=191)\n\n# ------------------------------------------------------------------\n# Usage:\n\n# a list of User records\nusers = list(User.objects.all())\n\n# a list of Profile records: 1 query\n# If a user has no profile then you get the original User record back\nprofiles = list(User.profiles.all())\n\n# we can explicitly perform the transform on the queryset\nprofiles = list(User.objects.select_related_profiles().all())\n\n# joining to profile tables: 1 query\n# This assumes that RetailLocation.company.manager is a FK ref to the user table\n# The syntax is a bit different because we can\'t modify the query generation\n# in an unrelated table \nqs = RetailLocation.objects.all()\nqs = User.objects.select_related_profiles(qs, \'company__manager\')\nlocation_managers = list((loc, loc.company.manager.profile) for loc in qs.all())\n```\n\n* There is also an authentication backend that will load profiles instead of just User records\n* If the `User` model has no `get_profile()` method then this backend is equivalent to the built-in django `django.contrib.auth.backends.ModelBackend`\n\n```python\n# ------------------------------------------------------------------\n# Profile authentication middleware\nAUTH_USER_MODEL = \'my_site.User\'\nAUTHENTICATION_BACKENDS = [\n    \'allianceutils.auth.backends.ProfileModelBackend\',\n]\n\n\ndef my_view(request):\n    # standard django AuthenticationMiddleware will call the authentication backend\n    profile = request.user  \n    return HttpResponse(\'Current user is \' + profile.username)\n\n```\n\n* Limitations:\n    * Profile iteration does not work with `.values()` or `.values_list()`\n    \n#### raise_validation_errors\n\n* The `raise_validation_errors` context manager enables cleaner code for constructing validation\n    * [Django documentation](https://docs.djangoproject.com/en/stable/ref/models/instances/#django.db.models.Model.clean) recommends raising a `ValidationError` when you encounter a problem\n    * This creates a poor user experience if there are multiple errors: the user only sees the first error and has to resubmit a form multiple times to fix problems\n* `raise_validation_errors` accepts an (optional) function to wrap\n    * The context manager returns a `ValidationError` subclass with an `add_error` function that follows the same rules as `django.forms.forms.BaseForm.add_error`\n    * If the wrapped function raises a `ValidationError` then this will be merged into the `ValidationError` returned by the context manager\n    * If the wrapped function raises any other exception then this will not be intercepted and the context block will not be executed \n    * At the end of a block,\n        * If code in the context block raised an exception (including a `ValidationError`) then this will not be caught\n        * If `ValidationError` the context manager returned has any errors (either from `ve.add_error()` or from the wrapped function) then this will be raised \n\n```\n    def clean(self):\n        with allianceutils.models.raise_validation_errors(super().clean) as ve:\n            if some_condition:\n                ve.add_error(None, \'model error message\')\n            if other_condition:\n                ve.add_error(\'fieldname\', \'field-specific error message\')\n            if other_condition:\n                ve.add_error(None, {\n                    \'fieldname1\': field-specific error message\',\n                    \'fieldname2\': field-specific error message\',\n                })\n            if something_bad:\n                raise RuntimeError(\'Oh no!\') \n            \n            # at the end of the context, ve will be raised if it contains any errors\n            #   - unless an exception was raised in the block (RuntimeError example above) in which case\n            #     the raised exception will take precedence\n```\n\n* Sometimes you already have functions that may raise a `ValidationError` and `add_error()` will not help\n    * The `capture_validation_error()` context manager solves this problem\n    * Note that due to the way context managers work, each potential `ValidationError` needs its own with `capture_validation_error` context \n\n```\n    def clean(self):\n        with allianceutils.models.raise_validation_errors() as ve:\n             with ve.capture_validation_error():\n                 self.func1()\n             with ve.capture_validation_error():\n                 self.func2()\n             with ve.capture_validation_error():\n                 raise ValidationError(\'bad things\')\n            # all raised ValidationErrors will be collected, merged and raised at the end of this block\n```\n\n### Rules\n\n* Utility functions that return predicates for use with [django-rules](https://github.com/dfunckt/django-rules)\n\n```\nfrom allianceutils.rules import has_any_perms, has_perms, has_perm\n\n# requires at least 1 listed permission\nrules.add_perm(\'northwind.publish_book\', has_any_perms(\'northwind.is_book_author\', \'northwind.is_book_editor\'))\n\n# requires listed permission\nrules.add_perm(\'northwind.unpublish_book\', has_perm(\'northwind.is_book_editor\'))\n\n# requires all listed permissions\nrules.add_perm(\'northwind.sublicense_book\', has_perms(\'northwind.is_book_editor\', \'northwind.can_sign_contracts\'))\n\n```  \n\n### Serializers\n\n#### JSON Ordered\n\n* A version of django\'s core json serializer that outputs field in sorted order\n* The built-in one uses a standard `dict` with completely unpredictable order which causes json diffs to show spurious changes\n\n* Setup\n    * Add to `SERIALIZATION_MODULES` in your settings\n    * This will allow you to do fixture dumps with `--format json_ordered`\n    * Note that django treats this as the file extension to use\n\n```python\nSERIALIZATION_MODULES = {\n    \'json_ordered\': \'allianceutils.serializers.json_ordered\',\n}\n```\n\n### Template Tags\n\n#### render_entry_point\n\n* Replaces old usage of [django-webpack-loader](https://github.com/ezhome/django-webpack-loader)\n   * At time of writing django-webpack-loader does not have a stable release that [works with webpack 4](https://github.com/owais/django-webpack-loader/issues/218)\n   * Worked at bundle level rather than entry point. See below for how we embed tags based on entry point.\n* Reads JSON files generated by [EntryPointBundleTracker](https://gitlab.internal.alliancesoftware.com.au/alliance/webpack-dev-utils/) and embeds the required bundles in the page\n   * Will output tags for all resources of the specified type. eg. Given JSON structure of:\n   ```json\n    {\n      "status": "done",\n      "entrypoints": {\n        "admin": [\n          {\n            "name": "runtime.bundle.js",\n            "contentHash": "e2b781da02d36dad3aff"\n          },\n          {\n            "name": "common.bundle.js",\n            "contentHash": "639269b921c8cf869c5f"\n          },\n          {\n            "name": "common.bundle.css",\n            "contentHash": "d60a0fa36613ea58a23d"\n          },\n          {\n            "name": "admin.bundle.js",\n            "contentHash": "c78fb252d4e00207afef"\n          }\n        ]\n      },\n      "publicPath": "/assets/"\n    }\n   ```\n   \n   Output for `{% render_entry_point \'admin\' \'js\' %}`:\n\n   ```html\n   <script type="text/javascript" src="/assets/runtime.bundle.js?e2b781da02d36dad3aff"></script>\n   <script type="text/javascript" src="/assets/common.bundle.js?639269b921c8cf869c5f"></script>\n   <script type="text/javascript" src="/assets/admin.bundle.js?c78fb252d4e00207afef"></script>\n   ```\n   \n   Output for `{% render_entry_point \'admin\' \'css\' %}`:\n\n   ```html\n   <link type="text/css" href="/assets/common.bundle.css?d60a0fa36613ea58a23d" rel="stylesheet" />\n   ```\n* As an entry point maps to a single HTML file it\'s expected you would only use this tag for a single entry point on a page but generally would call it for both `js` and `css`\n* Arguments\n  * `entry_point_name` - Name of the entry point. This should match one of the entries to \'entry\' in the webpack config.\n  * `resource_type` - The resource type to embed; either `js` or `css`.\n* Optional Arguments\n  * `attrs` - String representing extra attributes to pass to the HTML tag\n  * `config=\'DEFAULT\'` - String index into the settings `WEBPACK_LOADER` dict. Defaults to \'DEFAULT\'.\n* Config\n  * Configuration can be specified via the `WEBPACK_LOADER` setting. This is a dict indexed by the config name (defaults to \'DEFAULT\')\n  * Options\n    * `STATS_FILE` - the path to the stats file to read\n    * `INCLUDE_QUERY_HASH` - whether to include the content hash in the query string. Defaults to `true`.\n    * `BASE_URL` - a URL to prepend to all chunks when rendered. This can be used when files are stored on a different host (eg. CDN).\n\n* Example Usage\n\n```html\n{% load alliance_webpack %}\n<html>\n<head>\n  {% render_entry_point \'app\' \'css\' %}\n</head>\n<body>\n  \n  ...\n  \n  {% if DEBUG %}\n    {# See https://reactjs.org/docs/cross-origin-errors.html #}\n    {% render_entry_point entry_point \'js\' attrs="crossorigin" %}\n  {% else %}\n    {% render_entry_point entry_point \'js\' %}\n  {% endif %}\n</body>\n</html>\n```\n\n#### default_value\n\n* Sets default value(s) on the context in a template\n* This is useful because some built-in django templates raise warnings about unset variables (eg `is_popup` in the django admin template)\n* Note that some tags (eg `with`) save & restore the context state; if done inside such a template tag `default_value` will not persist when the state is restored \n\n```html\n{% load default_value %}\n{{ default_value myvar1=99 myvar2=myvar1|upper }}\n{{ myvar1 }} {{ myvar2 }}\n```\n\n### Util\n\n#### add_autoreload_extra_files\n\n* Adds files to the autoreloader watch list\n    * Works with both the built-in [`runserver`](https://docs.djangoproject.com/en/stable/ref/django-admin/#runserver)\n      and [`runserver_plus`](https://django-extensions.readthedocs.io/en/latest/runserver_plus.html) from `django-extensions`\n    * If `DEBUG` is not enabled then this will do nothing\n    * This should be called from inside the\n      [`ready()`](https://docs.djangoproject.com/en/stable/ref/applications/#django.apps.AppConfig.ready) method of\n      an [`AppConfig`](https://docs.djangoproject.com/en/stable/ref/applications/#configuring-applications) \n  \n```python\nclass MyAppConfig(AppConfig):\n    def ready(self):\n        extra_files = [\n          "/data/file.csv",\n        ]\n        add_autoreload_extra_files(extra_files)\n```\n\n#### camelize\n\n* Better version of [djangorestframework-camel-case](https://github.com/vbabiy/djangorestframework-camel-case)\n    * DRF-CC camel cases every single key in the data tree.\n* These functions allow you to indicate that certain keys are data, not field names\n\n\n```python\ntree = {\n    "first_name": "Mary",\n    "last_name": "Smith",\n    "servers": {\n        "server_west.mycompany.com": {\n            \'user_accounts\': {\n                \'mary_smith\': {\n                    \'home_dir\': \'/home/mary_smith\',\n                },\n            },\n        },\n    },\n}\n# the keys at tree[\'servers\'] and tree[\'servers\'][\'serve_west.mycompany.com\'][\'user_accounts\'] will not be camel cased\noutput_tree = allianceutils.util.camelize(tree, ignore=[\'servers\', \'servers.*.user_accounts\'])\noutput_tree == {\n    "firstName": "Mary",\n    "lastName": "Smith",\n    "servers": {\n        "server_west.mycompany.com": {\n            \'userAccounts\': {\n                \'mary_smith\': {\n                    \'home_dir\': \'/home/mary_smith\',\n                },\n            },\n        },\n    },\n}\n\n```\n\n* `allianceutils.util.camelize(data, ignores)` - underscore case => camel case a json tree of data\n* `allianceutils.util.underscorize(data, ignores)` - camel case => underscore case a json tree of data\n* `allianceutils.util.camel_to_underscore(str)` - underscore case => camel case a string\n* `allianceutils.util.underscore_to_camel(str)` - camel case => underscore case a string\n* It is assumed that words will not begin with numbers:\n    * `zoo_foo99_bar` is okay\n    * `zoo_foo_99bar` will result in an irreversible transformation (`zooFoo99bar` => `zoo_foo99_bar`) \n\n#### get_firstparty_apps\n\n`util.get_firstparty_apps` can be used to retrieve app_configs considered to be first party, ie, all that does not come from a third party package.\nThis is beneficial when you want to write your own checks by excluding things you dont really care - a sample usage can be found inside \'checks.py\', or\nused as such:\n\n```python\n\nfrom allianceutils.util import get_firstparty_apps\n\napp_configs = get_firstparty_apps()\nmodels_to_be_checked = {}\n\nfor app_config in app_configs:\n    models_to_be_checked.update({\n        model._meta.label: model\n        for model\n        in app_config.get_models()\n    })\n```\n\n#### python_to_django_date_format\n\n* Converts a python [strftime/strptime](https://docs.python.org/3/library/datetime.html#strftime-strptime-behavior) datetime format string into a [django template/PHP](https://docs.djangoproject.com/en/stable/ref/templates/builtins/#std:templatefilter-date) date format string\n* Codes with no equivalent will be dropped\n\nExample:\n```python\nallianceutils.util.date.python_to_django_date_format("%Y%m%d %H%M%S")\n# returns "Ymd His"\n```\n\n#### retry_fn\n\n* Repeatedly (up to a hard limit) call specified function while it raises specified exception types or until it returns\n\n```python\nfrom allianceutils.util import retry_fn\n\n# Generate next number in sequence for a model\n# Number here has unique constraint resulting in IntegrityError being thrown\n# whenever a duplicate is added. can be useful for working around mysql\'s lack\n# of sequences\ndef generate_number():\n    qs = MyModel.objects.aggregate(last_number=Max(F(\'card_number\')))\n    next_number = (qs.get(\'last_card_number\') or 0) + 1\n    self.card_number = card_number\n    super().save(*args, **kwargs)\nretry_fn(generate_number, (IntegrityError, ), 10)\n```\n\n## Experimental\n\n* These are experimental and may change without notice\n    * `document_reverse_accessors` management command  \n\n## Changelog\n\nSee [CHANGELOG.md](CHANGELOG.md)\n\n## Development\n\n### Release Process\n\n#### Poetry Config\n* Add test repository\n    * `poetry config repositories.testpypi https://test.pypi.org/legacy/`\n    * Generate an account API token at https://test.pypi.org/manage/account/token/\n    * `poetry config pypi-token.testpypi ${TOKEN}`\n        * On macs this will be stored in the `login` keychain at `poetry-repository-testpypi`\n* Main pypi repository\n    * Generate an account API token at https://pypi.org/manage/account/token/\n    * `poetry config pypi-token.pypi ${TOKEN}`\n        * On macs this will be stored in the `login` keychain at `poetry-repository-pypi`\n\n#### Publishing a New Release\n    * Update CHANGELOG.md with details of changes and new version\n    * Run `bin/build.py`. This will extract version from CHANGELOG.md, bump version in `pyproject.toml` and generate a build for publishing\n    * Tag with new version and update the version branch:\n        * `ver=$( poetry version --short ) && echo "Version: $ver"`\n        * `git tag v/$ver`\n        * `git push --tags`\n    * To publish to test.pypi.org\n        * `poetry publish --repository testpypi`\n    * To publish to pypi.org\n        * `poetry publish`\n\n\n',
-    'author': 'Alliance Software',
-    'author_email': 'support@alliancesoftware.com.au',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/AllianceSoftware/django-allianceutils/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6',
+# Alliance Utils
+
+![CI Tests](https://github.com/AllianceSoftware/django-allianceutils/workflows/Django%20CI/badge.svg)
+
+A collection of utilities for django projects from [Alliance Software](https://www.alliancesoftware.com.au/).
+
+* [Installation](#installation)
+* [Usage](#usage)
+    * [API](#api)
+    * [Auth](#auth)
+    * [Decorators](#decorators)
+    * [Management](#management)
+        * [Commands](#commands)
+        * [Checks](#checks)
+    * [Middleware](#middleware)
+    * [Migrations](#migrations)
+    * [Models](#models)
+    * [Rules](#rules)
+    * [Serializers](#serializers)
+    * [Template Tags](#template-tags)
+    * [Util](#util)
+* [Changelog](#changelog)
+
+## Installation
+
+`pip install django-allianceutils`
+
+## System Requirements
+
+* Tested with django 3.2 and 4.2
+  * Pull requests accepted for other versions, but at minimum we test against current LTS versions
+* Python >=3.8
+
+## Usage
+
+### API
+
+#### Mixins
+
+##### SerializerOptInFieldsMixin
+
+Regulates fields exposed on a Serializer by default & as requested based on query parameters or context.
+
+* Pass 'include_fields' / 'opt_in_fields' thru query params or context to use.
+* multiple fields can either be separated by comma
+  eg, `/?include_fields=first_name,email&opt_in_fields=gait_recognition_prediction`
+* or passed in the traditional list fashion
+  eg, `/?include_fields=first_name&include_fields=email&opt_in_fields=gait_recognition_prediction`
+* or mixed eg, `/?include_fields=first_name,email&include_fields=boo`
+* By default, all "fields" defined in serializer, minus those listed in "opt_in_fields" would be returned.
+* If "include_fields" is supplied, only fields requested this way would be returned.
+* If "opt_in_fields" is supplied, fields requested this way PLUS fields from #1 or #2 would be returned.
+* Pinned fields are always returned (defaults to primary key)
+
+Usage:
+
+```python
+class UserSerializer(SerializerOptInFieldsMixin, ModelSerializer):
+    class Meta:
+        model = User
+        fields = (
+            "id",
+            "first_name",
+            "last_name",
+            "email",
+            "region",
+            "activated_at",
+            "is_staff",
+        )
+        # These fields only returned if explicitly requested
+        opt_in_only_fields = ["activated_at", "is_staff"]
+```
+
+#### Permissions
+
+##### register_custom_permissions
+
+* Creates permissions that have no model by linking them to an empty content type
+* Django creates permissions as part of
+  the [`post_migrate` signal](https://docs.djangoproject.com/en/stable/ref/signals/#post-migrate)
+
+Usage
+
+```py
+def on_post_migrate(sender, **kwargs):
+    register_custom_permissions("myapp", ("my_perm", "My Permission"))
+```
+
+##### SimpleDjangoObjectPermissions
+
+Permission class for Django Rest Framework that adds support for object level permissions.
+
+Differs from just DRF's [DjangoObjectPermissions](https://www.django-rest-framework.org/api-guide/permissions/#object-level-permissions) because it
+* does not require a queryset
+* uses the same permission for every request http method and ViewSet method 
+
+Notes
+* The default django permissions system will [always return False](https://docs.djangoproject.com/en/stable/topics/auth/customizing/#handling-object-permissions) if given an object; you must be using another permissions backend
+* As per [DRF documentation](http://www.django-rest-framework.org/api-guide/permissions/#object-level-permissions): get_object() is only required if you want to implement object-level permissions
+* **WARNING** If you override `get_object()` then you need to *manually* invoke `self.check_object_permissions(self.request, obj)`
+* Will attempt to check permission both globally and on a per-object basis but considers it an error if the check returns True for both
+*   
+
+Usage
+* See [DRF permissions policy](https://www.django-rest-framework.org/api-guide/permissions/#setting-the-permission-policy) for details on apply Permissions policies globally
+
+* To apply to a specific view you need to set `permission_required`
+```python
+class MyAPIView(SimpleDjangoObjectPermissions, APIView):
+        permission_required = 'my_module.my_permission'
+        permission_classes = [allianceutils.api.permissions.SimpleDjangoObjectPermissions] 
+```
+
+If you have no object level permissions (eg. from rules) then it will just do a static permission check.
+
+##### GenericDjangoViewsetPermissions
+
+* Map viewset actions to Django permissions.
+  * The model used for permission is extracted from the ViewSet
+    * If you implement `get_permission_model` on the ViewSet that will be used
+    * Otherwise it will call `get_queryset` on the ViewSet and extract the model from the returned queryset 
+ * To alter this behaviour extends `GenericDjangoViewsetPermissions` and implement `get_model` 
+* Usage example:
+```
+class MyViewSet(GenericDjangoViewsetPermissions, viewsets.ModelViewSet):
+    queryset = MyModel.objects.all()
+    serializer_class = MySerializer
+```
+* `GenericDjangoViewsetPermissions.default_actions_to_perms_map` defines the default set of permissions. These can be extended or overridden using `actions_to_perms_map`:
+```
+class MyViewSet(GenericDjangoViewsetPermissions, viewsets.ModelViewSet):
+
+    # ...
+
+    actions_to_perms_map = {
+        'create': []
+    }
+```
+* No permissions will be required for the create action, but permissions for other actions will remain unchanged.
+* By default permissions checks are passed the relevant model instance for per-object permission checks
+    * This assumes that your backend doesn't ignore the model object (default django permissions simply ignore any object passed to a permissions check)
+    * Since there is no model object, functions decorated with `@list_route` will pass `None` as the permissions check object
+
+#### Parsers
+
+##### CamelCaseJSONParser
+
+Parser that recursively turns camelcase keys into underscored keys for JSON data.
+This can be set globally on the [DEFAULT_PARSER_CLASSES](https://www.django-rest-framework.org/api-guide/settings/#default_parser_classes)
+setting or on a ViewSet on the `parser_classes` property.
+
+##### CamelCaseMultiPartJSONParser
+
+Parser that recursively turns camelcase keys into underscored keys for JSON data and handles file uploads.
+This parser supports receiving JSON data where a field value anywhere in the structure can be a file.
+This is achieved on the frontend by converting a structure like:
+
+```js
+{
+    name: 'Test',
+    photo: File,
+}
+```
+
+And converting it to
+
+```js
+{
+    name: 'Test',
+    photo: '____ATTACHED_FILE_ID_1',
+}
+```
+
+This is then set on a field `jsonData` and the file is set on `____ATTACHED_FILE_ID_1` and submitted
+as multipart.
+This parser then handles parsing the JSON data into a dict and setting each attached file on the
+correct key in the dict.
+Note that this works with nested data (ie. any File anywhere in a nested JSON structure is supported).
+To activate this behaviour the `X-MultiPart-JSON` header must be set to '1' or 'true'. If this header
+is not set it falls back to the default behaviour of MultiPartParser
+This can be set globally on the [DEFAULT_PARSER_CLASSES](https://www.django-rest-framework.org/api-guide/settings/#default_parser_classes)
+setting or on a ViewSet on the `parser_classes` property.
+Example frontend code to activate:
+```js
+let fileCount = 0;
+const files = {};
+const replacer = (key, value) => {
+    if (value instanceof File) {
+        const id = `____ATTACHED_FILE_ID_${fileCount++}`;
+        files[id] = value;
+        return id;
+    }
+    return value;
+};
+const stringifiedData = JSON.stringify(data, replacer);
+const body = new FormData();
+const body.append('jsonData', stringifiedData);
+for (const [fileKey, file] of Object.entries(files)) {
+    body.append(fileKey, file);
+}
+// eg. using a presto Endpoint
+await myEndpoint.execute({
+    body,
+    headers: {
+        // Remove default content type from endpoint (eg. json)
+        'Content-Type': undefined,
+        'X-MultiPart-JSON': true,
+    },
+});
+```
+
+#### Renderers
+
+##### CamelCaseJSONRenderer
+
+Renderer that recursively turns underscore-cased keys into camel-cased keys.
+This can be set globally on the [DEFAULT_RENDERER_CLASSES](https://www.django-rest-framework.org/api-guide/settings/#default_renderer_classes)
+setting or on a ViewSet on the `renderer_classes` property.
+
+### Auth
+
+#### MinimalModelBackend
+
+* `allianceutils.auth.backends.MinimalModelBackend`
+    * Replaces the built-in django [ModelBackend](https://docs.djangoproject.com/en/stable/ref/contrib/auth/#django.contrib.auth.backends.ModelBackend)
+    * Provides django model-based authentication
+    * Removes the default authorization (permissions checks) except for checking `is_superuser` 
+
+#### ProfileModelBackend
+
+* Backends for use with [GenericUserProfile](#GenericUserProfile); see code examples there
+* `allianceutils.auth.backends.ProfileModelBackendMixin` - in combo with [AuthenticationMiddleware](https://docs.djangoproject.com/en/stable/ref/middleware/#django.contrib.auth.middleware.AuthenticationMiddleware) will set user profiles on `request.user`
+  * If you want  
+      * ~`allianceutils.auth.backends.ProfileModelBackend`~ - convenience class combined with case insensitive username & default django permissions backend
+          * this depended on [`authtools`](https://django-authtools.readthedocs.io/en/latest/) which appears to have been
+            abandoned and does not work with django >= 3.
+            If using django 3 then we recommended that you create your own backend in your app:
+            ```python
+              class ProfileModelBackend(ProfileModelBackendMixin, MinimalModelBackend):
+                  # you'll need to implement case insensitivity either here or in the User Model  
+                  pass
+            ```
+
+### Decorators
+
+#### gzip_page_ajax
+
+* Smarter version of django's [gzip_page](https://docs.djangoproject.com/en/stable/topics/http/decorators/#django.views.decorators.gzip.gzip_page):
+    * If settings.DEBUG not set, will always gzip
+    * If settings.DEBUG set, will gzip only if request is an ajax request
+* This allows you to use django-debug-toolbar in DEBUG mode (if you gzip a response then the debug toolbar middleware won't run)
+
+Example
+
+```
+
+@allianceutils.views.decorators.gzip_page_ajax
+def my_view(request: HttpRequest) -> httpResponse:
+    data = {
+        "message": "Hello World",
+    }
+    return django.http.JsonResponse(data) 
+
+```
+
+#### method_cache
+
+* Caches the results of a method on the object instance
+* There is no thread synchronization so in some circumstances the method may be called multiple times if multiple threads share the object 
+* Only works for regular object methods with no arguments other than `self`.
+    * Does not support `@classmethod` or `@staticmethod`
+    * If you want more powerful caching behaviour then you can
+      * use [`methodtools`](https://pypi.org/project/methodtools/)
+      * wrap `cachetools` (examples [here](https://github.com/tkem/cachetools/issues/107#issuecomment-436274285))
+* Similar to [`@cached_property`](https://docs.python.org/3/library/functools.html#functools.cached_property) except that it works on methods instead of properties
+* Differs from [`@lru_cache()`](https://docs.python.org/3/library/functools.html#functools.lru_cache) in that
+    * `lru_cache` uses a single cache for each decorated function
+    * `lru_cache` will block garbage collection of values in the cache 
+    * A `cache_clear()` method is attached to the function but unlike `lru_cache` it is scoped to an object instance   
+
+Usage
+```python
+class MyViewSet(ViewSet):
+
+    # ...
+
+    @method_cache
+    def get_object(self):
+        return super().get_object()
+
+obj = MyViewSet()
+obj.get_object() is obj.get_object()
+obj.get_object.cache_clear()   
+```
+
+### Management
+
+#### Commands
+
+##### OptionalAppCommand
+
+* A utility class that extends `django.core.management.base.BaseCommand` and adds optional argument(s) for django apps
+* If app names are passed on the command line `handle_app_config()` will be called with the `AppConfig` for each app otherwise it will be called with every first-party app (as determined by `isort`)
+
+
+Example:
+
+```
+class Command(allianceutils.management.commands.base.OptionalAppCommand):
+    def add_arguments(self, parser):
+        super().add_arguments(parser)
+        parser.add_argument('--type', choices=('name', 'label'), default='name')
+
+    def handle_app_config(self, app_config: AppConfig, **options):
+        if options['type'] == 'name':
+            print(f"Called with {app_config.name}")
+        if options['type'] == 'label':
+            print(f"Called with {app_config.label}")
+```  
+
+##### print_logging
+
+* Displays the current logging configuration in a hierarchical fashion
+* Requires [`logging_tree`](https://pypi.python.org/pypi/logging_tree) to be installed
+
+#### Checks
+
+* Checks with no configuration are functions that can be passed directly to [register](https://docs.djangoproject.com/en/3.1/topics/checks/)
+* Checks that expect parameters are classes that need to be instantiated
+
+Setting up django hooks:
+
+```python
+from django.apps import AppConfig
+from django.core.checks import register
+from django.core.checks import Tags
+
+from allianceutils.checks import check_admins
+from allianceutils.checks import check_db_constraints
+from allianceutils.checks import CheckExplicitTableNames
+from allianceutils.checks import check_git_hooks
+from allianceutils.checks import CheckReversibleFieldNames
+from allianceutils.checks import CheckUrlTrailingSlash
+
+class MyAppConfig(AppConfig):
+    # ...
+
+    def ready(self):
+        register(check=check_admins, tags=Tags.admin, deploy=True)
+        register(check=check_db_constraints, tags=Tags.database)
+        register(check=CheckExplicitTableNames(), tags=Tags.models)
+        register(check=check_git_hooks, tags=Tags.admin)
+        register(check=CheckReversibleFieldNames(), tags=Tags.models)
+        register(check=CheckUrlTrailingSlash(expect_trailing_slash=True), tags=Tags.url)        
+```
+
+##### CheckUrlTrailingSlash
+
+* Checks that your URLs are consistent with the `settings.APPEND_SLASH`  
+* Arguments:
+    * `ignore_attrs` - skip checks on url patterns where an attribute of the pattern matches something in here (see example above)
+        * Most relevant attributes of a `RegexURLResolver`:
+            * `_regex` - string used for regex matching. Defaults to `[r'^$']`
+            * `app_name` - app name (only works for `include()` patterns). Defaults to `['djdt']` (django debug toolbar)
+            * `namespace` - pattern defines a namespace
+            * `lookup_str` - string defining view to use. Defaults to `['django.views.static.serve']`
+        * Note that if you skip a resolver it will also skip checks on everything inside that resolver
+* Note: If using Django REST Framework's [`DefaultRouter`](http://www.django-rest-framework.org/api-guide/routers/#defaultrouter) then you need to turn off `include_format_suffixes`:
+
+```
+router = routers.DefaultRouter(trailing_slash=True)
+router.include_format_suffixes = False
+router.register(r'myurl', MyViewSet)
+urlpatterns += router.urls
+```
+
+
+##### check\_admins
+
+* Checks that `settings.ADMINS` has been properly set in settings files.
+
+##### check\_git\_hooks
+
+* Checks that git hookshave been set up, one of:
+  * `.git/hooks` directory has been symlinked to the project's `git-hooks`
+  * [`husky`](https://github.com/typicode/husky) hooks have been installed 
+* 
+
+##### check\_db\_constraints
+
+* Checks that all models that specify `db_constraints` in their Meta will generate unique constraint names when truncated by the database.
+
+##### CheckExplicitTableNames
+
+* Checks that all first-party models have `db_table` explicitly defined on their Meta class, and the table name is in lowercase
+* Arguments:
+    * `enforce_lowercase` - check that there are no uppercase characters in the table name
+    * `ignore_labels` - if an app label (eg `silk`) or app_label + model labels (eg `silk.request`)
+        matches something in `ignore_labels` then it will be ignored.
+        * `allianceutils.checks.DEFAULT_TABLE_NAME_CHECK_IGNORE` contains a default list of apps/models to ignore
+        * Can be either a `str` or a regex (anything that contains a `.match()` method) 
+
+##### CheckReversibleFieldNames
+
+* Checks that all models have fields names that are reversible with `underscorize`/`camelize`/`camel_to_underscore`/`underscore_to_camel`
+* Arguments:
+    * `ignore_labels` - ignore these apps/models: see `CheckExplicitTableNames`
+
+### Middleware
+
+#### HttpAuthMiddleware
+
+* Middleware to enable basic http auth to block unwanted traffic from search engines and random visitors
+    * Intended to be used on dev / staging servers
+    * Is not a full authorization system: is a single hardcoded username/password and should be used on top of a proper authorization system
+
+* Setup
+    * Add `allianceutils.middleware.HttpAuthMiddleware` to `MIDDLEWARE`.
+    * Add `HTTP_AUTH_USERNAME` and `HTTP_AUTH_PASSWORD` to appropriate setting file, e.g. `settings/production_staging.py`
+        * Remember that you shouldn't be hardcoding credentials in code: read content from env vars or file
+
+#### CurrentUserMiddleware
+
+* Middleware to enable accessing the currently logged-in user without a request object.
+    * Assumes that `threading.local` is not shared between requests (an assumption also made by django internationalisation) 
+
+* Setup
+    * Add `allianceutils.middleware.CurrentUserMiddleware` to `MIDDLEWARE`.
+
+* Usage
+
+```python
+from allianceutils.middleware import CurrentUserMiddleware
+
+user = CurrentUserMiddleware.get_user()
+```
+
+#### QueryCountMiddleware
+
+* Warns if query count reaches a given threshold
+    * Threshold can be changed by setting `settings.QUERY_COUNT_WARNING_THRESHOLD`
+
+* Usage
+    * Add `allianceutils.middleware.CurrentUserMiddleware` to `MIDDLEWARE`.
+    * Uses the `warnings` module to raise a warning; by default this is suppressed by django
+        * To ensure `QueryCountWarning` is never suppressed  
+
+```python
+warnings.simplefilter('always', allianceutils.middleware.QueryCountWarning)
+```
+
+* To increase the query count limit for one request, you can call `QueryCountMiddleware.increase_threshold(request, increment)` 
+* To set the query count limit for one request you can call `QueryCountMiddleware.set_threshold(request, threshold)`
+  * Rather than hardcode a new limit, `increase_threshold()` is generally preferable
+  * This can be useful to disable checks entirely (pass `0` as the new limit)
+
+
+```python
+def my_view(request, *args, **kwargs):
+    request.QUERY_COUNT_WARNING_THRESHOLD += 10
+    ...
+
+```
+ 
+
+### Migrations
+
+#### Run SQL function
+* Wrapper to `RunSQL` that reads SQL from a file instead of inline in python
+* The reason you would do this as an external file & function is so that squashed migrations don't become unwieldy (django will inline and strip whitespace in the SQL)
+
+Usage:
+```python
+class Migration(migrations.Migration):
+    # ...
+    operations = [
+        allianceutils.migrations.RunSQLFromFile('my_app', '0001_intial.sql'),
+    ]
+```
+
+### Models
+
+#### Utility functions / classes
+
+##### combine_querysets_as_manager
+* `allianceutils.models.combine_querysets_as_manager(Iterable[Queryset]) -> Manager`
+* Replacement for django_permanent.managers.MultiPassThroughManager which no longer works in django 1.8
+* Returns a new Manager instance that passes through calls to multiple underlying queryset_classes via inheritance
+
+##### NoDeleteModel
+
+* A model that blocks deletes in django
+    * Can still be deleted with manual queries
+* Read django docs about [manager inheritance](https://docs.djangoproject.com/en/stable/topics/db/managers/#custom-managers-and-model-inheritance)
+    * If you wish add your own manager, you need to combine the querysets:
+
+```python
+class MyModel(NoDeleteModel):
+        objects = combine_querysets_as_manager(NoDeleteQuerySet, MyQuerySet)
+```  
+
+#### GenericUserProfile
+Allows you to iterate over a `User` table and have it return a corresponding `Profile` record without generating extra queries
+
+Minimal example:
+
+```python
+# ------------------------------------------------------------------
+# base User model 
+
+# If you're using django auth instead of authtools, you can just use
+# GenericUserProfileManager instead of having to make your own manager class
+class UserManager(GenericUserProfileManagerMixin, authtools.models.UserManager):
+    pass
+
+class User(GenericUserProfile, authtools.models.AbstractEmailUser):
+    objects = UserManager()
+    profiles = UserManager(select_related_profiles=True)
+    
+    # these are the tables that should be select_related()/prefetch_related()
+    # to minimise queries
+    related_profile_tables = [
+        'customerprofile',
+        'adminprofile',
+    ]
+    
+    # the default implementation will iterate through the related profile tables
+    # and return the first profile it can find. If you have custom logic for
+    # choosing the profile for a user then you can do that here
+    #
+    # You would normally not access this directly but instead use the`.profile`
+    # property that caches the return value of `get_profile()` and works
+    # correctly for both user and profile records  
+    def get_profile(self) -> Model:
+        # custom logic
+        if datetime.now() > datetime.date(2000,1,1):
+            return self
+        return super().get_profile()
+
+
+# ------------------------------------------------------------------
+# Custom user profiles
+class CustomerProfile(User):
+    customer_details = models.CharField(max_length=191)
+
+
+class AdminProfile(User):
+    admin_details = models.CharField(max_length=191)
+
+# ------------------------------------------------------------------
+# Usage:
+
+# a list of User records
+users = list(User.objects.all())
+
+# a list of Profile records: 1 query
+# If a user has no profile then you get the original User record back
+profiles = list(User.profiles.all())
+
+# we can explicitly perform the transform on the queryset
+profiles = list(User.objects.select_related_profiles().all())
+
+# joining to profile tables: 1 query
+# This assumes that RetailLocation.company.manager is a FK ref to the user table
+# The syntax is a bit different because we can't modify the query generation
+# in an unrelated table 
+qs = RetailLocation.objects.all()
+qs = User.objects.select_related_profiles(qs, 'company__manager')
+location_managers = list((loc, loc.company.manager.profile) for loc in qs.all())
+```
+
+* There is also an authentication backend that will load profiles instead of just User records
+* If the `User` model has no `get_profile()` method then this backend is equivalent to the built-in django `django.contrib.auth.backends.ModelBackend`
+
+```python
+# ------------------------------------------------------------------
+# Profile authentication middleware
+AUTH_USER_MODEL = 'my_site.User'
+AUTHENTICATION_BACKENDS = [
+    'allianceutils.auth.backends.ProfileModelBackend',
+]
+
+
+def my_view(request):
+    # standard django AuthenticationMiddleware will call the authentication backend
+    profile = request.user  
+    return HttpResponse('Current user is ' + profile.username)
+
+```
+
+* Limitations:
+    * Profile iteration does not work with `.values()` or `.values_list()`
+    
+#### raise_validation_errors
+
+* The `raise_validation_errors` context manager enables cleaner code for constructing validation
+    * [Django documentation](https://docs.djangoproject.com/en/stable/ref/models/instances/#django.db.models.Model.clean) recommends raising a `ValidationError` when you encounter a problem
+    * This creates a poor user experience if there are multiple errors: the user only sees the first error and has to resubmit a form multiple times to fix problems
+* `raise_validation_errors` accepts an (optional) function to wrap
+    * The context manager returns a `ValidationError` subclass with an `add_error` function that follows the same rules as `django.forms.forms.BaseForm.add_error`
+    * If the wrapped function raises a `ValidationError` then this will be merged into the `ValidationError` returned by the context manager
+    * If the wrapped function raises any other exception then this will not be intercepted and the context block will not be executed 
+    * At the end of a block,
+        * If code in the context block raised an exception (including a `ValidationError`) then this will not be caught
+        * If `ValidationError` the context manager returned has any errors (either from `ve.add_error()` or from the wrapped function) then this will be raised 
+
+```
+    def clean(self):
+        with allianceutils.models.raise_validation_errors(super().clean) as ve:
+            if some_condition:
+                ve.add_error(None, 'model error message')
+            if other_condition:
+                ve.add_error('fieldname', 'field-specific error message')
+            if other_condition:
+                ve.add_error(None, {
+                    'fieldname1': field-specific error message',
+                    'fieldname2': field-specific error message',
+                })
+            if something_bad:
+                raise RuntimeError('Oh no!') 
+            
+            # at the end of the context, ve will be raised if it contains any errors
+            #   - unless an exception was raised in the block (RuntimeError example above) in which case
+            #     the raised exception will take precedence
+```
+
+* Sometimes you already have functions that may raise a `ValidationError` and `add_error()` will not help
+    * The `capture_validation_error()` context manager solves this problem
+    * Note that due to the way context managers work, each potential `ValidationError` needs its own with `capture_validation_error` context 
+
+```
+    def clean(self):
+        with allianceutils.models.raise_validation_errors() as ve:
+             with ve.capture_validation_error():
+                 self.func1()
+             with ve.capture_validation_error():
+                 self.func2()
+             with ve.capture_validation_error():
+                 raise ValidationError('bad things')
+            # all raised ValidationErrors will be collected, merged and raised at the end of this block
+```
+
+### Rules
+
+* Utility functions that return predicates for use with [django-rules](https://github.com/dfunckt/django-rules)
+
+```
+from allianceutils.rules import has_any_perms, has_perms, has_perm
+
+# requires at least 1 listed permission
+rules.add_perm('northwind.publish_book', has_any_perms('northwind.is_book_author', 'northwind.is_book_editor'))
+
+# requires listed permission
+rules.add_perm('northwind.unpublish_book', has_perm('northwind.is_book_editor'))
+
+# requires all listed permissions
+rules.add_perm('northwind.sublicense_book', has_perms('northwind.is_book_editor', 'northwind.can_sign_contracts'))
+
+```  
+
+### Serializers
+
+#### JSON Ordered
+
+* A version of django's core json serializer that outputs field in sorted order
+* The built-in one uses a standard `dict` with completely unpredictable order which causes json diffs to show spurious changes
+
+* Setup
+    * Add to `SERIALIZATION_MODULES` in your settings
+    * This will allow you to do fixture dumps with `--format json_ordered`
+    * Note that django treats this as the file extension to use
+
+```python
+SERIALIZATION_MODULES = {
+    'json_ordered': 'allianceutils.serializers.json_ordered',
+}
+```
+
+### Template Tags
+
+#### render_entry_point
+
+* Replaces old usage of [django-webpack-loader](https://github.com/ezhome/django-webpack-loader)
+   * At time of writing django-webpack-loader does not have a stable release that [works with webpack 4](https://github.com/owais/django-webpack-loader/issues/218)
+   * Worked at bundle level rather than entry point. See below for how we embed tags based on entry point.
+* Reads JSON files generated by [EntryPointBundleTracker](https://gitlab.internal.alliancesoftware.com.au/alliance/webpack-dev-utils/) and embeds the required bundles in the page
+   * Will output tags for all resources of the specified type. eg. Given JSON structure of:
+   ```json
+    {
+      "status": "done",
+      "entrypoints": {
+        "admin": [
+          {
+            "name": "runtime.bundle.js",
+            "contentHash": "e2b781da02d36dad3aff"
+          },
+          {
+            "name": "common.bundle.js",
+            "contentHash": "639269b921c8cf869c5f"
+          },
+          {
+            "name": "common.bundle.css",
+            "contentHash": "d60a0fa36613ea58a23d"
+          },
+          {
+            "name": "admin.bundle.js",
+            "contentHash": "c78fb252d4e00207afef"
+          }
+        ]
+      },
+      "publicPath": "/assets/"
+    }
+   ```
+   
+   Output for `{% render_entry_point 'admin' 'js' %}`:
+
+   ```html
+   <script type="text/javascript" src="/assets/runtime.bundle.js?e2b781da02d36dad3aff"></script>
+   <script type="text/javascript" src="/assets/common.bundle.js?639269b921c8cf869c5f"></script>
+   <script type="text/javascript" src="/assets/admin.bundle.js?c78fb252d4e00207afef"></script>
+   ```
+   
+   Output for `{% render_entry_point 'admin' 'css' %}`:
+
+   ```html
+   <link type="text/css" href="/assets/common.bundle.css?d60a0fa36613ea58a23d" rel="stylesheet" />
+   ```
+* As an entry point maps to a single HTML file it's expected you would only use this tag for a single entry point on a page but generally would call it for both `js` and `css`
+* Arguments
+  * `entry_point_name` - Name of the entry point. This should match one of the entries to 'entry' in the webpack config.
+  * `resource_type` - The resource type to embed; either `js` or `css`.
+* Optional Arguments
+  * `attrs` - String representing extra attributes to pass to the HTML tag
+  * `config='DEFAULT'` - String index into the settings `WEBPACK_LOADER` dict. Defaults to 'DEFAULT'.
+* Config
+  * Configuration can be specified via the `WEBPACK_LOADER` setting. This is a dict indexed by the config name (defaults to 'DEFAULT')
+  * Options
+    * `STATS_FILE` - the path to the stats file to read
+    * `INCLUDE_QUERY_HASH` - whether to include the content hash in the query string. Defaults to `true`.
+    * `BASE_URL` - a URL to prepend to all chunks when rendered. This can be used when files are stored on a different host (eg. CDN).
+
+* Example Usage
+
+```html
+{% load alliance_webpack %}
+<html>
+<head>
+  {% render_entry_point 'app' 'css' %}
+</head>
+<body>
+  
+  ...
+  
+  {% if DEBUG %}
+    {# See https://reactjs.org/docs/cross-origin-errors.html #}
+    {% render_entry_point entry_point 'js' attrs="crossorigin" %}
+  {% else %}
+    {% render_entry_point entry_point 'js' %}
+  {% endif %}
+</body>
+</html>
+```
+
+#### default_value
+
+* Sets default value(s) on the context in a template
+* This is useful because some built-in django templates raise warnings about unset variables (eg `is_popup` in the django admin template)
+* Note that some tags (eg `with`) save & restore the context state; if done inside such a template tag `default_value` will not persist when the state is restored 
+
+```html
+{% load default_value %}
+{{ default_value myvar1=99 myvar2=myvar1|upper }}
+{{ myvar1 }} {{ myvar2 }}
+```
+
+### Util
+
+#### add_autoreload_extra_files
+
+* Adds files to the autoreloader watch list
+    * Works with both the built-in [`runserver`](https://docs.djangoproject.com/en/stable/ref/django-admin/#runserver)
+      and [`runserver_plus`](https://django-extensions.readthedocs.io/en/latest/runserver_plus.html) from `django-extensions`
+    * If `DEBUG` is not enabled then this will do nothing
+    * This should be called from inside the
+      [`ready()`](https://docs.djangoproject.com/en/stable/ref/applications/#django.apps.AppConfig.ready) method of
+      an [`AppConfig`](https://docs.djangoproject.com/en/stable/ref/applications/#configuring-applications) 
+  
+```python
+class MyAppConfig(AppConfig):
+    def ready(self):
+        extra_files = [
+          "/data/file.csv",
+        ]
+        add_autoreload_extra_files(extra_files)
+```
+
+#### camelize
+
+* Better version of [djangorestframework-camel-case](https://github.com/vbabiy/djangorestframework-camel-case)
+    * DRF-CC camel cases every single key in the data tree.
+* These functions allow you to indicate that certain keys are data, not field names
+
+
+```python
+tree = {
+    "first_name": "Mary",
+    "last_name": "Smith",
+    "servers": {
+        "server_west.mycompany.com": {
+            'user_accounts': {
+                'mary_smith': {
+                    'home_dir': '/home/mary_smith',
+                },
+            },
+        },
+    },
 }
+# the keys at tree['servers'] and tree['servers']['serve_west.mycompany.com']['user_accounts'] will not be camel cased
+output_tree = allianceutils.util.camelize(tree, ignore=['servers', 'servers.*.user_accounts'])
+output_tree == {
+    "firstName": "Mary",
+    "lastName": "Smith",
+    "servers": {
+        "server_west.mycompany.com": {
+            'userAccounts': {
+                'mary_smith': {
+                    'home_dir': '/home/mary_smith',
+                },
+            },
+        },
+    },
+}
+
+```
+
+* `allianceutils.util.camelize(data, ignores)` - underscore case => camel case a json tree of data
+* `allianceutils.util.underscorize(data, ignores)` - camel case => underscore case a json tree of data
+* `allianceutils.util.camel_to_underscore(str)` - underscore case => camel case a string
+* `allianceutils.util.underscore_to_camel(str)` - camel case => underscore case a string
+* It is assumed that words will not begin with numbers:
+    * `zoo_foo99_bar` is okay
+    * `zoo_foo_99bar` will result in an irreversible transformation (`zooFoo99bar` => `zoo_foo99_bar`) 
+
+#### get_firstparty_apps
+
+`util.get_firstparty_apps` can be used to retrieve app_configs considered to be first party, ie, all that does not come from a third party package.
+This is beneficial when you want to write your own checks by excluding things you dont really care - a sample usage can be found inside 'checks.py', or
+used as such:
+
+```python
+
+from allianceutils.util import get_firstparty_apps
+
+app_configs = get_firstparty_apps()
+models_to_be_checked = {}
+
+for app_config in app_configs:
+    models_to_be_checked.update({
+        model._meta.label: model
+        for model
+        in app_config.get_models()
+    })
+```
+
+#### python_to_django_date_format
+
+* Converts a python [strftime/strptime](https://docs.python.org/3/library/datetime.html#strftime-strptime-behavior) datetime format string into a [django template/PHP](https://docs.djangoproject.com/en/stable/ref/templates/builtins/#std:templatefilter-date) date format string
+* Codes with no equivalent will be dropped
+
+Example:
+```python
+allianceutils.util.date.python_to_django_date_format("%Y%m%d %H%M%S")
+# returns "Ymd His"
+```
+
+#### retry_fn
+
+* Repeatedly (up to a hard limit) call specified function while it raises specified exception types or until it returns
+
+```python
+from allianceutils.util import retry_fn
+
+# Generate next number in sequence for a model
+# Number here has unique constraint resulting in IntegrityError being thrown
+# whenever a duplicate is added. can be useful for working around mysql's lack
+# of sequences
+def generate_number():
+    qs = MyModel.objects.aggregate(last_number=Max(F('card_number')))
+    next_number = (qs.get('last_card_number') or 0) + 1
+    self.card_number = card_number
+    super().save(*args, **kwargs)
+retry_fn(generate_number, (IntegrityError, ), 10)
+```
+
+## Experimental
+
+* These are experimental and may change without notice
+    * `document_reverse_accessors` management command  
+
+## Changelog
+
+See [CHANGELOG.md](CHANGELOG.md)
+
+## Development
+
+* To create a clean local environment
+  * `python3 -m venv venv && source venv/bin/activate && pip install --upgrade pip` 
+  * `poetry install --no-root --sync --only=main --extras=""`
+  * Note that due to [a poetry bug](https://github.com/python-poetry/poetry/issues/7364) extras are currently not removed
+  * This will install the latest django version; if you want to test a specific django version you need to `pip install` it manually 
+* Dev dependencies
+  * `poetry install --no-root --sync --with=dev --extras "extras mysql postgres"`
+
+### Release Process
+
+#### Poetry Config
+* Add test repository
+    * `poetry config repositories.testpypi https://test.pypi.org/legacy/`
+    * Generate an account API token at https://test.pypi.org/manage/account/token/
+    * `poetry config pypi-token.testpypi ${TOKEN}`
+        * On macs this will be stored in the `login` keychain at `poetry-repository-testpypi`
+* Main pypi repository
+    * Generate an account API token at https://pypi.org/manage/account/token/
+    * `poetry config pypi-token.pypi ${TOKEN}`
+        * On macs this will be stored in the `login` keychain at `poetry-repository-pypi`
+
+#### Publishing a New Release
+    * Update CHANGELOG.md with details of changes and new version
+    * Run `bin/build.py`. This will extract version from CHANGELOG.md, bump version in `pyproject.toml` and generate a build for publishing
+    * Tag with new version and update the version branch:
+        * `ver=$( poetry version --short ) && echo "Version: $ver"`
+        * `git tag v/$ver`
+        * `git push --tags`
+    * To publish to test.pypi.org
+        * `poetry publish --repository testpypi`
+    * To publish to pypi.org
+        * `poetry publish`
+
+
+### Testing
+* To run test cases
+  * The django settings module is `test_allianceutils/settings.py`
+    * The following env vars are optional but you may want to set them if the default don't match your local setup: 
+      * `DB_NAME`
+      * `DB_HOST`
+      * `DB_PORT`
+      * `DB_USER`
+      * `DB_PASSWORD`
+* [tox](https://tox.wiki/en/latest/)
+  * used to run tests against different django/python/database versions
+  * `tox` to run all tests. Will require that you have a postgres & mysql server running.
+    * `tox -f django42` will run the subset of tests that cover django 4.2. Check `tox.ini` for the list of tested environments. 
+* When you push to github a [github Actions](https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python) workflow will be triggered (see `.github/workflows/django.yml`)  
+
 
 
-setup(**setup_kwargs)
+TODO:
+- [x] mypy checks all pass
+- [x] github actions pass
+- [] stricter mypy settings?
+- [] flake8, black, isort
+- [x] can cachetools replace @method_cache?
+  - No; can use methodtools but is another dependency. just documented the alternative 
+- [x] Use collections.abc:
+  - no, doesn't work with 3.8
+- [x] Use | instead of Optional, Union
+  - no, doesn't work with 3.8
+- [] Remove legacy build settings (poetry shouldn't need setup.cfg, MANIFEST.in so can we remove them?)
+
```

