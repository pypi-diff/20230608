# Comparing `tmp/trio-websocket-0.9.1.tar.gz` & `tmp/trio-websocket-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trio-websocket-0.9.1.tar", last modified: Sun Dec  6 13:24:40 2020, max compression
+gzip compressed data, was "/Users/john/dev/trio/trio-websocket/dist/tmpbfrkcdho/trio-websocket-0.9.2.tar", last modified: Fri Feb  5 11:49:53 2021, max compression
```

## Comparing `trio-websocket-0.9.1.tar` & `trio-websocket-0.9.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 john       (501) staff       (20)        0 2020-12-06 13:24:40.734059 trio-websocket-0.9.1/
--rw-rw-r--   0 john       (501) staff       (20)     5526 2020-12-06 13:24:40.733497 trio-websocket-0.9.1/PKG-INFO
--rw-rw-r--   0 john       (501) staff       (20)     3716 2020-11-25 07:43:03.000000 trio-websocket-0.9.1/README.md
--rw-rw-r--   0 john       (501) staff       (20)       38 2020-12-06 13:24:40.734179 trio-websocket-0.9.1/setup.cfg
--rw-rw-r--   0 john       (501) staff       (20)     1723 2020-11-25 07:43:03.000000 trio-websocket-0.9.1/setup.py
-drwxrwxr-x   0 john       (501) staff       (20)        0 2020-12-06 13:24:40.730109 trio-websocket-0.9.1/trio_websocket/
--rw-rw-r--   0 john       (501) staff       (20)      434 2020-11-15 12:11:24.000000 trio-websocket-0.9.1/trio_websocket/__init__.py
--rw-rw-r--   0 john       (501) staff       (20)    55439 2020-12-06 13:09:02.000000 trio-websocket-0.9.1/trio_websocket/_impl.py
--rw-rw-r--   0 john       (501) staff       (20)       22 2020-12-06 13:21:40.000000 trio-websocket-0.9.1/trio_websocket/_version.py
-drwxrwxr-x   0 john       (501) staff       (20)        0 2020-12-06 13:24:40.732956 trio-websocket-0.9.1/trio_websocket.egg-info/
--rw-rw-r--   0 john       (501) staff       (20)     5526 2020-12-06 13:24:40.000000 trio-websocket-0.9.1/trio_websocket.egg-info/PKG-INFO
--rw-rw-r--   0 john       (501) staff       (20)      285 2020-12-06 13:24:40.000000 trio-websocket-0.9.1/trio_websocket.egg-info/SOURCES.txt
--rw-rw-r--   0 john       (501) staff       (20)        1 2020-12-06 13:24:40.000000 trio-websocket-0.9.1/trio_websocket.egg-info/dependency_links.txt
--rw-rw-r--   0 john       (501) staff       (20)       47 2020-12-06 13:24:40.000000 trio-websocket-0.9.1/trio_websocket.egg-info/requires.txt
--rw-rw-r--   0 john       (501) staff       (20)       15 2020-12-06 13:24:40.000000 trio-websocket-0.9.1/trio_websocket.egg-info/top_level.txt
+drwxrwxr-x   0 john       (501) staff       (20)        0 2021-02-05 11:49:53.388346 trio-websocket-0.9.2/
+-rw-rw-r--   0 john       (501) staff       (20)     5526 2021-02-05 11:49:53.387958 trio-websocket-0.9.2/PKG-INFO
+-rw-rw-r--   0 john       (501) staff       (20)     3716 2020-11-25 07:43:03.000000 trio-websocket-0.9.2/README.md
+-rw-rw-r--   0 john       (501) staff       (20)       38 2021-02-05 11:49:53.388475 trio-websocket-0.9.2/setup.cfg
+-rw-rw-r--   0 john       (501) staff       (20)     1723 2020-11-25 07:43:03.000000 trio-websocket-0.9.2/setup.py
+drwxrwxr-x   0 john       (501) staff       (20)        0 2021-02-05 11:49:53.384676 trio-websocket-0.9.2/trio_websocket/
+-rw-rw-r--   0 john       (501) staff       (20)      434 2020-11-15 12:11:24.000000 trio-websocket-0.9.2/trio_websocket/__init__.py
+-rw-rw-r--   0 john       (501) staff       (20)    55760 2021-02-05 11:44:48.000000 trio-websocket-0.9.2/trio_websocket/_impl.py
+-rw-rw-r--   0 john       (501) staff       (20)       22 2021-02-05 11:43:59.000000 trio-websocket-0.9.2/trio_websocket/_version.py
+drwxrwxr-x   0 john       (501) staff       (20)        0 2021-02-05 11:49:53.387367 trio-websocket-0.9.2/trio_websocket.egg-info/
+-rw-rw-r--   0 john       (501) staff       (20)     5526 2021-02-05 11:49:53.000000 trio-websocket-0.9.2/trio_websocket.egg-info/PKG-INFO
+-rw-rw-r--   0 john       (501) staff       (20)      285 2021-02-05 11:49:53.000000 trio-websocket-0.9.2/trio_websocket.egg-info/SOURCES.txt
+-rw-rw-r--   0 john       (501) staff       (20)        1 2021-02-05 11:49:53.000000 trio-websocket-0.9.2/trio_websocket.egg-info/dependency_links.txt
+-rw-rw-r--   0 john       (501) staff       (20)       47 2021-02-05 11:49:53.000000 trio-websocket-0.9.2/trio_websocket.egg-info/requires.txt
+-rw-rw-r--   0 john       (501) staff       (20)       15 2021-02-05 11:49:53.000000 trio-websocket-0.9.2/trio_websocket.egg-info/top_level.txt
```

### Comparing `trio-websocket-0.9.1/PKG-INFO` & `trio-websocket-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trio-websocket
-Version: 0.9.1
+Version: 0.9.2
 Summary: WebSocket library for Trio
 Home-page: https://github.com/HyperionGray/trio-websocket
 Author: Mark E. Haase
 Author-email: mehaase@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/HyperionGray/trio-websocket/issues
 Project-URL: Source, https://github.com/HyperionGray/trio-websocket
