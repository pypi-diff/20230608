# Comparing `tmp/ucall-0.5.0-cp39-cp39-manylinux_2_27_x86_64.manylinux_2_28_x86_64.whl.zip` & `tmp/ucall-0.5.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,23 @@
-Zip file size: 1336039 bytes, number of entries: 24
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 19:15 ucall/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 19:15 ucall-0.5.0.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 19:15 ucall./
--rw-r--r--  2.0 unx      171 b- defN 23-May-19 19:15 ucall/rich_uring.py
--rw-r--r--  2.0 unx    59794 b- defN 23-May-19 19:15 ucall/libbase64.a
--rw-r--r--  2.0 unx      171 b- defN 23-May-19 19:15 ucall/rich_posix.py
--rw-r--r--  2.0 unx     2043 b- defN 23-May-19 19:15 ucall/_server.py
--rw-r--r--  2.0 unx   341484 b- defN 23-May-19 19:15 ucall/libmbedtls.a
--rw-r--r--  2.0 unx   258716 b- defN 23-May-19 19:15 ucall/libsimdjson.a
--rwxr-xr-x  2.0 unx  1188352 b- defN 23-May-19 19:15 ucall/posix.so
--rw-r--r--  2.0 unx    56568 b- defN 23-May-19 19:15 ucall/libucall_server_posix.a
--rw-r--r--  2.0 unx     6330 b- defN 23-May-19 19:15 ucall/client.py
--rw-r--r--  2.0 unx   104752 b- defN 23-May-19 19:15 ucall/libmbedx509.a
--rw-r--r--  2.0 unx     3462 b- defN 23-May-19 19:15 ucall/cli.py
--rw-r--r--  2.0 unx   955080 b- defN 23-May-19 19:15 ucall/libmbedcrypto.a
--rw-r--r--  2.0 unx    61080 b- defN 23-May-19 19:15 ucall/libucall_server_uring.a
--rw-r--r--  2.0 unx        0 b- defN 23-May-19 19:15 ucall/__init__.py
--rwxr-xr-x  2.0 unx   452448 b- defN 23-May-19 19:15 ucall/uring.so
--rw-r--r--  2.0 unx        6 b- defN 23-May-19 19:15 ucall-0.5.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx    11357 b- defN 23-May-19 19:15 ucall-0.5.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1636 b- defN 23-May-19 19:15 ucall-0.5.0.dist-info/RECORD
--rw-r--r--  2.0 unx    12822 b- defN 23-May-19 19:15 ucall-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx      149 b- defN 23-May-19 19:15 ucall-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-May-19 19:15 ucall-0.5.0.dist-info/entry_points.txt
-24 files, 3516461 bytes uncompressed, 1333193 bytes compressed:  62.1%
+Zip file size: 1367731 bytes, number of entries: 21
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-08 16:54 ucall/__init__.py
+-rw-rw-rw-  2.0 fat     2117 b- defN 23-Jun-08 16:54 ucall/_server.py
+-rw-rw-rw-  2.0 fat     3578 b- defN 23-Jun-08 16:54 ucall/cli.py
+-rw-rw-rw-  2.0 fat     6547 b- defN 23-Jun-08 16:54 ucall/client.py
+-rw-rw-rw-  2.0 fat      178 b- defN 23-Jun-08 16:54 ucall/rich_posix.py
+-rw-rw-rw-  2.0 fat      178 b- defN 23-Jun-08 16:54 ucall/rich_uring.py
+-rw-rw-rw-  2.0 fat    37934 b- defN 23-Jun-08 17:00 ucall/Release/base64.lib
+-rw-rw-rw-  2.0 fat  1662764 b- defN 23-Jun-08 17:00 ucall/Release/mbedcrypto.lib
+-rw-rw-rw-  2.0 fat   684334 b- defN 23-Jun-08 17:00 ucall/Release/mbedtls.lib
+-rw-rw-rw-  2.0 fat   189292 b- defN 23-Jun-08 17:00 ucall/Release/mbedx509.lib
+-rw-rw-rw-  2.0 fat      728 b- defN 23-Jun-08 17:00 ucall/Release/posix.exp
+-rw-rw-rw-  2.0 fat     1698 b- defN 23-Jun-08 17:00 ucall/Release/posix.lib
+-rw-rw-rw-  2.0 fat   708608 b- defN 23-Jun-08 17:00 ucall/Release/posix.pyd
+-rw-rw-rw-  2.0 fat   395386 b- defN 23-Jun-08 17:00 ucall/Release/simdjson.lib
+-rw-rw-rw-  2.0 fat   146762 b- defN 23-Jun-08 17:00 ucall/Release/ucall_server_posix.lib
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-08 17:00 ucall-0.5.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    13177 b- defN 23-Jun-08 17:00 ucall-0.5.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-08 17:00 ucall-0.5.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       40 b- defN 23-Jun-08 17:00 ucall-0.5.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-08 17:00 ucall-0.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1666 b- defN 23-Jun-08 17:00 ucall-0.5.1.dist-info/RECORD
+21 files, 3866651 bytes uncompressed, 1365075 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -1,73 +1,64 @@
-Filename: ucall/
-Comment: 
-
-Filename: ucall-0.5.0.dist-info/
+Filename: ucall/__init__.py
 Comment: 
 
-Filename: ucall./
+Filename: ucall/_server.py
 Comment: 
 
-Filename: ucall/rich_uring.py
+Filename: ucall/cli.py
 Comment: 
 
-Filename: ucall/libbase64.a
+Filename: ucall/client.py
 Comment: 
 
 Filename: ucall/rich_posix.py
 Comment: 
 
-Filename: ucall/_server.py
-Comment: 
-
-Filename: ucall/libmbedtls.a
-Comment: 
-
-Filename: ucall/libsimdjson.a
+Filename: ucall/rich_uring.py
 Comment: 
 
-Filename: ucall/posix.so
+Filename: ucall/Release/base64.lib
 Comment: 
 
-Filename: ucall/libucall_server_posix.a
+Filename: ucall/Release/mbedcrypto.lib
 Comment: 
 
-Filename: ucall/client.py
+Filename: ucall/Release/mbedtls.lib
 Comment: 
 
-Filename: ucall/libmbedx509.a
+Filename: ucall/Release/mbedx509.lib
 Comment: 
 
-Filename: ucall/cli.py
+Filename: ucall/Release/posix.exp
 Comment: 
 
-Filename: ucall/libmbedcrypto.a
+Filename: ucall/Release/posix.lib
 Comment: 
 
-Filename: ucall/libucall_server_uring.a
+Filename: ucall/Release/posix.pyd
 Comment: 
 
-Filename: ucall/__init__.py
+Filename: ucall/Release/simdjson.lib
 Comment: 
 
-Filename: ucall/uring.so
+Filename: ucall/Release/ucall_server_posix.lib
 Comment: 
 
-Filename: ucall-0.5.0.dist-info/top_level.txt
+Filename: ucall-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: ucall-0.5.0.dist-info/LICENSE
+Filename: ucall-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: ucall-0.5.0.dist-info/RECORD
+Filename: ucall-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: ucall-0.5.0.dist-info/METADATA
+Filename: ucall-0.5.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ucall-0.5.0.dist-info/WHEEL
+Filename: ucall-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ucall-0.5.0.dist-info/entry_points.txt
+Filename: ucall-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## ucall/rich_uring.py

 * *Ordering differences only*

