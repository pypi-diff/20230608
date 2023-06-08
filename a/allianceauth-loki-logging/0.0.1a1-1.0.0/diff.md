# Comparing `tmp/allianceauth-loki-logging-0.0.1a1.tar.gz` & `tmp/allianceauth-loki-logging-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-loki-logging-0.0.1a1.tar", last modified: Sat Apr 22 00:26:07 2023, max compression
+gzip compressed data, was "allianceauth-loki-logging-1.0.0.tar", last modified: Thu Jun  8 10:47:23 2023, max compression
```

## Comparing `allianceauth-loki-logging-0.0.1a1.tar` & `allianceauth-loki-logging-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:26:07.934624 allianceauth-loki-logging-0.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-22 00:25:56.000000 allianceauth-loki-logging-0.0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-22 00:26:07.934624 allianceauth-loki-logging-0.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-22 00:25:56.000000 allianceauth-loki-logging-0.0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:26:07.934624 allianceauth-loki-logging-0.0.1a1/allianceauth-loki-logging/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-22 00:25:56.000000 allianceauth-loki-logging-0.0.1a1/allianceauth-loki-logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-22 00:25:56.000000 allianceauth-loki-logging-0.0.1a1/allianceauth-loki-logging/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-22 00:25:56.000000 allianceauth-loki-logging-0.0.1a1/allianceauth-loki-logging/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:26:07.934624 allianceauth-loki-logging-0.0.1a1/allianceauth_loki_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-22 00:26:07.000000 allianceauth-loki-logging-0.0.1a1/allianceauth_loki_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-22 00:26:07.000000 allianceauth-loki-logging-0.0.1a1/allianceauth_loki_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:26:07.000000 allianceauth-loki-logging-0.0.1a1/allianceauth_loki_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-22 00:26:07.000000 allianceauth-loki-logging-0.0.1a1/allianceauth_loki_logging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-22 00:26:07.000000 allianceauth-loki-logging-0.0.1a1/allianceauth_loki_logging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-22 00:26:07.934624 allianceauth-loki-logging-0.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-22 00:25:56.000000 allianceauth-loki-logging-0.0.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:47:23.791150 allianceauth-loki-logging-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-08 10:47:13.000000 allianceauth-loki-logging-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-08 10:47:23.791150 allianceauth-loki-logging-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-08 10:47:13.000000 allianceauth-loki-logging-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:47:23.791150 allianceauth-loki-logging-1.0.0/allianceauth_loki_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-08 10:47:13.000000 allianceauth-loki-logging-1.0.0/allianceauth_loki_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-08 10:47:13.000000 allianceauth-loki-logging-1.0.0/allianceauth_loki_logging/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-08 10:47:13.000000 allianceauth-loki-logging-1.0.0/allianceauth_loki_logging/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:47:23.791150 allianceauth-loki-logging-1.0.0/allianceauth_loki_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-08 10:47:23.000000 allianceauth-loki-logging-1.0.0/allianceauth_loki_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-08 10:47:23.000000 allianceauth-loki-logging-1.0.0/allianceauth_loki_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:47:23.000000 allianceauth-loki-logging-1.0.0/allianceauth_loki_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 10:47:23.000000 allianceauth-loki-logging-1.0.0/allianceauth_loki_logging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 10:47:23.000000 allianceauth-loki-logging-1.0.0/allianceauth_loki_logging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 10:47:23.795150 allianceauth-loki-logging-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-08 10:47:13.000000 allianceauth-loki-logging-1.0.0/setup.py
```

### Comparing `allianceauth-loki-logging-0.0.1a1/LICENSE` & `allianceauth-loki-logging-1.0.0/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Zepc Myers, 2022 h3nnn4n (Renan S Silva)
+Copyright (c) 2021 Zepc Myers, 2022 h3nnn4n (Renan S Silva), 2023 Aaron Kable
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `allianceauth-loki-logging-0.0.1a1/PKG-INFO` & `allianceauth-loki-logging-1.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,64 @@
-Metadata-Version: 2.1
-Name: allianceauth-loki-logging
-Version: 0.0.1a1
-Summary: A non-blocking django logging handler for Loki
-Home-page: https://github.com/Solar-Helix-Independent-Transport/allianceauth-loki-logging
-Author: aaronkable
-Author-email: aaronkable@gmail.com
-License: MIT
-Keywords: python,loki,grafana,logging,metrics,threaded
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Alliance Auth Loki Logger
 
 Python logging handler and formatter for [loki](https://grafana.com/oss/loki/)
 for django. Supports blocking calls and non blocking ones, using threading.
 
 Build on top of [django-loki-reloaded](https://github.com/zepc007/django-loki).
 
+# Why?
+
+A single location for all logs across auth, Separate to auth! With search and notifications etc. Complete with python trace type data for everything.
+
+![Logs 1](https://i.imgur.com/rYUsSDy.png)
+
+![Logs 2](https://i.imgur.com/maTS2qQ.png)
+
+![Logs 3](https://i.imgur.com/YS5pJiX.png)
+
 # Installation
 
-Using pip:
+Have a [loki instance configured and running](https://github.com/grafana/loki)
+
+### Bare Metal:
 
 ```shell
 pip install allianceauth-loki-logging
 ```
 
 or
 
 ```shell
 pip install git+https://github.com/Solar-Helix-Independent-Transport/allianceauth-loki-logging.git
 ```
 
+### Docker
+
+add this to your requirements file and rebuild your image
+
+```
+allianceauth-loki-logging>=1.0.0
+```
+
+or
+
+```
+allianceauth-loki-logging @ git+https://github.com/Solar-Helix-Independent-Transport/allianceauth-loki-logging.git
+```
+
 # Usage
 
 `LokiHandler` is a custom logging handler that pushes log messages to Loki.
 
-Modify your settings to integrate `allianceauth-loki-logging` with Django's logging:
+Modify your settings to integrate `allianceauth_loki_logging` with Django's logging:
 
-in your `local.py` add this at the end
+in your `local.py` add this at the end, Be sure to read the comments and update any that need to be updated. Specifically the url for loki.
 
 ```python
