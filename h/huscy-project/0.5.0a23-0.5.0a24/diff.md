# Comparing `tmp/huscy-project-0.5.0a23.tar.gz` & `tmp/huscy-project-0.5.0a24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy-project-0.5.0a23.tar", last modified: Fri Mar 10 12:13:35 2023, max compression
+gzip compressed data, was "huscy-project-0.5.0a24.tar", last modified: Thu Jun  8 12:58:37 2023, max compression
```

## Comparing `huscy-project-0.5.0a23.tar` & `huscy-project-0.5.0a24.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-03-10 12:13:35.263258 huscy-project-0.5.0a23/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       20 2022-06-30 08:39:15.000000 huscy-project-0.5.0a23/MANIFEST.in
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      253 2023-03-10 12:13:35.263258 huscy-project-0.5.0a23/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      911 2022-06-30 08:39:15.000000 huscy-project-0.5.0a23/README.md
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-03-10 12:13:35.259258 huscy-project-0.5.0a23/huscy_project/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      167 2023-03-10 12:06:30.000000 huscy-project-0.5.0a23/huscy_project/__init__.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-03-10 12:13:35.259258 huscy-project-0.5.0a23/huscy_project/__pycache__/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      358 2023-03-10 12:13:35.000000 huscy-project-0.5.0a23/huscy_project/__pycache__/__init__.cpython-310.pyc
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-03-10 12:13:35.259258 huscy-project-0.5.0a23/huscy_project/bin/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2022-06-30 08:39:15.000000 huscy-project-0.5.0a23/huscy_project/bin/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     2269 2022-06-30 08:39:15.000000 huscy-project-0.5.0a23/huscy_project/bin/huscy.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-03-10 12:13:35.263258 huscy-project-0.5.0a23/huscy_project/project_template/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-03-10 12:13:35.263258 huscy-project-0.5.0a23/huscy_project/project_template/config/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      417 2022-06-30 08:39:15.000000 huscy-project-0.5.0a23/huscy_project/project_template/config/asgi.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     3787 2023-03-10 12:04:05.000000 huscy-project-0.5.0a23/huscy_project/project_template/config/settings.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1748 2022-12-09 09:14:56.000000 huscy-project-0.5.0a23/huscy_project/project_template/config/urls.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      417 2022-06-30 08:39:15.000000 huscy-project-0.5.0a23/huscy_project/project_template/config/wsgi.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      368 2022-06-30 08:39:15.000000 huscy-project-0.5.0a23/huscy_project/project_template/makefile
--rwxrwxr-x   0 lotus     (1000) lotus     (1000)      662 2022-06-30 08:39:15.000000 huscy-project-0.5.0a23/huscy_project/project_template/manage.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-03-10 12:13:35.263258 huscy-project-0.5.0a23/huscy_project/project_template/media/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      102 2022-12-08 13:51:55.000000 huscy-project-0.5.0a23/huscy_project/project_template/media/README.md
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-03-10 12:13:35.263258 huscy-project-0.5.0a23/huscy_project/project_template/static/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      128 2022-12-08 13:51:55.000000 huscy-project-0.5.0a23/huscy_project/project_template/static/README.md
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-03-10 12:13:35.263258 huscy-project-0.5.0a23/huscy_project/project_template/templates/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1300 2022-06-30 08:39:15.000000 huscy-project-0.5.0a23/huscy_project/project_template/templates/index.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      113 2022-06-30 08:39:15.000000 huscy-project-0.5.0a23/huscy_project/views.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-03-10 12:13:35.259258 huscy-project-0.5.0a23/huscy_project.egg-info/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      253 2023-03-10 12:13:35.000000 huscy-project-0.5.0a23/huscy_project.egg-info/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      827 2023-03-10 12:13:35.000000 huscy-project-0.5.0a23/huscy_project.egg-info/SOURCES.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2023-03-10 12:13:35.000000 huscy-project-0.5.0a23/huscy_project.egg-info/dependency_links.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       56 2023-03-10 12:13:35.000000 huscy-project-0.5.0a23/huscy_project.egg-info/entry_points.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       27 2023-03-10 12:13:35.000000 huscy-project-0.5.0a23/huscy_project.egg-info/requires.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       14 2023-03-10 12:13:35.000000 huscy-project-0.5.0a23/huscy_project.egg-info/top_level.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2023-03-10 12:13:35.263258 huscy-project-0.5.0a23/setup.cfg
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      562 2023-03-10 11:23:38.000000 huscy-project-0.5.0a23/setup.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-08 12:58:37.279607 huscy-project-0.5.0a24/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       20 2022-06-30 08:39:15.000000 huscy-project-0.5.0a24/MANIFEST.in
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      253 2023-06-08 12:58:37.279607 huscy-project-0.5.0a24/PKG-INFO
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      911 2022-06-30 08:39:15.000000 huscy-project-0.5.0a24/README.md
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-08 12:58:37.279607 huscy-project-0.5.0a24/huscy_project/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      167 2023-06-08 12:56:52.000000 huscy-project-0.5.0a24/huscy_project/__init__.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-08 12:58:37.279607 huscy-project-0.5.0a24/huscy_project/__pycache__/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      358 2023-06-08 12:58:37.000000 huscy-project-0.5.0a24/huscy_project/__pycache__/__init__.cpython-310.pyc
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-08 12:58:37.279607 huscy-project-0.5.0a24/huscy_project/bin/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2022-06-30 08:39:15.000000 huscy-project-0.5.0a24/huscy_project/bin/__init__.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     2269 2022-06-30 08:39:15.000000 huscy-project-0.5.0a24/huscy_project/bin/huscy.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-08 12:58:37.279607 huscy-project-0.5.0a24/huscy_project/project_template/
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-08 12:58:37.279607 huscy-project-0.5.0a24/huscy_project/project_template/config/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      417 2022-06-30 08:39:15.000000 huscy-project-0.5.0a24/huscy_project/project_template/config/asgi.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     3787 2023-03-10 12:14:11.000000 huscy-project-0.5.0a24/huscy_project/project_template/config/settings.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1878 2023-06-08 12:58:10.000000 huscy-project-0.5.0a24/huscy_project/project_template/config/urls.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      417 2022-06-30 08:39:15.000000 huscy-project-0.5.0a24/huscy_project/project_template/config/wsgi.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      368 2022-06-30 08:39:15.000000 huscy-project-0.5.0a24/huscy_project/project_template/makefile
+-rwxrwxr-x   0 lotus     (1000) lotus     (1000)      662 2022-06-30 08:39:15.000000 huscy-project-0.5.0a24/huscy_project/project_template/manage.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-08 12:58:37.279607 huscy-project-0.5.0a24/huscy_project/project_template/media/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      102 2022-12-08 13:51:55.000000 huscy-project-0.5.0a24/huscy_project/project_template/media/README.md
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-08 12:58:37.279607 huscy-project-0.5.0a24/huscy_project/project_template/static/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      128 2022-12-08 13:51:55.000000 huscy-project-0.5.0a24/huscy_project/project_template/static/README.md
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-08 12:58:37.279607 huscy-project-0.5.0a24/huscy_project/project_template/templates/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1300 2022-06-30 08:39:15.000000 huscy-project-0.5.0a24/huscy_project/project_template/templates/index.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      113 2023-06-08 12:58:10.000000 huscy-project-0.5.0a24/huscy_project/views.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-06-08 12:58:37.279607 huscy-project-0.5.0a24/huscy_project.egg-info/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      253 2023-06-08 12:58:37.000000 huscy-project-0.5.0a24/huscy_project.egg-info/PKG-INFO
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      827 2023-06-08 12:58:37.000000 huscy-project-0.5.0a24/huscy_project.egg-info/SOURCES.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2023-06-08 12:58:37.000000 huscy-project-0.5.0a24/huscy_project.egg-info/dependency_links.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       56 2023-06-08 12:58:37.000000 huscy-project-0.5.0a24/huscy_project.egg-info/entry_points.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       27 2023-06-08 12:58:37.000000 huscy-project-0.5.0a24/huscy_project.egg-info/requires.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       14 2023-06-08 12:58:37.000000 huscy-project-0.5.0a24/huscy_project.egg-info/top_level.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2023-06-08 12:58:37.279607 huscy-project-0.5.0a24/setup.cfg
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      562 2023-03-10 12:14:11.000000 huscy-project-0.5.0a24/setup.py
```

### Comparing `huscy-project-0.5.0a23/README.md` & `huscy-project-0.5.0a24/README.md`

 * *Files identical despite different names*

### Comparing `huscy-project-0.5.0a23/huscy_project/bin/huscy.py` & `huscy-project-0.5.0a24/huscy_project/bin/huscy.py`

 * *Files identical despite different names*

### Comparing `huscy-project-0.5.0a23/huscy_project/project_template/config/settings.py` & `huscy-project-0.5.0a24/huscy_project/project_template/config/settings.py`

 * *Files identical despite different names*

### Comparing `huscy-project-0.5.0a23/huscy_project/project_template/config/urls.py` & `huscy-project-0.5.0a24/huscy_project/project_template/config/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,24 +14,26 @@
     2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 """
 import importlib
 
 from django.apps import apps
 from django.conf import settings
 from django.contrib import admin
+from django.contrib.auth.views import LoginView
 from django.views.generic import TemplateView
 from django.urls import include, path
 
 from rest_framework.authtoken.views import obtain_auth_token
 
 from huscy_project.views import health_check
 
 
 urlpatterns = [
     path('admin/', admin.site.urls),
+    path('accounts/login/', LoginView.as_view(template_name='admin/login.html')),
     path('', TemplateView.as_view(template_name='index.html')),
     path('health_check/', health_check),
     path('api-auth-token/', obtain_auth_token),
 ]
 
 if settings.DEBUG:
     urlpatterns.append(
```

### Comparing `huscy-project-0.5.0a23/huscy_project/project_template/manage.py` & `huscy-project-0.5.0a24/huscy_project/project_template/manage.py`

 * *Files identical despite different names*

### Comparing `huscy-project-0.5.0a23/huscy_project/project_template/templates/index.html` & `huscy-project-0.5.0a24/huscy_project/project_template/templates/index.html`

 * *Files identical despite different names*

### Comparing `huscy-project-0.5.0a23/huscy_project.egg-info/SOURCES.txt` & `huscy-project-0.5.0a24/huscy_project.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy-project-0.5.0a23/setup.py` & `huscy-project-0.5.0a24/setup.py`

 * *Files identical despite different names*

