# Comparing `tmp/zarrita-0.1.0a1.tar.gz` & `tmp/zarrita-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zarrita-0.1.0a1.tar", max compression
+gzip compressed data, was "zarrita-0.1.0a2.tar", max compression
```

## Comparing `zarrita-0.1.0a1.tar` & `zarrita-0.1.0a2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0     1105 2023-03-06 16:02:23.937960 zarrita-0.1.0a1/LICENSE
--rw-r--r--   0        0        0     2103 2023-03-06 15:57:36.388340 zarrita-0.1.0a1/README.md
--rw-r--r--   0        0        0      629 2023-03-10 15:53:07.138443 zarrita-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      135 2023-03-06 16:01:03.028793 zarrita-0.1.0a1/zarrita/__init__.py
--rw-r--r--   0        0        0    12166 2023-03-10 12:04:44.774824 zarrita-0.1.0a1/zarrita/array.py
--rw-r--r--   0        0        0     7013 2023-03-05 20:03:10.242773 zarrita-0.1.0a1/zarrita/codecs.py
--rw-r--r--   0        0        0     3559 2023-03-05 20:05:00.664843 zarrita-0.1.0a1/zarrita/common.py
--rw-r--r--   0        0        0     2716 2023-03-05 19:55:08.658268 zarrita-0.1.0a1/zarrita/group.py
--rw-r--r--   0        0        0     7254 2023-03-03 16:58:40.122249 zarrita-0.1.0a1/zarrita/indexing.py
--rw-r--r--   0        0        0    13863 2023-03-06 09:19:12.102017 zarrita-0.1.0a1/zarrita/sharding.py
--rw-r--r--   0        0        0     2684 2023-03-04 20:49:46.369189 zarrita-0.1.0a1/zarrita/store.py
--rw-r--r--   0        0        0     4385 2023-03-04 20:49:23.924576 zarrita-0.1.0a1/zarrita/value_handle.py
--rw-r--r--   0        0        0     2891 1970-01-01 00:00:00.000000 zarrita-0.1.0a1/setup.py
--rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 zarrita-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-05-09 09:12:03.956626 zarrita-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0     2741 2023-06-08 08:07:06.094114 zarrita-0.1.0a2/README.md
+-rw-r--r--   0        0        0      696 2023-06-08 08:07:52.106498 zarrita-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1085 2023-06-07 11:49:09.452172 zarrita-0.1.0a2/zarrita/__init__.py
+-rw-r--r--   0        0        0    19595 2023-06-07 19:18:11.589026 zarrita-0.1.0a2/zarrita/array.py
+-rw-r--r--   0        0        0    13242 2023-06-07 20:04:03.128152 zarrita-0.1.0a2/zarrita/array_v2.py
+-rw-r--r--   0        0        0    12285 2023-06-08 07:24:44.647554 zarrita-0.1.0a2/zarrita/codecs.py
+-rw-r--r--   0        0        0     4314 2023-06-07 20:03:42.377098 zarrita-0.1.0a2/zarrita/common.py
+-rw-r--r--   0        0        0     4181 2023-06-07 15:17:15.193840 zarrita-0.1.0a2/zarrita/group.py
+-rw-r--r--   0        0        0     4735 2023-06-07 15:17:10.125767 zarrita-0.1.0a2/zarrita/group_v2.py
+-rw-r--r--   0        0        0     7259 2023-06-07 12:49:15.942016 zarrita-0.1.0a2/zarrita/indexing.py
+-rw-r--r--   0        0        0     5374 2023-06-08 07:17:39.694424 zarrita-0.1.0a2/zarrita/metadata.py
+-rw-r--r--   0        0        0    20531 2023-06-07 18:32:25.846759 zarrita-0.1.0a2/zarrita/sharding.py
+-rw-r--r--   0        0        0     5391 2023-06-07 20:04:34.652580 zarrita-0.1.0a2/zarrita/store.py
+-rw-r--r--   0        0        0     2555 2023-06-02 09:33:41.528984 zarrita-0.1.0a2/zarrita/sync.py
+-rw-r--r--   0        0        0     3827 2023-06-06 13:35:33.794530 zarrita-0.1.0a2/zarrita/value_handle.py
+-rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 zarrita-0.1.0a2/PKG-INFO
```

### Comparing `zarrita-0.1.0a1/LICENSE` & `zarrita-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a1/README.md` & `zarrita-0.1.0a2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -10,76 +10,99 @@
 
 store = zarrita.FileSystemStore('file://./testdata')
 ```
 
 ## Create an array
 
 ```python
