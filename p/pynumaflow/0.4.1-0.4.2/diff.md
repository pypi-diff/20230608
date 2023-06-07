# Comparing `tmp/pynumaflow-0.4.1.tar.gz` & `tmp/pynumaflow-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumaflow-0.4.1.tar", max compression
+gzip compressed data, was "pynumaflow-0.4.2.tar", max compression
```

## Comparing `pynumaflow-0.4.1.tar` & `pynumaflow-0.4.2.tar`

### file list

```diff
@@ -1,47 +1,31 @@
--rw-r--r--   0        0        0    11357 2023-04-25 00:58:49.725827 pynumaflow-0.4.1/LICENSE
--rw-r--r--   0        0        0     3506 2023-04-25 00:58:49.725827 pynumaflow-0.4.1/README.md
--rw-r--r--   0        0        0      985 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/__init__.py
--rw-r--r--   0        0        0      511 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/_constants.py
--rw-r--r--   0        0        0      248 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/exceptions.py
--rw-r--r--   0        0        0      521 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/__init__.py
--rw-r--r--   0        0        0     9146 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/_dtypes.py
--rw-r--r--   0        0        0     1779 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/_udfunction_pb2.pyi
--rw-r--r--   0        0        0    13045 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/async_server.py
--rw-r--r--   0        0        0      512 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/asynciter.py
--rw-r--r--   0        0        0    11555 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/multiproc_server.py
--rw-r--r--   0        0        0        0 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/proto/__init__.py
--rw-r--r--   0        0        0     2029 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/proto/udfunction.proto
--rw-r--r--   0        0        0     3138 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/proto/udfunction_pb2.py
--rw-r--r--   0        0        0     7523 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/proto/udfunction_pb2_grpc.py
--rw-r--r--   0        0        0     9546 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/server.py
--rw-r--r--   0        0        0        0 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/info/__init__.py
--rw-r--r--   0        0        0     1594 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/info/server.py
--rw-r--r--   0        0        0     1249 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/info/types.py
--rw-r--r--   0        0        0      219 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/__init__.py
--rw-r--r--   0        0        0     3290 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/_dtypes.py
--rw-r--r--   0        0        0     2257 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/_udfunction_pb2.pyi
--rw-r--r--   0        0        0     5832 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/async_sink.py
--rw-r--r--   0        0        0        0 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/proto/__init__.py
--rw-r--r--   0        0        0     1716 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/proto/udsink.proto
--rw-r--r--   0        0        0     2513 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/proto/udsink_pb2.py
--rw-r--r--   0        0        0     4106 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/proto/udsink_pb2_grpc.py
--rw-r--r--   0        0        0     5100 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/server.py
--rw-r--r--   0        0        0       79 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/__init__.py
--rw-r--r--   0        0        0    13402 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/test_async_server.py
--rw-r--r--   0        0        0     4741 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/test_async_server_err.py
--rw-r--r--   0        0        0     6720 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/test_datatypes.py
--rw-r--r--   0        0        0     1940 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/test_info_server.py
--rw-r--r--   0        0        0     3889 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/test_messages.py
--rw-r--r--   0        0        0     3663 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/test_messagets.py
--rw-r--r--   0        0        0    10620 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/test_multiproc.py
--rw-r--r--   0        0        0    10117 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/tests/function/test_sync_server.py
--rw-r--r--   0        0        0     2800 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/tests/function/testing_utils.py
--rw-r--r--   0        0        0        0 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/tests/sink/__init__.py
--rw-r--r--   0        0        0     5153 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/tests/sink/test_async_sink.py
--rw-r--r--   0        0        0     3327 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/tests/sink/test_datatypes.py
--rw-r--r--   0        0        0     1305 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/tests/sink/test_responses.py
--rw-r--r--   0        0        0     5937 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/tests/sink/test_server.py
--rw-r--r--   0        0        0      170 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/types.py
--rw-r--r--   0        0        0     1358 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4696 1970-01-01 00:00:00.000000 pynumaflow-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-07 23:32:14.117722 pynumaflow-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4468 2023-06-07 23:32:14.117722 pynumaflow-0.4.2/README.md
+-rw-r--r--   0        0        0      985 2023-06-07 23:32:14.125722 pynumaflow-0.4.2/pynumaflow/__init__.py
+-rw-r--r--   0        0        0      511 2023-06-07 23:32:14.125722 pynumaflow-0.4.2/pynumaflow/_constants.py
+-rw-r--r--   0        0        0      248 2023-06-07 23:32:14.125722 pynumaflow-0.4.2/pynumaflow/exceptions.py
+-rw-r--r--   0        0        0      561 2023-06-07 23:32:14.125722 pynumaflow-0.4.2/pynumaflow/function/__init__.py
+-rw-r--r--   0        0        0     9858 2023-06-07 23:32:14.125722 pynumaflow-0.4.2/pynumaflow/function/_dtypes.py
+-rw-r--r--   0        0        0     1779 2023-06-07 23:32:14.125722 pynumaflow-0.4.2/pynumaflow/function/_udfunction_pb2.pyi
+-rw-r--r--   0        0        0    15112 2023-06-07 23:32:14.125722 pynumaflow-0.4.2/pynumaflow/function/async_server.py
+-rw-r--r--   0        0        0      512 2023-06-07 23:32:14.125722 pynumaflow-0.4.2/pynumaflow/function/asynciter.py
+-rw-r--r--   0        0        0    12367 2023-06-07 23:32:14.125722 pynumaflow-0.4.2/pynumaflow/function/multiproc_server.py
+-rw-r--r--   0        0        0        0 2023-06-07 23:32:14.125722 pynumaflow-0.4.2/pynumaflow/function/proto/__init__.py
+-rw-r--r--   0        0        0     2230 2023-06-07 23:32:14.125722 pynumaflow-0.4.2/pynumaflow/function/proto/udfunction.proto
+-rw-r--r--   0        0        0     3170 2023-06-07 23:32:14.125722 pynumaflow-0.4.2/pynumaflow/function/proto/udfunction_pb2.py
+-rw-r--r--   0        0        0     8966 2023-06-07 23:32:14.125722 pynumaflow-0.4.2/pynumaflow/function/proto/udfunction_pb2_grpc.py
+-rw-r--r--   0        0        0    10491 2023-06-07 23:32:14.129722 pynumaflow-0.4.2/pynumaflow/function/server.py
+-rw-r--r--   0        0        0        0 2023-06-07 23:32:14.129722 pynumaflow-0.4.2/pynumaflow/info/__init__.py
+-rw-r--r--   0        0        0     1594 2023-06-07 23:32:14.129722 pynumaflow-0.4.2/pynumaflow/info/server.py
+-rw-r--r--   0        0        0     1249 2023-06-07 23:32:14.129722 pynumaflow-0.4.2/pynumaflow/info/types.py
+-rw-r--r--   0        0        0      219 2023-06-07 23:32:14.129722 pynumaflow-0.4.2/pynumaflow/sink/__init__.py
+-rw-r--r--   0        0        0     4521 2023-06-07 23:32:14.129722 pynumaflow-0.4.2/pynumaflow/sink/_dtypes.py
+-rw-r--r--   0        0        0     2257 2023-06-07 23:32:14.129722 pynumaflow-0.4.2/pynumaflow/sink/_udfunction_pb2.pyi
+-rw-r--r--   0        0        0     5858 2023-06-07 23:32:14.129722 pynumaflow-0.4.2/pynumaflow/sink/async_sink.py
+-rw-r--r--   0        0        0        0 2023-06-07 23:32:14.129722 pynumaflow-0.4.2/pynumaflow/sink/proto/__init__.py
+-rw-r--r--   0        0        0     1716 2023-06-07 23:32:14.129722 pynumaflow-0.4.2/pynumaflow/sink/proto/udsink.proto
+-rw-r--r--   0        0        0     2454 2023-06-07 23:32:14.129722 pynumaflow-0.4.2/pynumaflow/sink/proto/udsink_pb2.py
+-rw-r--r--   0        0        0     4032 2023-06-07 23:32:14.129722 pynumaflow-0.4.2/pynumaflow/sink/proto/udsink_pb2_grpc.py
+-rw-r--r--   0        0        0     5119 2023-06-07 23:32:14.129722 pynumaflow-0.4.2/pynumaflow/sink/server.py
+-rw-r--r--   0        0        0      170 2023-06-07 23:32:14.129722 pynumaflow-0.4.2/pynumaflow/types.py
+-rw-r--r--   0        0        0     1688 2023-06-07 23:32:14.129722 pynumaflow-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5552 1970-01-01 00:00:00.000000 pynumaflow-0.4.2/PKG-INFO
```

### Comparing `pynumaflow-0.4.1/LICENSE` & `pynumaflow-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.1/pynumaflow/__init__.py` & `pynumaflow-0.4.2/pynumaflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.1/pynumaflow/function/__init__.py` & `pynumaflow-0.4.2/pynumaflow/function/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from pynumaflow.function._dtypes import (
     Message,
     Messages,
     MessageT,
     MessageTs,
     Datum,
+    DatumMetadata,
     IntervalWindow,
     Metadata,
     DROP,
 )
 from pynumaflow.function.async_server import AsyncServer
 from pynumaflow.function.multiproc_server import MultiProcServer
 from pynumaflow.function.server import Server
 
 __all__ = [
     "Message",
     "Messages",
     "MessageT",
     "MessageTs",
     "Datum",
+    "DatumMetadata",
     "IntervalWindow",
     "Metadata",
     "DROP",
     "Server",
     "AsyncServer",
     "MultiProcServer",
 ]
```

### Comparing `pynumaflow-0.4.1/pynumaflow/function/_dtypes.py` & `pynumaflow-0.4.2/pynumaflow/function/_dtypes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,144 +1,164 @@
 from asyncio import Task
+from collections.abc import Iterator, Sequence
 from dataclasses import dataclass
 from datetime import datetime
-from typing import TypeVar, List, Type
+from typing import TypeVar
+from warnings import warn
 
 from pynumaflow.function.asynciter import NonBlockingIterator
 
 DROP = "U+005C__DROP__"
 
 M = TypeVar("M", bound="Message")
 Ms = TypeVar("Ms", bound="Messages")
 MT = TypeVar("MT", bound="MessageT")
 MTs = TypeVar("MTs", bound="MessageTs")
 
 
-@dataclass
+@dataclass(init=False)
 class Message:
     """
     Basic datatype for data passing to the next vertex/vertices.
 
     Args:
-        _value: data in bytes
-         _keys: []string keys for vertex (optional)
-         _tags: []string tags for conditional forwarding (optional)
+        value: data in bytes
+        keys: []string keys for vertex (optional)
+        tags: []string tags for conditional forwarding (optional)
     """
 