```diff
@@ -1,7 +1,7 @@
-from ucall import uring as ucall
-from ucall._server import _Server
-
-
-class Server(_Server):
-    def __init__(self, **kwargs):
-        self.server = ucall.Server(**kwargs)
+from ucall import uring as ucall
+from ucall._server import _Server
+
+
+class Server(_Server):
+    def __init__(self, **kwargs):
+        self.server = ucall.Server(**kwargs)
```

## ucall/rich_posix.py

 * *Ordering differences only*

```diff
@@ -1,7 +1,7 @@
-from ucall import posix as ucall
-from ucall._server import _Server
-
-
-class Server(_Server):
-    def __init__(self, **kwargs):
-        self.server = ucall.Server(**kwargs)
+from ucall import posix as ucall
+from ucall._server import _Server
+
+
+class Server(_Server):
+    def __init__(self, **kwargs):
+        self.server = ucall.Server(**kwargs)
```

## ucall/_server.py

 * *Ordering differences only*

```diff
@@ -1,74 +1,74 @@
-import inspect
-from typing import Callable, get_type_hints
-from functools import wraps
-from io import BytesIO
-
-import numpy as np
-from PIL import Image
-
-
-class _Server:
-
-    def __init__(self) -> None:
-        self.server = None
-
-    def __call__(self, func: Callable):
-        return self.route(func)
-
-    def run(self, max_cycles: int = -1, max_seconds: float = -1):
-        return self.server.run(max_cycles, max_seconds)
-
-    def unpack(self, arg: bytes, hint: type):
-        if hint == bytes or hint == bytearray:
-            return arg
-
-        bin = BytesIO(arg)
-
-        if hint == np.ndarray:
-            return np.load(bin, allow_pickle=True)
-        if hint == Image.Image:
-            return Image.open(bin)
-
-    def pack(self, res):
-        if isinstance(res, np.ndarray):
-            buf = BytesIO()
-            np.save(buf, res)
-            return buf.getvalue()
-
-        if isinstance(res, Image.Image):
-            buf = BytesIO()
-            if not res.format:
-                res.format = 'tiff'
-            res.save(buf, res.format, compression='raw', compression_level=0)
-
-            return buf.getvalue()
-
-        return res
-
-    def route(self, func: Callable):
-        hints = get_type_hints(func)
-
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            new_args = []
-            new_kwargs = {}
-
-            for arg, hint in zip(args, hints.values()):
-                assert isinstance(hint, type), 'Hint must be a type!'
-                if isinstance(arg, bytes):
-                    new_args.append(self.unpack(arg, hint))
-                else:
-                    new_args.append(arg)
-
-            for kw, arg in kwargs.items():
-                if isinstance(arg, bytes):
-                    new_kwargs[kw] = self.unpack(arg, hints[kw])
-                else:
-                    new_kwargs[kw] = arg
-
-            res = func(*new_args, **new_kwargs)
-            return self.pack(res)
-
-        wrapper.__signature__ = inspect.signature(func)
-        self.server.route(wrapper)
-        return wrapper
+import inspect
+from typing import Callable, get_type_hints
+from functools import wraps
+from io import BytesIO
+
+import numpy as np
+from PIL import Image
+
+
+class _Server:
+
+    def __init__(self) -> None:
+        self.server = None
+
+    def __call__(self, func: Callable):
+        return self.route(func)
+
+    def run(self, max_cycles: int = -1, max_seconds: float = -1):
+        return self.server.run(max_cycles, max_seconds)
+
+    def unpack(self, arg: bytes, hint: type):
+        if hint == bytes or hint == bytearray:
+            return arg
+
+        bin = BytesIO(arg)
+
+        if hint == np.ndarray:
+            return np.load(bin, allow_pickle=True)
+        if hint == Image.Image:
+            return Image.open(bin)
+
+    def pack(self, res):
+        if isinstance(res, np.ndarray):
+            buf = BytesIO()
+            np.save(buf, res)
+            return buf.getvalue()
+
+        if isinstance(res, Image.Image):
+            buf = BytesIO()
+            if not res.format:
+                res.format = 'tiff'
+            res.save(buf, res.format, compression='raw', compression_level=0)
+
+            return buf.getvalue()
+
+        return res
+
+    def route(self, func: Callable):
+        hints = get_type_hints(func)
+
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            new_args = []
+            new_kwargs = {}
+
+            for arg, hint in zip(args, hints.values()):
+                assert isinstance(hint, type), 'Hint must be a type!'
+                if isinstance(arg, bytes):
+                    new_args.append(self.unpack(arg, hint))
+                else:
+                    new_args.append(arg)
+
+            for kw, arg in kwargs.items():
+                if isinstance(arg, bytes):
+                    new_kwargs[kw] = self.unpack(arg, hints[kw])
+                else:
+                    new_kwargs[kw] = arg
+
+            res = func(*new_args, **new_kwargs)
+            return self.pack(res)
+
+        wrapper.__signature__ = inspect.signature(func)
+        self.server.route(wrapper)
+        return wrapper
```

## ucall/client.py

 * *Ordering differences only*