-a = zarrita.Array.create(
+a = await zarrita.Array.create_async(
     store,
     'array',
     shape=(6, 10),
     dtype='int32',
     chunk_shape=(2, 5),
     codecs=[zarrita.codecs.gzip_codec(level=1)],
     attributes={'question': 'life', 'answer': 42}
 )
-a[:, :] = np.ones((6, 10), dtype='int32')
+await a.async_[:, :].set(np.ones((6, 10), dtype='int32'))
 ```
 
 ## Open an array
 
 ```python
-a = zarrita.Array.open(store, 'array')
-assert np.array_equal(a[:, :], np.ones((6, 10), dtype='int32'))
+a = await zarrita.Array.open_async(store, 'array')
+assert np.array_equal(await a.async_[:, :].get(), np.ones((6, 10), dtype='int32'))
 ```
 
 ## Create an array with sharding
 
 ```python
-a = zarrita.Array.create(
+a = await zarrita.Array.create_async(
     store,
     'sharding',
     shape=(16, 16),
     dtype='int32',
     chunk_shape=(16, 16),
     chunk_key_encoding=('v2', '.'),
     codecs=[
         zarrita.codecs.sharding_codec(
             chunk_shape=(8, 8),
             codecs=[zarrita.codecs.gzip_codec(level=1)]
         ),
     ],
 )
 data = np.arange(0, 16 * 16, dtype='int32').reshape((16, 16))
-a[:, :] = data
-assert np.array_equal(a[:, :], data)
+await a.async_[:, :].set(data)
+assert np.array_equal(await a.async_[:, :].get(), data)
 ```
 
 ## Create a group
 
 ```python
-g = zarrita.Group.create(store, 'group')
-g2 = g.create_group('group2')
-a = g2.create_array(
+g = await zarrita.Group.create_async(store, 'group')
+g2 = await g.create_group_async('group2')
+a = await g2.create_array_async(
     'array',
     shape=(16, 16),
     dtype='int32',
     chunk_shape=(16, 16),
 )
-a[:, :] = np.arange(0, 16 * 16, dtype='int32').reshape((16, 16))
+await a.async_[:, :].set(np.arange(0, 16 * 16, dtype='int32').reshape((16, 16)))
 ```
 
 ## Open a group
 
 ```python
-g = zarrita.Group.open(store, 'group')
+g = await zarrita.Group.open_async(store, 'group')
 g2 = g['group2']
 a = g['group2/array']
-assert np.array_equal(a[:, :], np.arange(0, 16 * 16, dtype='int32').reshape((16, 16)))
+assert np.array_equal(await a.asnyc_[:, :].get(), np.arange(0, 16 * 16, dtype='int32').reshape((16, 16)))
 ```
 
 # Credits
 
 This is a largely-rewritten fork of `zarrita` by [@alimanfoo](https://github.com/alimanfoo). It implements the Zarr v3 draft specification created by [@alimanfoo](https://github.com/alimanfoo), [@jstriebel](https://github.com/jstriebel), [@jbms](https://github.com/jbms) et al.
 
 Licensed under MIT
+
+# TODO
+
+- [x] Async
+- [x] sharding partial decode
+- [x] variable renaming
+- [x] type indexing
+- [x] value handle slices get and set
+- [x] codec classes
+- [x] metadata validation
+- [x] zarr v2
+- [x] open with v2/v3 auto-detect
+- [x] async gather in sharding
+- [x] async local store
+- [x] resize arrays
+- [x] check empty before create array
+- [ ] morton order in indexing
+- [ ] attrs -> dataclasses
+
+## Non-priority
+
+- Dask support
+- Buffer protocol
```

### Comparing `zarrita-0.1.0a1/pyproject.toml` & `zarrita-0.1.0a2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 [tool.poetry]
 name = "zarrita"
-version = "0.1.0a1"
+version = "0.1.0a2"
 description = ""
 authors = ["Norman Rzepka <code@normanrz.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 fsspec = "^2022.2.0"
 numpy = "^1.24.2"
 numcodecs = "^0.10.0"
 cattrs = "^22.2.0"
 attrs = "^22.2.0"
+crc32c = "^2.3.post0"
 
 [tool.poetry.group.dev.dependencies]
 webknossos = "^0.12.3"
 pytest = "^7.2.1"
 black = "^23.1.0"
 mypy = "^1.0.1"
 isort = "^5.12.0"
 pudb = "^2022.1.3"
 zarr = "^2.14.2"
+pytest-asyncio = "^0.21.0"
+ruff = "^0.0.271"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `zarrita-0.1.0a1/zarrita/array.py` & `zarrita-0.1.0a2/zarrita/codecs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,380 +1,411 @@
-import json
-from enum import Enum
-from typing import Any, Dict, Iterable, List, Literal, Optional, Tuple, Union
+from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING, Awaitable, Callable, List, Literal, Tuple, Union
 
 import numpy as np
-from attr import asdict, field, frozen
+from attr import asdict, frozen
+from numcodecs.blosc import Blosc
+from numcodecs.gzip import GZip
+
+from zarrita.common import BytesLike, to_thread
+from zarrita.metadata import (
+    BloscCodecConfigurationMetadata,
+    BloscCodecMetadata,
+    CodecMetadata,
+    EndianCodecConfigurationMetadata,
+    EndianCodecMetadata,
+    GzipCodecConfigurationMetadata,
+    GzipCodecMetadata,
+    ShardingCodecConfigurationMetadata,
+    ShardingCodecMetadata,
+    TransposeCodecConfigurationMetadata,
+    TransposeCodecMetadata,
+    data_type_to_numpy,
+)
+from zarrita.value_handle import (
+    ArrayValueHandle,
+    BufferValueHandle,
+    NoneValueHandle,
+    ValueHandle,
+)
+
+if TYPE_CHECKING:
+    from zarrita.array import CoreArrayMetadata
+
+
+async def _needs_array(
+    chunk_value_handle: ValueHandle,
+    array_metadata: "CoreArrayMetadata",
+    f: Callable[
+        [np.ndarray, "CoreArrayMetadata"], Awaitable[Union[None, np.ndarray, BytesLike]]
+    ],
+):
+    chunk_array = await chunk_value_handle.toarray()
+    if chunk_array is None:
+        return NoneValueHandle()
+    chunk_array = chunk_array.view(dtype=array_metadata.dtype)
+    result = await f(chunk_array, array_metadata)
+    if result is None:
+        return NoneValueHandle()
+    elif (
+        isinstance(result, bytes)
+        or isinstance(result, bytearray)
+        or isinstance(result, memoryview)
+    ):
+        return BufferValueHandle(result)
+    elif isinstance(result, np.ndarray):
+        return ArrayValueHandle(result)
+
+
+async def _needs_bytes(
+    chunk_value_handle: ValueHandle,
+    array_metadata: "CoreArrayMetadata",
+    f: Callable[
+        [BytesLike, "CoreArrayMetadata"], Awaitable[Union[None, np.ndarray, BytesLike]]
+    ],
+):
+    chunk_bytes = await chunk_value_handle.tobytes()
+    if chunk_bytes is None:
+        return NoneValueHandle()
+    result = await f(chunk_bytes, array_metadata)
+    if result is None:
+        return NoneValueHandle()
+    elif (
+        isinstance(result, bytes)
+        or isinstance(result, bytearray)
+        or isinstance(result, memoryview)
+    ):
+        return BufferValueHandle(result)
+    elif isinstance(result, np.ndarray):
+        return ArrayValueHandle(result)
+
+
+class Codec(ABC):
+    supports_partial_decode: bool
+    supports_partial_encode: bool
+    input_type: Literal["bytes", "array"]
+    output_type: Literal["bytes", "array"]
+
+    @abstractmethod
+    async def decode(
+        self,
+        chunk_value_handle: ValueHandle,
+        array_metadata: "CoreArrayMetadata",
+    ) -> ValueHandle:
+        pass
+
+    @abstractmethod
+    async def encode(
+        self,
+        chunk_value_handle: ValueHandle,
+        array_metadata: "CoreArrayMetadata",
+    ) -> ValueHandle:
+        pass
+
+    @staticmethod
+    def codecs_from_metadata(codecs_metadata: List["CodecMetadata"]) -> List["Codec"]:
+        out: List[Codec] = []
+        for codec_metadata in codecs_metadata:
+            if codec_metadata.name == "blosc":
+                out.append(BloscCodec.from_metadata(codec_metadata))
+            elif codec_metadata.name == "gzip":
+                out.append(GzipCodec.from_metadata(codec_metadata))
+            elif codec_metadata.name == "transpose":
+                out.append(TransposeCodec.from_metadata(codec_metadata))
+            elif codec_metadata.name == "endian":
+                out.append(EndianCodec.from_metadata(codec_metadata))
+            elif codec_metadata.name == "sharding_indexed":
+                from zarrita.sharding import ShardingCodec
 
-from zarrita.codecs import CodecMetadata
-from zarrita.common import ZARR_JSON, get_order, is_total_slice, make_cattr
-from zarrita.indexing import BasicIndexer
-from zarrita.store import Store
-from zarrita.value_handle import ArrayHandle, FileHandle, NoneHandle, ValueHandle
-
-
-class DataType(Enum):
-    bool = "bool"
-    int8 = "int8"
-    int16 = "int16"
-    int32 = "int32"
-    int64 = "int64"
-    uint8 = "uint8"
-    uint16 = "uint16"
-    uint32 = "uint32"
-    uint64 = "uint64"
-    float32 = "float32"
-    float64 = "float64"
-
-
-dtype_to_data_type = {
-    "bool": "bool",
-    "|i1": "int8",
-    "<i2": "int16",
-    "<i4": "int32",
-    "<i8": "int64",
-    "|u1": "uint8",
-    "<u2": "uint16",
-    "<u4": "uint32",
-    "<u8": "uint64",
-    "<f4": "float32",
-    "<f8": "float64",
-}
+                out.append(ShardingCodec.from_metadata(codec_metadata))
+            else:
+                raise RuntimeError(f"Unsupported codec: {codec_metadata}")
+        return out
 
 
-@frozen
-class RegularChunkGridConfigurationMetadata:
-    chunk_shape: Tuple[int, ...]
+class ArrayArrayCodec(Codec):
+    input_type = "array"
+    output_type = "array"
+
+    async def decode(
+        self,
+        chunk_value_handle: ValueHandle,
+        array_metadata: "CoreArrayMetadata",
+    ) -> ValueHandle:
+        return await _needs_array(chunk_value_handle, array_metadata, self.inner_decode)
+
+    @abstractmethod
+    async def inner_decode(
+        self,
+        chunk_array: np.ndarray,
+        array_metadata: "CoreArrayMetadata",
+    ) -> np.ndarray:
+        pass
+
+    async def encode(
+        self,
+        chunk_value_handle: ValueHandle,
+        array_metadata: "CoreArrayMetadata",
+    ) -> ValueHandle:
+        return await _needs_array(chunk_value_handle, array_metadata, self.inner_encode)
+
+    @abstractmethod
+    async def inner_encode(
+        self,
+        chunk_array: np.ndarray,
+        array_metadata: "CoreArrayMetadata",
+    ) -> np.ndarray:
+        pass
+
+
+class ArrayBytesCodec(Codec):
+    input_type = "array"
+    output_type = "bytes"
+
+    async def decode(
+        self,
+        chunk_value_handle: ValueHandle,
+        array_metadata: "CoreArrayMetadata",
+    ) -> ValueHandle:
+        return await _needs_bytes(chunk_value_handle, array_metadata, self.inner_decode)
+
+    @abstractmethod
+    async def inner_decode(
+        self,
+        chunk_array: BytesLike,
+        array_metadata: "CoreArrayMetadata",
+    ) -> np.ndarray:
+        pass
+
+    async def encode(
+        self,
+        chunk_value_handle: ValueHandle,
+        array_metadata: "CoreArrayMetadata",
+    ) -> ValueHandle:
+        return await _needs_array(chunk_value_handle, array_metadata, self.inner_encode)
+
+    @abstractmethod
+    async def inner_encode(
+        self,
+        chunk_array: np.ndarray,
+        array_metadata: "CoreArrayMetadata",
+    ) -> BytesLike:
+        pass
+
+
+class BytesBytesCodec(Codec):
+    input_type = "bytes"
+    output_type = "bytes"
+
+    async def decode(
+        self,
+        chunk_value_handle: ValueHandle,
+        array_metadata: "CoreArrayMetadata",
+    ) -> ValueHandle:
+        return await _needs_bytes(chunk_value_handle, array_metadata, self.inner_decode)
+
+    @abstractmethod
+    async def inner_decode(
+        self,
+        chunk_array: BytesLike,
+        array_metadata: "CoreArrayMetadata",
+    ) -> BytesLike:
+        pass
+
+    async def encode(
+        self,
+        chunk_value_handle: ValueHandle,
+        array_metadata: "CoreArrayMetadata",
+    ) -> ValueHandle:
+        return await _needs_bytes(chunk_value_handle, array_metadata, self.inner_encode)
+
+    @abstractmethod
+    async def inner_encode(
+        self,
+        chunk_array: BytesLike,
+        array_metadata: "CoreArrayMetadata",
+    ) -> BytesLike:
+        pass
 
 
 @frozen
-class RegularChunkGridMetadata:
-    configuration: RegularChunkGridConfigurationMetadata
-    name: Literal["regular"] = "regular"
+class BloscCodec(BytesBytesCodec):
+    configuration: BloscCodecConfigurationMetadata
 
+    @classmethod
+    def from_metadata(cls, codec_metadata: BloscCodecMetadata) -> "BloscCodec":
+        return cls(
+            configuration=codec_metadata.configuration,
+        )
 
-@frozen
-class DefaultChunkKeyEncodingConfigurationMetadata:
-    separator: Literal[".", "/"] = "/"
+    def _get_blosc_codec(self):
+        config_dict = asdict(self.configuration)
+        map_shuffle_str_to_int = {"noshuffle": 0, "shuffle": 1, "bitshuffle": 2}
+        config_dict["shuffle"] = map_shuffle_str_to_int[config_dict["shuffle"]]
+        return Blosc.from_config(config_dict)
+
+    async def inner_decode(
+        self,
+        chunk_bytes: bytes,
+        _array_metadata: "CoreArrayMetadata",
+    ) -> BytesLike:
+        return await to_thread(self._get_blosc_codec().decode, chunk_bytes)
+
+    async def inner_encode(
+        self,
+        chunk_bytes: bytes,
+        array_metadata: "CoreArrayMetadata",
+    ) -> BytesLike:
+        chunk_array = np.frombuffer(chunk_bytes, dtype=array_metadata.dtype)
+        return await to_thread(self._get_blosc_codec().encode, chunk_array)
 
 
 @frozen
-class DefaultChunkKeyEncodingMetadata:
-    configuration: DefaultChunkKeyEncodingConfigurationMetadata = (
-        DefaultChunkKeyEncodingConfigurationMetadata()
-    )
-    name: Literal["default"] = "default"
+class EndianCodec(ArrayBytesCodec):
+    configuration: EndianCodecConfigurationMetadata
 
-    def decode_chunk_key(self, chunk_key: str) -> Tuple[int, ...]:
-        if chunk_key == "c":
-            return ()
-        return tuple(map(int, chunk_key[1:].split(self.configuration.separator)))
+    @classmethod
+    def from_metadata(cls, codec_metadata: EndianCodecMetadata) -> "EndianCodec":
+        return cls(
+            configuration=codec_metadata.configuration,
+        )
 
-    def encode_chunk_key(self, chunk_coords: Tuple[int, ...]) -> str:
-        return self.configuration.separator.join(map(str, ("c",) + chunk_coords))
+    def _get_byteorder(self, array: np.ndarray) -> Literal["big", "little"]:
+        if array.dtype.byteorder == "<":
+            return "little"
+        elif array.dtype.byteorder == ">":
+            return "big"
+        else:
+            import sys
 
+            return sys.byteorder
 
-@frozen
-class V2ChunkKeyEncodingConfigurationMetadata:
-    separator: Literal[".", "/"] = "."
+    async def inner_decode(
+        self,
+        chunk_bytes: BytesLike,
+        array_metadata: "CoreArrayMetadata",
+    ) -> np.ndarray:
+        if self.configuration.endian == "little":
+            prefix = "<"
+        else:
+            prefix = ">"
+        dtype = np.dtype(f"{prefix}{data_type_to_numpy[array_metadata.data_type]}")
+        chunk_array = np.frombuffer(chunk_bytes, dtype)
+        return chunk_array
+
+    async def inner_encode(
+        self,
+        chunk_array: np.ndarray,
+        _array_metadata: "CoreArrayMetadata",
+    ) -> BytesLike:
+        byteorder = self._get_byteorder(chunk_array)
+        if self.configuration.endian != byteorder:
+            chunk_array = chunk_array.astype(
+                dtype=chunk_array.dtype.newbyteorder(byteorder)
+            )
+        return chunk_array.tobytes()
 
 
 @frozen
-class V2ChunkKeyEncodingMetadata:
-    configuration: V2ChunkKeyEncodingConfigurationMetadata = (
-        V2ChunkKeyEncodingConfigurationMetadata()
-    )
-    name: Literal["v2"] = "v2"
-
-    def decode_chunk_key(self, chunk_key: str) -> Tuple[int, ...]:
-        return tuple(map(int, chunk_key.split(self.configuration.separator)))
+class TransposeCodec(ArrayArrayCodec):
+    configuration: TransposeCodecConfigurationMetadata
 
-    def encode_chunk_key(self, chunk_coords: Tuple[int, ...]) -> str:
-        chunk_identifier = self.configuration.separator.join(map(str, chunk_coords))
-        return "0" if chunk_identifier == "" else chunk_identifier
-
-
-ChunkKeyEncodingMetadata = Union[
-    DefaultChunkKeyEncodingMetadata, V2ChunkKeyEncodingMetadata
-]
+    @classmethod
+    def from_metadata(cls, codec_metadata: TransposeCodecMetadata) -> "TransposeCodec":
+        return cls(
+            configuration=codec_metadata.configuration,
+        )
 
+    async def inner_decode(
+        self,
+        chunk_array: np.ndarray,
+        array_metadata: "CoreArrayMetadata",
+    ) -> np.ndarray:
+        new_order = self.configuration.order
+        chunk_array = chunk_array.view(np.dtype(array_metadata.data_type.value))
+        if isinstance(new_order, tuple):
+            chunk_array = chunk_array.transpose(new_order)
+        elif new_order == "F":
+            chunk_array = chunk_array.reshape(
+                array_metadata.chunk_shape,
+                order="F",
+            )
+        else:
+            chunk_array = chunk_array.reshape(
+                array_metadata.chunk_shape,
+                order="C",
+            )
+        return chunk_array
 
-@frozen
-class CoreArrayMetadata:
-    shape: Tuple[int, ...]
-    chunk_shape: Tuple[int, ...]
-    data_type: DataType
-    fill_value: Any
-
-    @property
-    def dtype(self) -> np.dtype:
-        return np.dtype(self.data_type.value)
+    async def inner_encode(
+        self,
+        chunk_array: np.ndarray,
+        _array_metadata: "CoreArrayMetadata",
+    ) -> np.ndarray:
+        new_order = self.configuration.order
+        if isinstance(new_order, tuple):
+            chunk_array = chunk_array.transpose(new_order).reshape(-1, order="C")
+        else:
+            chunk_array = chunk_array.ravel(order=new_order)
+        return chunk_array
 
 
 @frozen
-class ArrayMetadata:
-    shape: Tuple[int, ...]
-    data_type: DataType
-    chunk_grid: RegularChunkGridMetadata
-    chunk_key_encoding: ChunkKeyEncodingMetadata
-    fill_value: Any
-    attributes: Dict[str, Any] = field(factory=dict)
-    codecs: List[CodecMetadata] = field(factory=list)
-    dimension_names: Optional[Tuple[str, ...]] = None
-    zarr_format: Literal[3] = 3
-    node_type: Literal["array"] = "array"
-
-    @property
-    def dtype(self) -> np.dtype:
-        return np.dtype(self.data_type.value)
-
-
-class Array:
-    metadata: ArrayMetadata
-    store: "Store"
-    path: str
+class GzipCodec(BytesBytesCodec):
+    configuration: GzipCodecConfigurationMetadata
 
     @classmethod
-    def create(
-        cls,
-        store: "Store",
-        path: str,
-        *,
-        shape: Tuple[int, ...],
-        dtype: Union[str, np.dtype],
-        chunk_shape: Tuple[int, ...],
-        fill_value: Optional[Any] = None,
-        chunk_key_encoding: Union[
-            Tuple[Literal["default"], Literal[".", "/"]],
-            Tuple[Literal["v2"], Literal[".", "/"]],
-        ] = ("default", "/"),
-        codecs: Optional[Iterable[CodecMetadata]] = None,
-        dimension_names: Optional[Iterable[str]] = None,
-        attributes: Optional[Dict[str, Any]] = None,
-    ) -> "Array":
-        data_type = (
-            DataType[dtype]
-            if isinstance(dtype, str)
-            else DataType[dtype_to_data_type[dtype.str]]
-        )
-
-        metadata = ArrayMetadata(
-            shape=shape,
-            data_type=data_type,
-            chunk_grid=RegularChunkGridMetadata(
-                configuration=RegularChunkGridConfigurationMetadata(
-                    chunk_shape=chunk_shape
-                )
-            ),
-            chunk_key_encoding=(
-                V2ChunkKeyEncodingMetadata(
-                    configuration=V2ChunkKeyEncodingConfigurationMetadata(
-                        separator=chunk_key_encoding[1]
-                    )
-                )
-                if chunk_key_encoding[0] == "v2"
-                else DefaultChunkKeyEncodingMetadata(
-                    configuration=DefaultChunkKeyEncodingConfigurationMetadata(
-                        separator=chunk_key_encoding[1]
-                    )
-                )
-            ),
-            fill_value=fill_value,
-            codecs=list(codecs) if codecs else [],
-            dimension_names=tuple(dimension_names) if dimension_names else None,
-            attributes=attributes or {},
+    def from_metadata(cls, codec_metadata: GzipCodecMetadata) -> "GzipCodec":
+        return cls(
+            configuration=codec_metadata.configuration,
         )
-        array = cls()
-        array.metadata = metadata
-        array.store = store
-        array.path = path
-        array._save_metadata()
-        return array
 
-    @classmethod
-    def open(cls, store: "Store", path: str) -> "Array":
-        zarr_json_bytes = store.get(f"{path}/{ZARR_JSON}")
-        assert zarr_json_bytes is not None
-        return cls.from_json(store, path, json.loads(zarr_json_bytes))
-
-    @classmethod
-    def from_json(cls, store: Store, path: str, zarr_json: Any) -> "Array":
-        array = cls()
-        array.metadata = make_cattr().structure(zarr_json, ArrayMetadata)
-        array.store = store
-        array.path = path
-        return array
-
-    def _save_metadata(self) -> None:
-        def convert(o):
-            if isinstance(o, DataType):
-                return o.name
-            raise TypeError
-
-        self.store.set(
-            f"{self.path}/{ZARR_JSON}",
-            json.dumps(asdict(self.metadata), default=convert).encode(),
+    async def inner_decode(
+        self,
+        chunk_bytes: bytes,
+        _array_metadata: "CoreArrayMetadata",
+    ) -> BytesLike:
+        return await to_thread(GZip(self.configuration.level).decode, chunk_bytes)
+
+    async def inner_encode(
+        self,
+        chunk_bytes: bytes,
+        _array_metadata: "CoreArrayMetadata",
+    ) -> BytesLike:
+        return await to_thread(GZip(self.configuration.level).encode, chunk_bytes)
+
+
+def blosc_codec(
+    cname: Literal["lz4", "lz4hc", "blosclz", "zstd", "snappy", "zlib"] = "zstd",
+    clevel: int = 5,
+    shuffle: Literal["noshuffle", "shuffle", "bitshuffle"] = "noshuffle",
+    blocksize: int = 0,
+) -> BloscCodecMetadata:
+    return BloscCodecMetadata(
+        configuration=BloscCodecConfigurationMetadata(
+            cname=cname, clevel=clevel, shuffle=shuffle, blocksize=blocksize
         )
+    )
 
-    @property
-    def ndim(self) -> int:
-        return len(self.metadata.shape)
-
-    def __getitem__(self, selection: Union[slice, Tuple[slice, ...]]):
-        indexer = BasicIndexer(
-            selection,
-            shape=self.metadata.shape,
-            chunk_shape=self.metadata.chunk_grid.configuration.chunk_shape,
-        )
 
-        # setup output array
-        out = np.zeros(
-            indexer.shape,
-            dtype=self.metadata.dtype,
-            order=get_order(self.metadata.codecs),
-        )
+def endian_codec(endian: Literal["big", "little"]) -> EndianCodecMetadata:
+    return EndianCodecMetadata(configuration=EndianCodecConfigurationMetadata(endian))
 
-        # reading chunks and decoding them
-        for chunk_coords, chunk_selection, out_selection in indexer:
-            chunk_key = f"{self.path}/{self.metadata.chunk_key_encoding.encode_chunk_key(chunk_coords)}"
-            value_handle = FileHandle(self.store, chunk_key)
-            chunk = self._decode_chunk(value_handle, chunk_selection)
-            if chunk is not None:
-                tmp = chunk[chunk_selection]
-                out[out_selection] = tmp
-            elif self.metadata.fill_value is not None:
-                out[out_selection] = self.metadata.fill_value
-
-        if out.shape:
-            return out
-        else:
-            return out[()]
 
-    def _decode_chunk(
-        self, value_handle: ValueHandle, selection: Tuple[slice, ...]
-    ) -> Optional[np.ndarray]:
-        if isinstance(value_handle, NoneHandle):
-            return None
-
-        core_metadata = CoreArrayMetadata(
-            shape=self.metadata.shape,
-            chunk_shape=self.metadata.chunk_grid.configuration.chunk_shape,
-            data_type=self.metadata.data_type,
-            fill_value=self.metadata.fill_value,
-        )
-
-        # apply codecs in reverse order
-        for codec_metadata in self.metadata.codecs[::-1]:
-            value_handle = codec_metadata.decode(value_handle, selection, core_metadata)
-
-        chunk = value_handle.toarray()
-        if chunk is None:
-            return None
-
-        # ensure correct dtype
-        if str(chunk.dtype) != self.metadata.data_type.name:
-            chunk = chunk.view(self.metadata.dtype)
-
-        # ensure correct chunk shape
-        if chunk.shape != self.metadata.chunk_grid.configuration.chunk_shape:
-            chunk = chunk.reshape(self.metadata.chunk_grid.configuration.chunk_shape)
-
-        return chunk
-
-    def __setitem__(
-        self, selection: Union[slice, Tuple[slice, ...]], value: np.ndarray
-    ) -> None:
-        chunk_shape = self.metadata.chunk_grid.configuration.chunk_shape
-        indexer = BasicIndexer(
-            selection,
-            shape=self.metadata.shape,
-            chunk_shape=chunk_shape,
-        )
+def transpose_codec(
+    order: Union[Tuple[int, ...], Literal["C", "F"]]
+) -> TransposeCodecMetadata:
+    return TransposeCodecMetadata(
+        configuration=TransposeCodecConfigurationMetadata(order)
+    )
 
-        sel_shape = indexer.shape
 
-        # check value shape
-        if sel_shape == ():
-            # setting a single item
-            assert np.isscalar(value)
-        elif np.isscalar(value):
-            # setting a scalar value
-            pass
-        else:
-            if not hasattr(value, "shape"):
-                value = np.asarray(value, self.metadata.dtype)
-            assert value.shape == sel_shape
-
-        # merging with existing data and encoding chunks
-        for chunk_coords, chunk_selection, out_selection in indexer:
-            chunk_key = f"{self.path}/{self.metadata.chunk_key_encoding.encode_chunk_key(chunk_coords)}"
-            value_handle = FileHandle(self.store, chunk_key)
-
-            if is_total_slice(chunk_selection, chunk_shape):
-                # write entire chunks
-                if sel_shape == ():
-                    chunk = value
-                elif np.isscalar(value):
-                    chunk = np.empty(
-                        chunk_shape,
-                        dtype=self.metadata.dtype,
-                        order="C",
-                    )
-                    chunk.fill(value)
-                else:
-                    chunk = value[out_selection].astype(
-                        self.metadata.dtype, order="C", copy=False
-                    )
-            else:
-                # writing partial chunks
-                # read chunk first
-                tmp = self._decode_chunk(
-                    value_handle,
-                    tuple(slice(0, c) for c in chunk_shape),
-                )
-
-                # merge new value
-                if tmp is None:
-                    chunk = np.empty(
-                        chunk_shape,
-                        dtype=self.metadata.dtype,
-                        order="C",
-                    )
-                    if self.metadata.fill_value:
-                        chunk.fill(self.metadata.fill_value)
-                else:
-                    chunk = tmp.copy(order="K")  # make a writable copy
-                chunk[chunk_selection] = value[out_selection]
-
-            chunk_value: ValueHandle
-            if self.metadata.fill_value and np.all(chunk == self.metadata.fill_value):
-                # chunks that only contain fill_value will be removed
-                chunk_value = NoneHandle()
-            else:
-                chunk_value = self._encode_chunk(
-                    chunk,
-                    tuple(slice(0, c) for c in chunk_shape),
-                )
-
-            # write out chunk
-            value_handle[:] = chunk_value
-
-    def _encode_chunk(self, chunk_value: np.ndarray, selection: Tuple[slice, ...]):
-        core_metadata = CoreArrayMetadata(
-            shape=self.metadata.shape,
-            chunk_shape=self.metadata.chunk_grid.configuration.chunk_shape,
-            data_type=self.metadata.data_type,
-            fill_value=self.metadata.fill_value,
-        )
-        encoded_chunk_value: ValueHandle = ArrayHandle(chunk_value)
-        for codec in self.metadata.codecs:
-            encoded_chunk_value = codec.encode(
-                encoded_chunk_value,
-                selection,
-                core_metadata,
-            )
+def gzip_codec(level: int = 5) -> GzipCodecMetadata:
+    return GzipCodecMetadata(configuration=GzipCodecConfigurationMetadata(level))
 
-        return encoded_chunk_value
 
-    def __repr__(self):
-        path = self.path
-        return f"<Array {path}>"
+def sharding_codec(
+    chunk_shape: Tuple[int, ...], codecs: List[CodecMetadata] = []
+) -> ShardingCodecMetadata:
+    return ShardingCodecMetadata(
+        configuration=ShardingCodecConfigurationMetadata(chunk_shape, codecs)
+    )
```

### Comparing `zarrita-0.1.0a1/zarrita/common.py` & `zarrita-0.1.0a2/zarrita/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,53 @@
-from typing import TYPE_CHECKING, Any, Dict, ForwardRef, List, Literal, Tuple, Union
+import asyncio
+import contextvars
+import functools
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
+import numpy as np
 from cattr import Converter
 
 if TYPE_CHECKING:
-    from zarrita.codecs import CodecMetadata
+    pass
 
 
 ZARR_JSON = "zarr.json"
-
-
-def is_total_slice(item, shape):
-    """Determine whether `item` specifies a complete slice of array with the
-    given `shape`. Used to optimize __setitem__ operations on the Chunk
-    class."""
-
-    # N.B., assume shape is normalized
-
-    if item == Ellipsis:
-        return True
-    if item == slice(None):
-        return True
-    if isinstance(item, slice):
-        item = (item,)
-    if isinstance(item, tuple):
-        return all(
-            (
-                isinstance(s, slice)
-                and (
-                    (s == slice(None))
-                    or ((s.stop - s.start == l) and (s.step in [1, None]))
-                )
-            )
-            for s, l in zip(item, shape)
-        )
-    else:
-        raise TypeError("expected slice or tuple of slices, found %r" % item)
-
-
-def get_order(codecs: List["CodecMetadata"]) -> Literal["C", "F"]:
-    for codec in codecs:
-        if codec.name == "transpose":
-            order = codec.configuration.order
-            if not isinstance(order, tuple):
-                return order
-    return "C"
+ZARRAY_JSON = ".zarray"
+ZGROUP_JSON = ".zgroup"
+ZATTRS_JSON = ".zattrs"
+
+BytesLike = Union[bytes, bytearray, memoryview]
+ChunkCoords = Tuple[int, ...]
+SliceSelection = Tuple[slice, ...]
+Selection = Union[slice, SliceSelection]
 
 
 def make_cattr():
-    from zarrita.array import (
-        ChunkKeyEncodingMetadata,
-        DefaultChunkKeyEncodingMetadata,
-        V2ChunkKeyEncodingMetadata,
-    )
-    from zarrita.codecs import (
+    from zarrita.metadata import (
         BloscCodecMetadata,
+        ChunkKeyEncodingMetadata,
         CodecMetadata,
+        DefaultChunkKeyEncodingMetadata,
         EndianCodecMetadata,
         GzipCodecMetadata,
         ShardingCodecMetadata,
         TransposeCodecMetadata,
+        V2ChunkKeyEncodingMetadata,
     )
 
     dataset_converter = Converter()
 
     def _structure_chunk_key_encoding_metadata(
         d: Dict[str, Any], _t
     ) -> ChunkKeyEncodingMetadata:
@@ -107,8 +92,66 @@
 
     dataset_converter.register_structure_hook_factory(
         lambda t: str(t)
         == "typing.Union[typing.Literal['C', 'F'], typing.Tuple[int, ...]]",
         lambda t: _structure_order,
     )
 
+    # Needed for v2 fill_value
+    def _structure_fill_value(d: Any, _t=None) -> Union[None, int, float]:
+        if d is None:
+            return None
+        try:
+            return int(d)
+        except ValueError:
+            pass
+        try:
+            return float(d)
+        except ValueError:
+            pass
+        raise ValueError
+
+    dataset_converter.register_structure_hook_factory(
+        lambda t: str(t) == "typing.Union[NoneType, int, float]",
+        lambda t: _structure_fill_value,
+    )
+
+    # Needed for v2 dtype
+    dataset_converter.register_structure_hook(
+        np.dtype,
+        lambda d, _: np.dtype(d),
+    )
+
     return dataset_converter
+
+
+def product(tup: ChunkCoords) -> int:
+    return functools.reduce(lambda x, y: x * y, tup, 1)
+
+
+T = TypeVar("T", bound=Tuple)
+V = TypeVar("V")
+
+
+async def concurrent_map(
+    items: List[T], func: Callable[..., Awaitable[V]], limit: Optional[int] = None
+) -> List[V]:
+    if limit is None:
+        return await asyncio.gather(*[func(*item) for item in items])
+
+    else:
+        sem = asyncio.Semaphore(limit)
+
+        async def run(item):
+            async with sem:
+                return await func(*item)
+
+        return await asyncio.gather(
+            *[asyncio.ensure_future(run(item)) for item in items]
+        )
+
+
+async def to_thread(func, /, *args, **kwargs):
+    loop = asyncio.get_running_loop()
+    ctx = contextvars.copy_context()
+    func_call = functools.partial(ctx.run, func, *args, **kwargs)
+    return await loop.run_in_executor(None, func_call)
```

### Comparing `zarrita-0.1.0a1/zarrita/indexing.py` & `zarrita-0.1.0a2/zarrita/indexing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,135 +1,84 @@
 import itertools
 import math
-import numbers
-from typing import Any, NamedTuple, Tuple, Union
+from typing import Iterator, List, NamedTuple, Optional, Tuple
 
+from zarrita.common import ChunkCoords, Selection, SliceSelection, product
 
-def _ensure_tuple(v):
+
+def _ensure_tuple(v: Selection) -> SliceSelection:
     if not isinstance(v, tuple):
         v = (v,)
     return v
 
 
-def _err_too_many_indices(selection, shape):
+def _err_too_many_indices(selection: SliceSelection, shape: ChunkCoords):
     raise IndexError(
         "too many indices for array; expected {}, got {}".format(
             len(shape), len(selection)
         )
     )
 
 
-def _err_boundscheck(dim_len):
-    raise IndexError("index out of bounds for dimension with length {}".format(dim_len))
-
-
 def _err_negative_step():
     raise IndexError("only slices with step >= 1 are supported")
 
 
-def _check_selection_length(selection, shape):
+def _check_selection_length(selection: SliceSelection, shape: ChunkCoords):
     if len(selection) > len(shape):
         _err_too_many_indices(selection, shape)
 
 
-def _replace_ellipsis(selection, shape) -> Tuple[int, ...]:
+def _ensure_selection(
+    selection: Selection,
+    shape: ChunkCoords,
+) -> SliceSelection:
     selection = _ensure_tuple(selection)
 
-    # count number of ellipsis present
-    n_ellipsis = sum(1 for i in selection if i is Ellipsis)
-
-    if n_ellipsis > 1:
-        # more than 1 is an error
-        raise IndexError("an index can only have a single ellipsis ('...')")
-
-    elif n_ellipsis == 1:
-        # locate the ellipsis, count how many items to left and right
-        n_items_l = selection.index(Ellipsis)  # items to left of ellipsis
-        n_items_r = len(selection) - (n_items_l + 1)  # items to right of ellipsis
-        n_items = len(selection) - 1  # all non-ellipsis items
-
-        if n_items >= len(shape):
-            # ellipsis does nothing, just remove it
-            selection = tuple(i for i in selection if i != Ellipsis)
-
-        else:
-            # replace ellipsis with as many slices are needed for number of dims
-            new_item = selection[:n_items_l] + ((slice(None),) * (len(shape) - n_items))
-            if n_items_r:
-                new_item += selection[-n_items_r:]
-            selection = new_item
-
     # fill out selection if not completely specified
     if len(selection) < len(shape):
         selection += (slice(None),) * (len(shape) - len(selection))
 
     # check selection not too long
     _check_selection_length(selection, shape)
 
     return selection
 
 
 class _ChunkDimProjection(NamedTuple):
-    dim_chunk_ix: Any
-    dim_chunk_sel: Any
-    dim_out_sel: Any
-
-
-def _normalize_integer_selection(dim_sel, dim_len):
-    # normalize type to int
-    dim_sel = int(dim_sel)
-
-    # handle wraparound
-    if dim_sel < 0:
-        dim_sel = dim_len + dim_sel
-
-    # handle out of bounds
-    if dim_sel >= dim_len or dim_sel < 0:
-        _err_boundscheck(dim_len)
-
-    return dim_sel
-
-
-class _IntDimIndexer:
-    def __init__(self, dim_sel, dim_len, dim_chunk_len):
-        # normalize
-        dim_sel = _normalize_integer_selection(dim_sel, dim_len)
-
-        # store attributes
-        self.dim_sel = dim_sel
-        self.dim_len = dim_len
-        self.dim_chunk_len = dim_chunk_len
-        self.nitems = 1
-
-    def __iter__(self):
-        dim_chunk_ix = self.dim_sel // self.dim_chunk_len
-        dim_offset = dim_chunk_ix * self.dim_chunk_len
-        dim_chunk_sel = self.dim_sel - dim_offset
-        dim_out_sel = None
-        yield _ChunkDimProjection(dim_chunk_ix, dim_chunk_sel, dim_out_sel)
+    dim_chunk_ix: int
+    dim_chunk_sel: slice
+    dim_out_sel: Optional[slice]
 
 
 def _ceildiv(a, b):
     return math.ceil(a / b)
 
 
 class _SliceDimIndexer:
-    def __init__(self, dim_sel, dim_len, dim_chunk_len):
-        # normalize
+    dim_sel: slice
+    dim_len: int
+    dim_chunk_len: int
+    nitems: int
+
+    start: int
+    stop: int
+    step: int
+
+    def __init__(self, dim_sel: slice, dim_len: int, dim_chunk_len: int):
         self.start, self.stop, self.step = dim_sel.indices(dim_len)
         if self.step < 1:
             _err_negative_step()
 
-        # store attributes
         self.dim_len = dim_len
         self.dim_chunk_len = dim_chunk_len
         self.nitems = max(0, _ceildiv((self.stop - self.start), self.step))
         self.nchunks = _ceildiv(self.dim_len, self.dim_chunk_len)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[_ChunkDimProjection]:
         # figure out the range of chunks we need to visit
         dim_chunk_ix_from = self.start // self.dim_chunk_len
         dim_chunk_ix_to = _ceildiv(self.stop, self.dim_chunk_len)
 
         # iterate over chunks in range
         for dim_chunk_ix in range(dim_chunk_ix_from, dim_chunk_ix_to):
             # compute offsets for chunk within overall array
@@ -167,53 +116,102 @@
             )
             dim_out_sel = slice(dim_out_offset, dim_out_offset + dim_chunk_nitems)
 
             yield _ChunkDimProjection(dim_chunk_ix, dim_chunk_sel, dim_out_sel)
 
 
 class _ChunkProjection(NamedTuple):
-    chunk_coords: Any
-    chunk_selection: Any
-    out_selection: Any
+    chunk_coords: ChunkCoords
+    chunk_selection: SliceSelection
+    out_selection: SliceSelection
 
 
 class BasicIndexer:
+    dim_indexers: List[_SliceDimIndexer]
+    shape: ChunkCoords
+
     def __init__(
         self,
-        selection: Union[slice, Tuple[slice, ...]],
+        selection: Selection,
         shape: Tuple[int, ...],
         chunk_shape: Tuple[int, ...],
     ):
-        # handle ellipsis
-        selection2 = _replace_ellipsis(selection, shape)
-
         # setup per-dimension indexers
-        dim_indexers = []
-        for dim_sel, dim_len, dim_chunk_len in zip(selection2, shape, chunk_shape):
-            if isinstance(dim_sel, numbers.Integral):
-                dim_indexer = _IntDimIndexer(dim_sel, dim_len, dim_chunk_len)
-
-            elif isinstance(dim_sel, slice):
-                dim_indexer = _SliceDimIndexer(dim_sel, dim_len, dim_chunk_len)
-
-            else:
-                raise IndexError(
-                    "unsupported selection item for basic indexing; "
-                    "expected integer or slice, got {!r}".format(type(dim_sel))
-                )
-
-            dim_indexers.append(dim_indexer)
-
-        self.dim_indexers = dim_indexers
-        self.shape = tuple(
-            s.nitems for s in self.dim_indexers if not isinstance(s, _IntDimIndexer)
-        )
+        self.dim_indexers = [
+            _SliceDimIndexer(dim_sel, dim_len, dim_chunk_len)
+            for dim_sel, dim_len, dim_chunk_len in zip(
+                _ensure_selection(selection, shape), shape, chunk_shape
+            )
+        ]
+        self.shape = tuple(s.nitems for s in self.dim_indexers)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[_ChunkProjection]:
         for dim_projections in itertools.product(*self.dim_indexers):
             chunk_coords = tuple(p.dim_chunk_ix for p in dim_projections)
             chunk_selection = tuple(p.dim_chunk_sel for p in dim_projections)
             out_selection = tuple(
                 p.dim_out_sel for p in dim_projections if p.dim_out_sel is not None
             )
 
             yield _ChunkProjection(chunk_coords, chunk_selection, out_selection)
+
+
+def morton_order_iter(chunk_shape: ChunkCoords) -> Iterator[ChunkCoords]:
+    def decode_morton(z: int, chunk_shape: ChunkCoords) -> ChunkCoords:
+        # Inspired by compressed morton code as implemented in Neuroglancer
+        # https://github.com/google/neuroglancer/blob/master/src/neuroglancer/datasource/precomputed/volume.md#compressed-morton-code
+        bits = tuple(math.ceil(math.log2(c)) for c in chunk_shape)
+        max_coords_bits = max(*bits)
+        input_bit = 0
+        input_value = z
+        out = [0 for _ in range(len(chunk_shape))]
+
+        for coord_bit in range(max_coords_bits):
+            for dim in range(len(chunk_shape)):
+                if coord_bit < bits[dim]:
+                    bit = (input_value >> input_bit) & 1
+                    out[dim] |= bit << coord_bit
+                    input_bit += 1
+        return tuple(out)
+
+    for i in range(product(chunk_shape)):
+        yield decode_morton(i, chunk_shape)
+
+
+def c_order_iter(chunks_per_shard: ChunkCoords) -> Iterator[ChunkCoords]:
+    return itertools.product(*(range(x) for x in chunks_per_shard))
+
+
+def is_total_slice(item: Selection, shape: ChunkCoords):
+    """Determine whether `item` specifies a complete slice of array with the
+    given `shape`. Used to optimize __setitem__ operations on the Chunk
+    class."""
+
+    # N.B., assume shape is normalized
+    if item == slice(None):
+        return True
+    if isinstance(item, slice):
+        item = (item,)
+    if isinstance(item, tuple):
+        return all(
+            (
+                isinstance(dim_sel, slice)
+                and (
+                    (dim_sel == slice(None))
+                    or (
+                        (dim_sel.stop - dim_sel.start == dim_len)
+                        and (dim_sel.step in [1, None])
+                    )
+                )
+            )
+            for dim_sel, dim_len in zip(item, shape)
+        )
+    else:
+        raise TypeError("expected slice or tuple of slices, found %r" % item)
+
+
+def all_chunk_coords(
+    shape: ChunkCoords, chunk_shape: ChunkCoords
+) -> Iterator[ChunkCoords]:
+    return itertools.product(
+        *(range(0, _ceildiv(s, c)) for s, c in zip(shape, chunk_shape))
+    )
```

### Comparing `zarrita-0.1.0a1/zarrita/sharding.py` & `zarrita-0.1.0a2/zarrita/sharding.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,390 +1,587 @@
-import functools
-import itertools
-import math
-from typing import (
-    TYPE_CHECKING,
-    Dict,
-    Iterator,
-    List,
-    Literal,
-    NamedTuple,
-    Optional,
-    Set,
-    Tuple,
-    Union,
-)
+from typing import Iterator, List, Mapping, NamedTuple, Optional, Set, Tuple
 
 import numpy as np
-from attrs import field, frozen
-
-from zarrita.common import get_order, is_total_slice
-from zarrita.indexing import BasicIndexer
-from zarrita.value_handle import ArrayHandle, BufferHandle, NoneHandle, ValueHandle
-
-if TYPE_CHECKING:
-    from zarrita.array import CoreArrayMetadata
-    from zarrita.codecs import CodecMetadata
+from attrs import frozen
+from crc32c import crc32c
 
+from zarrita.codecs import ArrayBytesCodec, Codec
+from zarrita.common import (
+    BytesLike,
+    ChunkCoords,
+    SliceSelection,
+    concurrent_map,
+    product,
+)
+from zarrita.indexing import (
+    BasicIndexer,
+    c_order_iter,
+    is_total_slice,
+    morton_order_iter,
+)
+from zarrita.metadata import (
+    CoreArrayMetadata,
+    ShardingCodecConfigurationMetadata,
+    ShardingCodecMetadata,
+)
+from zarrita.value_handle import (
+    ArrayValueHandle,
+    BufferValueHandle,
+    NoneValueHandle,
+    ValueHandle,
+)
 
 MAX_UINT_64 = 2**64 - 1
 
 
-@frozen
-class ShardingCodecConfigurationMetadata:
-    chunk_shape: Tuple[int, ...]
-    codecs: List["CodecMetadata"] = field(factory=list)
-
-
-def product(tup: Tuple[int, ...]) -> int:
-    return functools.reduce(lambda x, y: x * y, tup, 1)
-
-
-def c_order_iter(chunk_shape: Tuple[int, ...]) -> Iterator[Tuple[int, ...]]:
-    return itertools.product(*(range(x) for x in chunk_shape))
-
-
-def morton_order_iter(chunk_shape: Tuple[int, ...]) -> Iterator[Tuple[int, ...]]:
-    def decode_morton(z: int, chunk_shape: Tuple[int, ...]) -> Tuple[int, ...]:
-        # Inspired by compressed morton code as implemented in Neuroglancer
-        # https://github.com/google/neuroglancer/blob/master/src/neuroglancer/datasource/precomputed/volume.md#compressed-morton-code
-        bits = tuple(math.ceil(math.log2(c)) for c in chunk_shape)
-        max_coords_bits = max(*bits)
-        input_bit = 0
-        input_value = z
-        out = [0 for _ in range(len(chunk_shape))]
-
-        for coord_bit in range(max_coords_bits):
-            for dim in range(len(chunk_shape)):
-                if coord_bit < bits[dim]:
-                    bit = (input_value >> input_bit) & 1
-                    out[dim] |= bit << coord_bit
-                    input_bit += 1
-        return tuple(out)
-
-    for i in range(product(chunk_shape)):
-        yield decode_morton(i, chunk_shape)
-
-
 class _ShardIndex(NamedTuple):
     # dtype uint64, shape (chunks_per_shard_0, chunks_per_shard_1, ..., 2)
     offsets_and_lengths: np.ndarray
 
-    def _localize_chunk(self, chunk: Tuple[int, ...]) -> Tuple[int, ...]:
+    def _localize_chunk(self, chunk_coords: ChunkCoords) -> ChunkCoords:
         return tuple(
             chunk_i % shard_i
-            for chunk_i, shard_i in zip(chunk, self.offsets_and_lengths.shape)
+            for chunk_i, shard_i in zip(chunk_coords, self.offsets_and_lengths.shape)
         )
 
     def is_all_empty(self) -> bool:
-        return np.array_equiv(self.offsets_and_lengths, MAX_UINT_64)
+        return bool(np.array_equiv(self.offsets_and_lengths, MAX_UINT_64))
 
-    def get_chunk_slice(self, chunk: Tuple[int, ...]) -> Optional[slice]:
-        localized_chunk = self._localize_chunk(chunk)
+    def get_chunk_slice(self, chunk_coords: ChunkCoords) -> Optional[slice]:
+        localized_chunk = self._localize_chunk(chunk_coords)
         chunk_start, chunk_len = self.offsets_and_lengths[localized_chunk]
         if (chunk_start, chunk_len) == (MAX_UINT_64, MAX_UINT_64):
             return None
         else:
             return slice(int(chunk_start), int(chunk_start + chunk_len))
 
     def set_chunk_slice(
-        self, chunk: Tuple[int, ...], chunk_slice: Optional[slice]
+        self, chunk_coords: ChunkCoords, chunk_slice: Optional[slice]
     ) -> None:
-        localized_chunk = self._localize_chunk(chunk)
+        localized_chunk = self._localize_chunk(chunk_coords)
         if chunk_slice is None:
             self.offsets_and_lengths[localized_chunk] = (MAX_UINT_64, MAX_UINT_64)
         else:
             self.offsets_and_lengths[localized_chunk] = (
                 chunk_slice.start,
                 chunk_slice.stop - chunk_slice.start,
             )
 
     def to_bytes(self) -> bytes:
-        return self.offsets_and_lengths.tobytes(order="C")
+        index_bytes = self.offsets_and_lengths.tobytes(order="C")
+        return index_bytes + np.uint32(crc32c(index_bytes)).tobytes()
 
     @property
     def byte_length(self) -> int:
         return self.index_byte_length(self.offsets_and_lengths.shape)
 
     @classmethod
     def from_bytes(
         cls,
-        buffer: Union[bytes, bytearray],
-        chunks_per_shard: Tuple[int, ...],
+        buffer: BytesLike,
+        chunks_per_shard: ChunkCoords,
     ) -> "_ShardIndex":
         try:
+            crc32_bytes = buffer[-4:]
+            index_bytes = buffer[:-4]
+
+            assert np.uint32(crc32c(index_bytes)).tobytes() == bytes(crc32_bytes)
+
             return cls(
                 offsets_and_lengths=np.frombuffer(
-                    bytearray(buffer), dtype="<u8"
+                    bytearray(index_bytes), dtype="<u8"
                 ).reshape(*chunks_per_shard, 2, order="C"),
             )
         except ValueError as e:  # pragma: no cover
             raise RuntimeError from e
 
     @classmethod
-    def create_empty(cls, chunks_per_shard: Tuple[int, ...]) -> "_ShardIndex":
-        # reserving 2*64bit per chunk for offset and length:
-        return cls.from_bytes(
-            MAX_UINT_64.to_bytes(8, byteorder="little")
-            * (2 * product(chunks_per_shard)),
-            chunks_per_shard=chunks_per_shard,
+    def create_empty(cls, chunks_per_shard: ChunkCoords) -> "_ShardIndex":
+        offsets_and_lengths = np.zeros(chunks_per_shard + (2,), dtype="<u8", order="C")
+        offsets_and_lengths.fill(MAX_UINT_64)
+        return cls(offsets_and_lengths)
+
+    @classmethod
+    def index_byte_length(cls, chunks_per_shard: ChunkCoords) -> int:
+        return 16 * product(chunks_per_shard) + 4
+
+
+class _ShardProxy(Mapping):
+    index: _ShardIndex
+    buf: BytesLike
+
+    @classmethod
+    def from_bytes(cls, buf: BytesLike, chunks_per_shard: ChunkCoords) -> "_ShardProxy":
+        index = _ShardIndex.from_bytes(
+            buf[-_ShardIndex.index_byte_length(chunks_per_shard) :],
+            chunks_per_shard,
         )
+        obj = cls()
+        obj.buf = memoryview(buf)
+        obj.index = index
+        return obj
 
     @classmethod
-    def index_byte_length(cls, chunks_per_shard: Tuple[int, ...]) -> int:
-        return 16 * product(chunks_per_shard)
+    def create_empty(cls, chunks_per_shard: ChunkCoords) -> "_ShardProxy":
+        index = _ShardIndex.create_empty(chunks_per_shard)
+        obj = cls()
+        obj.buf = memoryview(b"")
+        obj.index = index
+        return obj
+
+    def __getitem__(self, chunk_coords: ChunkCoords) -> Optional[BytesLike]:
+        chunk_byte_slice = self.index.get_chunk_slice(chunk_coords)
+        if chunk_byte_slice:
+            return self.buf[chunk_byte_slice]
+        return None
+
+    def __len__(self) -> int:
+        return int(self.index.offsets_and_lengths.size / 2)
+
+    def __iter__(self) -> Iterator[ChunkCoords]:
+        return c_order_iter(self.index.offsets_and_lengths.shape[:-1])
+
+
+class _ShardBuilder(_ShardProxy):
+    buf: bytearray
+    index: _ShardIndex
+
+    @classmethod
+    def merge_with_morton_order(
+        cls,
+        chunks_per_shard: ChunkCoords,
+        tombstones: Set[ChunkCoords],
+        *shard_dicts: Mapping[ChunkCoords, BytesLike]
+    ) -> "_ShardBuilder":
+        obj = cls.create_empty(chunks_per_shard)
+        for chunk_coords in morton_order_iter(chunks_per_shard):
+            if tombstones is not None and chunk_coords in tombstones:
+                continue
+            for shard_dict in shard_dicts:
+                maybe_value = shard_dict.get(chunk_coords, None)
+                if maybe_value is not None:
+                    obj.append(chunk_coords, maybe_value)
+        return obj
+
+    @classmethod
+    def create_empty(cls, chunks_per_shard: ChunkCoords) -> "_ShardBuilder":
+        obj = cls()
+        obj.buf = bytearray()
+        obj.index = _ShardIndex.create_empty(chunks_per_shard)
+        return obj
+
+    def append(self, chunk_coords: ChunkCoords, value: BytesLike):
+        chunk_start = len(self.buf)
+        chunk_length = len(value)
+        self.buf.extend(value)
+        self.index.set_chunk_slice(
+            chunk_coords, slice(chunk_start, chunk_start + chunk_length)
+        )
+
+    def finalize(self) -> BytesLike:
+        self.buf.extend(self.index.to_bytes())
+        return self.buf
 
 
 @frozen
-class ShardingCodecMetadata:
+class ShardingCodec(ArrayBytesCodec):
     configuration: ShardingCodecConfigurationMetadata
-    name: Literal["sharding_indexed"] = "sharding_indexed"
+    codecs: List[Codec]
+
+    @classmethod
+    def from_metadata(cls, codec_metadata: ShardingCodecMetadata) -> "ShardingCodec":
+        return cls(
+            configuration=codec_metadata.configuration,
+            codecs=Codec.codecs_from_metadata(codec_metadata.configuration.codecs),
+        )
+
+    async def inner_decode(
+        self, chunk_array: BytesLike, array_metadata: "CoreArrayMetadata"
+    ) -> np.ndarray:
+        # Not implemented because `decode` is overridden
+        raise NotImplementedError
+
+    async def inner_encode(
+        self, chunk_array: np.ndarray, array_metadata: CoreArrayMetadata
+    ) -> BytesLike:
+        # Not implemented because `encode` is overridden
+        raise NotImplementedError
 
-    def decode(
+    async def decode(
         self,
         value_handle: ValueHandle,
-        selection: Tuple[slice, ...],
         array_metadata: "CoreArrayMetadata",
     ) -> ValueHandle:
-        if isinstance(value_handle, NoneHandle):
-            return NoneHandle()
+        # print("decode")
+        if isinstance(value_handle, NoneValueHandle):
+            return NoneValueHandle()
 
         shard_shape = array_metadata.chunk_shape
         chunk_shape = self.configuration.chunk_shape
         chunks_per_shard = tuple(s // c for s, c in zip(shard_shape, chunk_shape))
 
         indexer = BasicIndexer(
-            selection,
+            tuple(slice(0, s) for s in shard_shape),
             shape=shard_shape,
             chunk_shape=chunk_shape,
         )
 
         # setup output array
         out = np.zeros(
             shard_shape,
             dtype=array_metadata.dtype,
-            order=get_order(self.configuration.codecs),
+            order=array_metadata.runtime_configuration.order,
+        )
+        shard_dict = await self._load_full_shard(value_handle, chunks_per_shard)
+
+        if shard_dict.index.is_all_empty():
+            return NoneValueHandle()
+
+        # decoding chunks and writing them into the output buffer
+        await concurrent_map(
+            [
+                (
+                    shard_dict,
+                    chunk_coords,
+                    chunk_selection,
+                    out_selection,
+                    array_metadata,
+                    out,
+                )
+                for chunk_coords, chunk_selection, out_selection in indexer
+            ],
+            self._read_chunk,
+            array_metadata.runtime_configuration.concurrency,
+        )
+
+        return ArrayValueHandle(out)
+
+    async def decode_partial(
+        self,
+        value_handle: ValueHandle,
+        selection: SliceSelection,
+        array_metadata: "CoreArrayMetadata",
+    ) -> ValueHandle:
+        # print("decode_partial")
+        if isinstance(value_handle, NoneValueHandle):
+            return NoneValueHandle()
+
+        shard_shape = array_metadata.chunk_shape
+        chunk_shape = self.configuration.chunk_shape
+        chunks_per_shard = tuple(s // c for s, c in zip(shard_shape, chunk_shape))
+
+        indexer = BasicIndexer(
+            selection,
+            shape=shard_shape,
+            chunk_shape=chunk_shape,
+        )
+
+        # setup output array
+        out = np.zeros(
+            indexer.shape,
+            dtype=array_metadata.dtype,
+            order=array_metadata.runtime_configuration.order,
         )
 
         indexed_chunks = list(indexer)
         all_chunk_coords = set(chunk_coords for chunk_coords, _, _ in indexed_chunks)
 
         # reading bytes of all requested chunks
-        shard_dict: Dict[Tuple[int, ...], ValueHandle] = {}
+        shard_dict: Mapping[ChunkCoords, BytesLike] = {}
         if self._is_total_shard(all_chunk_coords, chunks_per_shard):
             # read entire shard
-            shard_dict = self._load_full_shard(value_handle, chunks_per_shard)
+            shard_dict = await self._load_full_shard(value_handle, chunks_per_shard)
         else:
             # read some chunks within the shard
-            shard_index = self._load_shard_index(value_handle, chunks_per_shard)
+            shard_index = await self._load_shard_index(value_handle, chunks_per_shard)
             shard_dict = {}
             for chunk_coords in all_chunk_coords:
                 chunk_byte_slice = shard_index.get_chunk_slice(chunk_coords)
                 if chunk_byte_slice:
-                    chunk_bytes = value_handle[chunk_byte_slice].tobytes()
+                    chunk_bytes = await value_handle[chunk_byte_slice].tobytes()
                     if chunk_bytes:
-                        shard_dict[chunk_coords] = BufferHandle(chunk_bytes)
+                        shard_dict[chunk_coords] = chunk_bytes
 
         # decoding chunks and writing them into the output buffer
-        for chunk_coords, chunk_selection, out_selection in indexed_chunks:
-            chunk_value = shard_dict.get(chunk_coords, NoneHandle())
-            chunk = self._decode_chunk(chunk_value, chunk_selection, array_metadata)
-            if chunk is not None:
-                tmp = chunk[chunk_selection]
-                out[out_selection] = tmp
-            elif array_metadata.fill_value is not None:
-                out[out_selection] = array_metadata.fill_value
+        await concurrent_map(
+            [
+                (
+                    shard_dict,
+                    chunk_coords,
+                    chunk_selection,
+                    out_selection,
+                    array_metadata,
+                    out,
+                )
+                for chunk_coords, chunk_selection, out_selection in indexed_chunks
+            ],
+            self._read_chunk,
+            array_metadata.runtime_configuration.concurrency,
+        )
 
-        return ArrayHandle(out)
+        return ArrayValueHandle(out)
 
-    def _decode_chunk(
+    async def _read_chunk(
         self,
-        value_handle: ValueHandle,
-        selection: Tuple[slice, ...],
+        shard_dict: Mapping[ChunkCoords, Optional[BytesLike]],
+        chunk_coords: ChunkCoords,
+        chunk_selection: SliceSelection,
+        out_selection: SliceSelection,
+        array_metadata: "CoreArrayMetadata",
+        out: np.ndarray,
+    ):
+        chunk_value = shard_dict.get(chunk_coords, None)
+        chunk_array = await self._decode_chunk(chunk_value, array_metadata)
+        if chunk_array is not None:
+            tmp = chunk_array[chunk_selection]
+            out[out_selection] = tmp
+        else:
+            out[out_selection] = array_metadata.fill_value
+
+    async def _decode_chunk(
+        self,
+        value: Optional[BytesLike],
         array_metadata: "CoreArrayMetadata",
     ) -> Optional[np.ndarray]:
-        if isinstance(value_handle, NoneHandle):
+        if value is None:
             return None
 
+        value_handle: ValueHandle = BufferValueHandle(value)
+
         from zarrita.array import CoreArrayMetadata
 
         # rewriting the metadata to scope it to the shard
         core_metadata = CoreArrayMetadata(
             shape=array_metadata.chunk_shape,
             chunk_shape=self.configuration.chunk_shape,
             data_type=array_metadata.data_type,
             fill_value=array_metadata.fill_value,
+            runtime_configuration=array_metadata.runtime_configuration,
         )
 
-        # applying codecs in reverse order
-        for codec_metadata in self.configuration.codecs[::-1]:
-            value_handle = codec_metadata.decode(value_handle, selection, core_metadata)
+        # applying codecs in revers e order
+        for codec in self.codecs[::-1]:
+            value_handle = await codec.decode(value_handle, core_metadata)
 
-        chunk = value_handle.toarray()
-        if chunk is None:
+        chunk_array = await value_handle.toarray()
+        if chunk_array is None:
             return None
 
         # ensure correct dtype
-        if str(chunk.dtype) != array_metadata.data_type.name:
-            chunk = chunk.view(np.dtype(array_metadata.data_type.name))
+        if str(chunk_array.dtype) != array_metadata.data_type.name:
+            chunk_array = chunk_array.view(np.dtype(array_metadata.data_type.name))
 
         # ensure correct chunk shape
-        if chunk.shape != self.configuration.chunk_shape:
-            chunk = chunk.reshape(self.configuration.chunk_shape)
+        if chunk_array.shape != self.configuration.chunk_shape:
+            chunk_array = chunk_array.reshape(self.configuration.chunk_shape)
 
-        return chunk
+        return chunk_array
 
-    def encode(
+    async def encode(
         self,
         value: ValueHandle,
-        selection: Tuple[slice, ...],
         array_metadata: "CoreArrayMetadata",
     ) -> ValueHandle:
-        shard = value.toarray()
-        if shard is None:
-            return NoneHandle()
+        # print("encode")
+        shard_array = await value.toarray()
+        if shard_array is None:
+            return NoneValueHandle()
 
         shard_shape = array_metadata.chunk_shape
         chunk_shape = self.configuration.chunk_shape
         chunks_per_shard = tuple(s // c for s, c in zip(shard_shape, chunk_shape))
 
         indexer = list(
             BasicIndexer(
-                selection,
+                tuple(slice(0, s) for s in shard_shape),
                 shape=shard_shape,
                 chunk_shape=chunk_shape,
             )
         )
 
-        assert self._is_total_shard(
-            set(chunk_coords for chunk_coords, _, _ in indexer), chunks_per_shard
-        )
-
-        # assembling and encoding chunks within the shard
-        shard_dict: Dict[Tuple[int, ...], ValueHandle] = {}
-        for chunk_coords, chunk_selection, out_selection in indexer:
+        async def _write_chunk(
+            shard_array: np.ndarray,
+            chunk_coords: ChunkCoords,
+            chunk_selection: SliceSelection,
+            out_selection: SliceSelection,
+        ) -> Tuple[ChunkCoords, Optional[BytesLike]]:
             if is_total_slice(chunk_selection, chunk_shape):
-                chunk = shard[out_selection]
+                chunk_array = shard_array[out_selection]
             else:
                 # handling writing partial chunks
-                chunk = np.empty(
+                chunk_array = np.empty(
                     chunk_shape,
                     dtype=array_metadata.dtype,
-                    order="C",
+                    order=array_metadata.runtime_configuration.order,
                 )
-                if array_metadata.fill_value:
-                    chunk.fill(array_metadata.fill_value)
-                chunk[chunk_selection] = shard[out_selection]
-            if array_metadata.fill_value and np.all(chunk == array_metadata.fill_value):
-                shard_dict[chunk_coords] = NoneHandle()
+                chunk_array.fill(array_metadata.fill_value)
+                chunk_array[chunk_selection] = shard_array[out_selection]
+            if not np.array_equiv(chunk_array, array_metadata.fill_value):
+                return (
+                    chunk_coords,
+                    await self._encode_chunk(chunk_array, array_metadata),
+                )
+            return (chunk_coords, None)
+
+        # assembling and encoding chunks within the shard
+        encoded_chunks: List[
+            Tuple[ChunkCoords, Optional[BytesLike]]
+        ] = await concurrent_map(
+            [
+                (shard_array, chunk_coords, chunk_selection, out_selection)
+                for chunk_coords, chunk_selection, out_selection in indexer
+            ],
+            _write_chunk,
+            array_metadata.runtime_configuration.concurrency,
+        )
+        shard_builder = _ShardBuilder.create_empty(chunks_per_shard)
+        for chunk_coords, chunk_bytes in encoded_chunks:
+            if chunk_bytes is not None:
+                shard_builder.append(chunk_coords, chunk_bytes)
+
+        if shard_builder.index.is_all_empty():
+            return NoneValueHandle()
+        return BufferValueHandle(shard_builder.finalize())
+
+    async def encode_partial(
+        self,
+        old_value_handle: ValueHandle,
+        shard_array: np.ndarray,
+        selection: SliceSelection,
+        array_metadata: "CoreArrayMetadata",
+    ) -> ValueHandle:
+        # print("encode_partial")
+        shard_shape = array_metadata.chunk_shape
+        chunk_shape = self.configuration.chunk_shape
+        chunks_per_shard = tuple(s // c for s, c in zip(shard_shape, chunk_shape))
+
+        old_shard_dict = await self._load_full_shard(old_value_handle, chunks_per_shard)
+        new_shard_builder = _ShardBuilder.create_empty(chunks_per_shard)
+        tombstones: Set[ChunkCoords] = set()
+
+        indexer = list(
+            BasicIndexer(
+                selection,
+                shape=shard_shape,
+                chunk_shape=chunk_shape,
+            )
+        )
+
+        async def _write_chunk(
+            chunk_coords: ChunkCoords,
+            chunk_selection: SliceSelection,
+            out_selection: SliceSelection,
+        ) -> Tuple[ChunkCoords, Optional[BytesLike]]:
+            chunk_array = None
+            if is_total_slice(chunk_selection, chunk_shape):
+                chunk_array = shard_array[out_selection]
             else:
-                shard_dict[chunk_coords] = self._encode_chunk(
-                    chunk, chunk_selection, array_metadata
+                # handling writing partial chunks
+                # read chunk first
+                tmp = await self._decode_chunk(
+                    old_shard_dict.get(chunk_coords, None),
+                    array_metadata,
+                )
+                # merge new value
+                if tmp is None:
+                    chunk_array = np.empty(
+                        chunk_shape,
+                        dtype=array_metadata.dtype,
+                        order=array_metadata.runtime_configuration.order,
+                    )
+                    chunk_array.fill(array_metadata.fill_value)
+                else:
+                    chunk_array = tmp.copy(
+                        order=array_metadata.runtime_configuration.order
+                    )  # make a writable copy
+                chunk_array[chunk_selection] = shard_array[out_selection]
+
+            if not np.array_equiv(chunk_array, array_metadata.fill_value):
+                return (
+                    chunk_coords,
+                    await self._encode_chunk(chunk_array, array_metadata),
                 )
+            else:
+                return (chunk_coords, None)
+
+        encoded_chunks: List[
+            Tuple[ChunkCoords, Optional[BytesLike]]
+        ] = await concurrent_map(
+            [
+                (chunk_coords, chunk_selection, out_selection)
+                for chunk_coords, chunk_selection, out_selection in indexer
+            ],
+            _write_chunk,
+            array_metadata.runtime_configuration.concurrency,
+        )
+
+        for chunk_coords, chunk_bytes in encoded_chunks:
+            if chunk_bytes is not None:
+                new_shard_builder.append(chunk_coords, chunk_bytes)
+            else:
+                tombstones.add(chunk_coords)
+
+        shard_builder = _ShardBuilder.merge_with_morton_order(
+            chunks_per_shard, tombstones, new_shard_builder, old_shard_dict
+        )
 
-        if all(
-            isinstance(chunk_value, NoneHandle) for chunk_value in shard_dict.values()
-        ):
-            return NoneHandle()
-        return BufferHandle(self._build_shard(shard_dict, chunks_per_shard))
+        if shard_builder.index.is_all_empty():
+            return NoneValueHandle()
+        return BufferValueHandle(shard_builder.finalize())
 
-    def _encode_chunk(
+    async def _encode_chunk(
         self,
         chunk: np.ndarray,
-        selection: Tuple[slice, ...],
         array_metadata: "CoreArrayMetadata",
-    ):
+    ) -> BytesLike:
         from zarrita.array import CoreArrayMetadata
 
         # rewriting the metadata to scope it to the shard
-        core_metadata = CoreArrayMetadata(
+        CoreArrayMetadata(
             shape=array_metadata.chunk_shape,
             chunk_shape=self.configuration.chunk_shape,
             data_type=array_metadata.data_type,
             fill_value=array_metadata.fill_value,
+            runtime_configuration=array_metadata.runtime_configuration,
         )
 
-        encoded_chunk_value: ValueHandle = ArrayHandle(chunk)
-        for codec in self.configuration.codecs:
-            encoded_chunk_value = codec.encode(
+        encoded_chunk_value: ValueHandle = ArrayValueHandle(chunk)
+        for codec in self.codecs:
+            encoded_chunk_value = await codec.encode(
                 encoded_chunk_value,
-                selection,
-                core_metadata,
+                array_metadata,
             )
 
-        return encoded_chunk_value
+        encoded_chunk_bytes = await encoded_chunk_value.tobytes()
+        assert encoded_chunk_bytes is not None
+        return encoded_chunk_bytes
 
     def _is_total_shard(
-        self, all_chunk_coords: Set[Tuple[int, ...]], chunks_per_shard: Tuple[int, ...]
+        self, all_chunk_coords: Set[ChunkCoords], chunks_per_shard: ChunkCoords
     ) -> bool:
         return len(all_chunk_coords) == product(chunks_per_shard) and all(
             chunk_coords in all_chunk_coords
             for chunk_coords in c_order_iter(chunks_per_shard)
         )
 
-    def _load_shard_index(
-        self, value_handle: ValueHandle, chunks_per_shard: Tuple[int, ...]
+    async def _load_shard_index(
+        self, value_handle: ValueHandle, chunks_per_shard: ChunkCoords
     ) -> _ShardIndex:
-        index_bytes = value_handle[-_ShardIndex.index_byte_length(chunks_per_shard) :]
-        assert isinstance(index_bytes, bytes)
+        # print("load_shard_index")
+        index_bytes = await value_handle[
+            -_ShardIndex.index_byte_length(chunks_per_shard) :
+        ].tobytes()
+        assert isinstance(index_bytes, bytes), index_bytes
         if index_bytes is not None:
             return _ShardIndex.from_bytes(index_bytes, chunks_per_shard)
         else:
             return _ShardIndex.create_empty(chunks_per_shard)
 
-    def _build_shard(
-        self,
-        shard_dict: Dict[Tuple[int, ...], ValueHandle],
-        chunks_per_shard: Tuple[int, ...],
-    ) -> bytes:
-        shard_index = _ShardIndex.create_empty(chunks_per_shard)
-        byte_shard_dict = {
-            chunk_coords: chunk_value.tobytes()
-            for chunk_coords, chunk_value in shard_dict.items()
-        }
-
-        # output buffer
-        shard_bytes = bytearray(
-            sum(
-                len(chunk_bytes)
-                for chunk_bytes in byte_shard_dict.values()
-                if chunk_bytes is not None
-            )
-            + shard_index.byte_length
-        )
-
-        # write chunks within shard in morton order
-        byte_offset = 0
-        for chunk_coords in morton_order_iter(chunks_per_shard):
-            chunk_bytes = byte_shard_dict.get(chunk_coords, None)
-            if chunk_bytes is not None:
-                byte_offset_end = byte_offset + len(chunk_bytes)
-                shard_bytes[byte_offset : byte_offset + len(chunk_bytes)] = chunk_bytes
-                shard_index.set_chunk_slice(
-                    chunk_coords, slice(byte_offset, byte_offset_end)
-                )
-                byte_offset = byte_offset_end
-        shard_bytes[-shard_index.byte_length :] = shard_index.to_bytes()
-        return bytes(shard_bytes)
-
-    def _load_full_shard(
-        self, value_handle: ValueHandle, chunks_per_shard: Tuple[int, ...]
-    ) -> Dict[Tuple[int, ...], ValueHandle]:
-        shard_bytes = value_handle.tobytes()
+    async def _load_full_shard(
+        self, value_handle: ValueHandle, chunks_per_shard: ChunkCoords
+    ) -> _ShardProxy:
+        # print("load_full_shard")
+        shard_bytes = await value_handle.tobytes()
         if shard_bytes:
             assert isinstance(shard_bytes, bytes)
-            index_bytes = shard_bytes[
-                -_ShardIndex.index_byte_length(chunks_per_shard) :
-            ]
-            shard_index = _ShardIndex.from_bytes(index_bytes, chunks_per_shard)
-
-            shard_dict: Dict[Tuple[int, ...], ValueHandle] = {}
-            for chunk_coords in c_order_iter(chunks_per_shard):
-                chunk_byte_slice = shard_index.get_chunk_slice(chunk_coords)
-                if chunk_byte_slice is not None:
-                    shard_dict[chunk_coords] = BufferHandle(
-                        shard_bytes[chunk_byte_slice]
-                    )
-
-            return shard_dict
-        else:
-            return {}
+            return _ShardProxy.from_bytes(shard_bytes, chunks_per_shard)
+        return _ShardProxy.create_empty(chunks_per_shard)
```

### Comparing `zarrita-0.1.0a1/setup.py` & `zarrita-0.1.0a2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,130 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: zarrita
+Version: 0.1.0a2
+Summary: 
+License: MIT
+Author: Norman Rzepka
+Author-email: code@normanrz.com
+Requires-Python: >=3.8,<3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: attrs (>=22.2.0,<23.0.0)
+Requires-Dist: cattrs (>=22.2.0,<23.0.0)
+Requires-Dist: crc32c (>=2.3.post0,<3.0)
+Requires-Dist: fsspec (>=2022.2.0,<2023.0.0)
+Requires-Dist: numcodecs (>=0.10.0,<0.11.0)
+Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Description-Content-Type: text/markdown
+
+# Zarrita
+
+Zarrita is an experimental implementation of [Zarr v3](https://zarr-specs.readthedocs.io/en/latest/v3/core/v3.0.html) including [sharding](https://zarr.dev/zeps/draft/ZEP0002.html). This is only a technical proof of concept meant for generating sample datasets. Not recommended for production use.
+
+## Setup
+
+```python
+import zarrita
+import numpy as np
+
+store = zarrita.FileSystemStore('file://./testdata')
+```
+
+## Create an array
+
+```python
+a = await zarrita.Array.create_async(
+    store,
+    'array',
+    shape=(6, 10),
+    dtype='int32',
+    chunk_shape=(2, 5),
+    codecs=[zarrita.codecs.gzip_codec(level=1)],
+    attributes={'question': 'life', 'answer': 42}
+)
+await a.async_[:, :].set(np.ones((6, 10), dtype='int32'))
+```
+
+## Open an array
+
+```python
+a = await zarrita.Array.open_async(store, 'array')
+assert np.array_equal(await a.async_[:, :].get(), np.ones((6, 10), dtype='int32'))
+```
+
+## Create an array with sharding
+
+```python
+a = await zarrita.Array.create_async(
+    store,
+    'sharding',
+    shape=(16, 16),
+    dtype='int32',
+    chunk_shape=(16, 16),
+    chunk_key_encoding=('v2', '.'),
+    codecs=[
+        zarrita.codecs.sharding_codec(
+            chunk_shape=(8, 8),
+            codecs=[zarrita.codecs.gzip_codec(level=1)]
+        ),
+    ],
+)
+data = np.arange(0, 16 * 16, dtype='int32').reshape((16, 16))
+await a.async_[:, :].set(data)
+assert np.array_equal(await a.async_[:, :].get(), data)
+```
+
+## Create a group
+
+```python
+g = await zarrita.Group.create_async(store, 'group')
+g2 = await g.create_group_async('group2')
+a = await g2.create_array_async(
+    'array',
+    shape=(16, 16),
+    dtype='int32',
+    chunk_shape=(16, 16),
+)
+await a.async_[:, :].set(np.arange(0, 16 * 16, dtype='int32').reshape((16, 16)))
+```
+
+## Open a group
+
+```python
+g = await zarrita.Group.open_async(store, 'group')
+g2 = g['group2']
+a = g['group2/array']
+assert np.array_equal(await a.asnyc_[:, :].get(), np.arange(0, 16 * 16, dtype='int32').reshape((16, 16)))
+```
+
+# Credits
+
+This is a largely-rewritten fork of `zarrita` by [@alimanfoo](https://github.com/alimanfoo). It implements the Zarr v3 draft specification created by [@alimanfoo](https://github.com/alimanfoo), [@jstriebel](https://github.com/jstriebel), [@jbms](https://github.com/jbms) et al.
+
+Licensed under MIT
+
+# TODO
+
+- [x] Async
+- [x] sharding partial decode
+- [x] variable renaming
+- [x] type indexing
+- [x] value handle slices get and set
+- [x] codec classes
+- [x] metadata validation
+- [x] zarr v2
+- [x] open with v2/v3 auto-detect
+- [x] async gather in sharding
+- [x] async local store
+- [x] resize arrays
+- [x] check empty before create array
+- [ ] morton order in indexing
+- [ ] attrs -> dataclasses
 
-packages = \
-['zarrita']
+## Non-priority
 
-package_data = \
-{'': ['*']}
+- Dask support
+- Buffer protocol
 
-install_requires = \
-['attrs>=22.2.0,<23.0.0',
- 'cattrs>=22.2.0,<23.0.0',
- 'fsspec>=2022.2.0,<2023.0.0',
- 'numcodecs>=0.10.0,<0.11.0',
- 'numpy>=1.24.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'zarrita',
-    'version': '0.1.0a1',
-    'description': '',
-    'long_description': "# Zarrita\n\nZarrita is an experimental implementation of [Zarr v3](https://zarr-specs.readthedocs.io/en/latest/v3/core/v3.0.html) including [sharding](https://zarr.dev/zeps/draft/ZEP0002.html). This is only a technical proof of concept meant for generating sample datasets. Not recommended for production use.\n\n## Setup\n\n```python\nimport zarrita\nimport numpy as np\n\nstore = zarrita.FileSystemStore('file://./testdata')\n```\n\n## Create an array\n\n```python\na = zarrita.Array.create(\n    store,\n    'array',\n    shape=(6, 10),\n    dtype='int32',\n    chunk_shape=(2, 5),\n    codecs=[zarrita.codecs.gzip_codec(level=1)],\n    attributes={'question': 'life', 'answer': 42}\n)\na[:, :] = np.ones((6, 10), dtype='int32')\n```\n\n## Open an array\n\n```python\na = zarrita.Array.open(store, 'array')\nassert np.array_equal(a[:, :], np.ones((6, 10), dtype='int32'))\n```\n\n## Create an array with sharding\n\n```python\na = zarrita.Array.create(\n    store,\n    'sharding',\n    shape=(16, 16),\n    dtype='int32',\n    chunk_shape=(16, 16),\n    chunk_key_encoding=('v2', '.'),\n    codecs=[\n        zarrita.codecs.sharding_codec(\n            chunk_shape=(8, 8),\n            codecs=[zarrita.codecs.gzip_codec(level=1)]\n        ),\n    ],\n)\ndata = np.arange(0, 16 * 16, dtype='int32').reshape((16, 16))\na[:, :] = data\nassert np.array_equal(a[:, :], data)\n```\n\n## Create a group\n\n```python\ng = zarrita.Group.create(store, 'group')\ng2 = g.create_group('group2')\na = g2.create_array(\n    'array',\n    shape=(16, 16),\n    dtype='int32',\n    chunk_shape=(16, 16),\n)\na[:, :] = np.arange(0, 16 * 16, dtype='int32').reshape((16, 16))\n```\n\n## Open a group\n\n```python\ng = zarrita.Group.open(store, 'group')\ng2 = g['group2']\na = g['group2/array']\nassert np.array_equal(a[:, :], np.arange(0, 16 * 16, dtype='int32').reshape((16, 16)))\n```\n\n# Credits\n\nThis is a largely-rewritten fork of `zarrita` by [@alimanfoo](https://github.com/alimanfoo). It implements the Zarr v3 draft specification created by [@alimanfoo](https://github.com/alimanfoo), [@jstriebel](https://github.com/jstriebel), [@jbms](https://github.com/jbms) et al.\n\nLicensed under MIT\n",
-    'author': 'Norman Rzepka',
-    'author_email': 'code@normanrz.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
-
-
-setup(**setup_kwargs)
```

