# Comparing `tmp/django-alert-winglet-0.1.2.tar.gz` & `tmp/django-alert-winglet-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-alert-winglet-0.1.2.tar", last modified: Wed Jun  7 11:11:59 2023, max compression
+gzip compressed data, was "django-alert-winglet-0.1.3.tar", last modified: Thu Jun  8 12:55:21 2023, max compression
```

## Comparing `django-alert-winglet-0.1.2.tar` & `django-alert-winglet-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 11:11:59.283330 django-alert-winglet-0.1.2/
--rw-rw-rw-   0        0        0     1076 2023-06-06 16:54:37.000000 django-alert-winglet-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       37 2023-06-06 11:31:41.000000 django-alert-winglet-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2446 2023-06-07 11:11:59.283433 django-alert-winglet-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1529 2023-06-06 16:54:37.000000 django-alert-winglet-0.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-07 11:11:59.271668 django-alert-winglet-0.1.2/alert_wing/
--rw-rw-rw-   0        0        0        0 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.2/alert_wing/__init__.py
--rw-rw-rw-   0        0        0      157 2023-06-06 12:24:22.000000 django-alert-winglet-0.1.2/alert_wing/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-07 11:11:59.273162 django-alert-winglet-0.1.2/alert_wing/managers/
--rw-rw-rw-   0        0        0        0 2023-06-06 08:42:15.000000 django-alert-winglet-0.1.2/alert_wing/managers/__init__.py
--rw-rw-rw-   0        0        0      248 2023-06-06 08:42:15.000000 django-alert-winglet-0.1.2/alert_wing/managers/base_manager.py
--rw-rw-rw-   0        0        0     4558 2023-06-07 11:11:23.000000 django-alert-winglet-0.1.2/alert_wing/managers/discord_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-07 11:11:59.274739 django-alert-winglet-0.1.2/alert_wing/senders/
--rw-rw-rw-   0        0        0        0 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.2/alert_wing/senders/__init__.py
--rw-rw-rw-   0        0        0      142 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.2/alert_wing/senders/base.py
--rw-rw-rw-   0        0        0     4563 2023-06-06 17:08:24.000000 django-alert-winglet-0.1.2/alert_wing/senders/discord.py
-drwxrwxrwx   0        0        0        0 2023-06-07 11:11:59.282386 django-alert-winglet-0.1.2/django_alert_winglet.egg-info/
--rw-rw-rw-   0        0        0     2446 2023-06-07 11:11:59.000000 django-alert-winglet-0.1.2/django_alert_winglet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-06-07 11:11:59.000000 django-alert-winglet-0.1.2/django_alert_winglet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 11:11:59.000000 django-alert-winglet-0.1.2/django_alert_winglet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-07 11:11:59.000000 django-alert-winglet-0.1.2/django_alert_winglet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-07 11:11:59.000000 django-alert-winglet-0.1.2/django_alert_winglet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2023-06-06 11:27:00.000000 django-alert-winglet-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      992 2023-06-07 11:11:59.283996 django-alert-winglet-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-06-06 11:30:18.000000 django-alert-winglet-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:55:21.680963 django-alert-winglet-0.1.3/
+-rw-rw-rw-   0        0        0     1076 2023-06-06 16:54:37.000000 django-alert-winglet-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-06-06 11:31:41.000000 django-alert-winglet-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2446 2023-06-08 12:55:21.681129 django-alert-winglet-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1529 2023-06-06 16:54:37.000000 django-alert-winglet-0.1.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-08 12:55:21.654704 django-alert-winglet-0.1.3/alert_wing/
+-rw-rw-rw-   0        0        0        0 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.3/alert_wing/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-06-06 12:24:22.000000 django-alert-winglet-0.1.3/alert_wing/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:55:21.659669 django-alert-winglet-0.1.3/alert_wing/managers/
+-rw-rw-rw-   0        0        0        0 2023-06-06 08:42:15.000000 django-alert-winglet-0.1.3/alert_wing/managers/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-06-06 08:42:15.000000 django-alert-winglet-0.1.3/alert_wing/managers/base_manager.py
+-rw-rw-rw-   0        0        0     4573 2023-06-08 12:53:41.000000 django-alert-winglet-0.1.3/alert_wing/managers/discord_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:55:21.667400 django-alert-winglet-0.1.3/alert_wing/senders/
+-rw-rw-rw-   0        0        0        0 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.3/alert_wing/senders/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.3/alert_wing/senders/base.py
+-rw-rw-rw-   0        0        0     4563 2023-06-06 17:08:24.000000 django-alert-winglet-0.1.3/alert_wing/senders/discord.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:55:21.680463 django-alert-winglet-0.1.3/django_alert_winglet.egg-info/
+-rw-rw-rw-   0        0        0     2446 2023-06-08 12:55:21.000000 django-alert-winglet-0.1.3/django_alert_winglet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-06-08 12:55:21.000000 django-alert-winglet-0.1.3/django_alert_winglet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 12:55:21.000000 django-alert-winglet-0.1.3/django_alert_winglet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-08 12:55:21.000000 django-alert-winglet-0.1.3/django_alert_winglet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-08 12:55:21.000000 django-alert-winglet-0.1.3/django_alert_winglet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       90 2023-06-06 11:27:00.000000 django-alert-winglet-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      992 2023-06-08 12:55:21.681963 django-alert-winglet-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-06-06 11:30:18.000000 django-alert-winglet-0.1.3/setup.py
```

### Comparing `django-alert-winglet-0.1.2/LICENSE` & `django-alert-winglet-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-alert-winglet-0.1.2/PKG-INFO` & `django-alert-winglet-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-alert-winglet
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Django app to send any exception to discord channel.
 Author: Mojtaba
 Author-email: Mojtabadavi14@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