```diff
@@ -1,217 +1,217 @@
-import ssl
-import json
-import errno
-import base64
-import random
-import socket
-from io import BytesIO
-from typing import Union
-
-import numpy as np
-from PIL import Image
-
-
-def _receive_all(sock, buffer_size=4096):
-    header = sock.recv(4)
-    body = None
-    content_len = -1
-
-    if header == b'HTTP':
-        while b'\r\n\r\n' not in header:
-            chunk = sock.recv(1024)
-            if not chunk:
-                break
-            header += chunk
-
-        header, body = header.split(b'\r\n\r\n', 1)
-
-        pref = b'Content-Length:'
-        for line in header.splitlines():
-            if line.startswith(pref):
-                content_len = int(line[len(pref):].strip())
-                break
-    else:
-        body = header
-
-    content_len -= len(body)
-    while content_len != 0:
-        chunk = sock.recv(buffer_size)
-        if not chunk:
-            break
-        body += chunk
-        content_len -= len(chunk)
-
-    return body
-
-
-class Response:
-
-    def __init__(self, data):
-        self.data = data
-
-    @property
-    def json(self) -> Union[bool, int, float, str, dict, list, tuple]:
-        self.raise_for_status()
-        return self.data['result']
-
-    def raise_for_status(self):
-        if 'error' in self.data:
-            raise RuntimeError(self.data['error'])
-
-    @property
-    def bytes(self) -> bytes:
-        return base64.b64decode(self.json)
-
-    @property
-    def numpy(self) -> np.ndarray:
-        buf = BytesIO(self.bytes)
-        return np.load(buf, allow_pickle=True)
-
-    @property
-    def image(self) -> Image.Image:
-        buf = BytesIO(self.bytes)
-        return Image.open(buf)
-
-
-class Request:
-
-    def __init__(self, json):
-        self.data = json
-        self.packed = self.pack(json)
-
-    def _pack_numpy(self, array):
-        buf = BytesIO()
-        np.save(buf, array)
-        buf.seek(0)
-        return base64.b64encode(buf.getvalue()).decode()
-
-    def _pack_bytes(self, buffer):
-        return base64.b64encode(buffer).decode()
-
-    def _pack_pillow(self, image):
-        buf = BytesIO()
-        if not image.format:
-            image.format = 'tiff'
-        image.save(buf, image.format,  compression='raw', compression_level=0)
-        buf.seek(0)
-        return base64.b64encode(buf.getvalue()).decode()
-
-    def pack(self, req):
-        keys = None
-        if isinstance(req['params'], dict):
-            keys = req['params'].keys()
-        else:
-            keys = range(0, len(req['params']))
-
-        for k in keys:
-            if isinstance(req['params'][k], np.ndarray):
-                req['params'][k] = self._pack_numpy(req['params'][k])
-
-            elif isinstance(req['params'][k], Image.Image):
-                req['params'][k] = self._pack_pillow(req['params'][k])
-
-            elif isinstance(req['params'][k], bytes):
-                req['params'][k] = self._pack_bytes(req['params'][k])
-
-        return req
-
-
-class Client:
-    """JSON-RPC Client that uses classic sync Python `requests` to pass JSON calls over HTTP"""
-
-    def __init__(self, uri: str = '127.0.0.1', port: int = 8545, use_http: bool = True) -> None:
-        self.uri = uri
-        self.port = port
-        self.use_http = use_http
-        self.sock = None
-        self.http_template = f'POST / HTTP/1.1\r\nHost: {uri}:{port}\r\nUser-Agent: py-ucall\r\nAccept: */*\r\nConnection: keep-alive\r\nContent-Length: %i\r\nContent-Type: application/json\r\n\r\n'
-
-    def __getattr__(self, name):
-        def call(*args, **kwargs):
-            params = kwargs
-            if len(args) != 0:
-                assert len(
-                    kwargs) == 0, 'Can\'t mix positional and keyword parameters!'
-                params = args
-
-            return self.__call__({
-                'method': name,
-                'params': params,
-                'jsonrpc': '2.0',
-            })
-
-        return call
-
-    def _make_socket(self):
-        if not self._socket_is_closed():
-            return
-        self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.sock.connect((self.uri, self.port))
-
-    def _socket_is_closed(self) -> bool:
-        """
-        Returns True if the remote side did close the connection
-        """
-        if self.sock is None:
-            return True
-        try:
-            buf = self.sock.recv(1, socket.MSG_PEEK | socket.MSG_DONTWAIT)
-            if buf == b'':
-                return True
-        except BlockingIOError as exc:
-            if exc.errno != errno.EAGAIN:
-                raise
-        return False
-
-    def _send(self, json_data: dict):
-        json_data['id'] = random.randint(1, 2**16)
-        req_obj = Request(json_data)
-        request = json.dumps(req_obj.packed)
-        if self.use_http:
-            request = self.http_template % (len(request)) + request
-
-        self._make_socket()
-        self.sock.send(request.encode())
-
-    def _recv(self) -> Response:
-        response_bytes = _receive_all(self.sock)
-        response = json.loads(response_bytes)
-        return Response(response)
-
-    def __call__(self, jsonrpc: object) -> Response:
-        self._send(jsonrpc)
-        return self._recv()
-
-
-class ClientTLS(Client):
-    def __init__(
-            self, uri: str = '127.0.0.1', port: int = 8545, ssl_context: ssl.SSLContext = None,
-            allow_self_signed: bool = False, enable_session_resumption: bool = True) -> None:
-
-        super().__init__(uri, port, use_http=True)
-
-        if ssl_context is None:
-            ssl_context = ssl.create_default_context()
-            if allow_self_signed:
-                ssl_context.check_hostname = False
-                ssl_context.verify_mode = ssl.CERT_NONE
-
-        self.ssl_context = ssl_context
-        self.session = None
-        self.session_resumption = enable_session_resumption
-
-    def _make_socket(self):
-        if not self._socket_is_closed():
-            return
-        self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.sock = self.ssl_context.wrap_socket(
-            self.sock, server_hostname=self.uri, session=self.session)
-        self.sock.connect((self.uri, self.port))
-        if self.session_resumption:
-            self.session = self.sock.session
-
-    def _socket_is_closed(self) -> bool:
-        if self.sock is None:
-            return True
-        self.sock.read(1, None)
-        return self.sock.pending() <= 0
+import ssl
+import json
+import errno
+import base64
+import random
+import socket
+from io import BytesIO
+from typing import Union
+
+import numpy as np
+from PIL import Image
+
+
+def _receive_all(sock, buffer_size=4096):
+    header = sock.recv(4)
+    body = None
+    content_len = -1
+
+    if header == b'HTTP':
+        while b'\r\n\r\n' not in header:
+            chunk = sock.recv(1024)
+            if not chunk:
+                break
+            header += chunk
+
+        header, body = header.split(b'\r\n\r\n', 1)
+
+        pref = b'Content-Length:'
+        for line in header.splitlines():
+            if line.startswith(pref):
+                content_len = int(line[len(pref):].strip())
+                break
+    else:
+        body = header
+
+    content_len -= len(body)
+    while content_len != 0:
+        chunk = sock.recv(buffer_size)
+        if not chunk:
+            break
+        body += chunk
+        content_len -= len(chunk)
+
+    return body
+
+
+class Response:
+
+    def __init__(self, data):
+        self.data = data
+
+    @property
+    def json(self) -> Union[bool, int, float, str, dict, list, tuple]:
+        self.raise_for_status()
+        return self.data['result']
+
+    def raise_for_status(self):
+        if 'error' in self.data:
+            raise RuntimeError(self.data['error'])
+
+    @property
+    def bytes(self) -> bytes:
+        return base64.b64decode(self.json)
+
+    @property
+    def numpy(self) -> np.ndarray:
+        buf = BytesIO(self.bytes)
+        return np.load(buf, allow_pickle=True)
+
+    @property
+    def image(self) -> Image.Image:
+        buf = BytesIO(self.bytes)
+        return Image.open(buf)
+
+
+class Request:
+
+    def __init__(self, json):
+        self.data = json
+        self.packed = self.pack(json)
+
+    def _pack_numpy(self, array):
+        buf = BytesIO()
+        np.save(buf, array)
+        buf.seek(0)
+        return base64.b64encode(buf.getvalue()).decode()
+
+    def _pack_bytes(self, buffer):
+        return base64.b64encode(buffer).decode()
+
+    def _pack_pillow(self, image):
+        buf = BytesIO()
+        if not image.format:
+            image.format = 'tiff'
+        image.save(buf, image.format,  compression='raw', compression_level=0)
+        buf.seek(0)
+        return base64.b64encode(buf.getvalue()).decode()
+
+    def pack(self, req):
+        keys = None
+        if isinstance(req['params'], dict):
+            keys = req['params'].keys()
+        else:
+            keys = range(0, len(req['params']))
+
+        for k in keys:
+            if isinstance(req['params'][k], np.ndarray):
+                req['params'][k] = self._pack_numpy(req['params'][k])
+
+            elif isinstance(req['params'][k], Image.Image):
+                req['params'][k] = self._pack_pillow(req['params'][k])
+
+            elif isinstance(req['params'][k], bytes):
+                req['params'][k] = self._pack_bytes(req['params'][k])
+
+        return req
+
+
+class Client:
+    """JSON-RPC Client that uses classic sync Python `requests` to pass JSON calls over HTTP"""
+
+    def __init__(self, uri: str = '127.0.0.1', port: int = 8545, use_http: bool = True) -> None:
+        self.uri = uri
+        self.port = port
+        self.use_http = use_http
+        self.sock = None
+        self.http_template = f'POST / HTTP/1.1\r\nHost: {uri}:{port}\r\nUser-Agent: py-ucall\r\nAccept: */*\r\nConnection: keep-alive\r\nContent-Length: %i\r\nContent-Type: application/json\r\n\r\n'
+
+    def __getattr__(self, name):
+        def call(*args, **kwargs):
+            params = kwargs
+            if len(args) != 0:
+                assert len(
+                    kwargs) == 0, 'Can\'t mix positional and keyword parameters!'
+                params = args
+
+            return self.__call__({
+                'method': name,
+                'params': params,
+                'jsonrpc': '2.0',
+            })
+
+        return call
+
+    def _make_socket(self):
+        if not self._socket_is_closed():
+            return
+        self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self.sock.connect((self.uri, self.port))
+
+    def _socket_is_closed(self) -> bool:
+        """
+        Returns True if the remote side did close the connection
+        """
+        if self.sock is None:
+            return True
+        try:
+            buf = self.sock.recv(1, socket.MSG_PEEK | socket.MSG_DONTWAIT)
+            if buf == b'':
+                return True
+        except BlockingIOError as exc:
+            if exc.errno != errno.EAGAIN:
+                raise
+        return False
+
+    def _send(self, json_data: dict):
+        json_data['id'] = random.randint(1, 2**16)
+        req_obj = Request(json_data)
+        request = json.dumps(req_obj.packed)
+        if self.use_http:
+            request = self.http_template % (len(request)) + request
+
+        self._make_socket()
+        self.sock.send(request.encode())
+
+    def _recv(self) -> Response:
+        response_bytes = _receive_all(self.sock)
+        response = json.loads(response_bytes)
+        return Response(response)
+
+    def __call__(self, jsonrpc: object) -> Response:
+        self._send(jsonrpc)
+        return self._recv()
+
+
+class ClientTLS(Client):
+    def __init__(
+            self, uri: str = '127.0.0.1', port: int = 8545, ssl_context: ssl.SSLContext = None,
+            allow_self_signed: bool = False, enable_session_resumption: bool = True) -> None:
+
+        super().__init__(uri, port, use_http=True)
+
+        if ssl_context is None:
+            ssl_context = ssl.create_default_context()
+            if allow_self_signed:
+                ssl_context.check_hostname = False
+                ssl_context.verify_mode = ssl.CERT_NONE
+
+        self.ssl_context = ssl_context
+        self.session = None
+        self.session_resumption = enable_session_resumption
+
+    def _make_socket(self):
+        if not self._socket_is_closed():
+            return
+        self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self.sock = self.ssl_context.wrap_socket(
+            self.sock, server_hostname=self.uri, session=self.session)
+        self.sock.connect((self.uri, self.port))
+        if self.session_resumption:
+            self.session = self.sock.session
+
+    def _socket_is_closed(self) -> bool:
+        if self.sock is None:
+            return True
+        self.sock.read(1, None)
+        return self.sock.pending() <= 0
```

