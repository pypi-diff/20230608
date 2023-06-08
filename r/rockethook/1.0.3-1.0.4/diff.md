# Comparing `tmp/rockethook-1.0.3.tar.gz` & `tmp/rockethook-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rockethook-1.0.3.tar", last modified: Mon Feb 20 13:55:54 2017, max compression
+gzip compressed data, was "rockethook-1.0.4.tar", last modified: Thu Jun  8 16:33:36 2023, max compression
```

## Comparing `rockethook-1.0.3.tar` & `rockethook-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 gena      (1000) gena      (1000)        0 2017-02-20 13:55:54.000000 rockethook-1.0.3/
--rw-r--r--   0 gena      (1000) gena      (1000)     1804 2017-02-20 13:55:54.000000 rockethook-1.0.3/PKG-INFO
-drwxr-xr-x   0 gena      (1000) gena      (1000)        0 2017-02-20 13:55:54.000000 rockethook-1.0.3/rockethook/
--rw-r--r--   0 gena      (1000) gena      (1000)     5214 2017-02-20 13:54:44.000000 rockethook-1.0.3/rockethook/__init__.py
-drwxr-xr-x   0 gena      (1000) gena      (1000)        0 2017-02-20 13:55:54.000000 rockethook-1.0.3/rockethook.egg-info/
--rw-rw-r--   0 gena      (1000) gena      (1000)       11 2017-02-20 13:55:54.000000 rockethook-1.0.3/rockethook.egg-info/top_level.txt
--rw-rw-r--   0 gena      (1000) gena      (1000)     1804 2017-02-20 13:55:54.000000 rockethook-1.0.3/rockethook.egg-info/PKG-INFO
--rw-rw-r--   0 gena      (1000) gena      (1000)        1 2017-02-20 13:55:54.000000 rockethook-1.0.3/rockethook.egg-info/dependency_links.txt
--rw-rw-r--   0 gena      (1000) gena      (1000)      178 2017-02-20 13:55:54.000000 rockethook-1.0.3/rockethook.egg-info/SOURCES.txt
--rw-rw-r--   0 gena      (1000) gena      (1000)      552 2017-02-20 13:52:13.000000 rockethook-1.0.3/setup.py
--rw-r--r--   0 gena      (1000) gena      (1000)       59 2017-02-20 13:55:54.000000 rockethook-1.0.3/setup.cfg
--rw-r--r--   0 gena      (1000) gena      (1000)     1201 2016-11-30 14:55:04.000000 rockethook-1.0.3/README.rst
+drwxr-xr-x   0 Gennadii_Aleksandrov   (502) staff       (20)        0 2023-06-08 16:33:36.088077 rockethook-1.0.4/
+-rw-r--r--   0 Gennadii_Aleksandrov   (502) staff       (20)     1086 2023-06-08 16:05:06.000000 rockethook-1.0.4/LICENSE
+-rw-r--r--   0 Gennadii_Aleksandrov   (502) staff       (20)     1483 2023-06-08 16:33:36.087797 rockethook-1.0.4/PKG-INFO
+-rw-r--r--   0 Gennadii_Aleksandrov   (502) staff       (20)     1201 2023-06-08 16:05:06.000000 rockethook-1.0.4/README.rst
+drwxr-xr-x   0 Gennadii_Aleksandrov   (502) staff       (20)        0 2023-06-08 16:33:36.085471 rockethook-1.0.4/rockethook/
+-rw-r--r--   0 Gennadii_Aleksandrov   (502) staff       (20)     5238 2023-06-08 16:16:59.000000 rockethook-1.0.4/rockethook/__init__.py
+drwxr-xr-x   0 Gennadii_Aleksandrov   (502) staff       (20)        0 2023-06-08 16:33:36.087370 rockethook-1.0.4/rockethook.egg-info/
+-rw-r--r--   0 Gennadii_Aleksandrov   (502) staff       (20)     1483 2023-06-08 16:33:36.000000 rockethook-1.0.4/rockethook.egg-info/PKG-INFO
+-rw-r--r--   0 Gennadii_Aleksandrov   (502) staff       (20)      186 2023-06-08 16:33:36.000000 rockethook-1.0.4/rockethook.egg-info/SOURCES.txt
+-rw-r--r--   0 Gennadii_Aleksandrov   (502) staff       (20)        1 2023-06-08 16:33:36.000000 rockethook-1.0.4/rockethook.egg-info/dependency_links.txt
+-rw-r--r--   0 Gennadii_Aleksandrov   (502) staff       (20)       11 2023-06-08 16:33:36.000000 rockethook-1.0.4/rockethook.egg-info/top_level.txt
+-rw-r--r--   0 Gennadii_Aleksandrov   (502) staff       (20)       38 2023-06-08 16:33:36.088168 rockethook-1.0.4/setup.cfg
+-rw-r--r--   0 Gennadii_Aleksandrov   (502) staff       (20)      552 2023-06-08 16:05:56.000000 rockethook-1.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rockethook-1.0.3/PKG-INFO` & `rockethook-1.0.4/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,39 @@
-Metadata-Version: 1.0
-Name: rockethook
-Version: 1.0.3
-Summary: Simple library for posting to Rocket.Chat via webhooks a.k.a. integrations.
-Home-page: https://github.com/gevial/rockethook
-Author: Gennady Aleksandrov
-Author-email: gevial@yahoo.com
-License: MIT
-Description: Rockethook
-        ========================
-        
-        Simple library for posting to Rocket.Chat via webhooks a.k.a. integrations
-        
-        Installation
-        ++++++++++++
-        Rockethook can be installed from PyPi: :code:`pip install rockethook`
-        
-        Usage
-        +++++
-        
-        The idea behind this library is to create Webhook object and then post Messages with it.
-        You can create Message object and fulfill it with content (text and/or attachments) later.
-        
-        Or you can just :code:`Webhook.quick_post('Your message')` without bothering with Message objects.
-        
-        It is a very small library indeed, so the best explanation is an example of usage:
-        
-        >>> import rockethook
-        >>> my_hook = rockethook.Webhook('https://rocketchat.example.com', my_token)
-        >>> msg = rockethook.Message(icon_url='http://example.com/icon.png')
-        >>> msg.append_text('First line.')
-        >>> msg.append_text('Second line.')
-        >>> msg.add_attachment(
-        ...     title='Attach',
-        ...     title_link='http://example.com',
-        ...     image_url='http://example.com/img.png'
-        ... )
-        >>> my_hook.post(msg)
-        
-        To override default webhook's channel:
-        
-        >>> msg = rockethook.Message(channel="#my-channel")
-        
-        To quickly post simple text messages:
-        
-        >>> my_hook.quick_post('Hi!')
-        >>> my_hook.quick_post('Call me back\nPlease')
-        
-Platform: UNKNOWN
+Rockethook
+========================
+
+Simple library for posting to Rocket.Chat via webhooks a.k.a. integrations
+
+Installation
+++++++++++++
+Rockethook can be installed from PyPi: :code:`pip install rockethook`
+
+Usage
++++++
+
+The idea behind this library is to create Webhook object and then post Messages with it.
+You can create Message object and fulfill it with content (text and/or attachments) later.
+
+Or you can just :code:`Webhook.quick_post('Your message')` without bothering with Message objects.
+
+It is a very small library indeed, so the best explanation is an example of usage:
+
+>>> import rockethook
+>>> my_hook = rockethook.Webhook('https://rocketchat.example.com', my_token)
+>>> msg = rockethook.Message(icon_url='http://example.com/icon.png')
+>>> msg.append_text('First line.')
+>>> msg.append_text('Second line.')
+>>> msg.add_attachment(
+...     title='Attach',
+...     title_link='http://example.com',
+...     image_url='http://example.com/img.png'
+... )
+>>> my_hook.post(msg)
+
+To override default webhook's channel:
+
+>>> msg = rockethook.Message(channel="#my-channel")
+
+To quickly post simple text messages:
+
+>>> my_hook.quick_post('Hi!')
+>>> my_hook.quick_post('Call me back\nPlease')
```

### Comparing `rockethook-1.0.3/rockethook/__init__.py` & `rockethook-1.0.4/rockethook/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 post Messages with it. You can create Message object and fulfill it
 with content (text and/or attachments) later.
 
 Or you can just Webhook.quick_post('Your message') without bothering with Message objects.
 """
 
 import json
-import httplib
+import http.client as httplib
 import urllib
-
-from urlparse import urlparse
+from urllib.parse import urlparse
 
 
 class WebhookError(Exception):
     """Raised when Rocket.Chat server responses with non-JSON or with an explicit error."""
     def __init__(self, status, message):
         self.status = status
         self.message = 'Rocket.Chat server error, code {0}: {1}'.format(status, message)
@@ -72,15 +71,15 @@
             payload_dict['text'] = message.text
         if message.channel:
             payload_dict['channel'] = message.channel
         if message.icon_url:
             payload_dict['icon_url'] = message.icon_url
         if message.attachments:
             payload_dict['attachments'] = message.attachments
-        payload = 'payload=' + urllib.quote_plus(json.dumps(payload_dict))
+        payload = 'payload=' + urllib.parse.quote_plus(json.dumps(payload_dict))
         headers = {'Content-Type': 'application/x-www-form-urlencoded'}
 
         if self.scheme == 'https':
             conn = httplib.HTTPSConnection(self.server_fqdn)
         else:
             conn = httplib.HTTPConnection(self.server_fqdn)
         conn.request('POST', '/hooks/' + self.token, payload, headers)
```

### Comparing `rockethook-1.0.3/setup.py` & `rockethook-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 with open(join(dirname(__file__), 'README.rst')) as f:
     readme = f.read()
 
 setup(
     name='rockethook',
-    version='1.0.3',
+    version='1.0.4',
     description='Simple library for posting to Rocket.Chat via webhooks a.k.a. integrations.',
     long_description=readme,
     license='MIT',
     author='Gennady Aleksandrov',
     author_email='gevial@yahoo.com',
     url='https://github.com/gevial/rockethook',
     packages=find_packages(exclude=('tests', 'docs'))
```