```

### Comparing `trio-websocket-0.9.1/README.md` & `trio-websocket-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `trio-websocket-0.9.1/setup.py` & `trio-websocket-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `trio-websocket-0.9.1/trio_websocket/_impl.py` & `trio-websocket-0.9.2/trio_websocket/_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1090,14 +1090,20 @@
         '''
         self._for_testing_peer_closed_connection.set()
         await trio.sleep(0)
         if self._wsproto.state == ConnectionState.REMOTE_CLOSING:
             await self._send(event.response())
         await self._close_web_socket(event.code, event.reason or None)
         self._close_handshake.set()
+        # RFC: "When a server is instructed to Close the WebSocket Connection
+        #   it SHOULD initiate a TCP Close immediately, and when a client is
+        #   instructed to do the same, it SHOULD wait for a TCP Close from the
+        #   server."
+        if self.is_server:
+            await self._close_stream()
 
     async def _handle_message_event(self, event):
         '''
         Handle a message event.
 
         :param event:
         :type event: wsproto.events.BytesMessage or wsproto.events.TextMessage
```

### Comparing `trio-websocket-0.9.1/trio_websocket.egg-info/PKG-INFO` & `trio-websocket-0.9.2/trio_websocket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trio-websocket
-Version: 0.9.1
+Version: 0.9.2
 Summary: WebSocket library for Trio
 Home-page: https://github.com/HyperionGray/trio-websocket
 Author: Mark E. Haase
 Author-email: mehaase@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/HyperionGray/trio-websocket/issues
 Project-URL: Source, https://github.com/HyperionGray/trio-websocket
```