## ucall/cli.py

 * *Ordering differences only*

```diff
@@ -1,116 +1,116 @@
-from pydoc import locate
-from typing import Optional
-import json
-import argparse
-
-from PIL import Image
-
-from ucall.client import Client
-
-
-def get_kwargs(buffer):
-    kwargs = {}
-    if buffer is not None:
-        for arg in buffer:
-            sp = None
-            if '=' in arg:
-                sp = arg.split('=')
-            else:
-                raise KeyError('Missing key in kwarg argument')
-            kwargs[sp[0]] = sp[1]
-    return kwargs
-
-
-def cast(value: str, type_name: Optional[str]):
-    """Casts a single argument value to the expected `type_name` or guesses it."""
-    if type_name is None:
-        if value.isdigit():
-            return int(value)
-        if value.replace('.', '', 1).isdigit():
-            return float(value)
-        if value in ['True', 'False']:
-            return bool(value)
-        return value
-
-    type_name = type_name.lower()
-    if type_name == 'image':
-        return Image.open(value)
-    if type_name == 'binary':
-        return open(value, 'rb').read()
-
-    return locate(type_name)(value)
-
-
-def fix_types(args, kwargs):
-    """Casts `args` and `kwargs` to expected types."""
-    for i in range(len(args)):
-        if ':' in args[i]:
-            val, tp = args[i].split(':')
-            args[i] = cast(val, tp)
-        else:
-            args[i] = cast(args[i], None)
-    keys = list(kwargs.keys())
-    for k in keys:
-        if ':' in k:
-            key, tp = k.split(':')
-            val = kwargs.pop(k)
-            kwargs[key] = cast(val, tp)
-        else:
-            kwargs[k] = cast(kwargs[k], None)
-
-
-def add_specials(kwargs: dict, special: Optional[list[str]], type_name: str):
-    if special is None:
-        return
-    for x in special:
-        if not '=' in x:
-            raise KeyError(f'Missing key in {type_name} argument')
-        k, v = x.split('=')
-        kwargs[k + ':' + type_name] = v
-
-
-def cli():
-    parsed = get_parser().parse_args()
-    kwargs = get_kwargs(parsed.kwargs)
-    args = parsed.positional if parsed.positional else []
-
-    add_specials(kwargs, parsed.file, 'binary')
-    add_specials(kwargs, parsed.image, 'image')
-
-    fix_types(args, kwargs)
-    client = Client(uri=parsed.uri, port=parsed.port, use_http=True)
-    res = getattr(client, parsed.method)(*args, **kwargs)
-
-    if parsed.format == 'raw':
-        print(json.dumps(res.data, indent=4))
-    else:
-        try:
-            print(getattr(res, parsed.format))
-        except Exception as err:
-            print('Error:', err)
-
-
-def get_parser():
-    parser = argparse.ArgumentParser(description='UCall Client CLI')
-    parser.add_argument('method', type=str, help='Method name')
-
-    parser.add_argument('--uri', type=str, default='localhost',
-                        help='Server URI')
-    parser.add_argument('-p', '--port', type=int, default=8545,
-                        help='Server port')
-
-    parser.add_argument('kwargs', nargs='*', help='KEY[:TYPE]=VALUE arguments')
-    parser.add_argument('-f', '--file', nargs='*', help='Binary files')
-    parser.add_argument('-i', '--image', nargs='*', help='Image files')
-
-    parser.add_argument('--positional', nargs='*',
-                        help='Switch to positional arguments VALUE[:TYPE]')
-
-    parser.add_argument('--format', type=str,
-                        choices=['json', 'bytes', 'numpy', 'image', 'raw'], default='raw',
-                        help='How to parse and format the response')
-    return parser
-
-
-if __name__ == '__main__':
-    cli()
+from pydoc import locate
+from typing import Optional
+import json
+import argparse
+
+from PIL import Image
+
+from ucall.client import Client
+
+
+def get_kwargs(buffer):
+    kwargs = {}
+    if buffer is not None:
+        for arg in buffer:
+            sp = None
+            if '=' in arg:
+                sp = arg.split('=')
+            else:
+                raise KeyError('Missing key in kwarg argument')
+            kwargs[sp[0]] = sp[1]
+    return kwargs
+
+
+def cast(value: str, type_name: Optional[str]):
+    """Casts a single argument value to the expected `type_name` or guesses it."""
+    if type_name is None:
+        if value.isdigit():
+            return int(value)
+        if value.replace('.', '', 1).isdigit():
+            return float(value)
+        if value in ['True', 'False']:
+            return bool(value)
+        return value
+
+    type_name = type_name.lower()
+    if type_name == 'image':
+        return Image.open(value)
+    if type_name == 'binary':
+        return open(value, 'rb').read()
+
+    return locate(type_name)(value)
+
+
+def fix_types(args, kwargs):
+    """Casts `args` and `kwargs` to expected types."""
+    for i in range(len(args)):
+        if ':' in args[i]:
+            val, tp = args[i].split(':')
+            args[i] = cast(val, tp)
+        else:
+            args[i] = cast(args[i], None)
+    keys = list(kwargs.keys())
+    for k in keys:
+        if ':' in k:
+            key, tp = k.split(':')
+            val = kwargs.pop(k)
+            kwargs[key] = cast(val, tp)
+        else:
+            kwargs[k] = cast(kwargs[k], None)
+
+
+def add_specials(kwargs: dict, special: Optional[list[str]], type_name: str):
+    if special is None:
+        return
+    for x in special:
+        if not '=' in x:
+            raise KeyError(f'Missing key in {type_name} argument')
+        k, v = x.split('=')
+        kwargs[k + ':' + type_name] = v
+
+
+def cli():
+    parsed = get_parser().parse_args()
+    kwargs = get_kwargs(parsed.kwargs)
+    args = parsed.positional if parsed.positional else []
+
+    add_specials(kwargs, parsed.file, 'binary')
+    add_specials(kwargs, parsed.image, 'image')
+
+    fix_types(args, kwargs)
+    client = Client(uri=parsed.uri, port=parsed.port, use_http=True)
+    res = getattr(client, parsed.method)(*args, **kwargs)
+
+    if parsed.format == 'raw':
+        print(json.dumps(res.data, indent=4))
+    else:
+        try:
+            print(getattr(res, parsed.format))
+        except Exception as err:
+            print('Error:', err)
+
+
+def get_parser():
+    parser = argparse.ArgumentParser(description='UCall Client CLI')
+    parser.add_argument('method', type=str, help='Method name')
+
+    parser.add_argument('--uri', type=str, default='localhost',
+                        help='Server URI')
+    parser.add_argument('-p', '--port', type=int, default=8545,
+                        help='Server port')
+
+    parser.add_argument('kwargs', nargs='*', help='KEY[:TYPE]=VALUE arguments')
+    parser.add_argument('-f', '--file', nargs='*', help='Binary files')
+    parser.add_argument('-i', '--image', nargs='*', help='Image files')
+
+    parser.add_argument('--positional', nargs='*',
+                        help='Switch to positional arguments VALUE[:TYPE]')
+
+    parser.add_argument('--format', type=str,
+                        choices=['json', 'bytes', 'numpy', 'image', 'raw'], default='raw',
+                        help='How to parse and format the response')
+    return parser
+
+
+if __name__ == '__main__':
+    cli()
```

