# Comparing `tmp/mcproto-0.2.0.tar.gz` & `tmp/mcproto-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcproto-0.2.0.tar", max compression
+gzip compressed data, was "mcproto-0.3.0.tar", max compression
```

## Comparing `mcproto-0.2.0.tar` & `mcproto-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,34 @@
--rw-r--r--   0        0        0     2693 2022-12-30 00:34:06.536627 mcproto-0.2.0/LICENSE-THIRD-PARTY.txt
--rw-r--r--   0        0        0     7651 2022-12-30 00:34:06.536627 mcproto-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0    17352 2022-12-30 00:34:06.536627 mcproto-0.2.0/README.md
--rw-r--r--   0        0        0       35 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/__init__.py
--rw-r--r--   0        0        0     2426 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/buffer.py
--rw-r--r--   0        0        0     8685 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/connection.py
--rw-r--r--   0        0        0      590 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/packets/__init__.py
--rw-r--r--   0        0        0     1028 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/packets/abc.py
--rw-r--r--   0        0        0     3506 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/packets/interactions.py
--rw-r--r--   0        0        0     3720 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/packets/map.py
--rw-r--r--   0        0        0       35 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/packets/v757/__init__.py
--rw-r--r--   0        0        0       35 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/packets/v757/handshaking/__init__.py
--rw-r--r--   0        0        0     2201 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/packets/v757/handshaking/handshake.py
--rw-r--r--   0        0        0       35 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/packets/v757/status/__init__.py
--rw-r--r--   0        0        0      979 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/packets/v757/status/ping.py
--rw-r--r--   0        0        0     1378 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/packets/v757/status/status.py
--rw-r--r--   0        0        0      277 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/protocol/__init__.py
--rw-r--r--   0        0        0    24593 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/protocol/base_io.py
--rw-r--r--   0        0        0     1060 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/protocol/utils.py
--rw-r--r--   0        0        0        0 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/py.typed
--rw-r--r--   0        0        0       35 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/utils/__init__.py
--rw-r--r--   0        0        0     3301 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/utils/abc.py
--rw-r--r--   0        0        0     3186 2022-12-30 00:34:06.536627 mcproto-0.2.0/mcproto/utils/deprecation.py
--rw-r--r--   0        0        0     5420 2022-12-30 00:34:06.540627 mcproto-0.2.0/mcproto/utils/version.py
--rw-r--r--   0        0        0    10886 2022-12-30 00:34:06.540627 mcproto-0.2.0/mcproto/utils/version_map.py
--rw-r--r--   0        0        0     5283 2022-12-30 00:35:31.815885 mcproto-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    18689 1970-01-01 00:00:00.000000 mcproto-0.2.0/setup.py
--rw-r--r--   0        0        0    18831 1970-01-01 00:00:00.000000 mcproto-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2744 2023-06-08 15:40:16.419106 mcproto-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2924 2023-06-08 15:40:16.423106 mcproto-0.3.0/LICENSE-THIRD-PARTY.txt
+-rw-r--r--   0        0        0     7651 2023-06-08 15:40:16.423106 mcproto-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0    17616 2023-06-08 15:40:16.423106 mcproto-0.3.0/README.md
+-rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/__init__.py
+-rw-r--r--   0        0        0     3211 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/buffer.py
+-rw-r--r--   0        0        0    12532 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/connection.py
+-rw-r--r--   0        0        0      590 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/__init__.py
+-rw-r--r--   0        0        0     1028 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/abc.py
+-rw-r--r--   0        0        0     3514 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/interactions.py
+-rw-r--r--   0        0        0     3913 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/map.py
+-rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/__init__.py
+-rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/handshaking/__init__.py
+-rw-r--r--   0        0        0     2215 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/handshaking/handshake.py
+-rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/login/__init__.py
+-rw-r--r--   0        0        0     7924 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/login/login.py
+-rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/status/__init__.py
+-rw-r--r--   0        0        0     1150 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/status/ping.py
+-rw-r--r--   0        0        0     1492 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/packets/v757/status/status.py
+-rw-r--r--   0        0        0      277 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/protocol/__init__.py
+-rw-r--r--   0        0        0    24710 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/protocol/base_io.py
+-rw-r--r--   0        0        0     1553 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/protocol/utils.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/py.typed
+-rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/types/__init__.py
+-rw-r--r--   0        0        0      204 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/types/abc.py
+-rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/types/v757/__init__.py
+-rw-r--r--   0        0        0     2001 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/types/v757/chat.py
+-rw-r--r--   0        0        0      709 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/types/v757/uuid.py
+-rw-r--r--   0        0        0       35 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/utils/__init__.py
+-rw-r--r--   0        0        0     3415 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/utils/abc.py
+-rw-r--r--   0        0        0     4385 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/utils/deprecation.py
+-rw-r--r--   0        0        0    14537 2023-06-08 15:40:16.423106 mcproto-0.3.0/mcproto/utils/version_map.py
+-rw-r--r--   0        0        0     5879 2023-06-08 15:40:36.504008 mcproto-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    19005 1970-01-01 00:00:00.000000 mcproto-0.3.0/PKG-INFO
```

### Comparing `mcproto-0.2.0/LICENSE-THIRD-PARTY.txt` & `mcproto-0.3.0/LICENSE-THIRD-PARTY.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,19 @@
     - Copyright (c) 2020 Nekokatt
       Copyright (c) 2021-present davfsa
       All rights reserved.
         - .github/ISSUE_TEMPLATE/bug_report.yml: Template heavily inspired by original
         - .github/ISSUE_TEMPLATE/feature_request.yml: Template heavily inspired by original
         - .github/workflows/fragment-check.yml: Entire file
         - .github/workflows/prepare-release.yml: Workflow heavily inspired by original