-    _keys: List[str]
-    _tags: List[str]
-    _value: bytes = b""
+    __slots__ = ("_value", "_keys", "_tags")
+
+    _value: bytes
+    _keys: list[str]
+    _tags: list[str]
 
-    def __init__(self, value: bytes, keys=None, tags=None):
+    def __init__(self, value: bytes, keys: list[str] = None, tags: list[str] = None):
         """
         Creates a Message object to send value to a vertex.
         """
         self._keys = keys or []
         self._tags = tags or []
         self._value = value or b""
 
     # returns the Message Object which will be dropped
     @classmethod
-    def to_drop(cls: Type[M]) -> M:
+    def to_drop(cls: type[M]) -> M:
         return cls(b"", None, [DROP])
 
     @property
     def value(self) -> bytes:
         return self._value
 
     @property
-    def keys(self) -> List[str]:
+    def keys(self) -> list[str]:
         return self._keys
 
     @property
-    def tags(self) -> List[str]:
+    def tags(self) -> list[str]:
         return self._tags
 
 
-class Messages:
+class Messages(Sequence[M]):
     """
     Class to define a list of Message objects.
 
     Args:
         messages: list of Message objects.
     """
 
     __slots__ = ("_messages",)
 
     def __init__(self, *messages: M):
         self._messages = list(messages) or []
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self._messages)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return str(self)
 
+    def __len__(self) -> int:
+        return len(self._messages)
+
+    def __iter__(self) -> Iterator[M]:
+        return iter(self._messages)
+
+    def __getitem__(self, index: int) -> M:
+        if isinstance(index, slice):
+            raise TypeError("Slicing is not supported for Messages")
+        return self._messages[index]
+
     def append(self, message: Message) -> None:
         self._messages.append(message)
 