+LOKI_URL = "'http://loki:3100/loki/api/v1/push'
 ### Override the defaults from base.py
 LOGGING = {
     'version': 1,
     'disable_existing_loggers': False,
     'formatters': {
         'verbose': {
             'format': "[%(asctime)s] %(levelname)s [%(name)s:%(lineno)s] %(message)s",
@@ -66,66 +74,70 @@
             'class': 'logging.handlers.RotatingFileHandler',
             'filename': os.path.join(BASE_DIR, 'log/extensions.log'),
             'formatter': 'verbose',
             'maxBytes': 1024 * 1024 * 5,  # edit this line to change max log file size
             'backupCount': 5,  # edit this line to change number of log backups
         },
         'console': {
-            'level': 'DEBUG',  # edit this line to change logging level to console
+            'level': 'DEBUG' if DEBUG else 'INFO',  # edit this line to change logging level to console
             'class': 'logging.StreamHandler',
             'formatter': 'verbose',
         },
         'notifications': {  # creates notifications for users with logging_notifications permission
             'level': 'ERROR',  # edit this line to change logging level to notifications
             'class': 'allianceauth.notifications.handlers.NotificationHandler',
             'formatter': 'verbose',
         },
     },
     'loggers': {
         'allianceauth': {
-            'handlers': ['notifications'], ## untested need to test what this does
-            'level': 'DEBUG',
+            'handlers': ['notifications'],
+            'level': 'ERROR',
         },
         'extensions': {
-            'handlers': ['extension_file'], ## untested need to test what this does
-            'level': 'DEBUG',
+            'handlers': ['extension_file'], 
+            'level': 'DEBUG' if DEBUG else 'INFO',
         }
     }
 }
 
 ###  LOKI Specific settings
 LOGGING['formatters']['loki'] = {
-    'class': 'allianceauth-loki-logging.LokiFormatter'  # required
+    'class': 'allianceauth_loki_logging.LokiFormatter'  # required
 }
 
 print(f"Configuring Loki Log job to: {os.path.basename(os.sys.argv[0])}")
 
 LOGGING['handlers']['loki'] = {
     'level': 'DEBUG' if DEBUG else 'INFO',  # Required # We are auto setting the log level to only record debug when in debug.
-    'class': 'allianceauth-loki-logging.LokiHandler',  # Required
+    'class': 'allianceauth_loki_logging.LokiHandler',  # Required
     'formatter': 'loki',  #Required
     'timeout': 1,  # Post request timeout, default is 0.5. Optional
     # Loki url. Defaults to localhost. Optional.
-    'url': 'http://localhost:3100/loki/api/v1/push',
+    'url': , LOKI_URL,
     # Extra tags / labels to attach to the log. Optional, but usefull to differentiate instances.
-    'tags': {"job":os.path.basename(os.sys.argv[0])}, # Auto set the job to differentiate between celery, gunicorn, manage.py etc.
+    'tags': {
+        "job":os.path.basename(os.sys.argv[0]), # Auto set the job to differentiate between celery, gunicorn, manage.py etc.
+        # you could add extra tags here if you were running multiple auths and needed to be able to tell them apart in a single loki instance eg:
+        # "auth": "CoolAuth 1",
+    }, 
     # Push mode. Can be 'sync' or 'thread'. Sync is blocking, thread is non-blocking. Defaults to sync. Optional.
     'mode': 'thread',
 }
 
 LOGGING['root'] = { # Set the root logger
     'handlers': ['loki', 'console'],
     'level': 'DEBUG' if DEBUG else 'INFO', # Auto set the log level to only record debug when in debug
 }
 
 WORKER_HIJACK_ROOT_LOGGER = False  # Do not overide with celery logging.
 ```
 
-In your `supervisor.conf` update any workers to run at logging level DEBUG. `-l INFO`
-
-```conf
-....
-command= celery -A myauth worker -l DEBUG
-....
-```
+## Diagnosing issues with logs not being pushed in HIGHLY threaded environments
 
+add the following to your loki config to bypass the rate limits.
 
+```yaml
+limits_config:
+  max_streams_per_user: 0
+  max_global_streams_per_user: 0
+```
```

### Comparing `allianceauth-loki-logging-0.0.1a1/allianceauth-loki-logging/formatters.py` & `allianceauth-loki-logging-1.0.0/allianceauth_loki_logging/formatters.py`

 * *Files identical despite different names*

### Comparing `allianceauth-loki-logging-0.0.1a1/allianceauth-loki-logging/handlers.py` & `allianceauth-loki-logging-1.0.0/allianceauth_loki_logging/handlers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-loki-logging-0.0.1a1/setup.py` & `allianceauth-loki-logging-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 
 from setuptools import find_packages, setup
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
+#from allianceauth_loki_logging import __version__
+
+__version__ = "1.0.0"
+
 setup(
     name='allianceauth-loki-logging',
-    version='0.0.1a1',
-    packages=['allianceauth-loki-logging'],
+    version=__version__,
+    packages=find_packages(),
     url='https://github.com/Solar-Helix-Independent-Transport/allianceauth-loki-logging',
     license='MIT',
     author='aaronkable',
     author_email='aaronkable@gmail.com',
     description='A non-blocking django logging handler for Loki',
     long_description=README,
     long_description_content_type="text/markdown",
```