+        - .github/scripts/normalize_coverage.py: Entire file
+        - docs/_static/extra.css: Entire file
+    - Copyright (c) 2015-present Rapptz
+      All rights reserved.
+        - docs/pages/version_guarantees.rst: Entire file
 ---------------------------------------------------------------------------------------------------
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mcproto-0.2.0/LICENSE.txt` & `mcproto-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mcproto-0.2.0/README.md` & `mcproto-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-# <img src="https://i.imgur.com/nPCcxts.png" height=25> McProto
+# <img src="https://i.imgur.com/nPCcxts.png" style="height: 25px"> mcproto
 
 [![discord chat](https://img.shields.io/discord/936788458939224094.svg?logo=Discord)](https://discord.gg/C2wX7zduxC)
 ![supported python versions](https://img.shields.io/pypi/pyversions/mcproto.svg)
 [![current PyPI version](https://img.shields.io/pypi/v/mcproto.svg)](https://pypi.org/project/mcproto/)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/9464f1037f07a795de35/test_coverage)](https://codeclimate.com/github/py-mine/mcproto/test_coverage)
 [![Validation](https://github.com/ItsDrike/mcproto/actions/workflows/validation.yml/badge.svg)](https://github.com/ItsDrike/mcproto/actions/workflows/validation.yml)
 [![Unit tests](https://github.com/ItsDrike/mcproto/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/ItsDrike/mcproto/actions/workflows/unit-tests.yml)
+[![Docs](https://img.shields.io/readthedocs/mcproto?label=Docs)](https://mcproto.readthedocs.io/)
 
 This is a heavily Work-In-Progress library, which attempts to be a full wrapper around the minecraft protocol, allowing
 for simple interactions with minecraft servers, and perhaps even for use as a base to a full minecraft server
 implementation in python (though the speed will very likely be quite terrible, making it probably unusable as any
 real-world playable server).
 
 Currently, the library is very limited and doesn't yet have any documentation, so while contributions are welcome, fair
```

### Comparing `mcproto-0.2.0/mcproto/buffer.py` & `mcproto-0.3.0/mcproto/buffer.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,26 +9,34 @@
     __slots__ = ("pos",)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.pos = 0
 
     def write(self, data: bytes) -> None:
-        """Write new data into the buffer."""
+        """Write/Store given ``data`` into the buffer."""
         self.extend(data)
 
     def read(self, length: int) -> bytearray:
         """Read data stored in the buffer.
 
         Reading data doesn't remove that data, rather that data is treated as already read, and
-        next read will start from the first unread byte. If freeing the data is necessary, check the clear function.
+        next read will start from the first unread byte. If freeing the data is necessary, check
+        the :meth:`.clear` function.
 
-        Trying to read more data than is available will raise an IOError, however it will deplete the remaining data
-        and the partial data that was read will be a part of the error message. This behavior is here to mimic reading
-        from a socket connection.
+        :param length:
+            Amount of bytes to be read.
+
+            If the requested amount can't be read (buffer doesn't contain that much data/buffer
+            doesn't contain any data), an :exc:`IOError` will be reaised.
+
+            If there were some data in the buffer, but it was less than requested, this remaining
+            data will still be depleted and the partial data that was read will be a part of the
+            error message in the :exc:`IOError`. This behavior is here to mimic reading from a real
+            socket connection.
         """
         end = self.pos + length
 
         if end > len(self):
             data = self[self.pos : len(self)]
             bytes_read = len(self) - self.pos
             self.pos = len(self)
@@ -39,33 +47,42 @@
 
         try:
             return self[self.pos : end]
         finally:
             self.pos = end
 
     def clear(self, only_already_read: bool = False) -> None:
-        """
-        Clear out the stored data and reset position.
+        """Clear out the stored data and reset position.
 
-        If `only_already_read` is True, only clear out the data which was already read, and reset the position.
-        This is mostly useful to avoid keeping large chunks of data in memory for no reason.
+        :param only_already_read:
+            When set to ``True``, only the data that was already marked as read will be cleared,
+            and the position will be reset (to start at the remaining data). This can be useful
+            for avoiding needlessly storing large amounts of data in memory, if this data is no
+            longer useful.
+
+            Otherwise, if set to ``False``, all of the data is cleared, and the position is reset,
+            essentially resulting in a blank buffer.
         """
         if only_already_read:
             del self[: self.pos]
         else:
             super().clear()
         self.pos = 0
 
     def reset(self) -> None:
-        """Reset the position in the buffer."""
+        """Reset the position in the buffer.
+
+        Since the buffer doesn't automatically clear the already read data, it is possible to simply
+        reset the position and read the data it contains again.
+        """
         self.pos = 0
 
     def flush(self) -> bytearray:
         """Read all of the remaining data in the buffer and clear it out."""
         data = self[self.pos : len(self)]
         self.clear()
         return data
 
     @property
     def remaining(self) -> int:
-        """Get the amount of bytes that's still remaining in be buffer to be read."""
+        """Get the amount of bytes that's still remaining in the buffer to be read."""
         return len(self) - self.pos
```

### Comparing `mcproto-0.2.0/mcproto/connection.py` & `mcproto-0.3.0/mcproto/connection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import asyncio
+import errno
 import socket
 from abc import ABC, abstractmethod
 from typing import Generic, Optional, TypeVar
 
 import asyncio_dgram
 from typing_extensions import ParamSpec, Self
 
@@ -24,27 +25,37 @@
 T_SOCK = TypeVar("T_SOCK", bound=socket.socket)
 T_STREAMREADER = TypeVar("T_STREAMREADER", bound=asyncio.StreamReader)
 T_STREAMWRITER = TypeVar("T_STREAMWRITER", bound=asyncio.StreamWriter)
 T_DATAGRAM_CLIENT = TypeVar("T_DATAGRAM_CLIENT", bound=asyncio_dgram.aio.DatagramClient)
 
 
 class SyncConnection(BaseSyncReader, BaseSyncWriter, ABC):
+    """Base class for all classes handling synchronous connections."""
+
     __slots__ = ("closed",)
 
     def __init__(self):
         self.closed = False
 
     @classmethod
     @abstractmethod
     def make_client(cls, address: tuple[str, int], timeout: float) -> Self:
-        """Construct a client connection to given address."""
+        """Construct a client connection (Client -> Server) to given server ``address``.
+
+        :param address: Address of the server to connection to.
+        :param timeout:
+            Amount of seconds to wait for the connection to be established.
+            If connection can't be established within this time, :exc:`TimeoutError` will be raised.
+            This timeout is then also used for any further data receiving.
+        """
         raise NotImplementedError
 
     @abstractmethod
     def _close(self) -> None:
+        """Close the underlying connection."""
         raise NotImplementedError
 
     def close(self) -> None:
         """Close the connection (it cannot be used after this)."""
         self._close()
         self.closed = True
 
@@ -54,27 +65,37 @@
         return self
 
     def __exit__(self, *a, **kw) -> None:
         self.close()
 
 
 class AsyncConnection(BaseAsyncReader, BaseAsyncWriter, ABC):
+    """Base class for all classes handling asynchronous connections."""
+
     __slots__ = ("closed",)
 
     def __init__(self):
         self.closed = False
 
     @classmethod
     @abstractmethod
     async def make_client(cls, address: tuple[str, int], timeout: float) -> Self:
-        """Construct a client connection to given address."""
+        """Construct a client connection (Client -> Server) to given server ``address``.
+
+        :param address: Address of the server to connection to.
+        :param timeout:
+            Amount of seconds to wait for the connection to be established.
+            If connection can't be established within this time, :exc:`TimeoutError` will be raised.
+            This timeout is then also used for any further data receiving.
+        """
         raise NotImplementedError
 
     @abstractmethod
     async def _close(self) -> None:
+        """Close the underlying connection."""
         raise NotImplementedError
 
     async def close(self) -> None:
         """Close the connection (it cannot be used after this)."""
         await self._close()
         self.closed = True
 
@@ -84,32 +105,43 @@
         return self
 
     async def __aexit__(self, *a, **kw) -> None:
         await self.close()
 
 
 class TCPSyncConnection(SyncConnection, Generic[T_SOCK]):
+    """Synchronous connection using a TCP :class:`~socket.socket`."""
+
     __slots__ = ("socket",)
 
     def __init__(self, socket: T_SOCK):
         super().__init__()
         self.socket = socket
 
     @classmethod
     def make_client(cls, address: tuple[str, int], timeout: float) -> Self:
-        """Construct a client connection to given address."""
+        """Construct a client connection (Client -> Server) to given server ``address``.
+
+        :param address: Address of the server to connection to.
+        :param timeout:
+            Amount of seconds to wait for the connection to be established.
+            If connection can't be established within this time, :exc:`TimeoutError` will be raised.
+            This timeout is then also used for any further data receiving.
+        """
         sock = socket.create_connection(address, timeout=timeout)
         sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
         return cls(sock)
 
     def read(self, length: int) -> bytearray:
         """Receive data sent through the connection.
 
-        `length` controls how many bytes we want to receive. If the requested amount
-        of bytes isn't available to be received, IOError will be raised.
+        :param length:
+            Amount of bytes to be received. If the requested amount can't be received
+            (server didn't send that much data/server didn't send any data), an :exc:`IOError`
+            will be raised.
         """
         result = bytearray()
         while len(result) < length:
             new = self.socket.recv(length - len(result))
             if len(new) == 0:
                 # No information at all
                 if len(result) == 0:
@@ -120,43 +152,62 @@
                     f" Partial obtained data: {result!r}"
                 )
             result.extend(new)
 
         return result
 
     def write(self, data: bytes) -> None:
-        """Send given data over the connection."""
+        """Send given ``data`` over the connection."""
         self.socket.send(data)
 
     def _close(self) -> None:
-        """Close the connection (it cannot be used after this)."""
+        """Close the underlying connection."""
+        # Gracefully end the connection first (shutdown), informing the other side
+        # we're disconnecting, and waiting for them to disconnect cleanly (TCP FIN)
+        try:
+            self.socket.shutdown(socket.SHUT_RDWR)
+        except OSError as exc:
+            if exc.errno != errno.ENOTCONN:
+                raise
+
         self.socket.close()
 
 
 class TCPAsyncConnection(AsyncConnection, Generic[T_STREAMREADER, T_STREAMWRITER]):
+    """Asynchronous TCP connection using :class:`~asyncio.StreamWriter` and :class:`~asyncio.StreamReader`."""
+
     __slots__ = ("reader", "writer", "timeout")
 
     def __init__(self, reader: T_STREAMREADER, writer: T_STREAMWRITER, timeout: float):
         super().__init__()
         self.reader = reader
         self.writer = writer
         self.timeout = timeout
 
     @classmethod
     async def make_client(cls, address: tuple[str, int], timeout: float) -> Self:
-        """Construct a client connection to given address."""
+        """Construct a client connection (Client -> Server) to given server ``address``.
+
+        :param address: Address of the server to connection to.
+        :param timeout:
+            Amount of seconds to wait for the connection to be established.
+            If connection can't be established within this time, :exc:`TimeoutError` will be raised.
+            This timeout is then also used for any further data receiving.
+        """
         conn = asyncio.open_connection(address[0], address[1])
         reader, writer = await asyncio.wait_for(conn, timeout=timeout)
         return cls(reader, writer, timeout)
 
     async def read(self, length: int) -> bytearray:
         """Receive data sent through the connection.
 
-        `length` controls how many bytes we want to receive. If the requested amount
-        of bytes isn't available to be received, IOError will be raised.
+        :param length:
+            Amount of bytes to be received. If the requested amount can't be received
+            (server didn't send that much data/server didn't send any data), an :exc:`IOError`
+            will be raised.
         """
         result = bytearray()
         while len(result) < length:
             new = await asyncio.wait_for(self.reader.read(length - len(result)), timeout=self.timeout)
             if len(new) == 0:
                 # No information at all
                 if len(result) == 0:
@@ -167,90 +218,118 @@
                     f" Partial obtained data: {result!r}"
                 )
             result.extend(new)
 
         return result
 
     async def write(self, data: bytes) -> None:
-        """Send given data over the connection."""
+        """Send given ``data`` over the connection."""
         self.writer.write(data)
 
     async def _close(self) -> None:
-        """Close the connection (it cannot be used after this)."""
+        """Close the underlying connection."""
+        # Close automatically performs a graceful TCP connection shutdown too
         self.writer.close()
 
     @property
     def socket(self) -> socket.socket:
-        """Obtain the underlying socket behind the asyncio transport."""
+        """Obtain the underlying socket behind the :class:`~asyncio.Transport`."""
         return self.writer.transport._sock  # type: ignore
 
 
 class UDPSyncConnection(SyncConnection, Generic[T_SOCK]):
+    """Synchronous connection using a UDP :class:`~socket.socket`."""
+
     __slots__ = ("socket", "address")
 
     BUFFER_SIZE = 65535
 
     def __init__(self, socket: T_SOCK, address: tuple[str, int]):
         super().__init__()
         self.socket = socket
         self.address = address
 
     @classmethod
     def make_client(cls, address: tuple[str, int], timeout: float) -> Self:
-        """Construct a client connection to given address."""
+        """Construct a client connection (Client -> Server) to given server ``address``.
+
+        :param address: Address of the server to connection to.
+        :param timeout:
+            Amount of seconds to wait for the connection to be established.
+            If connection can't be established within this time, :exc:`TimeoutError` will be raised.
+            This timeout is then also used for any further data receiving.
+        """
         sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         sock.settimeout(timeout)
         return cls(sock, address)
 
     def read(self, length: Optional[int] = None) -> bytearray:
         """Receive data sent through the connection.
 
-        For UDP connections, `length` parameter is ignored and not required.
+        :param length:
+            For UDP connections, ``length`` parameter is ignored and not required.
+            Instead, UDP connections always read exactly :attr:`.BUFFER_SIZE` bytes.
+
+            If the requested amount can't be received (server didn't send that much
+            data/server didn't send any data), an :exc:`IOError` will be raised.
         """
         result = bytearray()
         while len(result) == 0:
             received_data, server_addr = self.socket.recvfrom(self.BUFFER_SIZE)
             result.extend(received_data)
         return result
 
     def write(self, data: bytes) -> None:
-        """Send given data over the connection."""
+        """Send given ``data`` over the connection."""
         self.socket.sendto(data, self.address)
 
     def _close(self) -> None:
-        """Close the connection (it cannot be used after this)."""
+        """Close the underlying connection."""
         self.socket.close()
 
 
 class UDPAsyncConnection(AsyncConnection, Generic[T_DATAGRAM_CLIENT]):
+    """Asynchronous UDP connection using :class:`~asyncio_dgram.DatagramClient`."""
+
     __slots__ = ("stream", "timeout")
 
     def __init__(self, stream: T_DATAGRAM_CLIENT, timeout: float):
         super().__init__()
         self.stream = stream
         self.timeout = timeout
 
     @classmethod
     async def make_client(cls, address: tuple[str, int], timeout: float) -> Self:
-        """Construct a client connection to given address."""
+        """Construct a client connection (Client -> Server) to given server ``address``.
+
+        :param address: Address of the server to connection to.
+        :param timeout:
+            Amount of seconds to wait for the connection to be established.
+            If connection can't be established within this time, :exc:`TimeoutError` will be raised.
+            This timeout is then also used for any further data receiving.
+        """
         conn = asyncio_dgram.connect(address)
         stream = await asyncio.wait_for(conn, timeout=timeout)
         return cls(stream, timeout)
 
     async def read(self, length: Optional[int] = None) -> bytearray:
         """Receive data sent through the connection.
 
-        For UDP connections, `length` parameter is ignored and not required.
+        :param length:
+            For UDP connections, ``length`` parameter is ignored and not required.
+
+            If the requested amount can't be received (server didn't send that much
+            data/server didn't send any data), an :exc:`IOError` will be raised.
         """
         result = bytearray()
         while len(result) == 0:
             received_data, server_addr = await asyncio.wait_for(self.stream.recv(), timeout=self.timeout)
             result.extend(received_data)
         return result
 
     async def write(self, data: bytes) -> None:
-        """Send given data over the connection."""
+        """Send given ``data`` over the connection."""
         await self.stream.send(data)
 
     async def _close(self) -> None:
-        """Close the connection (it cannot be used after this)."""
+        """Close the underlying connection."""
         self.stream.close()
```

### Comparing `mcproto-0.2.0/mcproto/packets/__init__.py` & `mcproto-0.3.0/mcproto/packets/__init__.py`

 * *Files identical despite different names*

### Comparing `mcproto-0.2.0/mcproto/packets/abc.py` & `mcproto-0.3.0/mcproto/packets/abc.py`

 * *Files identical despite different names*

### Comparing `mcproto-0.2.0/mcproto/packets/interactions.py` & `mcproto-0.3.0/mcproto/packets/interactions.py`

 * *Files 16% similar despite different names*

```diff
@@ -62,21 +62,21 @@
     packet_id = buf.read_varint()
     packet_data = buf.read(buf.remaining)
 
     return packet_map[packet_id].deserialize(Buffer(packet_data))
 
 
 def sync_write_packet(writer: BaseSyncWriter, packet: Packet, *, compressed: bool = False) -> None:
-    """Write given packet."""
+    """Write given ``packet``."""
     data_buf = _serialize_packet(packet, compressed=compressed)
     writer.write_bytearray(data_buf)
 
 
 async def async_write_packet(writer: BaseAsyncWriter, packet: Packet, *, compressed: bool = False) -> None:
-    """Write given packet."""
+    """Write given ``packet``."""
     data_buf = _serialize_packet(packet, compressed=compressed)
     await writer.write_bytearray(data_buf)
 
 
 def sync_read_packet(
     reader: BaseSyncReader,
     packet_map: Mapping[int, type[T_Packet]],
```

### Comparing `mcproto-0.2.0/mcproto/packets/map.py` & `mcproto-0.3.0/mcproto/packets/map.py`

 * *Files 20% similar despite different names*

```diff
@@ -53,40 +53,43 @@
         self,
         obj: Any,  # noqa: ANN401
         module_data: WalkableModuleData,
         protocol_version: int,
     ) -> TypeGuard[type[Packet]]:
         """Determine whether a member object should be considered as a valid component for given protocol version.
 
-        This method will be called for each potential member object (found when walking over all members of
-        __all__ from all submodules of the package for given protocol version).
+        When versioned components are obtained, all of the members listed in any module's ``__all__`` are
+        considered. This function serves as a filter, identifying whether a potential member object should be
+        considered as one of the versioned components.
 
-        This function shouldn't include any checks on whether an object is already registered in the version map
-        (key collisions), these are handled during the collection in load_version, all this function is responsible
-        for is checking whether this object is a valid component, components with conflicting keys are still
-        considered valid here, as they're handled elsewhere.
+        .. note:
+            This function shouldn't include any checks on whether an object is already registered in the version
+            map (key collisions), these are handled during the collection in :meth:`.load_version`, all this
+            function is responsible for is checking whether this object is a valid component, components with
+            conflicting keys are still considered valid here, as they're handled elsewhere.
 
-        Although if there is some additional data that needs to be unique for a component to be valid, which wouldn't
-        be caught as a key collision, this function can raise a ValueError.
+            However if there is some additional data that needs to be unique for a component to be valid, which
+            wouldn't be caught as a key collision, this function can raise a :exc:`ValueError`.
         """
         return issubclass(obj, Packet)
 
     @classmethod
     def _make_obtain_key(
         cls,
         obj: type[Packet],
         module_data: WalkableModuleData,
         protocol_version: int,
     ) -> tuple[PacketDirection, GameState, int]:
-        """Construct a unique obtain key for given object under given protocol version.
+        """Construct a unique obtain key for given versioned component (``obj``) under given ``protocol_version``.
 
-        Note: While the protocol version might be beneficial to know when constructing
-        the obtain key, it shouldn't be used directly as a part of the key, as the items
-        will already be split by their protocol versions, and this version will be known
-        at obtaining time.
+        .. note:
+            While the protocol version might be beneficial to know when constructing
+            the obtain key, it shouldn't be used directly as a part of the key, as the items
+            will already be split by their protocol versions, and this version will be known
+            at obtaining time.
         """
         if issubclass(obj, ClientBoundPacket):
             direction = PacketDirection.CLIENTBOUND
         elif issubclass(obj, ServerBoundPacket):
             direction = PacketDirection.SERVERBOUND
         else:
             raise ValueError("Invalid packet class: Neither server-bound not client-bound.")
```

### Comparing `mcproto-0.2.0/mcproto/packets/v757/handshaking/handshake.py` & `mcproto-0.3.0/mcproto/packets/v757/handshaking/handshake.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from enum import IntEnum
-from typing import ClassVar, Union
+from typing import ClassVar, Union, final
 
 from typing_extensions import Self
 
 from mcproto.buffer import Buffer
 from mcproto.packets.abc import GameState, ServerBoundPacket
 from mcproto.protocol.base_io import StructFormat
 
@@ -16,36 +16,37 @@
 
 
 class NextState(IntEnum):
     STATUS = 1
     LOGIN = 2
 
 
+@final
 class Handshake(ServerBoundPacket):
-    """Initializes connection between server and client. (Client -> Server)
-
-    :param int protocol_version: Protocol version number to be used.
-    :param str server_address: The host/address the client is connecting to.
-    :param int server_port: The port the client is connecting to.
-    :param Union[NextState, int] next_state: The next state for the server to move into.
-    """
+    """Initializes connection between server and client. (Client -> Server)"""
 
     PACKET_ID: ClassVar[int] = 0x00
     GAME_STATE: ClassVar[GameState] = GameState.HANDSHAKING
 
     __slots__ = ("protocol_version", "server_address", "server_port", "next_state")
 
     def __init__(
         self,
         *,
         protocol_version: int,
         server_address: str,
         server_port: int,
         next_state: Union[NextState, int],
     ):
+        """
+        :param protocol_version: Protocol version number to be used.
+        :param server_address: The host/address the client is connecting to.
+        :param server_port: The port the client is connecting to.
+        :param next_state: The next state for the server to move into.
+        """
         if isinstance(next_state, int):
             rev_lookup = {x.value: x for x in NextState.__members__.values()}
             try:
                 next_state = rev_lookup[next_state]
             except KeyError as exc:
                 raise ValueError("No such next_state.") from exc
```

### Comparing `mcproto-0.2.0/mcproto/packets/v757/status/ping.py` & `mcproto-0.3.0/mcproto/packets/v757/status/ping.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
 
-from typing import ClassVar
+from typing import ClassVar, final
 
 from typing_extensions import Self
 
 from mcproto.buffer import Buffer
 from mcproto.packets.abc import ClientBoundPacket, GameState, ServerBoundPacket
 from mcproto.protocol.base_io import StructFormat
 
 __all__ = ["PingPong"]
 
 
+@final
 class PingPong(ClientBoundPacket, ServerBoundPacket):
-    """Ping request/Pong response (Server <-> Client).
-
-    :param int payload: Random number to test out the connection (ideally a long one).
-    """
+    """Ping request/Pong response (Server <-> Client)."""
 
     __slots__ = ("payload",)
 
     PACKET_ID: ClassVar[int] = 0x01
     GAME_STATE: ClassVar[GameState] = GameState.STATUS
 
     def __init__(self, payload: int):
+        """
+        :param payload:
+            Random number to test out the connection. Ideally, this number should be quite big,
+            however it does need to fit within the limit of a signed long long (-2 ** 63 to 2 ** 63 - 1).
+        """
         self.payload = payload
 
     def serialize(self) -> Buffer:
         buf = Buffer()
         buf.write_value(StructFormat.LONGLONG, self.payload)
         return buf
```

### Comparing `mcproto-0.2.0/mcproto/packets/v757/status/status.py` & `mcproto-0.3.0/mcproto/packets/v757/status/status.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 from __future__ import annotations
 
 import json
-from typing import Any, ClassVar
+from typing import Any, ClassVar, final
 
 from typing_extensions import Self
 
 from mcproto.buffer import Buffer
 from mcproto.packets.abc import ClientBoundPacket, GameState, ServerBoundPacket
 
 __all__ = ["StatusRequest", "StatusResponse"]
 
 
+@final
 class StatusRequest(ServerBoundPacket):
     """Request from the client to get information on the server. (Client -> Server)"""
 
     __slots__ = ()
 
     PACKET_ID: ClassVar[int] = 0x00
     GAME_STATE: ClassVar[GameState] = GameState.STATUS
 
-    def serialize(self) -> Buffer:
+    def serialize(self) -> Buffer:  # pragma: no cover, nothing to test here.
         return Buffer()
 
     @classmethod
-    def deserialize(cls, buf: Buffer, /) -> Self:
+    def deserialize(cls, buf: Buffer, /) -> Self:  # pragma: no cover, nothing to test here.
         return cls()
 
 
+@final
 class StatusResponse(ClientBoundPacket):
-    """Response from the server to requesting client with status data information. (Server -> Client)
-
-    :param dict[str, Any] data: JSON response data sent back to the client.
-    """
+    """Response from the server to requesting client with status data information. (Server -> Client)"""
 
     __slots__ = ("data",)
 
     PACKET_ID: ClassVar[int] = 0x00
     GAME_STATE: ClassVar[GameState] = GameState.STATUS
 
     def __init__(self, data: dict[str, Any]):
+        """
+        :param data: JSON response data sent back to the client.
+        """
         self.data = data
 
     def serialize(self) -> Buffer:
         buf = Buffer()
         s = json.dumps(self.data)
         buf.write_utf(s)
         return buf
```

### Comparing `mcproto-0.2.0/mcproto/protocol/base_io.py` & `mcproto-0.3.0/mcproto/protocol/base_io.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,19 @@
 R = TypeVar("R")
 
 
 # region: Format types
 
 
 class StructFormat(str, Enum):
-    """All possible write/read struct types."""
+    """All possible write/read struct types.
+
+    .. seealso:
+        :module:`struct` module documentation.
+    """
 
     BOOL = "?"
     CHAR = "c"
     BYTE = "b"
     UBYTE = "B"
     SHORT = "h"
     USHORT = "H"
@@ -94,25 +98,25 @@
         ...
 
     @overload
     async def write_value(self, fmt: Literal[StructFormat.CHAR], value: str, /) -> None:
         ...
 
     async def write_value(self, fmt: StructFormat, value: object, /) -> None:
-        """Write a value of given struct format in big-endian mode."""
+        """Write a given ``value`` as given struct format (``fmt``) in big-endian mode."""
         await self.write(struct.pack(">" + fmt.value, value))
 
     async def _write_varuint(self, value: int, /, *, max_bits: Optional[int] = None) -> None:
         """Write an arbitrarily big unsigned integer in a variable length format.
 
         This is a standard way of transmitting ints, and it allows smaller numbers to take less bytes.
 
-        Writing will be limited up to integer values of `max_bits` bits, and trying to write bigger values will rase a
-        ValueError. Note that setting `max_bits` to for example 32 bits doesn't mean that at most 4 bytes will be sent,
-        in this case it would actually take at most 5 bytes, due to the variable encoding overhead.
+        Writing will be limited up to integer values of ``max_bits`` bits, and trying to write bigger values will rase
+        a :exc:`ValueError`. Note that setting ``max_bits`` to for example 32 bits doesn't mean that at most 4 bytes
+        will be sent, in this case it would actually take at most 5 bytes, due to the variable encoding overhead.
 
         Varints send bytes where 7 least significant bits are value bits, and the most significant bit is continuation
         flag bit. If this continuation bit is set (1), it indicates that there will be another varint byte sent after
         this one. The least significant group is written first, followed by each of the more significant groups, making
         varints little-endian, however in groups of 7 bits, not 8.
         """
         value_max = (1 << (max_bits)) - 1 if max_bits is not None else float("inf")
@@ -128,23 +132,23 @@
             await self.write_value(StructFormat.UBYTE, remaining & 0x7F | 0x80)
             # Subtract the value we've already sent (7 least significant bits)
             remaining >>= 7
 
     async def write_varint(self, value: int, /) -> None:
         """Write a 32-bit signed integer in a variable length format.
 
-        For more information about variable length format check `_write_varuint` docstring.
+        For more information about variable length format check :meth:`._write_varuint`.
         """
         val = to_twos_complement(value, bits=32)
         await self._write_varuint(val, max_bits=32)
 
     async def write_varlong(self, value: int, /) -> None:
         """Write a 64-bit signed integer in a variable length format.
 
-        For more information about variable length format check `_write_varuint` docstring.
+        For more information about variable length format check :meth:`._write_varuint`.
         """
         val = to_twos_complement(value, bits=64)
         await self._write_varuint(val, max_bits=64)
 
     async def write_bytearray(self, data: bytes, /) -> None:
         """Write an arbitrary sequence of bytes, prefixed with a varint of it's size."""
         await self.write_varint(len(data))
@@ -159,34 +163,32 @@
     async def write_utf(self, value: str, /) -> None:
         """Write a UTF-8 encoded string, prefixed with a varint of it's size (in bytes).
 
         The maximum amount of UTF-8 characters is limited to 32767.
 
         Individual UTF-8 characters can take up to 4 bytes, however most of the common ones take up less. Assuming the
         worst case of 4 bytes per every character, at most 131068 data bytes will be written + 3 additional bytes from
-        the varint encoding overhead. Note that the limit of 32767 characters holds, even if we're writing shorter
-        characters, and we wouldn't cross the 131068 bytes data limit.
+        the varint encoding overhead.
 
-        If the given string is longer than this, ValueError will be raised.
+        :raises ValueError:
+            If the given string ``value`` has more characters than the allowed maximum (32767).
         """
         if len(value) > 32767:
             raise ValueError("Maximum character limit for writing strings is 32767 characters.")
 
         data = bytearray(value, "utf-8")
         await self.write_varint(len(data))
         await self.write(data)
 
     async def write_optional(self, value: Optional[T], /, writer: Callable[[T], Awaitable[R]]) -> Optional[R]:
-        """Writes bool determining is value is present, if it is, also writes the value with writer function.
-
-        When the `value` is None, a bool of False will be written and function will end. Otherwise, if `value` isn't
-        None, True will be written, followed by calling the `writer` function wchich will be passed the `value` as the
-        only argument. This function is expected to properly write the value into this buffer/connection.
+        """Writes a bool showing if a ``value`` is present, if so, also writes this value with ``writer`` function.
 
-        Will return None if the `value` was None, or the value returned by the `writer` function.
+        * When ``value`` is ``None``, a bool of ``False`` will be written, and ``None`` is returned.
+        * When ``value`` is not ``None``, a bool of ``True`` is written, after which the ``writer`` function is called,
+          and the return value is forwarded.
         """
         if value is None:
             await self.write_value(StructFormat.BOOL, False)
             return None
 
         await self.write_value(StructFormat.BOOL, True)
         return await writer(value)
@@ -214,25 +216,25 @@
         ...
 
     @overload
     def write_value(self, fmt: Literal[StructFormat.CHAR], value: str, /) -> None:
         ...
 
     def write_value(self, fmt: StructFormat, value: object, /) -> None:
-        """Write a value of given struct format in big-endian mode."""
+        """Write a given ``value`` as given struct format (``fmt``) in big-endian mode."""
         self.write(struct.pack(">" + fmt.value, value))
 
     def _write_varuint(self, value: int, /, *, max_bits: Optional[int] = None) -> None:
         """Write an arbitrarily big unsigned integer in a variable length format.
 
         This is a standard way of transmitting ints, and it allows smaller numbers to take less bytes.
 
-        Writing will be limited up to integer values of `max_bits` bits, and trying to write bigger values will rase a
-        ValueError. Note that setting `max_bits` to for example 32 bits doesn't mean that at most 4 bytes will be sent,
-        in this case it would actually take at most 5 bytes, due to the variable encoding overhead.
+        Writing will be limited up to integer values of ``max_bits`` bits, and trying to write bigger values will rase
+        a :exc:`ValueError`. Note that setting ``max_bits`` to for example 32 bits doesn't mean that at most 4 bytes
+        will be sent, in this case it would actually take at most 5 bytes, due to the variable encoding overhead.
 
         Varints send bytes where 7 least significant bits are value bits, and the most significant bit is continuation
         flag bit. If this continuation bit is set (1), it indicates that there will be another varint byte sent after
         this one. The least significant group is written first, followed by each of the more significant groups, making
         varints little-endian, however in groups of 7 bits, not 8.
         """
         value_max = (1 << (max_bits)) - 1 if max_bits is not None else float("inf")
@@ -248,23 +250,23 @@
             self.write_value(StructFormat.UBYTE, remaining & 0x7F | 0x80)
             # Subtract the value we've already sent (7 least significant bits)
             remaining >>= 7
 
     def write_varint(self, value: int, /) -> None:
         """Write a 32-bit signed integer in a variable length format.
 
-        For more information about variable length format check `_write_varuint` docstring.
+        For more information about variable length format check :meth:`._write_varuint`.
         """
         val = to_twos_complement(value, bits=32)
         self._write_varuint(val, max_bits=32)
 
     def write_varlong(self, value: int, /) -> None:
         """Write a 64-bit signed integer in a variable length format.
 
-        For more information about variable length format check `_write_varuint` docstring.
+        For more information about variable length format check :meth:`._write_varuint` docstring.
         """
         val = to_twos_complement(value, bits=64)
         self._write_varuint(val, max_bits=64)
 
     def write_bytearray(self, data: bytes, /) -> None:
         """Write an arbitrary sequence of bytes, prefixed with a varint of it's size."""
         self.write_varint(len(data))
@@ -279,34 +281,32 @@
     def write_utf(self, value: str, /) -> None:
         """Write a UTF-8 encoded string, prefixed with a varint of it's size (in bytes).
 
         The maximum amount of UTF-8 characters is limited to 32767.
 
         Individual UTF-8 characters can take up to 4 bytes, however most of the common ones take up less. Assuming the
         worst case of 4 bytes per every character, at most 131068 data bytes will be written + 3 additional bytes from
-        the varint encoding overhead. Note that the limit of 32767 characters holds, even if we're writing shorter
-        characters, and we wouldn't cross the 131068 bytes data limit.
+        the varint encoding overhead.
 
-        If the given string is longer than this, ValueError will be raised.
+        :raises ValueError:
+            If the given string ``value`` has more characters than the allowed maximum (32767).
         """
         if len(value) > 32767:
             raise ValueError("Maximum character limit for writing strings is 32767 characters.")
 
         data = bytearray(value, "utf-8")
         self.write_varint(len(data))
         self.write(data)
 
     def write_optional(self, value: Optional[T], /, writer: Callable[[T], R]) -> Optional[R]:
-        """Writes bool determining is value is present, if it is, also writes the value with writer function.
-
-        When the `value` is None, a bool of False will be written and function will end. Otherwise, if `value` isn't
-        None, True will be written, followed by calling the `writer` function wchich will be passed the `value` as the
-        only argument. This function is expected to properly write the value into this buffer/connection.
+        """Writes a bool showing if a ``value`` is present, if so, also writes this value with ``writer`` function.
 
-        Will return None if the `value` was None, or the value returned by the `writer` function.
+        * When ``value`` is ``None``, a bool of ``False`` will be written, and ``None`` is returned.
+        * When ``value`` is not ``None``, a bool of ``True`` is written, after which the ``writer`` function is called,
+          and the return value is forwarded.
         """
         if value is None:
             self.write_value(StructFormat.BOOL, False)
             return None
 
         self.write_value(StructFormat.BOOL, True)
         return writer(value)
@@ -338,31 +338,31 @@
         ...
 
     @overload
     async def read_value(self, fmt: Literal[StructFormat.CHAR], /) -> str:
         ...
 
     async def read_value(self, fmt: StructFormat, /) -> object:
-        """Read a value into given struct format in big-endian mode.
+        """Read a value as given struct format (``fmt``) in big-endian mode.
 
         The amount of bytes to read will be determined based on the struct format automatically.
         """
         length = struct.calcsize(fmt.value)
         data = await self.read(length)
         unpacked = struct.unpack(">" + fmt.value, data)
         return unpacked[0]
 
     async def _read_varuint(self, *, max_bits: Optional[int] = None) -> int:
         """Read an arbitrarily big unsigned integer in a variable length format.
 
         This is a standard way of transmitting ints, and it allows smaller numbers to take less bytes.
 
-        Reading will be limited up to integer values of `max_bits` bits, and trying to read bigger values will rase an
-        IOError. Note that setting `max_bits` to for example 32 bits doesn't mean that at most 4 bytes will be read,
-        in this case it would actually read at most 5 bytes, due to the variable encoding overhead.
+        Reading will be limited up to integer values of ``max_bits`` bits, and trying to read bigger values will rase
+        an :exc:`IOError`. Note that setting ``max_bits`` to for example 32 bits doesn't mean that at most 4 bytes
+        will be read, in this case we would actually read at most 5 bytes, due to the variable encoding overhead.
 
         Varints send bytes where 7 least significant bits are value bits, and the most significant bit is continuation
         flag bit. If this continuation bit is set (1), it indicates that there will be another varint byte sent after
         this one. The least significant group is written first, followed by each of the more significant groups, making
         varints little-endian, however in groups of 7 bits, not 8.
         """
         value_max = (1 << (max_bits)) - 1 if max_bits is not None else float("inf")
@@ -384,24 +384,24 @@
                 break
 
         return result
 
     async def read_varint(self) -> int:
         """Read a 32-bit signed integer in a variable length format.
 
-        For more information about variable length format check `_read_varuint` docstring.
+        For more information about variable length format check :meth:`._read_varuint`.
         """
         unsigned_num = await self._read_varuint(max_bits=32)
         val = from_twos_complement(unsigned_num, bits=32)
         return val
 
     async def read_varlong(self) -> int:
         """Read a 64-bit signed integer in a variable length format.
 
-        For more information about variable length format check `_read_varuint` docstring.
+        For more information about variable length format check :meth:`._read_varuint`.
         """
         unsigned_num = await self._read_varuint(max_bits=64)
         val = from_twos_complement(unsigned_num, bits=64)
         return val
 
     async def read_bytearray(self, /) -> bytearray:
         """Read an arbitrary sequence of bytes, prefixed with a varint of it's size."""
@@ -420,38 +420,41 @@
     async def read_utf(self) -> str:
         """Read a UTF-8 encoded string, prefixed with a varint of it's size (in bytes).
 
         The maximum amount of UTF-8 characters is limited to 32767.
 
         Individual UTF-8 characters can take up to 4 bytes, however most of the common ones take up less. Assuming the
         worst case of 4 bytes per every character, at most 131068 data bytes will be read + 3 additional bytes from
-        the varint encoding overhead. Note that the while the limit of 32767 characters is enforced, this check only
-        happens after the data was already read.
+        the varint encoding overhead.
 
-        If the given string is longer than this, IOError will be raised.
+        :raises IOError:
+            * If the prefix varint is bigger than the maximum (131068) bytes, the string will not be read at all,
+              and :exc:`IOError` will be raised immediately.
+            * If the received string has more than the maximum amount of characters (32767). Note that in this case,
+              the string will still get read in it's entirety, since it fits into the maximum bytes limit (131068),
+              which was simply read at once. This limitation is here only to replicate the behavior of minecraft's
+              implementation.
         """
         length = await self.read_varint()
         if length > 131068:
             raise IOError(f"Maximum read limit for utf strings is 131068 bytes, got {length}.")
 
         data = await self.read(length)
         chars = data.decode("utf-8")
 
         if len(chars) > 32767:
             raise IOError(f"Maximum read limit for utf strings is 32767 characters, got {len(chars)}.")
 
         return chars
 
     async def read_optional(self, reader: Callable[[], Awaitable[R]]) -> Optional[R]:
-        """Reads bool determining is value is present, if it is, also reads the value with reader function.
-
-        When False is read, the function will not read anything and end. Otherwise, if True is read, the `reader`
-        function will be called, which is expected to properly read the value from this buffer/connection.
+        """Reads a bool showing if a value is present, if so, also reads this value with ``reader`` function.
 
-        Will return None if the False was encountered, or the value returned by the `reader` function.
+        * When ``False`` is read, the function will not read anything and ``None`` is returned.
+        * When ``True`` is read, the ``reader`` function is called, and it's return value is forwarded.
         """
         if not await self.read_value(StructFormat.BOOL):
             return None
 
         return await reader()
 
 
@@ -491,17 +494,17 @@
         return unpacked[0]
 
     def _read_varuint(self, *, max_bits: Optional[int] = None) -> int:
         """Read an arbitrarily big unsigned integer in a variable length format.
 
         This is a standard way of transmitting ints, and it allows smaller numbers to take less bytes.
 
-        Reading will be limited up to integer values of `max_bits` bits, and trying to read bigger values will rase an
-        IOError. Note that setting `max_bits` to for example 32 bits doesn't mean that at most 4 bytes will be read,
-        in this case it would actually read at most 5 bytes, due to the variable encoding overhead.
+        Reading will be limited up to integer values of ``max_bits`` bits, and trying to read bigger values will rase
+        an :exc:`IOError`. Note that setting ``max_bits`` to for example 32 bits doesn't mean that at most 4 bytes
+        will be read, in this case we would actually read at most 5 bytes, due to the variable encoding overhead.
 
         Varints send bytes where 7 least significant bits are value bits, and the most significant bit is continuation
         flag bit. If this continuation bit is set (1), it indicates that there will be another varint byte sent after
         this one. The least significant group is written first, followed by each of the more significant groups, making
         varints little-endian, however in groups of 7 bits, not 8.
         """
         value_max = (1 << (max_bits)) - 1 if max_bits is not None else float("inf")
@@ -523,24 +526,24 @@
                 break
 
         return result
 
     def read_varint(self) -> int:
         """Read a 32-bit signed integer in a variable length format.
 
-        For more information about variable length format check `_read_varuint` docstring.
+        For more information about variable length format check :meth:`._read_varuint`.
         """
         unsigned_num = self._read_varuint(max_bits=32)
         val = from_twos_complement(unsigned_num, bits=32)
         return val
 
     def read_varlong(self) -> int:
         """Read a 64-bit signed integer in a variable length format.
 
-        For more information about variable length format check `_read_varuint` docstring.
+        For more information about variable length format check :meth:`._read_varuint`.
         """
         unsigned_num = self._read_varuint(max_bits=64)
         val = from_twos_complement(unsigned_num, bits=64)
         return val
 
     def read_bytearray(self) -> bytearray:
         """Read an arbitrary sequence of bytes, prefixed with a varint of it's size."""
@@ -559,38 +562,41 @@
     def read_utf(self) -> str:
         """Read a UTF-8 encoded string, prefixed with a varint of it's size (in bytes).
 
         The maximum amount of UTF-8 characters is limited to 32767.
 
         Individual UTF-8 characters can take up to 4 bytes, however most of the common ones take up less. Assuming the
         worst case of 4 bytes per every character, at most 131068 data bytes will be read + 3 additional bytes from
-        the varint encoding overhead. Note that the while the limit of 32767 characters is enforced, this check only
-        happens after the data was already read.
+        the varint encoding overhead.
 
-        If the given string is longer than this, IOError will be raised.
+        :raises IOError:
+            * If the prefix varint is bigger than the maximum (131068) bytes, the string will not be read at all,
+              and :exc:`IOError` will be raised immediately.
+            * If the received string has more than the maximum amount of characters (32767). Note that in this case,
+              the string will still get read in it's entirety, since it fits into the maximum bytes limit (131068),
+              which was simply read at once. This limitation is here only to replicate the behavior of minecraft's
+              implementation.
         """
         length = self.read_varint()
         if length > 131068:
             raise IOError(f"Maximum read limit for utf strings is 131068 bytes, got {length}.")
 
         data = self.read(length)
         chars = data.decode("utf-8")
 
         if len(chars) > 32767:
             raise IOError(f"Maximum read limit for utf strings is 32767 characters, got {len(chars)}.")
 
         return chars
 
     def read_optional(self, reader: Callable[[], R]) -> Optional[R]:
-        """Reads bool determining is value is present, if it is, also reads the value with reader function.
-
-        When False is read, the function will not read anything and end. Otherwise, if True is read, the `reader`
-        function will be called, which is expected to properly read the value from this buffer/connection.
+        """Reads a bool showing if a value is present, if so, also reads this value with ``reader`` function.
 
-        Will return None if the False was encountered, or the value returned by the `reader` function.
+        * When ``False`` is read, the function will not read anything and ``None`` is returned.
+        * When ``True`` is read, the ``reader`` function is called, and it's return value is forwarded.
         """
         if not self.read_value(StructFormat.BOOL):
             return None
 
         return reader()
```

### Comparing `mcproto-0.2.0/mcproto/utils/abc.py` & `mcproto-0.3.0/mcproto/utils/abc.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,29 +10,30 @@
 
 __all__ = ["RequiredParamsABCMixin", "Serializable"]
 
 
 class RequiredParamsABCMixin:
     """Mixin class to ABCs that require certain attributes to be set in order to allow initialization.
 
-    This class performs a similar check to what ABCs already do for abstractmethods, but for class
-    variables. The required class variable names are set with _REQUIRED_CLASS_VARS class variable,
-    which itself is automatically required.
+    This class performs a similar check to what :class:`~abc.ABC` already des with abstractmethods,
+    but for class variables. The required class variable names are set with :attr:`._REQUIRED_CLASS_VARS`
+    class variable, which itself is automatically required.
 
     Just like with ABCs, this doesn't prevent creation of classes without these required class vars
-    missing, only initialization is prevented. This is done to allow creation of a more specific, but
+    defined, only initialization is prevented. This is done to allow creation of a more specific, but
     still abstract class.
 
-    Additionally, you can also define _REQUIRED_CLASS_VARS_NO_MRO class var, holding names of class vars
-    which should be defined on given class directly. That means inheritance will be ignored so even if a
-    subclass defines the required class var, unless the latest class also defines it, this check will fail.
-
-    This is often useful for classes that are expected to be slotted, as each subclass need to define
-    __slots__, otherwise a __dict__ will automatically be made for it. However this is entirely optional,
-    and if _REQUIRED_CLASS_VARS_NO_MRO isn't set, no such check will be performed.
+    Additionally, you can also define :attr:`._REQUIRED_CLASS_VARS_NO_MRO` class var, holding names of
+    class vars which should be defined on given class directly. That means inheritance will be ignored
+    so even if a subclass defines the required class var, unless the latest class also defines it, this
+    check will fail.
+
+    This is often useful for classes that are expected to be slotted, as each subclass will need to define
+    ``__slots__``, otherwise a ``__dict__`` will automatically be made for it. However this is entirely
+    optional, and if :attr:`._REQUIRED_CLASS_VARS_NO_MRO` isn't set, this check is skipped.
     """
 
     __slots__ = ()
 
     _REQUIRRED_CLASS_VARS: ClassVar[Sequence[str]]
     _REQUIRED_CLASS_VARS_NO_MRO: ClassVar[Sequence[str]]
 
@@ -59,21 +60,21 @@
                     emsg += f" ({req_no_mro_attr} found in a subclass, but not explicitly in {cls.__name__})"
                 raise TypeError(emsg)
 
         return super().__new__(cls)
 
 
 class Serializable(ABC):
-    """Base class for any type that should be (de)serializable into/from given buffer data."""
+    """Base class for any type that should be (de)serializable into/from :class:`~mcproto.Buffer` data."""
 
     __slots__ = ()
 
     @abstractmethod
     def serialize(self) -> Buffer:
-        """Represent the object as a transmittable sequence of bytes."""
+        """Represent the object as a :class:`~mcproto.Buffer` (transmittable sequence of bytes)."""
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
     def deserialize(cls, buf: Buffer, /) -> Self:
-        """Construct the object from it's received byte representation."""
+        """Construct the object from a :class:`~mcproto.Buffer` (transmitable sequence of bytes)."""
         raise NotImplementedError
```

### Comparing `mcproto-0.2.0/mcproto/utils/version_map.py` & `mcproto-0.3.0/mcproto/utils/version_map.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,141 +23,186 @@
     info: pkgutil.ModuleInfo
     member_names: Sequence[str]
 
 
 class VersionMap(ABC, RequiredParamsABCMixin, Generic[K, V]):
     """Base class for map classes that allow obtaining versioned implementations for same components.
 
-    Some components (classes) need to be versioned as they might change between different protocol
-    versions. VersionMap classes are responsible for finding the implementation for given component
-    that matches the requested version for.
+    Some components (classes, functions, constants, ...) need to be versioned as they might change
+    between different protocol versions. :class:`.VersionMap` classes are responsible for finding the
+    implementation for given component that matches the requested version for.
 
     If the exact requested version is not found, the closest older/lesser version will be used instead,
     however as this might cause issues, a user warning will be produced alongside this happening.
 
-    NOTE: If you need typed implementations, you are advised to instead import the versioned class
-    directly, as due to the dynamic nature of this map, and the changing nature of the versioned
-    implementations, no type information can be provided here.
-
-    WARNING: You are not expected to initialize these mapping classes! That should be left for the
-    library to handle and provide a map for each individual versioned components.
+    .. note:
+        If you need typed implementations, you should import the versioned components directly, as due
+        to the dynamic nature of this map, and the changing nature of the versioned implementations,
+        no type information can be provided here.
+
+    .. warning:
+        You are not expected to initialize these mapping classes yourself! That should be left for
+        the library to handle and provide a map for each individual versioned components.
     """
 
-    # TODO: Describe the obtain key, lazy loading and preload_all in init
-
     # TODO: Look into generating stubs somehow to preserve the type information even with how
     # dynamic this class is. (Could require making this class generic over a literal int, being
     # the version).
 
     _REQUIRED_CLASS_VARS: ClassVar[Sequence[str]] = [
         "SUPPORTED_VERSIONS",
         "_SEARCH_DIR_QUALNAME",
         "COMPATIBLE_FALLBACK_VERSIONS",
     ]
 
+    #: Set of all versions that have complete implementations, with package for the version
     SUPPORTED_VERSIONS: ClassVar[set[int]]
+    #: Set of all versions that are fully compatible with an older supported version that they safely fall back to
     COMPATIBLE_FALLBACK_VERSIONS: ClassVar[set[int]]
+    #: Fully qualified name of the package, containing individual versioned packages
     _SEARCH_DIR_QUALNAME: ClassVar[str]
 
     __slots__ = ("_version_map",)
 
     def __init__(self, preload_all: bool = False):
+        """
+        :param preload_all:
+            By default, the individual versioned components are loaded lazily, once requested.
+            However if this is set to ``True``, the components from all :attr:`.SUPPORTED_VERSIONS`
+            will all get loaded on initialization.
+        """
         self._version_map: dict[int, dict[K, V]] = {}
 
         if preload_all:
             for version in self.SUPPORTED_VERSIONS:
                 self.load_version(version)
 
     def load_version(self, protocol_version: int) -> None:
-        """Load all components for given protocol version."""
+        """Load all components for given protocol version.
+
+        Go through all versioned components found for the requested version (from all submodules in the
+        package for given version.) and store them into an internal version map. Each component is stored
+        under it's corresponding obtain key.
+
+        :raises ValueError:
+            Raised if a key collision occurs (obtain key of multiple distinct versioned components is the same).
+        """
         for key, member in self._walk_valid_components(protocol_version):
             dct = self._version_map.setdefault(protocol_version, {})
 
             if key in dct:
                 raise ValueError(f"Value {member} already registered (key collision: {key})")
 
             dct[key] = member
 
     def obtain(self, protocol_version: int, key: K) -> V:
-        """Obtain component for given protocol version, that matches the obtain key."""
+        """Obtain component for given protocol version, that matches the obtain key.
+
+        This function works lazily, and only loads the required components for given ``protocol_version``
+        if they're not already loaded. If loading does occr, the requested version is stored internally
+        and will simply be accessed next time this function is called with the same ``protocol_version``.
+
+        Once loaded, a versioned component that matches the given obtain ``key`` is returned.
+
+        .. note:
+            If given ``protocol_version`` isn't supported, a fallback version is picked
+            (see: :meth:`._get_supported_protocol_version`).
+        """
         protocol_version = self._get_supported_protocol_version(protocol_version)
 
         # Lazy loading: if this protocol version isn't in the version map, it wasn't yet loaded, do so now.
         if protocol_version not in self._version_map:
             self.load_version(protocol_version)
 
         return self._version_map[protocol_version][key]
 
     def make_version_map(self, protocol_version: int) -> dict[K, V]:
-        """Construct a dictionary mapping (obtain key -> value) for values of given protocol version."""
+        """Obtain a dictionary mapping of obtain key -> versioned component, with all components for given version.
+
+        This function works lazily, and only loads the required components for given ``protocol_version``
+        if they're not already loaded. If loading does occur, the requested version is stored internally and
+        will simply be accessed next time this function is called with the same ``protocol_version``.
+
+        The returned dictionary is a copy of the internal one, as we don't want the user to be able to modify it.
+
+        .. note:
+            If given ``protocol_version`` isn't supported, a fallback version is picked
+            (see: :meth:`._get_supported_protocol_version`).
+        """
         protocol_version = self._get_supported_protocol_version(protocol_version)
 
         # Lazy loading: if this protocol version isn't in the version map, it wasn't yet loaded, do so now.
         if protocol_version not in self._version_map:
             self.load_version(protocol_version)
 
         return self._version_map[protocol_version].copy()
 
     @abstractmethod
     def _check_obj(
-        self, obj: Any, module_data: WalkableModuleData, protocol_version: int  # noqa: ANN401
+        self,
+        obj: Any,  # noqa: ANN401
+        module_data: WalkableModuleData,
+        protocol_version: int,
     ) -> TypeGuard[V]:
         """Determine whether a member object should be considered as a valid component for given protocol version.
 
-        This method will be called for each potential member object (found when walking over all members of
-        __all__ from all submodules of the package for given protocol version).
-
-        This function shouldn't include any checks on whether an object is already registered in the version map
-        (key collisions), these are handled during the collection in load_version, all this function is responsible
-        for is checking whether this object is a valid component, components with conflicting keys are still
-        considered valid here, as they're handled elsewhere.
+        When versioned components are obtained, all of the members listed in any module's ``__all__`` are
+        considered. This function serves as a filter, identifying whether a potential member object should be
+        considered as one of the versioned components.
+
+        .. note:
+            This function shouldn't include any checks on whether an object is already registered in the version
+            map (key collisions), these are handled during the collection in :meth:`.load_version`, all this
+            function is responsible for is checking whether this object is a valid component, components with
+            conflicting keys are still considered valid here, as they're handled elsewhere.
 
-        Although if there is some additional data that needs to be unique for a component to be valid, which wouldn't
-        be caught as a key collision, this function can raise a ValueError.
+            However if there is some additional data that needs to be unique for a component to be valid, which
+            wouldn't be caught as a key collision, this function can raise a :exc:`ValueError`.
         """
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
     def _make_obtain_key(cls, obj: V, module_data: WalkableModuleData, protocol_version: int) -> K:
-        """Construct a unique obtain key for given object under given protocol version.
+        """Construct a unique obtain key for given versioned component (``obj``) under given ``protocol_version``.
 
-
-        Note: While the protocol version might be beneficial to know when constructing
-        the obtain key, it shouldn't be used directly as a part of the key, as the items
-        will already be split by their protocol versions, and this version will be known
-        at obtaining time.
+        .. note:
+            While the protocol version might be beneficial to know when constructing
+            the obtain key, it shouldn't be used directly as a part of the key, as the items
+            will already be split by their protocol versions, and this version will be known
+            at obtaining time.
         """
         raise NotImplementedError
 
     @classmethod
     def _get_package_module(cls, protocol_version: int) -> ModuleType:
         """Obtain the package module containing all components specific to given protocol version.
 
-        This relies on the _SEARCH_DIR_QUALNAME and naming scheme of v{protocol_version} for the modules.
+        This relies on the :attr:`._SEARCH_DIR_QUALNAME` class variable, and naming scheme of
+        v{protocol_version} for the modules contained in this directory.
         """
         module_name = f"{cls._SEARCH_DIR_QUALNAME}.v{protocol_version}"
         try:
             module = importlib.import_module(module_name)
         except ModuleNotFoundError as exc:
             raise ValueError(
                 f"Protocol version ({protocol_version}) isn't supported, yet it was listed as supported. Report this!"
             ) from exc
 
         return module
 
     @classmethod
     def _walk_submodules(cls, module: ModuleType) -> Iterator[WalkableModuleData]:
-        """Go over all submodules of given module, that properly specify __all__.
+        """Go over all submodules of given module, that specify ``__all__``.
 
         The yielded modules are expected to contain the versioned component items.
 
-        If a submodule that doesn't define __all__ is present, it will be skipped, as we don't
+        If a submodule that doesn't define ``__all__`` is present, it will be skipped, as we don't
         consider it walkable. (Walking over all variables defined in this module isn't viable,
-        since it would include imports etc. making defining __all__ a requirement.)
+        since it would include imports etc. making defining ``__all__`` a requirement.)
         """
 
         def on_error(name: str) -> NoReturn:
             raise ImportError(name=name)
 
         for module_info in pkgutil.walk_packages(module.__path__, f"{module.__name__}.", onerror=on_error):
             imported_module = importlib.import_module(module_info.name)
@@ -173,46 +218,65 @@
                 if not isinstance(member_name, str):
                     raise TypeError(f"Module {module_info.name!r}'s __all__ contains non-string item.")
 
             yield WalkableModuleData(imported_module, module_info, member_names)
 
     @classmethod
     def _walk_members(cls, module_data: WalkableModuleData) -> Iterator[object]:
-        """Go over all members specified in __all__ of given walkable (sub)module.
+        """Go over all members specified in ``__all__`` of given walkable (sub)module.
 
-        Yields all
+        :return:
+            Iterator yielding every object defined in ``__all__`` of given module. These objects
+            are obtained directly using ``getattr`` from the imported module.
+
+        :raises TypeError:
+            Raised when an attribute defined in ``__all__`` can't be obtained using ``getattr``.
+            This would suggest the module has incorrectly defined ``__all__``, as it includes values
+            that aren't actually defined in the module.
         """
         for member_name in module_data.member_names:
             try:
                 member = getattr(module_data.module, member_name)
             except AttributeError as exc:
                 module_name = module_data.info.name
                 raise TypeError(f"Member {member_name!r} of {module_name!r} module isn't defined.") from exc
 
             yield member
 
     def _walk_valid_components(self, protocol_version: int) -> Iterator[tuple[K, V]]:
-        """Go over all components/members belonging to given protocol version."""
+        """Go over all components/members belonging to given protocol version.
+
+        This method walks over all submodules in the versioned module (see: :meth:`._get_package_module`),
+        in which we go over all members present in ``__all__`` of this submodule (see :meth:`._walk_submodules`),
+        after which a :meth:`_check_obj` check is performed, ensuring the obtained member/component is one that
+        should be versioned.
+
+        :return:
+            A tuple containing the obtain key (see: :meth:`._make_obtain_key`), and the versioned component/member.
+        """
         version_module = self._get_package_module(protocol_version)
         for module_data in self._walk_submodules(version_module):
             for member in self._walk_members(module_data):
                 if self._check_obj(member, module_data, protocol_version):
                     key = self._make_obtain_key(member, module_data, protocol_version)
                     yield key, member
 
     def _get_supported_protocol_version(self, protocol_version: int) -> int:
-        """Given a protocol version, return closest older supported version, or the version itself.
+        """Given a ``protocol_version``, return closest older supported version, or the version itself.
 
-        - If given protocol version is one of supported versions, this function will simply return it.
-        - Otherwise, search for the closest older version to the requested version
-            - If there is no older version in the supported version, ValueError is raised
-            - If the requested version is in COMPATIBLE_FALLBACK_VERSIONS, this fallback will be
+        * If given ``protocol_version`` is one of :attr:`.SUPPORTED_VERSIONS`, return it.
+        * Otherwise, search for the closest older supported version to the provided ``protocol_version``.
+            * If there is no older version in the supported version, :exc:`ValueError` is raised
+            * If the requested version is in :attr:`.COMPATIBLE_FALLBACK_VERSIONS`, this fallback will be
               considered safe, and no errors/warnings will be produced.
-            - Otherwise, the closest version will still be returned, but a UserWarning will be emitted
+            * Otherwise, the closest version will still be returned, but a :exc:`UserWarning` will be emitted
               mentioning that this fallback occurred and that the version might not be fully compatible.
+
+        :raises ValueError:
+            The requested version isn't supported, and there is no supported older version to fallback to.
         """
 
         if protocol_version in self.SUPPORTED_VERSIONS:
             return protocol_version
 
         # Pick the most recent, but older version to the one that was requested
         older_versions = filter(lambda version: version < protocol_version, self.SUPPORTED_VERSIONS)
@@ -227,10 +291,11 @@
         # Since using an older/lesser version to the one that was requested is a fallback behavior and
         # could easily cause issues, emit a warning here, unless the version was explicitly marked compatible.
         if protocol_version not in self.COMPATIBLE_FALLBACK_VERSIONS:
             warnings.warn(
                 f"Falling back to older protocol version {protocol_version_closest}, "
                 f"as the requested version ({protocol_version}) isn't supported.",
                 category=UserWarning,
+                stacklevel=3,
             )
 
         return protocol_version_closest
```

### Comparing `mcproto-0.2.0/pyproject.toml` & `mcproto-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "mcproto"
-version = "0.2.0" # Versioning handled by poetry-dynamic-versioning
-description = "Library providing easy interactions with minecraft sevrers"
+version = "0.3.0" # Versioning handled by poetry-dynamic-versioning
+description = "Library providing easy interactions with minecraft servers"
 authors = ["ItsDrike <itsdrike@protonmail.com>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/py-mine/mcproto"
+documentation = "https://mcproto.readthedocs.io/"
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
   "Natural Language :: English",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
@@ -20,78 +21,99 @@
   "Programming Language :: Python :: 3.11",
   "Topic :: Games/Entertainment",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: System :: Networking",
   "Typing :: Typed",
 ]
+include = ["CHANGELOG.md"]
 packages = [{ include = "mcproto" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
 asyncio-dgram = "^2.1.2"
 typing-extensions = "^4.4.0"
+semantic-version = "^2.10.0"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^2.18.1"
-taskipy = "^1.10.2"
+pre-commit = ">=2.18.1,<4.0.0"
+taskipy = "^1.10.4"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.1.2"
-pytest-asyncio = "^0.18.3"
-pytest-cov = "^3.0.0"
+pytest = "^7.3.1"
+pytest-asyncio = "^0.21.0"
+pytest-cov = ">=3,<5"
 
 [tool.poetry.group.lint.dependencies]
 flake8 = "^6.0.0"
-flake8-annotations = "^2.9.0"
+flake8-annotations = ">=2.9,<4.0"
 flake8-bandit = "^4.1.1"
-flake8-bugbear = "^22.3.23"
+flake8-bugbear = "^23.6.5"
 flake8-builtins = "^2.1.0"
-flake8-comprehensions = "^3.10.1"
-flake8-dunder-all = {git = "https://github.com/python-formate/flake8-dunder-all.git"}
-flake8-functions = "^0.0.7"
-flake8-future-annotations = "^0.0.5"
-flake8-noqa = "^1.3.0"
+flake8-comprehensions = "^3.12.0"
+flake8-dunder-all = "^0.3.0"
+flake8-functions = "^0.0.8"
+flake8-future-annotations = ">=0.0.5,<1.1.1"
+flake8-noqa = "^1.3.1"
 flake8-pep3101 = "^2.0.0"
 flake8-pep585 = { version = "^0.1.5", python = ">=3.9" }
 flake8-print = "^5.0.0"
 flake8-printf-formatting = "^1.1.2"
 flake8-pytest-style = "^1.6.0"
 flake8-raise = "^0.0.5"
-flake8-simplify = "^0.19.2"
+flake8-simplify = "^0.20.0"
 flake8-tidy-imports = "^4.6.0"
-pep8-naming = "^0.12.1"
-black = "^22.3.0"
+pep8-naming = "^0.13.3"
+black = ">=22.3,<24.0"
 isort = "^5.10.1"
-pyright = "^1.1.239"
-codespell = {extras = ["tomli"], version = "^2.2.2"}
+pyright = "^1.1.313"
 slotscheck = "^0.16.1"
 
 [tool.poetry.group.release.dependencies]
 towncrier = "^22.12.0"
 
 [tool.poetry.group.release-ci]
 optional = true
 
 [tool.poetry.group.release-ci.dependencies]
-poetry-dynamic-versioning = "^0.21.3"
+poetry-dynamic-versioning = "^0.22.0"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^6.2.1"
+tomli = { version = "^2.0.1", python = "<3.11" }
+m2r2 = "^0.3.3.post2"
+packaging = "^23.1"
+sphinx-autodoc-typehints = "^1.23"
+sphinx-copybutton = "^0.5.2"
+furo = ">=2022.12.7"
+sphinxcontrib-towncrier = "^0.3.2a0"
+
+[tool.poetry.group.docs-ci]
+optional = true
+
+[tool.poetry.group.docs-ci.dependencies]
+poetry-dynamic-versioning = "^0.22.0"
+taskipy = "^1.10.4"
 
 [tool.black]
 line-length = 119
 
 [tool.isort]
 profile = "black"
 line_length = 119
 atomic = true
 order_by_type = false
 case_sensitive = true
 combine_as_imports = true
 
 [tool.codespell]
-skip = "./.venv/*,./htmlcov/*,./.git,./.mypy_cache/*,./.pytest_cache/*"
+skip = "./.venv/*,./htmlcov/*,./.git,./.mypy_cache/*,./.pytest_cache/*,./poetry.lock"
 ignore-words-list = "ned"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 asyncio_mode = "auto"
 testpaths = ["tests"]
 addopts = "--strict-markers --cov --no-cov-on-fail"
@@ -100,58 +122,58 @@
 precision = 2
 fail_under = 20
 show_missing = true
 skip_covered = false
 skip_empty = false
 sort = "cover"
 exclude_lines = [
-    "\\#\\s*pragma: no cover\\s",
-    "^\\s*if (typing\\.)?TYPE_CHECKING:\\s",
-    "^\\s*@(abc\\.)?abstractmethod\\s",
-    "^\\s*@(typing\\.)?overload\\s",
+    "\\#\\s*pragma: no cover",
+    "^\\s*if (typing\\.)?TYPE_CHECKING:",
+    "^\\s*@(abc\\.)?abstractmethod",
+    "^\\s*@(typing\\.)?overload",
     "^\\s*def __repr__\\(",
-    "^\\s*class .*\\bProtocol\\):\\s",
-    "^\\s*raise NotImplementedError\\s",
-    "^\\s*return NotImplemented\\s",
-    "^\\s*\\.\\.\\.\\s",
+    "^\\s*class .*\\bProtocol\\):",
+    "^\\s*raise NotImplementedError",
+    "^\\s*return NotImplemented",
+    "^\\s*\\.\\.\\.",
 ]
 
 [tool.coverage.run]
 relative_files = true
 parallel = true
 branch = true
 timid = false
 source = ["mcproto"]
 
 [tool.towncrier]
 package = "mcproto"
-package_dir = "mcproto"
 directory = "changes"
 template = "changes/.template.rst"
 filename = "CHANGELOG.md"
 issue_format = "[#{issue}](https://github.com/py-mine/mcproto/issues/{issue})"
 orphan_prefix = "+"   # Use '+' instead of number for fragments not connected to any PR
 underlines = [2, 3]  # We use this for heading levels (see template file)
 type = [
     { name = "Breaking Changes",            directory = "breaking",      showcontent = true },
     { name = "Deprecation",                 directory = "deprecation",   showcontent = true },
     { name = "Features",                    directory = "feature",       showcontent = true },
     { name = "Bugfixes",                    directory = "bugfix",        showcontent = true },
-    { name = "Documentation Improvements",  directory = "documentation", showcontent = true },
+    { name = "Documentation Improvements",  directory = "docs",          showcontent = true },
     { name = "Internal Changes",            directory = "internal",      showcontent = true },
 ]
 
 [tool.slotscheck]
 strict-imports = true
 require-superclass = true
 require-subclass = true
 exclude-modules = '''
 (
   ^test  # ignore any tests
-  |^mcproto\.utils\.version # Dataclasses below python 3.10 don't support __slots__ due to default value fields being treated as classvars.
+  |^.github/scripts  # Ignore any CI scripts
+  |^mcproto\.utils\.version  # Dataclasses below python 3.10 don't support __slots__ due to default value fields being treated as classvars.
 )
 '''
 
 [tool.taskipy.tasks]
 precommit = "pre-commit install"
 lint = "pre-commit run --all-files"
 black = "black ."
@@ -161,14 +183,15 @@
 codespell = "codespell ."
 slotscheck = "slotscheck -m mcproto"
 test = "pytest -v --failed-first"
 retest = "pytest -v --last-failed"
 test-nocov = "pytest -v --no-cov --failed-first"
 retest-nocov = "pytest -v --no-cov --last-failed"
 changelog-preview = "towncrier build --draft --version next"
+docs = "sphinx-build -b dirhtml -d ./docs/_build/doctrees -W -E -T --keep-going ./docs ./docs/_build/html"
 
 [tool.poetry-dynamic-versioning]
 enable = true
 bump = true
 vcs = "git"
 style = "pep440"
```

### Comparing `mcproto-0.2.0/setup.py` & `mcproto-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,412 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mcproto
+Version: 0.3.0
+Summary: Library providing easy interactions with minecraft servers
+Home-page: https://github.com/py-mine/mcproto
+License: LGPL-3.0-or-later
+Author: ItsDrike
+Author-email: itsdrike@protonmail.com
+Requires-Python: >=3.8.1,<4
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Games/Entertainment
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Networking
+Classifier: Typing :: Typed
+Requires-Dist: asyncio-dgram (>=2.1.2,<3.0.0)
+Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
+Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
+Project-URL: Documentation, https://mcproto.readthedocs.io/
+Project-URL: Repository, https://github.com/py-mine/mcproto
+Description-Content-Type: text/markdown
 
-packages = \
-['mcproto',
- 'mcproto.packets',
- 'mcproto.packets.v757',
- 'mcproto.packets.v757.handshaking',
- 'mcproto.packets.v757.status',
- 'mcproto.protocol',
- 'mcproto.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['asyncio-dgram>=2.1.2,<3.0.0', 'typing-extensions>=4.4.0,<5.0.0']
-
-setup_kwargs = {
-    'name': 'mcproto',
-    'version': '0.2.0',
-    'description': 'Library providing easy interactions with minecraft sevrers',
-    'long_description': '# <img src="https://i.imgur.com/nPCcxts.png" height=25> McProto\n\n[![discord chat](https://img.shields.io/discord/936788458939224094.svg?logo=Discord)](https://discord.gg/C2wX7zduxC)\n![supported python versions](https://img.shields.io/pypi/pyversions/mcproto.svg)\n[![current PyPI version](https://img.shields.io/pypi/v/mcproto.svg)](https://pypi.org/project/mcproto/)\n[![Validation](https://github.com/ItsDrike/mcproto/actions/workflows/validation.yml/badge.svg)](https://github.com/ItsDrike/mcproto/actions/workflows/validation.yml)\n[![Unit tests](https://github.com/ItsDrike/mcproto/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/ItsDrike/mcproto/actions/workflows/unit-tests.yml)\n\nThis is a heavily Work-In-Progress library, which attempts to be a full wrapper around the minecraft protocol, allowing\nfor simple interactions with minecraft servers, and perhaps even for use as a base to a full minecraft server\nimplementation in python (though the speed will very likely be quite terrible, making it probably unusable as any\nreal-world playable server).\n\nCurrently, the library is very limited and doesn\'t yet have any documentation, so while contributions are welcome, fair\nwarning that there is a lot to comprehend in the code-base and it may be challenging to understand it all.\n\n## Installation\n\nMcproto is available on [PyPI](https://pypi.org/project/mcproto/), and can be installed trivially with:\n\n```bash\npython3 -m pip install mcproto\n```\n\nThat said, as mcproto is still in development, the PyPI version will likely go out of date quite soon. This means that\nit may lack some already implemented features, or contain already fixed bugs. For that reason, you can also consider\ninstalling mcproto through git, to get the most recent version. But know that while this will mean you\'ll be getting\nall of the new features, this version is much more likely to contain bugs than the one on PyPI, so make your decision\nwisely. To install the latest version from git, you can use the command below:\n\n```bash\npython3 -m pip install \'mcproto @ git+https://github.com/py-mine/mcproto@main\'\n```\n\nAlternatively, if you want to poke around with mcproto\'s code, you can always include mcproto as a full [git\nsubmodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules) to your project, or just git clone it directly and play\naround with it from REPL.\n\n## Examples\n\nSince there is no documentation, to satisfy some curious minds that really want to use this library even in this\nheavily unfinished state, here\'s a few simple snippets of it in practice:\n\n### Manual communication with the server\n\nAs sending entire packets is still being worked on, the best solution to communicate with a server is to send the data\nmanually, using our connection reader/writer, and buffers (being readers/writers, but only from bytearrays as opposed\nto using an actual connection).\n\nFair warning: This example is pretty long, but that\'s because it aims to explain the minecraft protocol to people that\nsee it for the first time, and so a lot of explanation comments are included. But the code itself is actually quite\nsimple, due to a bunch of helpful read/write methods the library already provides.\n\n```python\nimport json\nimport asyncio\n\nfrom mcproto.buffer import Buffer\nfrom mcproto.connection import TCPAsyncConnection\nfrom mcproto.protocol.base_io import StructFormat\n\n\nasync def handshake(conn: TCPAsyncConnection, ip: str, port: int = 25565) -> None:\n    # As a simple example, let\'s request status info from a server.\n    # (this is what you see in the multiplayer server list, i.e. the server\'s motd, icon, info\n    # about how many players are connected, etc.)\n\n    # To do this, we first need to understand how are minecraft packets composed, and take a look\n    # at the specific packets that we\'re interested in. Thankfully, there\'s an amazing community\n    # made wiki that documents all of this! You can find it at https://wiki.vg/\n\n    # Alright then, let\'s take a look at the (uncompressed) packet format specification:\n    # https://wiki.vg/Protocol#Packet_format\n    # From the wiki, we can see that a packet is composed of 3 fields:\n    # - Packet length (in bytes), sent as a variable length integer\n    #       combined length of the 2 fields below\n    # - Packet ID, also sent as varint\n    #       each packet has a unique number, that we use to find out which packet it is\n    # - Data, specific to the individual packet\n    #       every packet can hold different kind of data, this will be shown in the packet\'s\n    #       specification (you can find these in wiki.vg)\n\n    # Ok then, with this knowledge, let\'s establish a connection with our server, and request\n    # status. To do this, we fist need to send a handshake packet. Let\'s do it:\n\n    # Let\'s take a look at what data the Handshake packet should contain:\n    # https://wiki.vg/Protocol#Handshake\n    handshake = Buffer()\n    # We use 47 for the protocol version, as it\'s quite old, and will work with almost any server\n    handshake.write_varint(47)\n    handshake.write_utf(ip)\n    handshake.write_value(StructFormat.USHORT, port)\n    handshake.write_varint(1)  # Intention to query status\n\n    # Nice! Now that we have the packet data, let\'s follow the packet format and send it.\n    # Let\'s prepare another buffer that will contain the last 2 fields (packet id and data)\n    # combined. We do this since the first field will require us to know the size of these\n    # two combined, so let\'s just put them into 1 buffer.\n    packet = Buffer()\n    packet.write_varint(0)  # Handshake packet has packet ID of 0\n    packet.write(handshake)  # Full data from our handshake packet\n\n    # And now, it\'s time to send it!\n    await conn.write_varint(len(packet))  # First field (size of packet id + data)\n    await conn.write(packet)  # Second + Third fields (packet id + data)\n\n\nasync def status(conn: TCPAsyncConnection, ip: str, port: int = 25565) -> dict:\n    # This function will be called right after a handshake\n    # Sending this packet told the server recognize our connection, and since we\'ve specified\n    # the intention to query status, it then moved us to STATUS game state.\n\n    # Different game states have different packets that we can send out, for example there is a\n    # game state for login, that we\'re put into while joining the server, and from it, we tell\n    # the server our username player UUID, etc.\n\n    # The packet IDs are unique to each game state, so since we\'re now in status state, a packet\n    # with ID of 0 is no longer the handshake packet, but rather the status request packet\n    # (precisely what we need).\n    # https://wiki.vg/Protocol#Status_Request\n\n    # The status request packet is empty, and doesn\'t contain any data, it just instructs the\n    # server to send us back a status response packet. Let\'s send it!\n    packet = Buffer()\n    packet.write_varint(0)  # Status request packet ID\n\n    await conn.write_varint(len(packet))\n    await conn.write(packet)\n\n    # Now, let\'s receive the response packet from the server\n    # Remember, the packet format states that we first receive a length, then packet id, then data\n    _response_len = await conn.read_varint()\n    _response = await conn.read(_response_len)  # will give us a bytearray\n\n    # Amazing, we\'ve just received data from the server! But it\'s just bytes, let\'s turn it into\n    # a Buffer object, which includes helpful methods that allow us to read from it\n    response = Buffer(_response)\n    packet_id = response.read_varint()  # Remember, 2nd field is the packet ID\n\n    # Let\'s see it then, what packet did we get?\n    print(packet_id)  # 0\n\n    # Interesting, this packet has an ID of 0, but wasn\'t that the status request packet? We wanted\n    # a response tho. Well, actually, if we take a look at the status response packet at the wiki,\n    # it really has an ID of 0:\n    # https://wiki.vg/Protocol#Status_Response\n    # Aha, so not only are packet ids unique between game states, they\'re also unique between the\n    # direction a server bound packet (sent by client, with server as the destination) can have an\n    # id of 0, while a client bound packet (sent by server, with client as the destination) can\n    # have the same id, and mean something else.\n\n    # Alright then, so we know what we got is a status response packet, let\'s read the wiki a bit\n    # further and see what data it actually contains, and see how we can get it out. Hmmm, it\n    # contains a UTF-8 encoded string that represents JSON data, ok, so let\'s get that string, it\'s\n    # still in our buffer.\n    received_string = response.read_utf()\n\n    # Now, let\'s just use the json module, convert the string into some json object (in this case,\n    # a dict)\n    data = json.loads(received_string)\n    return data\n\nasync def main():\n    # That\'s it, all that\'s left is actually calling our functions now\n\n    ip = "mc.hypixel.net"\n    port = 25565\n\n    async with (await TCPAsyncConnection.make_client((ip, port), 2)) as connection:\n        await handshake(connection, ip, port)\n        data = await status(connection, ip, port)\n\n    # Wohoo, we got the status data! Let\'s see it\n    print(data["players"]["max"])  # This is the server\'s max player amount (slots)\n    print(data["players"]["online"])  # This is how many people are currently online\n    print(data["description"])  # And here\'s the motd\n\n    # There\'s a bunch of other things in this data, try it out, see what you can find!\n\ndef start():\n    # Just some boilerplate code that can run our asynchronous main function\n    asyncio.run(main())\n```\n\n### Using packet classes for communication\n\n#### Obtaining the packet map\n\nThe first thing you\'ll need to understand about packet classes in mcproto is that they\'re versioned depending on the\nprotocol version you\'re using. As we\'ve already seen with minecraft packets, they\'re following a certain format, and\nfor given packet direction and game state, the packet numbers are unique.\n\nThis is how we can detect what packet is being received, but because of the different versions that the library can\nsupport, we will need to use a packet map, that will contain all of the mappings for given protocol version, from\nwhich, knowing the state and direction, we can get a dictionary with packet IDs as keys, and the individual packet\nclasses as values.\n\nThis dictionary is crucial to receiving packets, as it\'s the only thing that tells us which packet class should be\nused, once we receive a packet and learn about the packet id. Otherwise we wouldn\'t know what to do with the data we\nobtained.\n\nThe first game state we\'ll be in, before doing anything will always be the handshaking state, so let\'s see how we could\ngenerate this dictionary for this state, for all of the receiving (client bound) packets.\n\n```python\nfrom mcproto.packets import PACKET_MAP\nfrom mcproto.packets.abc import PacketDirection, GameState\n\nhandshaking_packet_map = PACKET_MAP.make_id_map(\n    protocol_version=757,\n    direction=PacketDirection.CLIENTBOUND,\n    game_state=GameState.HANDSHAKING\n)\n\nprint(handshaking_packet_map)  # {}\n```\n\nNotice that the packet map is actually empty, and this is simply because there (currently) aren\'t any client bound\npackets a server can send out for the handshaking game state. Let\'s see the status gamestate instead:\n\n```python\nstatus_packet_map = PACKET_MAP.make_id_map(\n    protocol_version=757,\n    direction=PacketDirection.CLIENTBOUND,\n    game_state=GameState.STATUS,\n)\n\nprint(status_packet_map)  # Will print:\n# {1: mcproto.packets.v757.status.ping.PingPong, 0: mcproto.packets.v757.status.status.StatusResponse}\n```\n\nCool! These are all of the packets, with their IDs that the server can send in STATUS game state.\n\n#### Creating our own packets\n\n\nNow, we could create a similar packet map for sending out the packets, and just use it to construct our packets,\nhowever this is not the recommended approach, as it\'s kind of hard to remember all of the packet IDs, and (at least\ncurrently) it means not having any typing information about what packet class will we get. For that reason, it\'s\nrecommended to import packets that we want to send out manually, like so:\n\n```python\nfrom mcproto.packets.v757.handshaking.handshake import Handshake, NextState\n\nmy_handshake = Handshake(\n    # Once again, we use an old protocol version so that even older servers will work\n    protocol_version=47,\n    server_address="mc.hypixel.net",\n    server_port=25565,\n    next_state=NextState.STATUS,\n)\n```\n\nThat\'s it! We\'ve now constructed a full handshake packet with all of the data it should contain. You might remember\nfrom the example above, that we originally had to look at the protocol specification, find the handshake packet and\nconstruct it\'s data as a Buffer with all of these variables.\n\nWith these packet classes, you can simply follow your editor\'s function hints to see what this packet requires, pass it\nin and the data will be constructed for you from these attributes, once we\'ll be to sending it.\n\nFor completion, let\'s also construct the status request packet that we were sending to instruct the server to send us\nback the status response packet.\n\n```python\nfrom mcproto.packets.v757.status.status import StatusRequest\n\nmy_status_request = StatusRequest()\n```\n\nThis one was even easier, as the status request packet alone doesn\'t contain any special data, it\'s just a request to\nthe server to send us some data back.\n\n#### Sending packets\n\nTo actually send out a packet to the server, we\'ll need to create a connection, and use the custom functions\nresponsible for sending packets out. Let\'s see it:\n\n```python\nfrom mcproto.packets import async_write_packet\nfrom mcproto.connection import TCPAsyncConnection\n\nasync def main():\n    ip = "mc.hypixel.net"\n    port = 25565\n\n    async with (await TCPAsyncConnection.make_client((ip, port), 2)) as connection:\n        await async_write_packet(connection, my_handshake)  \n        # my_handshake is a packet we\'ve created in the example before\n```\n\nHow quick was that? Now compare this to the manual version.\n\n#### Receiving packets\n\nAlright, we might now know how to send a packet, but how do we receive one? Let\'s see:\n\n```python\nfrom mcproto.packets import PACKET_MAP\n\n# Let\'s prepare the packet map we\'ll be using, say we\'re already in the STATUS game state now\nSTATUS_PACKET_MAP = PACKET_MAP.make_id_map(\n    protocol_version=757,\n    direction=PacketDirection.CLIENTBOUND,\n    game_state=GameState.STATUS\n)\n\n# Let\'s say we already have a connection at this moment, after all, how else would\n# we\'ve gotten into the STATUS game state.\n# Also, let\'s do something different, let\'s say we have a synchronous connection\nfrom mcproto.connection import TCPSyncConnection\nconn: TCPSyncConnection\n\n# With a synchronous connection, comes synchronous reader, so instead of using async_read_packet,\n# we\'ll use sync_read_packet here\nfrom mcproto.packets import sync_read_packet\n\npacket = sync_read_packet(conn, STATUS_PACKET_MAP)\n\n# Cool! We\'ve got back a packet, but what packet is it? Let\'s import the packet classes it could\n# be and check against them\nfrom mcproto.packets.v757.status.status import StatusResponse\nfrom mcproto.packets.v757.status.ping import PingPong\n\nif isinstance(packet, StatusResponse):\n    ...\nelif isinstance(packet, PingPong):\n    ...\nelse:\n    raise Exception("Impossible, there aren\'t other client bound packets in the STATUS game state")\n```\n\n#### Requesting status\n\nNow let\'s actually do something meaningful, and replicate the entire example from the manual version using packets,\nlet\'s see just how much simpler it will be:\n\n```python\nfrom mcproto.connection import TCPAsyncConnection\nfrom mcproto.packets import async_write_packet, async_read_packet, PACKET_MAP\nfrom mcproto.packets.abc import PacketDirection, GameState\nfrom mcproto.packets.v757.handshaking.handshake import Handshake, NextState\nfrom mcproto.packets.v757.status.status import StatusRequest, StatusResponse\n\nSTATUS_PACKET_MAP = PACKET_MAP.make_id_map(\n    protocol_version=757,\n    direction=PacketDirection.CLIENTBOUND,\n    game_state=GameState.STATUS\n)\n\n\nasync def get_status(ip: str, port: int) -> dict:\n    handshake_packet = Handshake(\n        protocol_version=47,\n        server_address=ip,\n        server_port=port,\n        next_state=NextState.STATUS,\n    )\n    status_req_packet = StatusRequest()\n\n    async with (await TCPAsyncConnection.make_client((ip, port), 2)) as connection:\n        # We start out at HANDSHAKING game state\n        await async_write_packet(connection, handshake_packet)  \n        # After sending the handshake, we told the server to now move us into the STATUS game state\n        await async_write_packet(connection, status_req_packet)  \n        # Since we\'re still in STATUS game state, we use the status packet map when reading\n        packet = await async_read_packet(connection, STATUS_PACKET_MAP)\n\n    # Now that we\'ve got back the packet, we no longer need the connection, we won\'t be sending\n    # anything else. Let\'s just make sure it really is the packet we expected\n    if not isinstance(packet, StatusResponse):\n        raise ValueError(f"We\'ve got an unexpected packet back: {packet!r}")\n\n    # Now that we know we\'re dealing with a status response, let\'s get out it\'s data, and return in\n    return packet.data\n```\n\nWell, that wasn\'t so hard, was it?\n',
-    'author': 'ItsDrike',
-    'author_email': 'itsdrike@protonmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/py-mine/mcproto',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8.1,<4',
-}
+# <img src="https://i.imgur.com/nPCcxts.png" style="height: 25px"> mcproto
 
+[![discord chat](https://img.shields.io/discord/936788458939224094.svg?logo=Discord)](https://discord.gg/C2wX7zduxC)
+![supported python versions](https://img.shields.io/pypi/pyversions/mcproto.svg)
+[![current PyPI version](https://img.shields.io/pypi/v/mcproto.svg)](https://pypi.org/project/mcproto/)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/9464f1037f07a795de35/test_coverage)](https://codeclimate.com/github/py-mine/mcproto/test_coverage)
+[![Validation](https://github.com/ItsDrike/mcproto/actions/workflows/validation.yml/badge.svg)](https://github.com/ItsDrike/mcproto/actions/workflows/validation.yml)
+[![Unit tests](https://github.com/ItsDrike/mcproto/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/ItsDrike/mcproto/actions/workflows/unit-tests.yml)
+[![Docs](https://img.shields.io/readthedocs/mcproto?label=Docs)](https://mcproto.readthedocs.io/)
+
+This is a heavily Work-In-Progress library, which attempts to be a full wrapper around the minecraft protocol, allowing
+for simple interactions with minecraft servers, and perhaps even for use as a base to a full minecraft server
+implementation in python (though the speed will very likely be quite terrible, making it probably unusable as any
+real-world playable server).
+
+Currently, the library is very limited and doesn't yet have any documentation, so while contributions are welcome, fair
+warning that there is a lot to comprehend in the code-base and it may be challenging to understand it all.
+
+## Installation
+
+Mcproto is available on [PyPI](https://pypi.org/project/mcproto/), and can be installed trivially with:
+
+```bash
+python3 -m pip install mcproto
+```
+
+That said, as mcproto is still in development, the PyPI version will likely go out of date quite soon. This means that
+it may lack some already implemented features, or contain already fixed bugs. For that reason, you can also consider
+installing mcproto through git, to get the most recent version. But know that while this will mean you'll be getting
+all of the new features, this version is much more likely to contain bugs than the one on PyPI, so make your decision
+wisely. To install the latest version from git, you can use the command below:
+
+```bash
+python3 -m pip install 'mcproto @ git+https://github.com/py-mine/mcproto@main'
+```
+
+Alternatively, if you want to poke around with mcproto's code, you can always include mcproto as a full [git
+submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules) to your project, or just git clone it directly and play
+around with it from REPL.
+
+## Examples
+
+Since there is no documentation, to satisfy some curious minds that really want to use this library even in this
+heavily unfinished state, here's a few simple snippets of it in practice:
+
+### Manual communication with the server
+
+As sending entire packets is still being worked on, the best solution to communicate with a server is to send the data
+manually, using our connection reader/writer, and buffers (being readers/writers, but only from bytearrays as opposed
+to using an actual connection).
+
+Fair warning: This example is pretty long, but that's because it aims to explain the minecraft protocol to people that
+see it for the first time, and so a lot of explanation comments are included. But the code itself is actually quite
+simple, due to a bunch of helpful read/write methods the library already provides.
+
+```python
+import json
+import asyncio
+
+from mcproto.buffer import Buffer
+from mcproto.connection import TCPAsyncConnection
+from mcproto.protocol.base_io import StructFormat
+
+
+async def handshake(conn: TCPAsyncConnection, ip: str, port: int = 25565) -> None:
+    # As a simple example, let's request status info from a server.
+    # (this is what you see in the multiplayer server list, i.e. the server's motd, icon, info
+    # about how many players are connected, etc.)
+
+    # To do this, we first need to understand how are minecraft packets composed, and take a look
+    # at the specific packets that we're interested in. Thankfully, there's an amazing community
+    # made wiki that documents all of this! You can find it at https://wiki.vg/
+
+    # Alright then, let's take a look at the (uncompressed) packet format specification:
+    # https://wiki.vg/Protocol#Packet_format
+    # From the wiki, we can see that a packet is composed of 3 fields:
+    # - Packet length (in bytes), sent as a variable length integer
+    #       combined length of the 2 fields below
+    # - Packet ID, also sent as varint
+    #       each packet has a unique number, that we use to find out which packet it is
+    # - Data, specific to the individual packet
+    #       every packet can hold different kind of data, this will be shown in the packet's
+    #       specification (you can find these in wiki.vg)
+
+    # Ok then, with this knowledge, let's establish a connection with our server, and request
+    # status. To do this, we fist need to send a handshake packet. Let's do it:
+
+    # Let's take a look at what data the Handshake packet should contain:
+    # https://wiki.vg/Protocol#Handshake
+    handshake = Buffer()
+    # We use 47 for the protocol version, as it's quite old, and will work with almost any server
+    handshake.write_varint(47)
+    handshake.write_utf(ip)
+    handshake.write_value(StructFormat.USHORT, port)
+    handshake.write_varint(1)  # Intention to query status
+
+    # Nice! Now that we have the packet data, let's follow the packet format and send it.
+    # Let's prepare another buffer that will contain the last 2 fields (packet id and data)
+    # combined. We do this since the first field will require us to know the size of these
+    # two combined, so let's just put them into 1 buffer.
+    packet = Buffer()
+    packet.write_varint(0)  # Handshake packet has packet ID of 0
+    packet.write(handshake)  # Full data from our handshake packet
+
+    # And now, it's time to send it!
+    await conn.write_varint(len(packet))  # First field (size of packet id + data)
+    await conn.write(packet)  # Second + Third fields (packet id + data)
+
+
+async def status(conn: TCPAsyncConnection, ip: str, port: int = 25565) -> dict:
+    # This function will be called right after a handshake
+    # Sending this packet told the server recognize our connection, and since we've specified
+    # the intention to query status, it then moved us to STATUS game state.
+
+    # Different game states have different packets that we can send out, for example there is a
+    # game state for login, that we're put into while joining the server, and from it, we tell
+    # the server our username player UUID, etc.
+
+    # The packet IDs are unique to each game state, so since we're now in status state, a packet
+    # with ID of 0 is no longer the handshake packet, but rather the status request packet
+    # (precisely what we need).
+    # https://wiki.vg/Protocol#Status_Request
+
+    # The status request packet is empty, and doesn't contain any data, it just instructs the
+    # server to send us back a status response packet. Let's send it!
+    packet = Buffer()
+    packet.write_varint(0)  # Status request packet ID
+
+    await conn.write_varint(len(packet))
+    await conn.write(packet)
+
+    # Now, let's receive the response packet from the server
+    # Remember, the packet format states that we first receive a length, then packet id, then data
+    _response_len = await conn.read_varint()
+    _response = await conn.read(_response_len)  # will give us a bytearray
+
+    # Amazing, we've just received data from the server! But it's just bytes, let's turn it into
+    # a Buffer object, which includes helpful methods that allow us to read from it
+    response = Buffer(_response)
+    packet_id = response.read_varint()  # Remember, 2nd field is the packet ID
+
+    # Let's see it then, what packet did we get?
+    print(packet_id)  # 0
+
+    # Interesting, this packet has an ID of 0, but wasn't that the status request packet? We wanted
+    # a response tho. Well, actually, if we take a look at the status response packet at the wiki,
+    # it really has an ID of 0:
+    # https://wiki.vg/Protocol#Status_Response
+    # Aha, so not only are packet ids unique between game states, they're also unique between the
+    # direction a server bound packet (sent by client, with server as the destination) can have an
+    # id of 0, while a client bound packet (sent by server, with client as the destination) can
+    # have the same id, and mean something else.
+
+    # Alright then, so we know what we got is a status response packet, let's read the wiki a bit
+    # further and see what data it actually contains, and see how we can get it out. Hmmm, it
+    # contains a UTF-8 encoded string that represents JSON data, ok, so let's get that string, it's
+    # still in our buffer.
+    received_string = response.read_utf()
+
+    # Now, let's just use the json module, convert the string into some json object (in this case,
+    # a dict)
+    data = json.loads(received_string)
+    return data
+
+async def main():
+    # That's it, all that's left is actually calling our functions now
+
+    ip = "mc.hypixel.net"
+    port = 25565
+
+    async with (await TCPAsyncConnection.make_client((ip, port), 2)) as connection:
+        await handshake(connection, ip, port)
+        data = await status(connection, ip, port)
+
+    # Wohoo, we got the status data! Let's see it
+    print(data["players"]["max"])  # This is the server's max player amount (slots)
+    print(data["players"]["online"])  # This is how many people are currently online
+    print(data["description"])  # And here's the motd
+
+    # There's a bunch of other things in this data, try it out, see what you can find!
+
+def start():
+    # Just some boilerplate code that can run our asynchronous main function
+    asyncio.run(main())
+```
+
+### Using packet classes for communication
+
+#### Obtaining the packet map
+
+The first thing you'll need to understand about packet classes in mcproto is that they're versioned depending on the
+protocol version you're using. As we've already seen with minecraft packets, they're following a certain format, and
+for given packet direction and game state, the packet numbers are unique.
+
+This is how we can detect what packet is being received, but because of the different versions that the library can
+support, we will need to use a packet map, that will contain all of the mappings for given protocol version, from
+which, knowing the state and direction, we can get a dictionary with packet IDs as keys, and the individual packet
+classes as values.
+
+This dictionary is crucial to receiving packets, as it's the only thing that tells us which packet class should be
+used, once we receive a packet and learn about the packet id. Otherwise we wouldn't know what to do with the data we
+obtained.
+
+The first game state we'll be in, before doing anything will always be the handshaking state, so let's see how we could
+generate this dictionary for this state, for all of the receiving (client bound) packets.
+
+```python
+from mcproto.packets import PACKET_MAP
+from mcproto.packets.abc import PacketDirection, GameState
+
+handshaking_packet_map = PACKET_MAP.make_id_map(
+    protocol_version=757,
+    direction=PacketDirection.CLIENTBOUND,
+    game_state=GameState.HANDSHAKING
+)
+
+print(handshaking_packet_map)  # {}
+```
+
+Notice that the packet map is actually empty, and this is simply because there (currently) aren't any client bound
+packets a server can send out for the handshaking game state. Let's see the status gamestate instead:
+
+```python
+status_packet_map = PACKET_MAP.make_id_map(
+    protocol_version=757,
+    direction=PacketDirection.CLIENTBOUND,
+    game_state=GameState.STATUS,
+)
+
+print(status_packet_map)  # Will print:
+# {1: mcproto.packets.v757.status.ping.PingPong, 0: mcproto.packets.v757.status.status.StatusResponse}
+```
+
+Cool! These are all of the packets, with their IDs that the server can send in STATUS game state.
+
+#### Creating our own packets
+
+
+Now, we could create a similar packet map for sending out the packets, and just use it to construct our packets,
+however this is not the recommended approach, as it's kind of hard to remember all of the packet IDs, and (at least
+currently) it means not having any typing information about what packet class will we get. For that reason, it's
+recommended to import packets that we want to send out manually, like so:
+
+```python
+from mcproto.packets.v757.handshaking.handshake import Handshake, NextState
+
+my_handshake = Handshake(
+    # Once again, we use an old protocol version so that even older servers will work
+    protocol_version=47,
+    server_address="mc.hypixel.net",
+    server_port=25565,
+    next_state=NextState.STATUS,
+)
+```
+
+That's it! We've now constructed a full handshake packet with all of the data it should contain. You might remember
+from the example above, that we originally had to look at the protocol specification, find the handshake packet and
+construct it's data as a Buffer with all of these variables.
+
+With these packet classes, you can simply follow your editor's function hints to see what this packet requires, pass it
+in and the data will be constructed for you from these attributes, once we'll be to sending it.
+
+For completion, let's also construct the status request packet that we were sending to instruct the server to send us
+back the status response packet.
+
+```python
+from mcproto.packets.v757.status.status import StatusRequest
+
+my_status_request = StatusRequest()
+```
+
+This one was even easier, as the status request packet alone doesn't contain any special data, it's just a request to
+the server to send us some data back.
+
+#### Sending packets
+
+To actually send out a packet to the server, we'll need to create a connection, and use the custom functions
+responsible for sending packets out. Let's see it:
+
+```python
+from mcproto.packets import async_write_packet
+from mcproto.connection import TCPAsyncConnection
+
+async def main():
+    ip = "mc.hypixel.net"
+    port = 25565
+
+    async with (await TCPAsyncConnection.make_client((ip, port), 2)) as connection:
+        await async_write_packet(connection, my_handshake)  
+        # my_handshake is a packet we've created in the example before
+```
+
+How quick was that? Now compare this to the manual version.
+
+#### Receiving packets
+
+Alright, we might now know how to send a packet, but how do we receive one? Let's see:
+
+```python
+from mcproto.packets import PACKET_MAP
+
+# Let's prepare the packet map we'll be using, say we're already in the STATUS game state now
+STATUS_PACKET_MAP = PACKET_MAP.make_id_map(
+    protocol_version=757,
+    direction=PacketDirection.CLIENTBOUND,
+    game_state=GameState.STATUS
+)
+
+# Let's say we already have a connection at this moment, after all, how else would
+# we've gotten into the STATUS game state.
+# Also, let's do something different, let's say we have a synchronous connection
+from mcproto.connection import TCPSyncConnection
+conn: TCPSyncConnection
+
+# With a synchronous connection, comes synchronous reader, so instead of using async_read_packet,
+# we'll use sync_read_packet here
+from mcproto.packets import sync_read_packet
+
+packet = sync_read_packet(conn, STATUS_PACKET_MAP)
+
+# Cool! We've got back a packet, but what packet is it? Let's import the packet classes it could
+# be and check against them
+from mcproto.packets.v757.status.status import StatusResponse
+from mcproto.packets.v757.status.ping import PingPong
+
+if isinstance(packet, StatusResponse):
+    ...
+elif isinstance(packet, PingPong):
+    ...
+else:
+    raise Exception("Impossible, there aren't other client bound packets in the STATUS game state")
+```
+
+#### Requesting status
+
+Now let's actually do something meaningful, and replicate the entire example from the manual version using packets,
+let's see just how much simpler it will be:
+
+```python
+from mcproto.connection import TCPAsyncConnection
+from mcproto.packets import async_write_packet, async_read_packet, PACKET_MAP
+from mcproto.packets.abc import PacketDirection, GameState
+from mcproto.packets.v757.handshaking.handshake import Handshake, NextState
+from mcproto.packets.v757.status.status import StatusRequest, StatusResponse
+
+STATUS_PACKET_MAP = PACKET_MAP.make_id_map(
+    protocol_version=757,
+    direction=PacketDirection.CLIENTBOUND,
+    game_state=GameState.STATUS
+)
+
+
+async def get_status(ip: str, port: int) -> dict:
+    handshake_packet = Handshake(
+        protocol_version=47,
+        server_address=ip,
+        server_port=port,
+        next_state=NextState.STATUS,
+    )
+    status_req_packet = StatusRequest()
+
+    async with (await TCPAsyncConnection.make_client((ip, port), 2)) as connection:
+        # We start out at HANDSHAKING game state
+        await async_write_packet(connection, handshake_packet)  
+        # After sending the handshake, we told the server to now move us into the STATUS game state
+        await async_write_packet(connection, status_req_packet)  
+        # Since we're still in STATUS game state, we use the status packet map when reading
+        packet = await async_read_packet(connection, STATUS_PACKET_MAP)
+
+    # Now that we've got back the packet, we no longer need the connection, we won't be sending
+    # anything else. Let's just make sure it really is the packet we expected
+    if not isinstance(packet, StatusResponse):
+        raise ValueError(f"We've got an unexpected packet back: {packet!r}")
+
+    # Now that we know we're dealing with a status response, let's get out it's data, and return in
+    return packet.data
+```
+
+Well, that wasn't so hard, was it?
 
-setup(**setup_kwargs)
```