-    def items(self) -> List[Message]:
+    def items(self) -> list[Message]:
+        warn(
+            "Using items is deprecated and will be removed in v0.5. "
+            "Iterate or index the Messages object instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         return self._messages
 
-    def dumps(self) -> str:
-        return str(self)
-
-    def loads(self) -> Ms:
-        pass
 
-
-@dataclass
+@dataclass(init=False)
 class MessageT:
     """
     Basic datatype for data passing to the next vertex/vertices.
 
     Args:
-        _value: data in bytes
-        _event_time: event time of the message, usually extracted from the payload.
-         _keys: []string keys for vertex (optional)
-         _tags: []string tags for conditional forwarding (optional)
+        value: data in bytes
+        event_time: event time of the message, usually extracted from the payload.
+        keys: []string keys for vertex (optional)
+        tags: []string tags for conditional forwarding (optional)
     """
 
-    _keys: List[str]
-    _tags: List[str]
-    _value: bytes = b""
-    # There is no year 0, so setting following as default event time.
-    _event_time: datetime = datetime(1, 1, 1, 0, 0)
+    __slots__ = ("_value", "_keys", "_tags", "_event_time")
+
+    _keys: list[str]
+    _tags: list[str]
+    _value: bytes
+    _event_time: datetime
 
-    def __init__(self, value: bytes, event_time: datetime, keys=None, tags=None):
+    def __init__(
+        self, value: bytes, event_time: datetime, keys: list[str] = None, tags: list[str] = None
+    ):
         """
         Creates a MessageT object to send value to a vertex.
         """
         self._tags = tags or []
         self._keys = keys or []
+
+        # There is no year 0, so setting following as default event time.
         self._event_time = event_time or datetime(1, 1, 1, 0, 0)
         self._value = value or b""
 
     @classmethod
-    def to_drop(cls: Type[MT]) -> MT:
+    def to_drop(cls: type[MT]) -> MT:
         return cls(b"", datetime(1, 1, 1, 0, 0), None, [DROP])
 
     @property
     def event_time(self) -> datetime:
         return self._event_time
 
     @property
-    def keys(self) -> List[str]:
+    def keys(self) -> list[str]:
         return self._keys
 
     @property
     def value(self) -> bytes:
         return self._value
 
     @property
-    def tags(self) -> List[str]:
+    def tags(self) -> list[str]:
         return self._tags
 
 
-class MessageTs:
+class MessageTs(Sequence[MT]):
     """
     Class to define a list of MessageT objects.
 
     Args:
         message_ts: list of MessageT objects.
     """
 
@@ -149,90 +169,111 @@
 
     def __str__(self):
         return str(self._message_ts)
 
     def __repr__(self):
         return str(self)
 
+    def __len__(self) -> int:
+        return len(self._message_ts)
+
+    def __iter__(self) -> Iterator[M]:
+        return iter(self._message_ts)
+
+    def __getitem__(self, index: int) -> M:
+        if isinstance(index, slice):
+            raise TypeError("Slicing is not supported for MessageTs")
+        return self._message_ts[index]
+
     def append(self, message_t: MessageT) -> None:
         self._message_ts.append(message_t)
 
-    def items(self) -> List[MessageT]:
+    def items(self) -> list[MessageT]:
+        warn(
+            "Using items is deprecated and will be removed in v0.5. "
+            "Iterate or index the Messages object instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         return self._message_ts
 
-    def dumps(self) -> str:
-        return str(self)
-
-    def loads(self) -> Ms:
-        pass
-
 
+@dataclass(init=False)
 class DatumMetadata:
     """
     Class to define the metadata information for the event.
     Args:
-        msg_id: the id of the event.
-        num_delivered: the number the event has been delivered.
+        msg_id: the id of the event. (default: "")
+        num_delivered: the number the event has been delivered. (default: 0)
     >>> # Example usage
     >>> from pynumaflow.function import DatumMetadata
-    >>> msg_id = "id"
-    >>> num_delivered = 1
-    >>> d = Datum(id=msg_id, num_delivered=num_delivered)
+    >>> d = Datum(id="id", num_delivered=1)
     """
 
+    __slots__ = ("_id", "_num_delivered")
+
+    _id: str
+    _num_delivered: int
+
     def __init__(
         self,
         msg_id: str,
         num_delivered: int,
     ):
         self._id = msg_id or ""
         self._num_delivered = num_delivered or 0
 
-    def __str__(self):
-        return f"id: {self._id}, " f"num_delivered: {str(self._num_delivered)}"
-
-    def __repr__(self):
-        return str(self)
-
     @property
     def id(self) -> str:
         """Returns the id of the event."""
         return self._id
 
     @property
     def num_delivered(self):
         """Returns the number the event has been delivered."""
         return self._num_delivered
 
 
+@dataclass(init=False)
 class Datum:
     """
     Class to define the important information for the event.
     Args:
         keys: the keys of the event.
         value: the payload of the event.
         event_time: the event time of the event.
         watermark: the watermark of the event.
         metadata: the metadata of the event.
     >>> # Example usage
     >>> from pynumaflow.function import Datum
     >>> from datetime import datetime, timezone
-    >>> keys = ["test_key"]
     >>> payload = bytes("test_mock_message", encoding="utf-8")
     >>> t1 = datetime.fromtimestamp(1662998400, timezone.utc)
     >>> t2 = datetime.fromtimestamp(1662998460, timezone.utc)
     >>> metadata = DatumMetadata(msg_id="test_id", num_delivered=1)
-    >>> d = Datum(keys=keys, value=payload, event_time=t1, watermark=t2, metadata=metadata
+    >>> d = Datum(
+    ...       keys=["test_key"],
+    ...       value=payload,
+    ...       event_time=t1,
+    ...       watermark=t2,
+    ...       metadata=DatumMetadata(msg_id="test_id", num_delivered=1)
+    ...    )
     """
 
     __slots__ = ("_keys", "_value", "_event_time", "_watermark", "_metadata")
 
+    _keys: list[str]
+    _value: bytes
+    _event_time: datetime
+    _watermark: datetime
+    _metadata: DatumMetadata
+
     def __init__(
         self,
-        keys: List[str],
+        keys: list[str],
         value: bytes,
         event_time: datetime,
         watermark: datetime,
         metadata: DatumMetadata,
     ):
         self._keys = keys or list()
         self._value = value or b""
@@ -240,28 +281,15 @@
             raise TypeError(f"Wrong data type: {type(event_time)} for Datum.event_time")
         self._event_time = event_time
         if not isinstance(watermark, datetime):
             raise TypeError(f"Wrong data type: {type(watermark)} for Datum.watermark")
         self._watermark = watermark
         self._metadata = metadata
 
-    def __str__(self):
-        value_string = self._value.decode("utf-8")
-        return (
-            f"keys: {self._keys}, "
-            f"value: {value_string}, "
-            f"event_time: {str(self._event_time)}, "
-            f"watermark: {str(self._watermark)}, "
-            f"metadata: {str(self._metadata)}"
-        )
-
-    def __repr__(self):
-        return str(self)
-
-    def keys(self) -> List[str]:
+    def keys(self) -> list[str]:
         """Returns the keys of the event"""
         return self._keys
 
     @property
     def value(self) -> bytes:
         """Returns the value of the event."""
         return self._value
@@ -278,77 +306,72 @@
 
     @property
     def metadata(self) -> DatumMetadata:
         """Returns the metadata of the event."""
         return self._metadata
 
 
+@dataclass(init=False)
 class IntervalWindow:
     """Defines the start and end of the interval window for the event."""
 
     __slots__ = ("_start", "_end")
 
+    _start: datetime
+    _end: datetime
+
     def __init__(self, start: datetime, end: datetime):
         self._start = start
         self._end = end
 
-    def __str__(self):
-        return f"start: {self._start}, end: {self._end}"
-
-    def __repr__(self):
-        return str(self)
-
     @property
     def start(self):
         """Returns the start point of the interval window."""
         return self._start
 
     @property
     def end(self):
         """Returns the end point of the interval window."""
         return self._end
 
 
+@dataclass(init=False)
 class Metadata:
     """Defines the metadata for the event."""
 
     __slots__ = ("_interval_window",)
 
+    _interval_window: IntervalWindow
+
     def __init__(self, interval_window: IntervalWindow):
         self._interval_window = interval_window
 
-    def __str__(self):
-        return f"interval_window: {self._interval_window}"
-
-    def __repr__(self):
-        return str(self)
-
     @property
     def interval_window(self):
         """Returns the interval window for the event."""
         return self._interval_window
 
 
+@dataclass
 class ReduceResult:
     """Defines the object to hold the result of reduce computation."""
 
     __slots__ = ("_future", "_iterator", "_key")
 
-    def __init__(self, future: Task, iterator: NonBlockingIterator, keys: List[str]):
-        self._future = future
-        self._iterator = iterator
-        self._key = keys
+    _future: Task
+    _iterator: NonBlockingIterator
+    _key: list[str]
 
     @property
     def future(self):
         """Returns the future result of computation."""
         return self._future
 
     @property
     def iterator(self):
         """Returns the handle to the producer queue."""
         return self._iterator
 
     @property
-    def keys(self) -> List[str]:
+    def keys(self) -> list[str]:
         """Returns the keys of the partition."""
         return self._key
```

### Comparing `pynumaflow-0.4.1/pynumaflow/function/_udfunction_pb2.pyi` & `pynumaflow-0.4.2/pynumaflow/function/_udfunction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.1/pynumaflow/function/async_server.py` & `pynumaflow-0.4.2/pynumaflow/function/async_server.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 import asyncio
 import logging
 import multiprocessing
 import os
+
 from datetime import datetime, timezone
-from typing import Callable, AsyncIterable, List
+from typing import Callable
+from collections.abc import AsyncIterable
 
 import grpc
 from google.protobuf import empty_pb2 as _empty_pb2
 
 from pynumaflow import setup_logging
 from pynumaflow._constants import (
     FUNCTION_SOCK_PATH,
     WIN_START_TIME,
     WIN_END_TIME,
     MAX_MESSAGE_SIZE,
     STREAM_EOF,
     DELIMITER,
 )
-from pynumaflow.function import Messages, MessageTs, Datum, IntervalWindow, Metadata
+from pynumaflow.function import Message, Messages, MessageTs, Datum, IntervalWindow, Metadata
 from pynumaflow.function._dtypes import ReduceResult, DatumMetadata
 from pynumaflow.function.asynciter import NonBlockingIterator
 from pynumaflow.function.proto import udfunction_pb2
 from pynumaflow.function.proto import udfunction_pb2_grpc
 from pynumaflow.types import NumaflowServicerContext
 from pynumaflow.info.server import get_sdk_version, write as info_server_write
 from pynumaflow.info.types import ServerInfo, Protocol, Language, SERVER_INFO_FILE_PATH
 
 _LOGGER = setup_logging(__name__)
 if os.getenv("PYTHONDEBUG"):
     _LOGGER.setLevel(logging.DEBUG)
 
-UDFMapCallable = Callable[[List[str], Datum], Messages]
-UDFMapTCallable = Callable[[List[str], Datum], MessageTs]
-UDFReduceCallable = Callable[[List[str], AsyncIterable[Datum], Metadata], Messages]
+UDFMapCallable = Callable[[list[str], Datum], Messages]
+UDFMapStreamCallable = Callable[[list[str], Datum], AsyncIterable[Message]]
+UDFMapTCallable = Callable[[list[str], Datum], MessageTs]
+UDFReduceCallable = Callable[[list[str], AsyncIterable[Datum], Metadata], Messages]
 _PROCESS_COUNT = multiprocessing.cpu_count()
 MAX_THREADS = int(os.getenv("MAX_THREADS", 0)) or (_PROCESS_COUNT * 4)
 
 
 async def datum_generator(
     request_iterator: AsyncIterable[udfunction_pb2.DatumRequest],
 ) -> AsyncIterable[Datum]:
@@ -57,14 +60,15 @@
 class AsyncServer(udfunction_pb2_grpc.UserDefinedFunctionServicer):
     """
     Provides an interface to write a User Defined Function (UDFunction)
     which will be exposed over gRPC.
 
     Args:
         map_handler: Function callable following the type signature of UDFMapCallable
+        map_stream_handler: Function callable following the type signature of UDFMapStreamCallable
         mapt_handler: Function callable following the type signature of UDFMapTCallable
         reduce_handler: Function callable following the type signature of UDFReduceCallable
         sock_path: Path to the UNIX Domain Socket
         max_message_size: The max message size in bytes the server can receive and send
         max_threads: The max number of threads to be spawned;
                      defaults to number of processors x4
 
@@ -77,49 +81,61 @@
     >>> async def map_handler(key: [str], datum: Datum) -> Messages:
     ...   val = datum.value
     ...   _ = datum.event_time
     ...   _ = datum.watermark
     ...   messages = Messages(Message(val, keys=keys))
     ...   return messages
     ...
-    ...async def mapT_handler(key: [str], datum: Datum) -> Messages:
+    >>> async def map_stream_handler(key: [str], datums: Datum) -> AsyncIterable[Message]:
+    ...    val = datum.value
+    ...    _ = datum.event_time
+    ...    _ = datum.watermark
+    ...    for i in range(10):
+    ...        yield Message(val, keys=keys)
+    ...
+    ... async def mapT_handler(key: [str], datum: Datum) -> Messages:
     ...         "Not supported"
     ...
-    >>> async def reduce_handler(key: str, datums: Iterator[Datum], md: Metadata) -> Messages:
+    >>> async def reduce_handler(key: str, datums: AsyncIterable[Datum], md: Metadata) -> Messages:
     ...   interval_window = md.interval_window
     ...   counter = 0
     ...   async for _ in datums:
     ...     counter += 1
     ...   msg = (
     ...       f"counter:{counter} interval_window_start:{interval_window.start} "
     ...       f"interval_window_end:{interval_window.end}"
     ...   )
     ...   return Messages(Message(value=str.encode(msg), keys=keys))
     ...
     >>> grpc_server = AsyncServer(
     ...   reduce_handler=reduce_handler,
     ...   map_handler=map_handler,
+    ...   map_stream_handler=map_stream_handler,
     ... )
     >>> aiorun.run(grpc_server.start())
     """
 
     def __init__(
         self,
         map_handler: UDFMapCallable = None,
         mapt_handler: UDFMapTCallable = None,
         reduce_handler: UDFReduceCallable = None,
+        map_stream_handler: UDFMapStreamCallable = None,
         sock_path=FUNCTION_SOCK_PATH,
         max_message_size=MAX_MESSAGE_SIZE,
         max_threads=MAX_THREADS,
     ):
-        if not (map_handler or mapt_handler or reduce_handler):
-            raise ValueError("Require a valid map/mapt handler and/or a valid reduce handler.")
+        if not (map_handler or mapt_handler or map_stream_handler or reduce_handler):
+            raise ValueError(
+                "Require a valid map/map_stream/mapt handler and/or a valid reduce handler."
+            )
 
         self.__map_handler: UDFMapCallable = map_handler
         self.__mapt_handler: UDFMapTCallable = mapt_handler
+        self.__map_stream_handler: UDFMapStreamCallable = map_stream_handler
         self.__reduce_handler: UDFReduceCallable = reduce_handler
         self.sock_path = f"unix://{sock_path}"
         self._max_message_size = max_message_size
         self._max_threads = max_threads
         self.cleanup_coroutines = []
         # Collection for storing strong references to all running tasks.
         # Event loop only keeps a weak reference, which can cause it to
@@ -164,28 +180,61 @@
     async def MapTFn(
         self, request: udfunction_pb2.DatumRequest, context: NumaflowServicerContext
     ) -> udfunction_pb2.DatumResponseList:
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         return udfunction_pb2.DatumResponseList(elements=[])
 
-    async def __invoke_map(self, keys: List[str], req: Datum):
+    async def __invoke_map(self, keys: list[str], req: Datum):
         try:
             msgs = await self.__map_handler(keys, req)
         except Exception as err:
             _LOGGER.critical("UDFError, re-raising the error: %r", err, exc_info=True)
             raise err
         datums = []
-        for msg in msgs.items():
+        for msg in msgs:
             datums.append(
                 udfunction_pb2.DatumResponse(keys=msg.keys, value=msg.value, tags=msg.tags)
             )
 
         return datums
 
+    async def MapStreamFn(
+        self,
+        request: udfunction_pb2.DatumRequest,
+        context: NumaflowServicerContext,
+    ) -> AsyncIterable[udfunction_pb2.DatumResponse]:
+        """
+        Applies a map function to a datum stream in streaming mode.
+        The pascal case function name comes from the proto udfunction_pb2_grpc.py file.
+        """
+
+        async for res in self.__invoke_map_stream(
+            list(request.keys),
+            Datum(
+                keys=list(request.keys),
+                value=request.value,
+                event_time=request.event_time.event_time.ToDatetime(),
+                watermark=request.watermark.watermark.ToDatetime(),
+                metadata=DatumMetadata(
+                    msg_id=request.metadata.id,
+                    num_delivered=request.metadata.num_delivered,
+                ),
+            ),
+        ):
+            yield res
+
+    async def __invoke_map_stream(self, keys: list[str], req: Datum):
+        try:
+            async for msg in self.__map_stream_handler(keys, req):
+                yield udfunction_pb2.DatumResponse(keys=msg.keys, value=msg.value, tags=msg.tags)
+        except Exception as err:
+            _LOGGER.critical("UDFError, re-raising the error: %r", err, exc_info=True)
+            raise err
+
     async def ReduceFn(
         self,
         request_iterator: AsyncIterable[udfunction_pb2.DatumRequest],
         context: NumaflowServicerContext,
     ) -> udfunction_pb2.DatumResponseList:
         """
         Applies a reduce function to a datum stream.
@@ -267,24 +316,24 @@
         for unified_key in callable_dict:
             fut = callable_dict[unified_key].future
             tasks.append(fut)
 
         return tasks
 
     async def __invoke_reduce(
-        self, keys: List[str], request_iterator: AsyncIterable[Datum], md: Metadata
+        self, keys: list[str], request_iterator: AsyncIterable[Datum], md: Metadata
     ):
         try:
             msgs = await self.__reduce_handler(keys, request_iterator, md)
         except Exception as err:
             _LOGGER.critical("UDFError, re-raising the error: %r", err, exc_info=True)
             raise err
 
         datum_responses = []
-        for msg in msgs.items():
+        for msg in msgs:
             datum_responses.append(
                 udfunction_pb2.DatumResponse(keys=msg.keys, value=msg.value, tags=msg.tags)
             )
 
         return datum_responses
 
     async def IsReady(
@@ -297,14 +346,15 @@
         return udfunction_pb2.ReadyResponse(ready=True)
 
     async def __serve_async(self, server) -> None:
         udfunction_pb2_grpc.add_UserDefinedFunctionServicer_to_server(
             AsyncServer(
                 map_handler=self.__map_handler,
                 mapt_handler=self.__mapt_handler,
+                map_stream_handler=self.__map_stream_handler,
                 reduce_handler=self.__reduce_handler,
             ),
             server,
         )
         server.add_insecure_port(self.sock_path)
         _LOGGER.info("GRPC Async Server listening on: %s", self.sock_path)
         await server.start()
```

### Comparing `pynumaflow-0.4.1/pynumaflow/function/asynciter.py` & `pynumaflow-0.4.2/pynumaflow/function/asynciter.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.1/pynumaflow/function/multiproc_server.py` & `pynumaflow-0.4.2/pynumaflow/function/multiproc_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import contextlib
 import logging
 import multiprocessing
 import os
 import socket
 from concurrent import futures
-from typing import Callable, AsyncIterable, List
+from typing import Callable
+from collections.abc import AsyncIterable
 
 import grpc
 from google.protobuf import empty_pb2 as _empty_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 
 from pynumaflow import setup_logging
 from pynumaflow._constants import (
     MAX_MESSAGE_SIZE,
 )
 from pynumaflow._constants import MULTIPROC_FUNCTION_SOCK_PORT, MULTIPROC_FUNCTION_SOCK_ADDR
 from pynumaflow.exceptions import SocketError
-from pynumaflow.function import Messages, MessageTs, Datum, Metadata
+from pynumaflow.function import Message, Messages, MessageTs, Datum, Metadata
 from pynumaflow.function._dtypes import DatumMetadata
 from pynumaflow.function.proto import udfunction_pb2
 from pynumaflow.function.proto import udfunction_pb2_grpc
 from pynumaflow.types import NumaflowServicerContext
 from pynumaflow.info.server import (
     get_sdk_version,
     write as info_server_write,
@@ -34,26 +35,28 @@
     METADATA_ENVS,
 )
 
 _LOGGER = setup_logging(__name__)
 if os.getenv("PYTHONDEBUG"):
     _LOGGER.setLevel(logging.DEBUG)
 
-UDFMapCallable = Callable[[List[str], Datum], Messages]
-UDFMapTCallable = Callable[[List[str], Datum], MessageTs]
-UDFReduceCallable = Callable[[List[str], AsyncIterable[Datum], Metadata], Messages]
+UDFMapCallable = Callable[[list[str], Datum], Messages]
+UDFMapTCallable = Callable[[list[str], Datum], MessageTs]
+UDFMapStreamCallable = Callable[[list[str], Datum], AsyncIterable[Message]]
+UDFReduceCallable = Callable[[list[str], AsyncIterable[Datum], Metadata], Messages]
 
 
 class MultiProcServer(udfunction_pb2_grpc.UserDefinedFunctionServicer):
     """
     Provides an interface to write a User Defined Function (UDFunction)
     which will be exposed over gRPC.
 
     Args:
         map_handler: Function callable following the type signature of UDFMapCallable
+        map_stream_handler: Function callable following the type signature of UDFMapStreamCallable
         mapt_handler: Function callable following the type signature of UDFMapTCallable
         reduce_handler: Function callable following the type signature of UDFReduceCallable
         sock_path: Path to the UNIX Domain Socket
         max_message_size: The max message size in bytes the server can receive and send
         max_threads: The max number of threads to be spawned;
                      defaults to number of processors x4
 
@@ -65,16 +68,16 @@
     >>> def map_handler(key: [str], datum: Datum) -> Messages:
     ...   val = datum.value
     ...   _ = datum.event_time
     ...   _ = datum.watermark
     ...   messages = Messages(Message(val, keys=keys))
     ...   return messages
     ...
-    ... def reduce_handler(key: str, datums: Iterator[Datum], md: Metadata) -> Messages:
-    ...           "Not supported"
+    >>> def map_stream_handler(key: [str], datums: Datum) -> AsyncIterable[Message]:
+    ...         "Not supported"
     ...
     >>> def mapt_handler(key: [str], datum: Datum) -> MessageTs:
     ...   val = datum.value
     ...   new_event_time = datetime.time()
     ...   _ = datum.watermark
     ...   message_t_s = MessageTs(MessageT(val, event_time=new_event_time, keys=key))
     ...   return message_t_s
@@ -86,23 +89,27 @@
     ... )
     >>> grpc_server.start()
     """
 
     def __init__(
         self,
         map_handler: UDFMapCallable = None,
+        map_stream_handler: UDFMapStreamCallable = None,
         mapt_handler: UDFMapTCallable = None,
         reduce_handler: UDFReduceCallable = None,
         sock_path=MULTIPROC_FUNCTION_SOCK_PORT,
         max_message_size=MAX_MESSAGE_SIZE,
     ):
-        if not (map_handler or mapt_handler or reduce_handler):
-            raise ValueError("Require a valid map/mapt handler and/or a valid reduce handler.")
+        if not (map_handler or map_stream_handler or mapt_handler or reduce_handler):
+            raise ValueError(
+                "Require a valid map/mapstream/mapt handler and/or a valid reduce handler."
+            )
 
         self.__map_handler: UDFMapCallable = map_handler
+        self.__map_stream_handler: UDFMapStreamCallable = map_stream_handler
         self.__mapt_handler: UDFMapTCallable = mapt_handler
         self.__reduce_handler: UDFReduceCallable = reduce_handler
         self._max_message_size = max_message_size
         self.cleanup_coroutines = []
         # Collection for storing strong references to all running tasks.
         # Event loop only keeps a weak reference, which can cause it to
         # get lost during execution.
@@ -147,21 +154,34 @@
             _LOGGER.critical("UDFError, re-raising the error: %r", err, exc_info=True)
             context.set_code(grpc.StatusCode.UNKNOWN)
             context.set_details(str(err))
             return udfunction_pb2.DatumResponseList(elements=[])
 
         datums = []
 
-        for msg in msgs.items():
+        for msg in msgs:
             datums.append(
                 udfunction_pb2.DatumResponse(keys=msg.keys, value=msg.value, tags=msg.tags)
             )
 
         return udfunction_pb2.DatumResponseList(elements=datums)
 
+    def MapStreamFn(
+        self,
+        request: udfunction_pb2.DatumRequest,
+        context: NumaflowServicerContext,
+    ) -> AsyncIterable[udfunction_pb2.DatumResponse]:
+        """
+        This method is not implemented because we return the messages
+        in a single stream.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        yield from ()
+
     def MapTFn(
         self, request: udfunction_pb2.DatumRequest, context: NumaflowServicerContext
     ) -> udfunction_pb2.DatumResponseList:
         """
         Applies a function to each datum element.
         The pascal case function name comes from the generated udfunction_pb2_grpc.py file.
         """
@@ -185,15 +205,15 @@
         except Exception as err:
             _LOGGER.critical("UDFError, re-raising the error: %r", err, exc_info=True)
             context.set_code(grpc.StatusCode.UNKNOWN)
             context.set_details(str(err))
             return udfunction_pb2.DatumResponseList(elements=[])
 
         datums = []
-        for msgt in msgts.items():
+        for msgt in msgts:
             event_time_timestamp = _timestamp_pb2.Timestamp()
             event_time_timestamp.FromDatetime(dt=msgt.event_time)
             watermark_timestamp = _timestamp_pb2.Timestamp()
             watermark_timestamp.FromDatetime(dt=request.watermark.watermark.ToDatetime())
             datums.append(
                 udfunction_pb2.DatumResponse(
                     keys=list(msgt.keys),
```

### Comparing `pynumaflow-0.4.1/pynumaflow/function/proto/udfunction.proto` & `pynumaflow-0.4.2/pynumaflow/function/proto/udfunction.proto`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 syntax = "proto3";
 
 import "google/protobuf/timestamp.proto";
 import "google/protobuf/empty.proto";
 
 package function.v1;
 
-
 service UserDefinedFunction {
-  // MapFn applies a function to each datum element.
+  // MapFn applies a function to each datum request element.
   rpc MapFn(DatumRequest) returns (DatumResponseList);
 
-  // MapTFn applies a function to each datum element.
+  // MapStreamFn applies a function to each datum request element and returns a stream.
+  rpc MapStreamFn(DatumRequest) returns (stream DatumResponse);
+
+  // MapTFn applies a function to each datum request element.
   // In addition to map function, MapTFn also supports assigning a new event time to datum.
   // MapTFn can be used only at source vertex by source data transformer.
   rpc MapTFn(DatumRequest) returns (DatumResponseList);
 
-  // ReduceFn applies a reduce function to a datum stream.
+  // ReduceFn applies a reduce function to a datum request stream.
   rpc ReduceFn(stream DatumRequest) returns (stream DatumResponseList);
 
   // IsReady is the heartbeat endpoint for gRPC.
   rpc IsReady(google.protobuf.Empty) returns (ReadyResponse);
 }
 
 message EventTime {
@@ -32,15 +34,15 @@
 message Watermark {
   // watermark is the monotonically increasing time which denotes completeness for the given time for the given vertex.
   google.protobuf.Timestamp watermark = 1;
   // future we can add LATE, ON_TIME etc.
 }
 
 /**
- * Metadata of a datum element.
+ * Metadata of a datum request element.
  */
 message Metadata {
   string id = 1;
   uint64 num_delivered = 2;
 }
 
 /**
@@ -62,15 +64,15 @@
   bytes value = 2;
   EventTime event_time = 3;
   Watermark watermark = 4;
   repeated string tags = 5;
 }
 
 /**
- * DatumList represents a list of datum elements.
+ * DatumResponseList represents a list of datum response elements.
  */
 message DatumResponseList {
   repeated DatumResponse elements = 1;
 }
 
 /**
  * ReadyResponse is the health check result.
```

### Comparing `pynumaflow-0.4.1/pynumaflow/function/proto/udfunction_pb2.py` & `pynumaflow-0.4.2/pynumaflow/function/proto/udfunction_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,43 +2,40 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: udfunction.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x10udfunction.proto\x12\x0b\x66unction.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto";\n\tEventTime\x12.\n\nevent_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp":\n\tWatermark\x12-\n\twatermark\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp"-\n\x08Metadata\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\rnum_delivered\x18\x02 \x01(\x04"\xab\x01\n\x0c\x44\x61tumRequest\x12\x0c\n\x04keys\x18\x01 \x03(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12*\n\nevent_time\x18\x03 \x01(\x0b\x32\x16.function.v1.EventTime\x12)\n\twatermark\x18\x04 \x01(\x0b\x32\x16.function.v1.Watermark\x12\'\n\x08metadata\x18\x05 \x01(\x0b\x32\x15.function.v1.Metadata"\x91\x01\n\rDatumResponse\x12\x0c\n\x04keys\x18\x01 \x03(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12*\n\nevent_time\x18\x03 \x01(\x0b\x32\x16.function.v1.EventTime\x12)\n\twatermark\x18\x04 \x01(\x0b\x32\x16.function.v1.Watermark\x12\x0c\n\x04tags\x18\x05 \x03(\t"A\n\x11\x44\x61tumResponseList\x12,\n\x08\x65lements\x18\x01 \x03(\x0b\x32\x1a.function.v1.DatumResponse"\x1e\n\rReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\x32\xa8\x02\n\x13UserDefinedFunction\x12\x42\n\x05MapFn\x12\x19.function.v1.DatumRequest\x1a\x1e.function.v1.DatumResponseList\x12\x43\n\x06MapTFn\x12\x19.function.v1.DatumRequest\x1a\x1e.function.v1.DatumResponseList\x12I\n\x08ReduceFn\x12\x19.function.v1.DatumRequest\x1a\x1e.function.v1.DatumResponseList(\x01\x30\x01\x12=\n\x07IsReady\x12\x16.google.protobuf.Empty\x1a\x1a.function.v1.ReadyResponseb\x06proto3'
-)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10udfunction.proto\x12\x0b\x66unction.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\";\n\tEventTime\x12.\n\nevent_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\":\n\tWatermark\x12-\n\twatermark\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"-\n\x08Metadata\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\rnum_delivered\x18\x02 \x01(\x04\"\xab\x01\n\x0c\x44\x61tumRequest\x12\x0c\n\x04keys\x18\x01 \x03(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12*\n\nevent_time\x18\x03 \x01(\x0b\x32\x16.function.v1.EventTime\x12)\n\twatermark\x18\x04 \x01(\x0b\x32\x16.function.v1.Watermark\x12\'\n\x08metadata\x18\x05 \x01(\x0b\x32\x15.function.v1.Metadata\"\x91\x01\n\rDatumResponse\x12\x0c\n\x04keys\x18\x01 \x03(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12*\n\nevent_time\x18\x03 \x01(\x0b\x32\x16.function.v1.EventTime\x12)\n\twatermark\x18\x04 \x01(\x0b\x32\x16.function.v1.Watermark\x12\x0c\n\x04tags\x18\x05 \x03(\t\"A\n\x11\x44\x61tumResponseList\x12,\n\x08\x65lements\x18\x01 \x03(\x0b\x32\x1a.function.v1.DatumResponse\"\x1e\n\rReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\x32\xf0\x02\n\x13UserDefinedFunction\x12\x42\n\x05MapFn\x12\x19.function.v1.DatumRequest\x1a\x1e.function.v1.DatumResponseList\x12\x46\n\x0bMapStreamFn\x12\x19.function.v1.DatumRequest\x1a\x1a.function.v1.DatumResponse0\x01\x12\x43\n\x06MapTFn\x12\x19.function.v1.DatumRequest\x1a\x1e.function.v1.DatumResponseList\x12I\n\x08ReduceFn\x12\x19.function.v1.DatumRequest\x1a\x1e.function.v1.DatumResponseList(\x01\x30\x01\x12=\n\x07IsReady\x12\x16.google.protobuf.Empty\x1a\x1a.function.v1.ReadyResponseb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "udfunction_pb2", globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'udfunction_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
-    DESCRIPTOR._options = None
-    _EVENTTIME._serialized_start = 95
-    _EVENTTIME._serialized_end = 154
-    _WATERMARK._serialized_start = 156
-    _WATERMARK._serialized_end = 214
-    _METADATA._serialized_start = 216
-    _METADATA._serialized_end = 261
-    _DATUMREQUEST._serialized_start = 264
-    _DATUMREQUEST._serialized_end = 435
-    _DATUMRESPONSE._serialized_start = 438
-    _DATUMRESPONSE._serialized_end = 583
-    _DATUMRESPONSELIST._serialized_start = 585
-    _DATUMRESPONSELIST._serialized_end = 650
-    _READYRESPONSE._serialized_start = 652
-    _READYRESPONSE._serialized_end = 682
-    _USERDEFINEDFUNCTION._serialized_start = 685
-    _USERDEFINEDFUNCTION._serialized_end = 981
+  DESCRIPTOR._options = None
+  _EVENTTIME._serialized_start=95
+  _EVENTTIME._serialized_end=154
+  _WATERMARK._serialized_start=156
+  _WATERMARK._serialized_end=214
+  _METADATA._serialized_start=216
+  _METADATA._serialized_end=261
+  _DATUMREQUEST._serialized_start=264
+  _DATUMREQUEST._serialized_end=435
+  _DATUMRESPONSE._serialized_start=438
+  _DATUMRESPONSE._serialized_end=583
+  _DATUMRESPONSELIST._serialized_start=585
+  _DATUMRESPONSELIST._serialized_end=650
+  _READYRESPONSE._serialized_start=652
+  _READYRESPONSE._serialized_end=682
+  _USERDEFINEDFUNCTION._serialized_start=685
+  _USERDEFINEDFUNCTION._serialized_end=1053
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pynumaflow-0.4.1/pynumaflow/function/proto/udfunction_pb2_grpc.py` & `pynumaflow-0.4.2/pynumaflow/function/proto/udfunction_pb2_grpc.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,207 +12,195 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.MapFn = channel.unary_unary(
-            "/function.v1.UserDefinedFunction/MapFn",
-            request_serializer=udfunction__pb2.DatumRequest.SerializeToString,
-            response_deserializer=udfunction__pb2.DatumResponseList.FromString,
-        )
+                '/function.v1.UserDefinedFunction/MapFn',
+                request_serializer=udfunction__pb2.DatumRequest.SerializeToString,
+                response_deserializer=udfunction__pb2.DatumResponseList.FromString,
+                )
+        self.MapStreamFn = channel.unary_stream(
+                '/function.v1.UserDefinedFunction/MapStreamFn',
+                request_serializer=udfunction__pb2.DatumRequest.SerializeToString,
+                response_deserializer=udfunction__pb2.DatumResponse.FromString,
+                )
         self.MapTFn = channel.unary_unary(
-            "/function.v1.UserDefinedFunction/MapTFn",
-            request_serializer=udfunction__pb2.DatumRequest.SerializeToString,
-            response_deserializer=udfunction__pb2.DatumResponseList.FromString,
-        )
+                '/function.v1.UserDefinedFunction/MapTFn',
+                request_serializer=udfunction__pb2.DatumRequest.SerializeToString,
+                response_deserializer=udfunction__pb2.DatumResponseList.FromString,
+                )
         self.ReduceFn = channel.stream_stream(
-            "/function.v1.UserDefinedFunction/ReduceFn",
-            request_serializer=udfunction__pb2.DatumRequest.SerializeToString,
-            response_deserializer=udfunction__pb2.DatumResponseList.FromString,
-        )
+                '/function.v1.UserDefinedFunction/ReduceFn',
+                request_serializer=udfunction__pb2.DatumRequest.SerializeToString,
+                response_deserializer=udfunction__pb2.DatumResponseList.FromString,
+                )
         self.IsReady = channel.unary_unary(
-            "/function.v1.UserDefinedFunction/IsReady",
-            request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            response_deserializer=udfunction__pb2.ReadyResponse.FromString,
-        )
+                '/function.v1.UserDefinedFunction/IsReady',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=udfunction__pb2.ReadyResponse.FromString,
+                )
 
 
 class UserDefinedFunctionServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def MapFn(self, request, context):