## Comparing `ucall-0.5.0.dist-info/LICENSE` & `ucall-0.5.1.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

## Comparing `ucall-0.5.0.dist-info/METADATA` & `ucall-0.5.1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,364 +1,364 @@
-Metadata-Version: 2.1
-Name: ucall
-Version: 0.5.0
-Summary: Up to 100x Faster FastAPI. JSON-RPC with io_uring, SIMD-acceleration, and pure CPython bindings
-Home-page: https://github.com/unum-cloud/ucall
-Author: Ashot Vardanian
-Author-email: info@unum.cloud
-License: Apache-2.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: C
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Programming Language :: C
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Communications :: File Sharing
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: System :: Networking
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy (>=1.16)
-Requires-Dist: pillow
-
-<h1 align="center">UCall</h1>
-<h3 align="center">
-JSON Remote Procedure Calls Library<br/>
-Up to 100x Faster than FastAPI<br/>
-</h3>
-<br/>
-
-<p align="center">
-<a href="https://discord.gg/xuDmpbEDnQ"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/discord.svg" alt="Discord"></a>
-&nbsp;&nbsp;&nbsp;
-<a href="https://www.linkedin.com/company/unum-cloud/"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/linkedin.svg" alt="LinkedIn"></a>
-&nbsp;&nbsp;&nbsp;
-<a href="https://twitter.com/unum_cloud"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/twitter.svg" alt="Twitter"></a>
-&nbsp;&nbsp;&nbsp;
-<a href="https://unum.cloud/post"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/blog.svg" alt="Blog"></a>
-&nbsp;&nbsp;&nbsp;
-<a href="https://github.com/unum-cloud/ucall"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/github.svg" alt="GitHub"></a>
-</p>
-
----
-
-Most modern networking is built either on slow and ambiguous REST APIs or unnecessarily complex gRPC.
-FastAPI, for example, looks very approachable.
-We aim to be equally or even simpler to use.
-
-<table width="100%">
-<tr>
-<th width="50%">FastAPI</th><th width="50%">UCall</th>
-</tr>
-<tr>
-<td>
-
-```sh
-pip install fastapi uvicorn
-```
-
-</td>
-<td>
-
-```sh
-pip install ucall
-```
-
-</td>
-</tr>
-<tr>
-<td>
-
-```python
-from fastapi import FastAPI
-import uvicorn
-
-server = FastAPI()
-
-@server.get('/sum')
-def sum(a: int, b: int):
-    return a + b
-
-uvicorn.run(...)    
-```
-
-</td>
-<td>
-
-```python
-from ucall.posix import Server
-# from ucall.uring import Server on 5.19+
-
-server = Server()
-
-@server
-def sum(a: int, b: int):
-    return a + b
-
-server.run()    
-```
-
-</td>
-</tr>
-</table>
-
-It takes over a millisecond to handle a trivial FastAPI call on a recent 8-core CPU.
-In that time, light could have traveled 300 km through optics to the neighboring city or country, in my case.
-How does UCall compare to FastAPI and gRPC?
-
-| Setup                   |   🔁   | Server | Latency w 1 client | Throughput w 32 clients |
-| :---------------------- | :---: | :----: | -----------------: | ----------------------: |
-| Fast API over REST      |   ❌   |   🐍    |           1'203 μs |               3'184 rps |
-| Fast API over WebSocket |   ✅   |   🐍    |              86 μs |            11'356 rps ¹ |
-| gRPC ²                  |   ✅   |   🐍    |             164 μs |               9'849 rps |
-|                         |       |        |                    |                         |
-| UCall with POSIX        |   ❌   |   C    |              62 μs |              79'000 rps |
-| UCall with io_uring     |   ✅   |   🐍    |              40 μs |             210'000 rps |
-| UCall with io_uring     |   ✅   |   C    |              22 μs |             231'000 rps |
-
-<details>
-  <summary>Table legend</summary>
-
-All benchmarks were conducted on AWS on general purpose instances with **Ubuntu 22.10 AMI**.
-It is the first major AMI to come with **Linux Kernel 5.19**, featuring much wider `io_uring` support for networking operations.
-These specific numbers were obtained on `c7g.metal` beefy instances with Graviton 3 chips.
-
-- The 🔁 column marks, if the TCP/IP connection is being reused during subsequent requests.
-- The "server" column defines the programming language, in which the server was implemented.
-- The "latency" column report the amount of time between sending a request and receiving a response. μ stands for micro, μs subsequently means microseconds.
-- The "throughput" column reports the number of Requests Per Second when querying the same server application from multiple client processes running on the same machine.
-
-> ¹ FastAPI couldn't process concurrent requests with WebSockets.
-
-> ² We tried generating C++ backends with gRPC, but its numbers, suspiciously, weren't better. There is also an async gRPC option, that wasn't tried.
-
-</details>
-
-## How is that possible?!
-
-How can a tiny pet-project with just a couple thousand lines of code compete with two of the most established networking libraries?
-**UCall stands on the shoulders of Giants**:
-
-- `io_uring` for interrupt-less IO.
-  - `io_uring_prep_read_fixed` on 5.1+.
-  - `io_uring_prep_accept_direct` on 5.19+.
-  - `io_uring_register_files_sparse` on 5.19+.
-  - `IORING_SETUP_COOP_TASKRUN` optional on 5.19+.
-  - `IORING_SETUP_SINGLE_ISSUER` optional on 6.0+.
-
-- SIMD-accelerated parsers with manual memory control.
-  - [`simdjson`][simdjson] to parse JSON faster than gRPC can unpack `ProtoBuf`.
-  - [`Turbo-Base64`][base64] to decode binary values from a `Base64` form.
-  - [`picohttpparser`][picohttpparser] to navigate HTTP headers.
-
-You have already seen the latency of the round trip..., the throughput in requests per second..., want to see the bandwidth?
-Try yourself!
-
-```python
-@server
-def echo(data: bytes):
-    return data
-```
-
-## More Functionality than FastAPI
-
-FastAPI supports native type, while UCall supports `numpy.ndarray`, `PIL.Image` and other custom types.
-This comes handy when you build real applications or want to deploy Multi-Modal AI, like we do with [UForm](https://github.com/unum-cloud/uform).
-
-```python
-from ucall.rich_posix import Server
-import ufrom
-
-server = Server()
-model = uform.get_model('unum-cloud/uform-vl-multilingual')
-
-@server
-def vectorize(description: str, photo: PIL.Image.Image) -> numpy.ndarray:
-    image = model.preprocess_image(photo)
-    tokens = model.preprocess_text(description)
-    joint_embedding = model.encode_multimodal(image=image, text=tokens)
-
-    return joint_embedding.cpu().detach().numpy()
-```
-
-We also have our own optional `Client` class that helps with those custom types.
-
-```python
-from ucall.client import Client
-
-client = Client()
-# Explicit JSON-RPC call:
-response = client({
-    'method': 'vectorize',
-    'params': {
-        'description': description,
-        'image': image,
-    },
-    'jsonrpc': '2.0',
-    'id': 100,
-})
-# Or the same with syntactic sugar:
-response = client.vectorize(description=description, image=image) 
-```
-
-## CLI like [cURL](https://curl.se/docs/manpage.html)
-
-Aside from the Python `Client`, we provide an easy-to-use Command Line Interface, which comes with `pip install ucall`.
-It allow you to call a remote server, upload files, with direct support for images and NumPy arrays.
-Translating previous example into a Bash script, to call the server on the same machine:
-
-```sh
-ucall vectorize description='Product description' -i image=./local/path.png
-```
-
-To address a remote server:
-
-```sh
-ucall vectorize description='Product description' -i image=./local/path.png --uri 0.0.0.0 -p 8545
-```
-
-To print the docs, use `ucall -h`:
-
-```txt
-usage: ucall [-h] [--uri URI] [--port PORT] [-f [FILE ...]] [-i [IMAGE ...]] [--positional [POSITIONAL ...]] method [kwargs ...]
-
-UCall Client CLI
-
-positional arguments:
-  method                method name
-  kwargs                method arguments
-
-options:
-  -h, --help            show this help message and exit
-  --uri URI             server uri
-  --port PORT           server port
-  -f [FILE ...], --file [FILE ...]
-                        method positional arguments
-  -i [IMAGE ...], --image [IMAGE ...]
-                        method positional arguments
-  --positional [POSITIONAL ...]
-                        method positional arguments
-```
-
-You can also explicitly annotate types, to distinguish integers, floats, and strings, to avoid ambiguity.
-
-```
-ucall auth id=256
-ucall auth id:int=256
-ucall auth id:str=256
-```
-
-## Free Tier Throughput
-
-We will leave bandwidth measurements to enthusiasts, but will share some more numbers.
-The general logic is that you can't squeeze high performance from Free-Tier machines.
-Currently AWS provides following options: `t2.micro` and `t4g.small`, on older Intel and newer Graviton 2 chips.
-This library is so fast, that it doesn't need more than 1 core, so you can run a fast server even on a tiny Free-Tier server!
-
-| Setup                   |   🔁   | Server | Clients | `t2.micro` | `t4g.small` |
-| :---------------------- | :---: | :----: | :-----: | ---------: | ----------: |
-| Fast API over REST      |   ❌   |   🐍    |    1    |    328 rps |     424 rps |
-| Fast API over WebSocket |   ✅   |   🐍    |    1    |  1'504 rps |   3'051 rps |
-| gRPC                    |   ✅   |   🐍    |    1    |  1'169 rps |   1'974 rps |
-|                         |       |        |         |            |             |
-| UCall with POSIX        |   ❌   |   C    |    1    |  1'082 rps |   2'438 rps |
-| UCall with io_uring     |   ✅   |   C    |    1    |          - |   5'864 rps |
-| UCall with POSIX        |   ❌   |   C    |   32    |  3'399 rps |  39'877 rps |
-| UCall with io_uring     |   ✅   |   C    |   32    |          - |  88'455 rps |
-
-In this case, every server was bombarded by requests from 1 or a fleet of 32 other instances in the same availability zone.
-If you want to reproduce those benchmarks, check out the [`sum` examples on GitHub][sum-examples].
-
-## Quick Start
-
-For Python:
-
-```sh
-pip install ucall
-```
-
-For CMake projects:
-
-```cmake
-include(FetchContent)
-FetchContent_Declare(
-    ucall
-    GIT_REPOSITORY https://github.com/unum-cloud/ucall
-    GIT_SHALLOW TRUE
-)
-FetchContent_MakeAvailable(ucall)
-include_directories(${ucall_SOURCE_DIR}/include)
-```
-
-The C usage example is mouthful compared to Python.
-We wanted to make it as lightweight as possible and to allow optional arguments without dynamic allocations and named lookups.
-So unlike the Python layer, we expect the user to manually extract the arguments from the call context with `ucall_param_named_i64()`, and its siblings.
-
-```c
-#include <cstdio.h>
-#include <ucall/ucall.h>
-
-static void sum(ucall_call_t call, ucall_callback_tag_t) {
-    int64_t a{}, b{};
-    char printed_sum[256]{};
-    bool got_a = ucall_param_named_i64(call, "a", 0, &a);
-    bool got_b = ucall_param_named_i64(call, "b", 0, &b);
-    if (!got_a || !got_b)
-        return ucall_call_reply_error_invalid_params(call);
-
-    int len = snprintf(printed_sum, 256, "%ll", a + b);
-    ucall_call_reply_content(call, printed_sum, len);
-}
-
-int main(int argc, char** argv) {
-
-    ucall_server_t server{};
-    ucall_config_t config{};
-
-    ucall_init(&config, &server);
-    ucall_add_procedure(server, "sum", &sum, NULL);
-    ucall_take_calls(server, 0);
-    ucall_free(server);
-    return 0;
-}
-```
-
-## Roadmap
-
-- [x] Batch Requests
-- [x] JSON-RPC over raw TCP sockets
-- [x] JSON-RPC over TCP with HTTP
-- [x] Concurrent sessions
-- [x] NumPy `array` and Pillow serialization
-- [ ] HTTP**S** support
-- [ ] Batch-capable endpoints for ML
-- [ ] Zero-ETL relay calls
-- [ ] Integrating with [UKV][ukv]
-- [ ] WebSockets for web interfaces
-- [ ] AF_XDP and UDP-based analogs on Linux
-
-> Want to affect the roadmap and request a feature? Join the discussions on Discord.
-
-## Why JSON-RPC?
-
-- Transport independent: UDP, TCP, bring what you want.
-- Application layer is optional: use HTTP or not.
-- Unlike REST APIs, there is just one way to pass arguments.
-
-[simdjson]: https://github.com/simdjson/simdjson
-[base64]: https://github.com/powturbo/Turbo-Base64
-[picohttpparser]: https://github.com/h2o/picohttpparser
-[sum-examples]: https://github.com/unum-cloud/ucall/tree/dev/examples/sum
-[ukv]: https://github.com/unum-cloud/ukv
+Metadata-Version: 2.1
+Name: ucall
+Version: 0.5.1
+Summary: Up to 100x Faster FastAPI. JSON-RPC with io_uring, SIMD-acceleration, and pure CPython bindings
+Home-page: https://github.com/unum-cloud/ucall
+Author: Ashot Vardanian
+Author-email: info@unum.cloud
+License: Apache-2.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: C
+Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: C
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Communications :: File Sharing
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: System :: Networking
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pillow
+
+<h1 align="center">UCall</h1>
+<h3 align="center">
+JSON Remote Procedure Calls Library<br/>
+Up to 100x Faster than FastAPI<br/>
+</h3>
+<br/>
+
+<p align="center">
+<a href="https://discord.gg/xuDmpbEDnQ"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/discord.svg" alt="Discord"></a>
+&nbsp;&nbsp;&nbsp;
+<a href="https://www.linkedin.com/company/unum-cloud/"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/linkedin.svg" alt="LinkedIn"></a>
+&nbsp;&nbsp;&nbsp;
+<a href="https://twitter.com/unum_cloud"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/twitter.svg" alt="Twitter"></a>
+&nbsp;&nbsp;&nbsp;
+<a href="https://unum.cloud/post"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/blog.svg" alt="Blog"></a>
+&nbsp;&nbsp;&nbsp;
+<a href="https://github.com/unum-cloud/ucall"><img height="25" src="https://github.com/unum-cloud/ukv/raw/main/assets/icons/github.svg" alt="GitHub"></a>
+</p>
+
+---
+
+Most modern networking is built either on slow and ambiguous REST APIs or unnecessarily complex gRPC.
+FastAPI, for example, looks very approachable.
+We aim to be equally or even simpler to use.
+
+<table width="100%">
+<tr>
+<th width="50%">FastAPI</th><th width="50%">UCall</th>
+</tr>
+<tr>
+<td>
+
+```sh
+pip install fastapi uvicorn
+```
+
+</td>
+<td>
+
+```sh
+pip install ucall
+```
+
+</td>
+</tr>
+<tr>
+<td>
+
+```python
+from fastapi import FastAPI
+import uvicorn
+
+server = FastAPI()
+
+@server.get('/sum')
+def sum(a: int, b: int):
+    return a + b
+
+uvicorn.run(...)    
+```
+
+</td>
+<td>
+
+```python
+from ucall.posix import Server
+# from ucall.uring import Server on 5.19+
+
+server = Server()
+
+@server
+def sum(a: int, b: int):
+    return a + b
+
+server.run()    
+```
+
+</td>
+</tr>
+</table>
+
+It takes over a millisecond to handle a trivial FastAPI call on a recent 8-core CPU.
+In that time, light could have traveled 300 km through optics to the neighboring city or country, in my case.
+How does UCall compare to FastAPI and gRPC?
+
+| Setup                   |   🔁   | Server | Latency w 1 client | Throughput w 32 clients |
+| :---------------------- | :---: | :----: | -----------------: | ----------------------: |
+| Fast API over REST      |   ❌   |   🐍    |           1'203 μs |               3'184 rps |
+| Fast API over WebSocket |   ✅   |   🐍    |              86 μs |            11'356 rps ¹ |
+| gRPC ²                  |   ✅   |   🐍    |             164 μs |               9'849 rps |
+|                         |       |        |                    |                         |
+| UCall with POSIX        |   ❌   |   C    |              62 μs |              79'000 rps |
+| UCall with io_uring     |   ✅   |   🐍    |              40 μs |             210'000 rps |
+| UCall with io_uring     |   ✅   |   C    |              22 μs |             231'000 rps |
+
+<details>
+  <summary>Table legend</summary>
+
+All benchmarks were conducted on AWS on general purpose instances with **Ubuntu 22.10 AMI**.
+It is the first major AMI to come with **Linux Kernel 5.19**, featuring much wider `io_uring` support for networking operations.
+These specific numbers were obtained on `c7g.metal` beefy instances with Graviton 3 chips.
+
+- The 🔁 column marks, if the TCP/IP connection is being reused during subsequent requests.
+- The "server" column defines the programming language, in which the server was implemented.
+- The "latency" column report the amount of time between sending a request and receiving a response. μ stands for micro, μs subsequently means microseconds.
+- The "throughput" column reports the number of Requests Per Second when querying the same server application from multiple client processes running on the same machine.
+
+> ¹ FastAPI couldn't process concurrent requests with WebSockets.
+
+> ² We tried generating C++ backends with gRPC, but its numbers, suspiciously, weren't better. There is also an async gRPC option, that wasn't tried.
+
+</details>
+
+## How is that possible?!
+
+How can a tiny pet-project with just a couple thousand lines of code compete with two of the most established networking libraries?
+**UCall stands on the shoulders of Giants**:
+
+- `io_uring` for interrupt-less IO.
+  - `io_uring_prep_read_fixed` on 5.1+.
+  - `io_uring_prep_accept_direct` on 5.19+.
+  - `io_uring_register_files_sparse` on 5.19+.
+  - `IORING_SETUP_COOP_TASKRUN` optional on 5.19+.
+  - `IORING_SETUP_SINGLE_ISSUER` optional on 6.0+.
+
+- SIMD-accelerated parsers with manual memory control.
+  - [`simdjson`][simdjson] to parse JSON faster than gRPC can unpack `ProtoBuf`.
+  - [`Turbo-Base64`][base64] to decode binary values from a `Base64` form.
+  - [`picohttpparser`][picohttpparser] to navigate HTTP headers.
+
+You have already seen the latency of the round trip..., the throughput in requests per second..., want to see the bandwidth?
+Try yourself!
+
+```python
+@server
+def echo(data: bytes):
+    return data
+```
+
+## More Functionality than FastAPI
+
+FastAPI supports native type, while UCall supports `numpy.ndarray`, `PIL.Image` and other custom types.
+This comes handy when you build real applications or want to deploy Multi-Modal AI, like we do with [UForm](https://github.com/unum-cloud/uform).
+
+```python
+from ucall.rich_posix import Server
+import ufrom
+
+server = Server()
+model = uform.get_model('unum-cloud/uform-vl-multilingual')
+
+@server
+def vectorize(description: str, photo: PIL.Image.Image) -> numpy.ndarray:
+    image = model.preprocess_image(photo)
+    tokens = model.preprocess_text(description)
+    joint_embedding = model.encode_multimodal(image=image, text=tokens)
+
+    return joint_embedding.cpu().detach().numpy()
+```
+
+We also have our own optional `Client` class that helps with those custom types.
+
+```python
+from ucall.client import Client
+
+client = Client()
+# Explicit JSON-RPC call:
+response = client({
+    'method': 'vectorize',
+    'params': {
+        'description': description,
+        'image': image,
+    },
+    'jsonrpc': '2.0',
+    'id': 100,
+})
+# Or the same with syntactic sugar:
+response = client.vectorize(description=description, image=image) 
+```
+
+## CLI like [cURL](https://curl.se/docs/manpage.html)
+
+Aside from the Python `Client`, we provide an easy-to-use Command Line Interface, which comes with `pip install ucall`.
+It allow you to call a remote server, upload files, with direct support for images and NumPy arrays.
+Translating previous example into a Bash script, to call the server on the same machine:
+
+```sh
+ucall vectorize description='Product description' -i image=./local/path.png
+```
+
+To address a remote server:
+
+```sh
+ucall vectorize description='Product description' -i image=./local/path.png --uri 0.0.0.0 -p 8545
+```
+
+To print the docs, use `ucall -h`:
+
+```txt
+usage: ucall [-h] [--uri URI] [--port PORT] [-f [FILE ...]] [-i [IMAGE ...]] [--positional [POSITIONAL ...]] method [kwargs ...]
+
+UCall Client CLI
+
+positional arguments:
+  method                method name
+  kwargs                method arguments
+
+options:
+  -h, --help            show this help message and exit
+  --uri URI             server uri
+  --port PORT           server port
+  -f [FILE ...], --file [FILE ...]
+                        method positional arguments
+  -i [IMAGE ...], --image [IMAGE ...]
+                        method positional arguments
+  --positional [POSITIONAL ...]
+                        method positional arguments
+```
+
+You can also explicitly annotate types, to distinguish integers, floats, and strings, to avoid ambiguity.
+
+```
+ucall auth id=256
+ucall auth id:int=256
+ucall auth id:str=256
+```
+
+## Free Tier Throughput
+
+We will leave bandwidth measurements to enthusiasts, but will share some more numbers.
+The general logic is that you can't squeeze high performance from Free-Tier machines.
+Currently AWS provides following options: `t2.micro` and `t4g.small`, on older Intel and newer Graviton 2 chips.
+This library is so fast, that it doesn't need more than 1 core, so you can run a fast server even on a tiny Free-Tier server!
+
+| Setup                   |   🔁   | Server | Clients | `t2.micro` | `t4g.small` |
+| :---------------------- | :---: | :----: | :-----: | ---------: | ----------: |
+| Fast API over REST      |   ❌   |   🐍    |    1    |    328 rps |     424 rps |
+| Fast API over WebSocket |   ✅   |   🐍    |    1    |  1'504 rps |   3'051 rps |
+| gRPC                    |   ✅   |   🐍    |    1    |  1'169 rps |   1'974 rps |
+|                         |       |        |         |            |             |
+| UCall with POSIX        |   ❌   |   C    |    1    |  1'082 rps |   2'438 rps |
+| UCall with io_uring     |   ✅   |   C    |    1    |          - |   5'864 rps |
+| UCall with POSIX        |   ❌   |   C    |   32    |  3'399 rps |  39'877 rps |
+| UCall with io_uring     |   ✅   |   C    |   32    |          - |  88'455 rps |
+
+In this case, every server was bombarded by requests from 1 or a fleet of 32 other instances in the same availability zone.
+If you want to reproduce those benchmarks, check out the [`sum` examples on GitHub][sum-examples].
+
+## Quick Start
+
+For Python:
+
+```sh
+pip install ucall
+```
+
+For CMake projects:
+
+```cmake
+include(FetchContent)
+FetchContent_Declare(
+    ucall
+    GIT_REPOSITORY https://github.com/unum-cloud/ucall
+    GIT_SHALLOW TRUE
+)
+FetchContent_MakeAvailable(ucall)
+include_directories(${ucall_SOURCE_DIR}/include)
+```
+
+The C usage example is mouthful compared to Python.
+We wanted to make it as lightweight as possible and to allow optional arguments without dynamic allocations and named lookups.
+So unlike the Python layer, we expect the user to manually extract the arguments from the call context with `ucall_param_named_i64()`, and its siblings.
+
+```c
+#include <cstdio.h>
+#include <ucall/ucall.h>
+
+static void sum(ucall_call_t call, ucall_callback_tag_t) {
+    int64_t a{}, b{};
+    char printed_sum[256]{};
+    bool got_a = ucall_param_named_i64(call, "a", 0, &a);
+    bool got_b = ucall_param_named_i64(call, "b", 0, &b);
+    if (!got_a || !got_b)
+        return ucall_call_reply_error_invalid_params(call);
+
+    int len = snprintf(printed_sum, 256, "%ll", a + b);
+    ucall_call_reply_content(call, printed_sum, len);
+}
+
+int main(int argc, char** argv) {
+
+    ucall_server_t server{};
+    ucall_config_t config{};
+
+    ucall_init(&config, &server);
+    ucall_add_procedure(server, "sum", &sum, NULL);
+    ucall_take_calls(server, 0);
+    ucall_free(server);
+    return 0;
+}
+```
+
+## Roadmap
+
+- [x] Batch Requests
+- [x] JSON-RPC over raw TCP sockets
+- [x] JSON-RPC over TCP with HTTP
+- [x] Concurrent sessions
+- [x] NumPy `array` and Pillow serialization
+- [ ] HTTP**S** support
+- [ ] Batch-capable endpoints for ML
+- [ ] Zero-ETL relay calls
+- [ ] Integrating with [UKV][ukv]
+- [ ] WebSockets for web interfaces
+- [ ] AF_XDP and UDP-based analogs on Linux
+
+> Want to affect the roadmap and request a feature? Join the discussions on Discord.
+
+## Why JSON-RPC?
+
+- Transport independent: UDP, TCP, bring what you want.
+- Application layer is optional: use HTTP or not.
+- Unlike REST APIs, there is just one way to pass arguments.
+
+[simdjson]: https://github.com/simdjson/simdjson
+[base64]: https://github.com/powturbo/Turbo-Base64
+[picohttpparser]: https://github.com/h2o/picohttpparser
+[sum-examples]: https://github.com/unum-cloud/ucall/tree/dev/examples/sum
+[ukv]: https://github.com/unum-cloud/ukv
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ucall Version: 0.5.0 Summary: Up to 100x Faster
+Metadata-Version: 2.1 Name: ucall Version: 0.5.1 Summary: Up to 100x Faster
 FastAPI. JSON-RPC with io_uring, SIMD-acceleration, and pure CPython bindings
 Home-page: https://github.com/unum-cloud/ucall Author: Ashot Vardanian Author-
 email: info@unum.cloud License: Apache-2.0 Classifier: Development Status :: 5
 - Production/Stable Classifier: Natural Language :: English Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Information
 Technology Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
@@ -12,15 +12,15 @@
 System :: MacOS Classifier: Programming Language :: C Classifier: Programming
 Language :: C++ Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Topic :: Communications :: File Sharing Classifier:
 Topic :: Internet :: WWW/HTTP Classifier: Topic :: System :: Networking
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: numpy (>=1.16) Requires-Dist: pillow
+LICENSE Requires-Dist: numpy Requires-Dist: pillow
                               ****** UCall ******
                    **** JSON Remote Procedure Calls Library
                         Up to 100x Faster than FastAPI
                                       ****
 
         [Discord]     [LinkedIn]     [Twitter]     [Blog]     [GitHub]
 --- Most modern networking is built either on slow and ambiguous REST APIs or
```