```

### Comparing `django-alert-winglet-0.1.2/README.rst` & `django-alert-winglet-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-alert-winglet-0.1.2/alert_wing/managers/discord_manager.py` & `django-alert-winglet-0.1.3/alert_wing/managers/discord_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import traceback
 
 import discord
 from discord import Embed
 from django.utils import timezone
 
-from alert_wing.managers.base_manager import BaseManager
+from apps.alert_wing.managers.base_manager import BaseManager
+
 
 class DiscordEmbedManager(BaseManager):
     """
     A class for managing Discord embed messages for exception handling.
 
     Args:
         exc (Exception): The exception instance.
@@ -65,40 +66,43 @@
             self.embed = self.setup_embed()
 
     def setup_embed(self) -> discord.Embed:
         return Embed(
             title=self.title, description=self.description, colour=self.embed_color
         )
 
-    def _frame_summary_handler(self, frame_summary):
+    def _frame_summary_handler(self, frame_summary: list):
         """
-        Handle the formatting of a frame summary.
+        Handle the formatting of a frame summary list.
 
         Args:
-            frame_summary (traceback.FrameSummary): Frame summary object.
+            frame_summary (traceback.FrameSummary): Frame summary object list.
 
         Returns:
-            str: Formatted frame summary.
+            list: Formatted frame summary.
         """
-        stack_summary_handler = traceback.StackSummary()
-        return stack_summary_handler.format_frame_summary(frame_summary=frame_summary)
+        return traceback.format_list(frame_summary)
 
     def format_exception(self) -> tuple[str, str]:
         """
         Format the exception and return formatted text and extra detail.
 
         Returns:
             tuple[str, str]: Formatted exception and extra detail.
         """
         request = self.exc.__traceback__.tb_frame.f_locals.get("request")
-        frame_summary_list = traceback.extract_tb(self.exc.__traceback__)[-2:]
+        frame_summary_obj_list = traceback.extract_tb(self.exc.__traceback__)[-2:]
+
+        formatted_frame_summary_list = self._frame_summary_handler(
+            frame_summary_obj_list
+        )
 
         formatted_exc = (
-            f"{self._frame_summary_handler(frame_summary_list[0])}\n"
-            f"{self._frame_summary_handler(frame_summary_list[1])}"
+            f"{formatted_frame_summary_list[0]}\n"
+            f"{formatted_frame_summary_list[1]}"
             f"{str(self.exc)}\n"
         )
         extra_detail = (
             f"Request API  -> {request.build_absolute_uri() if request is not None else None}\n"
             f"Request Method -> {request.method}"
         )
         return formatted_exc, extra_detail
```

### Comparing `django-alert-winglet-0.1.2/alert_wing/senders/discord.py` & `django-alert-winglet-0.1.3/alert_wing/senders/discord.py`

 * *Files identical despite different names*

### Comparing `django-alert-winglet-0.1.2/django_alert_winglet.egg-info/PKG-INFO` & `django-alert-winglet-0.1.3/django_alert_winglet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-alert-winglet
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Django app to send any exception to discord channel.
 Author: Mojtaba
 Author-email: Mojtabadavi14@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
```

### Comparing `django-alert-winglet-0.1.2/django_alert_winglet.egg-info/SOURCES.txt` & `django-alert-winglet-0.1.3/django_alert_winglet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-alert-winglet-0.1.2/setup.cfg` & `django-alert-winglet-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 616c 6572 742d   = django-alert-
 00000020: 7769 6e67 6c65 740d 0a76 6572 7369 6f6e  winglet..version
-00000030: 203d 2030 2e31 2e32 0d0a 6465 7363 7269   = 0.1.2..descri
+00000030: 203d 2030 2e31 2e33 0d0a 6465 7363 7269   = 0.1.3..descri
 00000040: 7074 696f 6e20 3d20 4120 446a 616e 676f  ption = A Django
 00000050: 2061 7070 2074 6f20 7365 6e64 2061 6e79   app to send any
 00000060: 2065 7863 6570 7469 6f6e 2074 6f20 6469   exception to di
 00000070: 7363 6f72 6420 6368 616e 6e65 6c2e 0d0a  scord channel...
 00000080: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000090: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 000000a0: 7465 7874 2f78 2d72 7374 0d0a 6c6f 6e67  text/x-rst..long
```

