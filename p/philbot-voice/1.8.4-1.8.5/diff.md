# Comparing `tmp/philbot_voice-1.8.4.tar.gz` & `tmp/philbot_voice-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.8.4.tar", max compression
+gzip compressed data, was "philbot_voice-1.8.5.tar", max compression
```

## Comparing `philbot_voice-1.8.4.tar` & `philbot_voice-1.8.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-08 10:31:51.675288 philbot_voice-1.8.4/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-08 10:31:51.675288 philbot_voice-1.8.4/philbot-voice/__main__.py
--rw-r--r--   0        0        0    34454 2023-06-08 10:31:51.675288 philbot_voice-1.8.4/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-08 10:31:51.675288 philbot_voice-1.8.4/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-08 10:45:43.747449 philbot_voice-1.8.5/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-08 10:45:43.747449 philbot_voice-1.8.5/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    34459 2023-06-08 10:45:43.751450 philbot_voice-1.8.5/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-08 10:45:43.751450 philbot_voice-1.8.5/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.8.5/PKG-INFO
```

### Comparing `philbot_voice-1.8.4/philbot-voice/voice.py` & `philbot_voice-1.8.5/philbot-voice/voice.py`

 * *Files 0% similar despite different names*

```diff
@@ -761,20 +761,20 @@
     if not request.headers.get('x-authorization'): return Response('Unauthorized', status=401)
     if request.headers['x-authorization'] != os.environ['DISCORD_API_TOKEN']: return Response('Forbidden', status=403)
     guild_id = request.json['guild_id']
     context = get_context(guild_id)
     if not context or not context.is_connecting():
         return 'false'
     end = time_millis() + 1000 * 5
-    tryy = 1
+    tryy = 100
     while time_millis() < end:
         context = get_context(guild_id)
         if context and context.is_connected():
             return 'true'
-        time.sleep(tryy * 100)
+        time.sleep(tryy / 1000.0)
         tryy = tryy * 2
     return 'false'
 
 def cleanup():
     for file in os.listdir(STORAGE_DIRECTORY):
         if os.path.getmtime(STORAGE_DIRECTORY + '/' + file) + 60 * 60 < time_seconds():
             try:
```

### Comparing `philbot_voice-1.8.4/pyproject.toml` & `philbot_voice-1.8.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.8.4"
+version = "1.8.5"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.8.4/PKG-INFO` & `philbot_voice-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.8.4
+Version: 1.8.5
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