-        """MapFn applies a function to each datum element."""
+        """MapFn applies a function to each datum request element.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def MapStreamFn(self, request, context):
+        """MapStreamFn applies a function to each datum request element and returns a stream.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def MapTFn(self, request, context):
-        """MapTFn applies a function to each datum element.
+        """MapTFn applies a function to each datum request element.
         In addition to map function, MapTFn also supports assigning a new event time to datum.
         MapTFn can be used only at source vertex by source data transformer.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def ReduceFn(self, request_iterator, context):
-        """ReduceFn applies a reduce function to a datum stream."""
+        """ReduceFn applies a reduce function to a datum request stream.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def IsReady(self, request, context):
-        """IsReady is the heartbeat endpoint for gRPC."""
+        """IsReady is the heartbeat endpoint for gRPC.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
 
 def add_UserDefinedFunctionServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "MapFn": grpc.unary_unary_rpc_method_handler(
-            servicer.MapFn,
-            request_deserializer=udfunction__pb2.DatumRequest.FromString,
-            response_serializer=udfunction__pb2.DatumResponseList.SerializeToString,
-        ),
-        "MapTFn": grpc.unary_unary_rpc_method_handler(
-            servicer.MapTFn,
-            request_deserializer=udfunction__pb2.DatumRequest.FromString,
-            response_serializer=udfunction__pb2.DatumResponseList.SerializeToString,
-        ),
-        "ReduceFn": grpc.stream_stream_rpc_method_handler(
-            servicer.ReduceFn,
-            request_deserializer=udfunction__pb2.DatumRequest.FromString,
-            response_serializer=udfunction__pb2.DatumResponseList.SerializeToString,
-        ),
-        "IsReady": grpc.unary_unary_rpc_method_handler(
-            servicer.IsReady,
-            request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            response_serializer=udfunction__pb2.ReadyResponse.SerializeToString,
-        ),
+            'MapFn': grpc.unary_unary_rpc_method_handler(
+                    servicer.MapFn,
+                    request_deserializer=udfunction__pb2.DatumRequest.FromString,
+                    response_serializer=udfunction__pb2.DatumResponseList.SerializeToString,
+            ),
+            'MapStreamFn': grpc.unary_stream_rpc_method_handler(
+                    servicer.MapStreamFn,
+                    request_deserializer=udfunction__pb2.DatumRequest.FromString,
+                    response_serializer=udfunction__pb2.DatumResponse.SerializeToString,
+            ),
+            'MapTFn': grpc.unary_unary_rpc_method_handler(
+                    servicer.MapTFn,
+                    request_deserializer=udfunction__pb2.DatumRequest.FromString,
+                    response_serializer=udfunction__pb2.DatumResponseList.SerializeToString,
+            ),
+            'ReduceFn': grpc.stream_stream_rpc_method_handler(
+                    servicer.ReduceFn,
+                    request_deserializer=udfunction__pb2.DatumRequest.FromString,
+                    response_serializer=udfunction__pb2.DatumResponseList.SerializeToString,
+            ),
+            'IsReady': grpc.unary_unary_rpc_method_handler(
+                    servicer.IsReady,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=udfunction__pb2.ReadyResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "function.v1.UserDefinedFunction", rpc_method_handlers
-    )
+            'function.v1.UserDefinedFunction', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
-# This class is part of an EXPERIMENTAL API.
+ # This class is part of an EXPERIMENTAL API.
 class UserDefinedFunction(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def MapFn(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def MapFn(request,
             target,
-            "/function.v1.UserDefinedFunction/MapFn",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/function.v1.UserDefinedFunction/MapFn',
             udfunction__pb2.DatumRequest.SerializeToString,
             udfunction__pb2.DatumResponseList.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def MapStreamFn(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/function.v1.UserDefinedFunction/MapStreamFn',
+            udfunction__pb2.DatumRequest.SerializeToString,
+            udfunction__pb2.DatumResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def MapTFn(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def MapTFn(request,
             target,
-            "/function.v1.UserDefinedFunction/MapTFn",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/function.v1.UserDefinedFunction/MapTFn',
             udfunction__pb2.DatumRequest.SerializeToString,
             udfunction__pb2.DatumResponseList.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ReduceFn(
-        request_iterator,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.stream_stream(
-            request_iterator,
+    def ReduceFn(request_iterator,
             target,
-            "/function.v1.UserDefinedFunction/ReduceFn",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.stream_stream(request_iterator, target, '/function.v1.UserDefinedFunction/ReduceFn',
             udfunction__pb2.DatumRequest.SerializeToString,
             udfunction__pb2.DatumResponseList.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def IsReady(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def IsReady(request,
             target,
-            "/function.v1.UserDefinedFunction/IsReady",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/function.v1.UserDefinedFunction/IsReady',
             google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             udfunction__pb2.ReadyResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `pynumaflow-0.4.1/pynumaflow/function/server.py` & `pynumaflow-0.4.2/pynumaflow/function/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 import logging
 import multiprocessing
 import os
 from concurrent.futures import ThreadPoolExecutor
-from typing import Callable, AsyncIterable, List
+from typing import Callable
+from collections.abc import AsyncIterable
 
 import grpc
 from google.protobuf import empty_pb2 as _empty_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from pynumaflow.info.server import get_sdk_version, write as info_server_write
 from pynumaflow.info.types import ServerInfo, Protocol, Language, SERVER_INFO_FILE_PATH
 
 from pynumaflow import setup_logging
 from pynumaflow._constants import (
     FUNCTION_SOCK_PATH,
     MAX_MESSAGE_SIZE,
 )
-from pynumaflow.function import Messages, MessageTs, Datum, Metadata
+from pynumaflow.function import Message, Messages, MessageTs, Datum, Metadata
 from pynumaflow.function._dtypes import DatumMetadata
 from pynumaflow.function.proto import udfunction_pb2
 from pynumaflow.function.proto import udfunction_pb2_grpc
 from pynumaflow.types import NumaflowServicerContext
 
 _LOGGER = setup_logging(__name__)
 if os.getenv("PYTHONDEBUG"):
     _LOGGER.setLevel(logging.DEBUG)
 
-UDFMapCallable = Callable[[List[str], Datum], Messages]
-UDFMapTCallable = Callable[[List[str], Datum], MessageTs]
-UDFReduceCallable = Callable[[List[str], AsyncIterable[Datum], Metadata], Messages]
+UDFMapCallable = Callable[[list[str], Datum], Messages]
+UDFMapStreamCallable = Callable[[list[str], Datum], AsyncIterable[Message]]
+UDFMapTCallable = Callable[[list[str], Datum], MessageTs]
+UDFReduceCallable = Callable[[list[str], AsyncIterable[Datum], Metadata], Messages]
 _PROCESS_COUNT = multiprocessing.cpu_count()
 MAX_THREADS = int(os.getenv("MAX_THREADS", 0)) or (_PROCESS_COUNT * 4)
 
 
 class Server(udfunction_pb2_grpc.UserDefinedFunctionServicer):
     """
     Provides an interface to write a User Defined Function (UDFunction)
     which will be exposed over a Synchronous gRPC server.
 
     Args:
         map_handler: Function callable following the type signature of UDFMapCallable
+        map_stream_handler: Function callable following the type signature of UDFMapStreamCallable
         mapt_handler: Function callable following the type signature of UDFMapTCallable
         reduce_handler: Function callable following the type signature of UDFReduceCallable
         sock_path: Path to the UNIX Domain Socket
         max_message_size: The max message size in bytes the server can receive and send
         max_threads: The max number of threads to be spawned;
                      defaults to number of processors x4
 
@@ -54,14 +57,17 @@
     >>> def map_handler(key: [str], datum: Datum) -> Messages:
     ...   val = datum.value
     ...   _ = datum.event_time
     ...   _ = datum.watermark
     ...   messages = Messages(Message(val, keys=keys))
     ...   return messages
     ...
+    ... def map_stream_handler(key: [str], datums: Datum) -> AsyncIterable[Message]:
+    ...           "Not supported"
+    ...
     ... def reduce_handler(key: str, datums: Iterator[Datum], md: Metadata) -> Messages:
     ...           "Not supported"
     ...
     >>> def mapt_handler(key: [str], datum: Datum) -> MessageTs:
     ...   val = datum.value
     ...   new_event_time = datetime.time()
     ...   _ = datum.watermark
@@ -74,24 +80,28 @@
     ... )
     >>> grpc_server.start()
     """
 
     def __init__(
         self,
         map_handler: UDFMapCallable = None,
+        map_stream_handler: UDFMapStreamCallable = None,
         mapt_handler: UDFMapTCallable = None,
         reduce_handler: UDFReduceCallable = None,
         sock_path=FUNCTION_SOCK_PATH,
         max_message_size=MAX_MESSAGE_SIZE,
         max_threads=MAX_THREADS,
     ):
-        if not (map_handler or mapt_handler or reduce_handler):
-            raise ValueError("Require a valid map/mapt handler and/or a valid reduce handler.")
+        if not (map_handler or map_stream_handler or mapt_handler or reduce_handler):
+            raise ValueError(
+                "Require a valid map/mapstream/mapt handler and/or a valid reduce handler."
+            )
 
         self.__map_handler: UDFMapCallable = map_handler
+        self.__map_stream_handler: UDFMapStreamCallable = map_stream_handler
         self.__mapt_handler: UDFMapTCallable = mapt_handler
         self.__reduce_handler: UDFReduceCallable = reduce_handler
         self.sock_path = f"unix://{sock_path}"
         self._max_message_size = max_message_size
         self._max_threads = max_threads
         self.cleanup_coroutines = []
         # Collection for storing strong references to all running tasks.
@@ -131,21 +141,34 @@
             _LOGGER.critical("UDFError, re-raising the error: %r", err, exc_info=True)
             context.set_code(grpc.StatusCode.UNKNOWN)
             context.set_details(str(err))
             return udfunction_pb2.DatumResponseList(elements=[])
 
         datums = []
 
-        for msg in msgs.items():
+        for msg in msgs:
             datums.append(
                 udfunction_pb2.DatumResponse(keys=msg.keys, value=msg.value, tags=msg.tags)
             )
 
         return udfunction_pb2.DatumResponseList(elements=datums)
 
+    def MapStreamFn(
+        self,
+        request: udfunction_pb2.DatumRequest,
+        context: NumaflowServicerContext,
+    ) -> AsyncIterable[udfunction_pb2.DatumResponse]:
+        """
+        This method is not implemented because we return the messages
+        in a single stream.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        yield from ()
+
     def MapTFn(
         self, request: udfunction_pb2.DatumRequest, context: NumaflowServicerContext
     ) -> udfunction_pb2.DatumResponseList:
         """
         Applies a function to each datum element.
         The pascal case function name comes from the generated udfunction_pb2_grpc.py file.
         """
@@ -169,15 +192,15 @@
         except Exception as err:
             _LOGGER.critical("UDFError, re-raising the error: %r", err, exc_info=True)
             context.set_code(grpc.StatusCode.UNKNOWN)
             context.set_details(str(err))
             return udfunction_pb2.DatumResponseList(elements=[])
 
         datums = []
-        for msgt in msgts.items():
+        for msgt in msgts:
             event_time_timestamp = _timestamp_pb2.Timestamp()
             event_time_timestamp.FromDatetime(dt=msgt.event_time)
             watermark_timestamp = _timestamp_pb2.Timestamp()
             watermark_timestamp.FromDatetime(dt=request.watermark.watermark.ToDatetime())
             datums.append(
                 udfunction_pb2.DatumResponse(
                     keys=list(msgt.keys),
```

### Comparing `pynumaflow-0.4.1/pynumaflow/info/server.py` & `pynumaflow-0.4.2/pynumaflow/info/server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.1/pynumaflow/info/types.py` & `pynumaflow-0.4.2/pynumaflow/info/types.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.1/pynumaflow/sink/_dtypes.py` & `pynumaflow-0.4.2/pynumaflow/sink/_dtypes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,87 @@
 from dataclasses import dataclass
 from datetime import datetime
-from typing import List, TypeVar, Type, Optional
+from typing import TypeVar, Optional
+from collections.abc import Sequence, Iterator
+from warnings import warn
 
 R = TypeVar("R", bound="Response")
 Rs = TypeVar("Rs", bound="Responses")
 
 
-@dataclass(frozen=True)
+@dataclass
 class Response:
+    """
+    Basic datatype for UDSink response.
+
+    Args:
+        id: the id of the event.
+        success: boolean indicating whether the event was successfully processed.
+        err: error message if the event was not successfully processed.
+    """
+
     id: str
     success: bool
     err: Optional[str]
 
+    __slots__ = ("id", "success", "err")
+
     @classmethod
-    def as_success(cls: Type[R], id_: str) -> R:
+    def as_success(cls: type[R], id_: str) -> R:
         return Response(id=id_, success=True, err=None)
 
     @classmethod
-    def as_failure(cls: Type[R], id_: str, err_msg: str) -> R:
+    def as_failure(cls: type[R], id_: str, err_msg: str) -> R:
         return Response(id=id_, success=False, err=err_msg)
 
 
-class Responses:
+class Responses(Sequence[R]):
+    """
+    Container to hold a list of Response instances.
+
+    Args:
+        responses: list of Response instances.
+    """
+
+    __slots__ = ("_responses",)
+
     def __init__(self, *responses: R):
         self._responses = list(responses) or []
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self._responses)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return str(self)
 
+    def __len__(self) -> int:
+        return len(self._responses)
+
+    def __iter__(self) -> Iterator[R]:
+        return iter(self._responses)
+
+    def __getitem__(self, index: int) -> R:
+        if isinstance(index, slice):
+            raise TypeError("Slicing is not supported for Responses")
+        return self._responses[index]
+
     def append(self, response: R) -> None:
-        return self._responses.append(response)
+        self._responses.append(response)
 
-    def items(self) -> List[R]:
+    def items(self) -> list[R]:
+        warn(
+            "Using items is deprecated and will be removed in v0.5. "
+            "Iterate or index the Responses object instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         return self._responses
 
-    def dumps(self) -> str:
-        return str(self)
-
 
+@dataclass(init=False, repr=False)
 class Datum:
     """
     Class to define the important information for the event.
     Args:
         keys: the keys of the event.
         value: the payload of the event.
         event_time: the event time of the event.
@@ -56,17 +93,25 @@
     >>> t1 = datetime.fromtimestamp(1662998400, timezone.utc)
     >>> t2 = datetime.fromtimestamp(1662998460, timezone.utc)
     >>> msg_id = "test_id"
     >>> output_keys = ["test_key"]
     >>> d = Datum(keys=output_keys, sink_msg_id=msg_id, value=payload, event_time=t1, watermark=t2)
     """
 
+    __slots__ = ("_keys", "_id", "_value", "_event_time", "_watermark")
+
+    _keys: list[str]
+    _id: str
+    _value: bytes
+    _event_time: datetime
+    _watermark: datetime
+
     def __init__(
         self,
-        keys: List[str],
+        keys: list[str],
         sink_msg_id: str,
         value: bytes,
         event_time: datetime,
         watermark: datetime,
     ):
         self._keys = keys
         self._id = sink_msg_id or ""
@@ -92,15 +137,15 @@
 
     @property
     def id(self) -> str:
         """Returns the id of the event."""
         return self._id
 
     @property
-    def keys(self) -> List[str]:
+    def keys(self) -> list[str]:
         """Returns the keys of the event."""
         return self._keys
 
     @property
     def value(self) -> bytes:
         """Returns the value of the event."""
         return self._value
```

### Comparing `pynumaflow-0.4.1/pynumaflow/sink/_udfunction_pb2.pyi` & `pynumaflow-0.4.2/pynumaflow/sink/_udfunction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.1/pynumaflow/sink/async_sink.py` & `pynumaflow-0.4.2/pynumaflow/sink/async_sink.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import multiprocessing
 import os
-from typing import Callable, Iterator, AsyncIterable
+from collections.abc import AsyncIterable, Awaitable
+from typing import Callable
 
 import grpc
 from google.protobuf import empty_pb2 as _empty_pb2
 
 from pynumaflow import setup_logging
 from pynumaflow._constants import (
     SINK_SOCK_PATH,
@@ -17,15 +18,15 @@
 from pynumaflow.sink.proto import udsink_pb2_grpc, udsink_pb2
 from pynumaflow.types import NumaflowServicerContext
 
 _LOGGER = setup_logging(__name__)
 if os.getenv("PYTHONDEBUG"):
     _LOGGER.setLevel(logging.DEBUG)
 
-UDSinkCallable = Callable[[Iterator[Datum]], Responses]
+UDSinkCallable = Callable[[AsyncIterable[Datum]], Awaitable[Responses]]
 _PROCESS_COUNT = multiprocessing.cpu_count()
 MAX_THREADS = int(os.getenv("MAX_THREADS", 0)) or (_PROCESS_COUNT * 4)
 
 
 async def datum_generator(
     request_iterator: AsyncIterable[udsink_pb2.DatumRequest],
 ) -> AsyncIterable[Datum]:
@@ -49,15 +50,15 @@
         sink_handler: Function callable following the type signature of UDSinkCallable
         sock_path: Path to the UNIX Domain Socket
         max_message_size: The max message size in bytes the server can receive and send
         max_threads: The max number of threads to be spawned;
                      defaults to number of processors x 4
 
     Example invocation:
-    >>> from typing import List
+    >>> import aiorun
     >>> from pynumaflow.sink import Datum, Responses, Response, Sink
     >>> async def my_handler(datums: AsyncIterable[Datum]) -> Responses:
     ...   responses = Responses()
     ...   async for msg in datums:
     ...     responses.append(Response.as_success(msg.id))
     ...   return responses
     >>> grpc_server = AsyncSink(my_handler)
@@ -104,15 +105,15 @@
         except Exception as err:
             err_msg = "UDSinkError: %r" % err
             _LOGGER.critical(err_msg, exc_info=True)
             rspns = Responses()
             async for _datum in datum_iterator:
                 rspns.append(Response.as_failure(_datum.id, err_msg))
         responses = []
-        for rspn in rspns.items():
+        for rspn in rspns:
             responses.append(
                 udsink_pb2.Response(id=rspn.id, success=rspn.success, err_msg=rspn.err)
             )
         return responses
 
     async def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
```

### Comparing `pynumaflow-0.4.1/pynumaflow/sink/proto/udsink.proto` & `pynumaflow-0.4.2/pynumaflow/sink/proto/udsink.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.1/pynumaflow/sink/proto/udsink_pb2.py` & `pynumaflow-0.4.2/pynumaflow/sink/proto/udsink_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,41 +2,38 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: udsink.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x0cudsink.proto\x12\x07sink.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto";\n\tEventTime\x12.\n\nevent_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp":\n\tWatermark\x12-\n\twatermark\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp"\x86\x01\n\x0c\x44\x61tumRequest\x12\x0c\n\x04keys\x18\x01 \x03(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12&\n\nevent_time\x18\x03 \x01(\x0b\x32\x12.sink.v1.EventTime\x12%\n\twatermark\x18\x04 \x01(\x0b\x32\x12.sink.v1.Watermark\x12\n\n\x02id\x18\x05 \x01(\t"\x1e\n\rReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08"8\n\x08Response\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x0f\n\x07\x65rr_msg\x18\x03 \x01(\t"4\n\x0cResponseList\x12$\n\tresponses\x18\x01 \x03(\x0b\x32\x11.sink.v1.Response2\x86\x01\n\x0fUserDefinedSink\x12\x38\n\x06SinkFn\x12\x15.sink.v1.DatumRequest\x1a\x15.sink.v1.ResponseList(\x01\x12\x39\n\x07IsReady\x12\x16.google.protobuf.Empty\x1a\x16.sink.v1.ReadyResponseb\x06proto3'
-)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cudsink.proto\x12\x07sink.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\";\n\tEventTime\x12.\n\nevent_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\":\n\tWatermark\x12-\n\twatermark\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x86\x01\n\x0c\x44\x61tumRequest\x12\x0c\n\x04keys\x18\x01 \x03(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12&\n\nevent_time\x18\x03 \x01(\x0b\x32\x12.sink.v1.EventTime\x12%\n\twatermark\x18\x04 \x01(\x0b\x32\x12.sink.v1.Watermark\x12\n\n\x02id\x18\x05 \x01(\t\"\x1e\n\rReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\"8\n\x08Response\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x0f\n\x07\x65rr_msg\x18\x03 \x01(\t\"4\n\x0cResponseList\x12$\n\tresponses\x18\x01 \x03(\x0b\x32\x11.sink.v1.Response2\x86\x01\n\x0fUserDefinedSink\x12\x38\n\x06SinkFn\x12\x15.sink.v1.DatumRequest\x1a\x15.sink.v1.ResponseList(\x01\x12\x39\n\x07IsReady\x12\x16.google.protobuf.Empty\x1a\x16.sink.v1.ReadyResponseb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "udsink_pb2", globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'udsink_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
-    DESCRIPTOR._options = None
-    _EVENTTIME._serialized_start = 87
-    _EVENTTIME._serialized_end = 146
-    _WATERMARK._serialized_start = 148
-    _WATERMARK._serialized_end = 206
-    _DATUMREQUEST._serialized_start = 209
-    _DATUMREQUEST._serialized_end = 343
-    _READYRESPONSE._serialized_start = 345
-    _READYRESPONSE._serialized_end = 375
-    _RESPONSE._serialized_start = 377
-    _RESPONSE._serialized_end = 433
-    _RESPONSELIST._serialized_start = 435
-    _RESPONSELIST._serialized_end = 487
-    _USERDEFINEDSINK._serialized_start = 490
-    _USERDEFINEDSINK._serialized_end = 624
+  DESCRIPTOR._options = None
+  _EVENTTIME._serialized_start=87
+  _EVENTTIME._serialized_end=146
+  _WATERMARK._serialized_start=148
+  _WATERMARK._serialized_end=206
+  _DATUMREQUEST._serialized_start=209
+  _DATUMREQUEST._serialized_end=343
+  _READYRESPONSE._serialized_start=345
+  _READYRESPONSE._serialized_end=375
+  _RESPONSE._serialized_start=377
+  _RESPONSE._serialized_end=433
+  _RESPONSELIST._serialized_start=435
+  _RESPONSELIST._serialized_end=487
+  _USERDEFINEDSINK._serialized_start=490
+  _USERDEFINEDSINK._serialized_end=624
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pynumaflow-0.4.1/pynumaflow/sink/proto/udsink_pb2_grpc.py` & `pynumaflow-0.4.2/pynumaflow/sink/proto/udsink_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,114 +12,91 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.SinkFn = channel.stream_unary(
-            "/sink.v1.UserDefinedSink/SinkFn",
-            request_serializer=udsink__pb2.DatumRequest.SerializeToString,
-            response_deserializer=udsink__pb2.ResponseList.FromString,
-        )
+                '/sink.v1.UserDefinedSink/SinkFn',
+                request_serializer=udsink__pb2.DatumRequest.SerializeToString,
+                response_deserializer=udsink__pb2.ResponseList.FromString,
+                )
         self.IsReady = channel.unary_unary(
-            "/sink.v1.UserDefinedSink/IsReady",
-            request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            response_deserializer=udsink__pb2.ReadyResponse.FromString,
-        )
+                '/sink.v1.UserDefinedSink/IsReady',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=udsink__pb2.ReadyResponse.FromString,
+                )
 
 
 class UserDefinedSinkServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def SinkFn(self, request_iterator, context):
-        """SinkFn writes the Datum to a user defined sink."""
+        """SinkFn writes the Datum to a user defined sink.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def IsReady(self, request, context):
-        """IsReady is the heartbeat endpoint for gRPC."""
+        """IsReady is the heartbeat endpoint for gRPC.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
 
 def add_UserDefinedSinkServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "SinkFn": grpc.stream_unary_rpc_method_handler(
-            servicer.SinkFn,
-            request_deserializer=udsink__pb2.DatumRequest.FromString,
-            response_serializer=udsink__pb2.ResponseList.SerializeToString,
-        ),
-        "IsReady": grpc.unary_unary_rpc_method_handler(
-            servicer.IsReady,
-            request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-            response_serializer=udsink__pb2.ReadyResponse.SerializeToString,
-        ),
+            'SinkFn': grpc.stream_unary_rpc_method_handler(
+                    servicer.SinkFn,
+                    request_deserializer=udsink__pb2.DatumRequest.FromString,
+                    response_serializer=udsink__pb2.ResponseList.SerializeToString,
+            ),
+            'IsReady': grpc.unary_unary_rpc_method_handler(
+                    servicer.IsReady,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=udsink__pb2.ReadyResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "sink.v1.UserDefinedSink", rpc_method_handlers
-    )
+            'sink.v1.UserDefinedSink', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
-# This class is part of an EXPERIMENTAL API.
+ # This class is part of an EXPERIMENTAL API.
 class UserDefinedSink(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def SinkFn(
-        request_iterator,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.stream_unary(
-            request_iterator,
+    def SinkFn(request_iterator,
             target,
-            "/sink.v1.UserDefinedSink/SinkFn",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.stream_unary(request_iterator, target, '/sink.v1.UserDefinedSink/SinkFn',
             udsink__pb2.DatumRequest.SerializeToString,
             udsink__pb2.ResponseList.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def IsReady(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def IsReady(request,
             target,
-            "/sink.v1.UserDefinedSink/IsReady",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/sink.v1.UserDefinedSink/IsReady',
             google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             udsink__pb2.ReadyResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `pynumaflow-0.4.1/pynumaflow/sink/server.py` & `pynumaflow-0.4.2/pynumaflow/sink/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import multiprocessing
 import os
 from concurrent.futures import ThreadPoolExecutor
-from typing import Callable, Iterator, Iterable
+from typing import Callable
+from collections.abc import Iterator, Iterable
 
 import grpc
 from google.protobuf import empty_pb2 as _empty_pb2
 
 from pynumaflow import setup_logging
 from pynumaflow._constants import (
     SINK_SOCK_PATH,
@@ -96,15 +97,15 @@
             err_msg = "UDSinkError: %r" % err
             _LOGGER.critical(err_msg, exc_info=True)
             rspns = Responses()
             for _datum in datum_iterator:
                 rspns.append(Response.as_failure(_datum.id, err_msg))
 
         responses = []
-        for rspn in rspns.items():
+        for rspn in rspns:
             responses.append(
                 udsink_pb2.Response(id=rspn.id, success=rspn.success, err_msg=rspn.err)
             )
 
         return udsink_pb2.ResponseList(responses=responses)
 
     def IsReady(
```

### Comparing `pynumaflow-0.4.1/pyproject.toml` & `pynumaflow-0.4.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynumaflow"
-version = "0.4.1"
+version = "0.4.2"
 description = "Provides the interfaces of writing Python User Defined Functions and Sinks for NumaFlow."
 authors = ["NumaFlow Developers"]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Vigith Maurice <vigith@gmail.com>",
@@ -22,31 +22,34 @@
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 grpcio = "^1.48.1"
 grpcio-tools = "^1.48.1"
 google-cloud = "^0.34.0"
 google-api-core = "^2.11.0"
 protobuf = ">=3.20,<5.0"
+aiorun = "^2022.11.1"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^3.0"
-black = "^22.1"
+black = "^23.1"
 grpcio-testing = "^1.48.1"
-flake8 = "^4.0.1"
+ruff = "^0.0.264"
+pre-commit = "^3.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
+target-version = ["py39"]
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
@@ -54,9 +57,24 @@
   | \.venv
   | \.idea
   | _build
   | buck-out
   | build
   | dist
   | tests/.*/setup.py
+  | function/proto
+  | sink/proto
 )/
 '''
+
+[tool.ruff]
+line-length = 100
+src = ["pynumaflow", "tests", "examples"]
+select = ["E", "F", "UP"]
+target-version = "py39"
+show-fixes = true
+show-source = true
+extend-exclude = [
+    "*_pb2.py",
+    "*_pb2*.py",
+    "*.pyi"
+]
```

### Comparing `pynumaflow-0.4.1/PKG-INFO` & `pynumaflow-0.4.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,102 @@
-Metadata-Version: 2.1
-Name: pynumaflow
-Version: 0.4.1
-Summary: Provides the interfaces of writing Python User Defined Functions and Sinks for NumaFlow.
-Home-page: https://github.com/numaproj/numaflow-python
-License: Apache-2.0
-Author: NumaFlow Developers
-Maintainer: Avik Basu
-Maintainer-email: avikbasu93@gmail.com
-Requires-Python: >=3.9,<3.12
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: google-api-core (>=2.11.0,<3.0.0)
-Requires-Dist: google-cloud (>=0.34.0,<0.35.0)
-Requires-Dist: grpcio (>=1.48.1,<2.0.0)
-Requires-Dist: grpcio-tools (>=1.48.1,<2.0.0)
-Requires-Dist: protobuf (>=3.20,<5.0)
-Project-URL: Repository, https://github.com/numaproj/numaflow-python
-Description-Content-Type: text/markdown
-
 # Python SDK for Numaflow
 
-This SDK provides the interface for writing [UDFs](https://numaflow.numaproj.io/user-guide/user-defined-functions/user-defined-functions/) 
+[![Build](https://github.com/numaproj/numaflow-python/actions/workflows/ci.yml/badge.svg)](https://github.com/numaproj/numaflow-python/actions/workflows/ci.yml)
+[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
+[![Release Version](https://img.shields.io/github/v/release/numaproj/numaflow-python?label=pynumaflow)](https://github.com/numaproj/numaflow-python/releases/latest)
+
+
+This SDK provides the interface for writing [UDFs](https://numaflow.numaproj.io/user-guide/user-defined-functions/user-defined-functions/)
 and [UDSinks](https://numaflow.numaproj.io/user-guide/sinks/user-defined-sinks/) in Python.
 
+## Installation
+
+Install the package using pip.
+```bash
+pip install pynumaflow
+```
+
+### Build locally
+
+This project uses [Poetry](https://python-poetry.org/) for dependency management and packaging.
+To build the package locally, run the following command from the root of the project.
+
+```bash
+make setup
+````
+
+To run unit tests:
+```bash
+make test
+```
+
+To format code style using black and ruff:
+```bash
+make lint
+```
+
+Setup [pre-commit](https://pre-commit.com/) hooks:
+```bash
+pre-commit install
+```
+
 ## Implement a User Defined Function (UDF)
 
 
 ### Map
 
 ```python
 from pynumaflow.function import Messages, Message, Datum, Server
-from typing import List
 
 
-def my_handler(keys: List[str], datum: Datum) -> Messages:
+def my_handler(keys: list[str], datum: Datum) -> Messages:
     val = datum.value
     _ = datum.event_time
     _ = datum.watermark
-    messages = Messages(Message(value=val, keys=keys))
-    return messages
+    return Messages(Message(value=val, keys=keys))
 
 
 if __name__ == "__main__":
     grpc_server = Server(map_handler=my_handler)
     grpc_server.start()
 ```
 ### MapT - Map with event time assignment capability
 In addition to the regular Map function, MapT supports assigning a new event time to the message.
 MapT is only supported at source vertex to enable (a) early data filtering and (b) watermark assignment by extracting new event time from the message payload.
 
 ```python
-import datetime
+from datetime import datetime
 from pynumaflow.function import MessageTs, MessageT, Datum, Server
-from typing import List
 
 
-def mapt_handler(keys: List[str], datum: Datum) -> MessageTs:
+def mapt_handler(keys: list[str], datum: Datum) -> MessageTs:
     val = datum.value
-    new_event_time = datetime.time()
+    new_event_time = datetime.now()
     _ = datum.watermark
-    message_t_s = MessageTs(MessageT(new_event_time, val, keys))
+    message_t_s = MessageTs(MessageT(val, event_time=new_event_time, keys=keys))
     return message_t_s
 
 
 if __name__ == "__main__":
     grpc_server = Server(mapt_handler=mapt_handler)
     grpc_server.start()
 ```
 
 ### Reduce
 
 ```python
 import aiorun
-import asyncio
 from typing import Iterator, List
 from pynumaflow.function import Messages, Message, Datum, Metadata, AsyncServer
 
 
-async def my_handler(keys: List[str], datums: Iterator[Datum], md: Metadata) -> Messages:
+async def my_handler(
+    keys: List[str], datums: Iterator[Datum], md: Metadata
+) -> Messages:
     interval_window = md.interval_window
     counter = 0
     async for _ in datums:
         counter += 1
     msg = (
         f"counter:{counter} interval_window_start:{interval_window.start} "
         f"interval_window_end:{interval_window.end}"
@@ -99,15 +106,15 @@
 
 if __name__ == "__main__":
     grpc_server = AsyncServer(reduce_handler=my_handler)
     aiorun.run(grpc_server.start())
 ```
 
 ### Sample Image
-A sample UDF [Dockerfile](examples/function/forward_message/Dockerfile) is provided 
+A sample UDF [Dockerfile](examples/function/forward_message/Dockerfile) is provided
 under [examples](examples/function/forward_message).
 
 ## Implement a User Defined Sink (UDSink)
 
 ```python
 from typing import Iterator
 from pynumaflow.sink import Datum, Responses, Response, Sink
@@ -124,22 +131,24 @@
 if __name__ == "__main__":
     grpc_server = Sink(my_handler)
     grpc_server.start()
 ```
 
 ### Sample Image
 
-A sample UDSink [Dockerfile](examples/sink/log/Dockerfile) is provided 
+A sample UDSink [Dockerfile](examples/sink/log/Dockerfile) is provided
 under [examples](examples/sink/log).
 
 ### Datum Metadata
 The Datum object contains the message payload and metadata. Currently, there are two fields
 in metadata: the message ID, the message delivery count to indicate how many times the message
 has been delivered. You can use these metadata to implement customized logic. For example,
 ```python
 ...
-def my_handler(keys: List[str], datum: Datum) -> Messages:
+
+
+def my_handler(keys: list[str], datum: Datum) -> Messages:
     num_delivered = datum.metadata.num_delivered
     # Choose to do specific actions, if the message delivery count reaches a certain threshold.
     if num_delivered > 3:
         ...
 ```
```

