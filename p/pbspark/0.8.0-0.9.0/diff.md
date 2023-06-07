# Comparing `tmp/pbspark-0.8.0.tar.gz` & `tmp/pbspark-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbspark-0.8.0.tar", max compression
+gzip compressed data, was "pbspark-0.9.0.tar", max compression
```

## Comparing `pbspark-0.8.0.tar` & `pbspark-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     2244 2023-01-11 19:56:09.110415 pbspark-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     1073 2021-11-28 05:54:47.474621 pbspark-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     9834 2022-09-23 00:21:19.767564 pbspark-0.8.0/README.md
--rw-r--r--   0        0        0      209 2022-06-13 04:22:50.556320 pbspark-0.8.0/pbspark/__init__.py
--rw-r--r--   0        0        0    31126 2023-01-11 19:42:50.101837 pbspark-0.8.0/pbspark/_proto.py
--rw-r--r--   0        0        0      919 2022-05-19 02:33:56.387609 pbspark-0.8.0/pbspark/_timestamp.py
--rw-r--r--   0        0        0       22 2023-01-11 19:56:09.110937 pbspark-0.8.0/pbspark/_version.py
--rw-r--r--   0        0        0     1540 2023-01-11 19:56:09.111246 pbspark-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    10772 1970-01-01 00:00:00.000000 pbspark-0.8.0/setup.py
--rw-r--r--   0        0        0    10765 1970-01-01 00:00:00.000000 pbspark-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2295 2023-06-07 23:21:36.848237 pbspark-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1073 2021-11-28 05:54:47.474621 pbspark-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     9834 2022-09-23 00:21:19.767564 pbspark-0.9.0/README.md
+-rw-r--r--   0        0        0      209 2022-06-13 04:22:50.556320 pbspark-0.9.0/pbspark/__init__.py
+-rw-r--r--   0        0        0    31126 2023-01-11 19:42:50.101837 pbspark-0.9.0/pbspark/_proto.py
+-rw-r--r--   0        0        0      919 2022-05-19 02:33:56.387609 pbspark-0.9.0/pbspark/_timestamp.py
+-rw-r--r--   0        0        0       22 2023-06-07 23:21:36.848583 pbspark-0.9.0/pbspark/_version.py
+-rw-r--r--   0        0        0     1540 2023-06-07 23:21:36.849454 pbspark-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10816 1970-01-01 00:00:00.000000 pbspark-0.9.0/PKG-INFO
```

### Comparing `pbspark-0.8.0/CHANGELOG.md` & `pbspark-0.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 2023-06-07 - 0.9.0
+
+* Relax pyspark constraint
+
 ## 2023-01-11 - 0.8.0
 
 * Breaking: Provide the same kwargs used in the protobuf lib on encoding/decoding rather than the ``options`` dict, except ``DescriptorPool`` which is unserializable.
 * Breaking: Change param ``mc`` -> ``message_converter`` on top level functions.
 
 ## 2022-07-07 - 0.7.0
```

### Comparing `pbspark-0.8.0/LICENSE.txt` & `pbspark-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pbspark-0.8.0/README.md` & `pbspark-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pbspark-0.8.0/pbspark/_proto.py` & `pbspark-0.9.0/pbspark/_proto.py`

 * *Files identical despite different names*

### Comparing `pbspark-0.8.0/pbspark/_timestamp.py` & `pbspark-0.9.0/pbspark/_timestamp.py`

 * *Files identical despite different names*

### Comparing `pbspark-0.8.0/pyproject.toml` & `pbspark-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pbspark"
-version = "0.8.0"
+version = "0.9.0"
 description = "Convert between protobuf messages and pyspark dataframes"
 authors = ["flynn <crf204@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/crflynn/pbspark"
 repository = "https://github.com/crflynn/pbspark"
 documentation = "https://github.com/crflynn/pbspark"
@@ -19,15 +19,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Topic :: Database",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pyspark = ">=3.2.0"
+pyspark = ">=3.1.1"
 protobuf = ">=3.20.0"
 
 [tool.poetry.dev-dependencies]
 black = "^21.11b1"
 isort = "^5.10.1"
 pytest = "^6.2.5"
 mypy-protobuf = "^3.0.0"
```

### Comparing `pbspark-0.8.0/setup.py` & `pbspark-0.9.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,282 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pbspark
+Version: 0.9.0
+Summary: Convert between protobuf messages and pyspark dataframes
+Home-page: https://github.com/crflynn/pbspark
+License: MIT
+Keywords: spark,protobuf,pyspark
+Author: flynn
+Author-email: crf204@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database
+Requires-Dist: protobuf (>=3.20.0)
+Requires-Dist: pyspark (>=3.1.1)
+Project-URL: Documentation, https://github.com/crflynn/pbspark
+Project-URL: Repository, https://github.com/crflynn/pbspark
+Description-Content-Type: text/markdown
 
-packages = \
-['pbspark']
+# pbspark
 
-package_data = \
-{'': ['*']}
+This package provides a way to convert protobuf messages into pyspark dataframes and vice versa using pyspark `udf`s.
 
-install_requires = \
-['protobuf>=3.20.0', 'pyspark>=3.2.0']
-
-setup_kwargs = {
-    'name': 'pbspark',
-    'version': '0.8.0',
-    'description': 'Convert between protobuf messages and pyspark dataframes',
-    'long_description': '# pbspark\n\nThis package provides a way to convert protobuf messages into pyspark dataframes and vice versa using pyspark `udf`s.\n\n## Installation\n\nTo install:\n\n```bash\npip install pbspark\n```\n\n## Usage\n\nSuppose we have a pyspark DataFrame which contains a column `value` which has protobuf encoded messages of our `SimpleMessage`:\n\n```protobuf\nsyntax = "proto3";\n\npackage example;\n\nmessage SimpleMessage {\n  string name = 1;\n  int64 quantity = 2;\n  float measure = 3;\n}\n```\n\n### Basic conversion functions\n\nThere are two functions for operating on columns, `to_protobuf` and `from_protobuf`. These operations convert to/from an encoded protobuf column to a column of a struct representing the inferred message structure. `MessageConverter` instances (discussed below) can optionally be passed to these functions.\n\n```python\nfrom pyspark.sql.session import SparkSession\nfrom example.example_pb2 import SimpleMessage\nfrom pbspark import from_protobuf\nfrom pbspark import to_protobuf\n\nspark = SparkSession.builder.getOrCreate()\n\nexample = SimpleMessage(name="hello", quantity=5, measure=12.3)\ndata = [{"value": example.SerializeToString()}]\ndf_encoded = spark.createDataFrame(data)\n\ndf_decoded = df_encoded.select(from_protobuf(df_encoded.value, SimpleMessage).alias("value"))\ndf_expanded = df_decoded.select("value.*")\ndf_expanded.show()\n\n# +-----+--------+-------+\n# | name|quantity|measure|\n# +-----+--------+-------+\n# |hello|       5|   12.3|\n# +-----+--------+-------+\n\ndf_reencoded = df_decoded.select(to_protobuf(df_decoded.value, SimpleMessage).alias("value"))\n```\n\nThere are two helper functions, `df_to_protobuf` and `df_from_protobuf` for use on dataframes. They have a kwarg `expanded`, which will also take care of expanding/contracting the data between the single `value` column used in these examples and a dataframe which contains a column for each message field. `MessageConverter` instances (discussed below) can optionally be passed to these functions.\n\n```python\nfrom pyspark.sql.session import SparkSession\nfrom example.example_pb2 import SimpleMessage\nfrom pbspark import df_from_protobuf\nfrom pbspark import df_to_protobuf\n\nspark = SparkSession.builder.getOrCreate()\n\nexample = SimpleMessage(name="hello", quantity=5, measure=12.3)\ndata = [{"value": example.SerializeToString()}]\ndf_encoded = spark.createDataFrame(data)\n\n# expanded=True will perform a `.select("value.*")` after converting,\n# resulting in each protobuf field having its own column\ndf_expanded = df_from_protobuf(df_encoded, SimpleMessage, expanded=True)\ndf_expanded.show()\n\n# +-----+--------+-------+\n# | name|quantity|measure|\n# +-----+--------+-------+\n# |hello|       5|   12.3|\n# +-----+--------+-------+\n\n# expanded=True will first pack data using `struct([df[c] for c in df.columns])`,\n# use this if the passed dataframe is already expanded\ndf_reencoded = df_to_protobuf(df_expanded, SimpleMessage, expanded=True)\n```\n\n### Column conversion using the `MessageConverter`\n\nThe four helper functions above are also available as methods on the `MessageConverter` class. Using an instance of `MessageConverter` we can decode the column of encoded messages into a column of spark `StructType` and then expand the fields.\n\n```python\nfrom pyspark.sql.session import SparkSession\nfrom pbspark import MessageConverter\nfrom example.example_pb2 import SimpleMessage\n\nspark = SparkSession.builder.getOrCreate()\n\nexample = SimpleMessage(name="hello", quantity=5, measure=12.3)\ndata = [{"value": example.SerializeToString()}]\ndf_encoded = spark.createDataFrame(data)\n\nmc = MessageConverter()\ndf_decoded = df_encoded.select(mc.from_protobuf(df_encoded.value, SimpleMessage).alias("value"))\ndf_expanded = df_decoded.select("value.*")\ndf_expanded.show()\n\n# +-----+--------+-------+\n# | name|quantity|measure|\n# +-----+--------+-------+\n# |hello|       5|   12.3|\n# +-----+--------+-------+\n\ndf_expanded.schema\n# StructType(List(StructField(name,StringType,true),StructField(quantity,IntegerType,true),StructField(measure,FloatType,true))\n```\n\nWe can also re-encode them into protobuf.\n\n```python\ndf_reencoded = df_decoded.select(mc.to_protobuf(df_decoded.value, SimpleMessage).alias("value"))\n```\n\nFor expanded data, we can also encode after packing into a struct column:\n\n```python\nfrom pyspark.sql.functions import struct\n\ndf_unexpanded = df_expanded.select(\n    struct([df_expanded[c] for c in df_expanded.columns]).alias("value")\n)\ndf_reencoded = df_unexpanded.select(\n    mc.to_protobuf(df_unexpanded.value, SimpleMessage).alias("value")\n)\n```\n\n### Conversion details\n\nInternally, `pbspark` uses protobuf\'s `MessageToDict`, which deserializes everything into JSON compatible objects by default. The exceptions are\n* protobuf\'s bytes type, which `MessageToDict` would decode to a base64-encoded string; `pbspark` will decode any bytes fields directly to a spark `BinaryType`.\n* protobuf\'s well known type, Timestamp type, which `MessageToDict` would decode to a string; `pbspark` will decode any Timestamp messages directly to a spark `TimestampType` (via python datetime objects).\n* protobuf\'s int64 types, which `MessageToDict` would decode to a string for compatibility reasons; `pbspark` will decode these to `LongType`.\n\n### Custom conversion of message types\n\nCustom serde is also supported. Suppose we use our `NestedMessage` from the repository\'s example and we want to serialize the key and value together into a single string.\n\n```protobuf\nmessage NestedMessage {\n  string key = 1;\n  string value = 2;\n}\n```\n\nWe can create and register a custom serializer with the `MessageConverter`.\n\n```python\nfrom pbspark import MessageConverter\nfrom example.example_pb2 import ExampleMessage\nfrom example.example_pb2 import NestedMessage\nfrom pyspark.sql.types import StringType\n\nmc = MessageConverter()\n\n# register a custom serializer\n# this will serialize the NestedMessages into a string rather than a\n# struct with `key` and `value` fields\nencode_nested = lambda message:  message.key + ":" + message.value\n\nmc.register_serializer(NestedMessage, encode_nested, StringType())\n\n# ...\n\nfrom pyspark.sql.session import SparkSession\nfrom pyspark import SparkContext\nfrom pyspark.serializers import CloudPickleSerializer\n\nsc = SparkContext(serializer=CloudPickleSerializer())\nspark = SparkSession(sc).builder.getOrCreate()\n\nmessage = ExampleMessage(nested=NestedMessage(key="hello", value="world"))\ndata = [{"value": message.SerializeToString()}]\ndf_encoded = spark.createDataFrame(data)\n\ndf_decoded = df_encoded.select(mc.from_protobuf(df_encoded.value, ExampleMessage).alias("value"))\n# rather than a struct the value of `nested` is a string\ndf_decoded.select("value.nested").show()\n\n# +-----------+\n# |     nested|\n# +-----------+\n# |hello:world|\n# +-----------+\n```\n\n### How to write conversion functions\n\nMore generally, custom serde functions should be written in the following format.\n\n```python\n# Encoding takes a message instance and returns the result\n# of the custom transformation.\ndef encode_nested(message: NestedMessage) -> str:\n    return message.key + ":" + message.value\n\n# Decoding takes the encoded value, a message instance, and path string\n# and populates the fields of the message instance. It returns `None`.\n# The path str is used in the protobuf parser to log parse error info.\n# Note that the first argument type should match the return type of the\n# encoder if using both.\ndef decode_nested(s: str, message: NestedMessage, path: str):\n    key, value = s.split(":")\n    message.key = key\n    message.value = value\n```\n\n### Avoiding PicklingErrors\n\nA seemingly common issue with protobuf and distributed processing is when a `PicklingError` is encountered when transmitting (pickling) protobuf message types from a main process to a fork. To avoid this, you need to ensure that the fully qualified module name in your protoc-generated python file is the same as the module path from which the message type is imported. In other words, for the example here, the descriptor module passed to the builder is `example.example_pb2`\n\n```python\n# from example/example_pb2.py\n_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "example.example_pb2", globals())\n                                                     ^^^^^^^^^^^^^^^^^^^\n```\n\nAnd to import the message type we would call the same module path:\n\n```python\nfrom example.example_pb2 import ExampleMessage\n     ^^^^^^^^^^^^^^^^^^^\n```\n\nNote that the import module is the same as the one passed to the builder from the protoc-generated python. If these do not match, then you will encounter a `PicklingError`. From the pickle documentation: *pickle can save and restore class instances transparently, however the class definition must be importable and live in the same module as when the object was stored.*\n\nTo ensure that the module path is correct, you should run `protoc` from the relative root path of your proto files. For example, in this project, in the `Makefile` under the `gen` command, we call `protoc` from the project root rather than from within the `example` directory.\n\n```makefile\nexport PROTO_PATH=.\n\ngen:\n\tpoetry run protoc -I $$PROTO_PATH --python_out=$$PROTO_PATH --mypy_out=$$PROTO_PATH --proto_path=$$PROTO_PATH $$PROTO_PATH/example/*.proto\n```\n\n### Known issues\n\n`RecursionError` when using self-referencing protobuf messages. Spark schemas do not allow for arbitrary depth, so protobuf messages which are circular- or self-referencing will result in infinite recursion errors when inferring the schema. If you have message structures like this you should resort to creating custom conversion functions, which forcibly limit the structural depth when converting these messages.\n\n## Development\n\nEnsure that [asdf](https://asdf-vm.com/) is installed, then run `make setup`.\n\n* To format code `make fmt`\n* To test code `make test`\n* To run protoc `make gen`\n',
-    'author': 'flynn',
-    'author_email': 'crf204@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/crflynn/pbspark',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+## Installation
+
+To install:
+
+```bash
+pip install pbspark
+```
+
+## Usage
+
+Suppose we have a pyspark DataFrame which contains a column `value` which has protobuf encoded messages of our `SimpleMessage`:
+
+```protobuf
+syntax = "proto3";
+
+package example;
+
+message SimpleMessage {
+  string name = 1;
+  int64 quantity = 2;
+  float measure = 3;
 }
+```
+
+### Basic conversion functions
+
+There are two functions for operating on columns, `to_protobuf` and `from_protobuf`. These operations convert to/from an encoded protobuf column to a column of a struct representing the inferred message structure. `MessageConverter` instances (discussed below) can optionally be passed to these functions.
+
+```python
+from pyspark.sql.session import SparkSession
+from example.example_pb2 import SimpleMessage
+from pbspark import from_protobuf
+from pbspark import to_protobuf
+
+spark = SparkSession.builder.getOrCreate()
+
+example = SimpleMessage(name="hello", quantity=5, measure=12.3)
+data = [{"value": example.SerializeToString()}]
+df_encoded = spark.createDataFrame(data)
+
+df_decoded = df_encoded.select(from_protobuf(df_encoded.value, SimpleMessage).alias("value"))
+df_expanded = df_decoded.select("value.*")
+df_expanded.show()
+
+# +-----+--------+-------+
+# | name|quantity|measure|
+# +-----+--------+-------+
+# |hello|       5|   12.3|
+# +-----+--------+-------+
+
+df_reencoded = df_decoded.select(to_protobuf(df_decoded.value, SimpleMessage).alias("value"))
+```
+
+There are two helper functions, `df_to_protobuf` and `df_from_protobuf` for use on dataframes. They have a kwarg `expanded`, which will also take care of expanding/contracting the data between the single `value` column used in these examples and a dataframe which contains a column for each message field. `MessageConverter` instances (discussed below) can optionally be passed to these functions.
+
+```python
+from pyspark.sql.session import SparkSession
+from example.example_pb2 import SimpleMessage
+from pbspark import df_from_protobuf
+from pbspark import df_to_protobuf
+
+spark = SparkSession.builder.getOrCreate()
+
+example = SimpleMessage(name="hello", quantity=5, measure=12.3)
+data = [{"value": example.SerializeToString()}]
+df_encoded = spark.createDataFrame(data)
+
+# expanded=True will perform a `.select("value.*")` after converting,
+# resulting in each protobuf field having its own column
+df_expanded = df_from_protobuf(df_encoded, SimpleMessage, expanded=True)
+df_expanded.show()
+
+# +-----+--------+-------+
+# | name|quantity|measure|
+# +-----+--------+-------+
+# |hello|       5|   12.3|
+# +-----+--------+-------+
+
+# expanded=True will first pack data using `struct([df[c] for c in df.columns])`,
+# use this if the passed dataframe is already expanded
+df_reencoded = df_to_protobuf(df_expanded, SimpleMessage, expanded=True)
+```
+
+### Column conversion using the `MessageConverter`
+
+The four helper functions above are also available as methods on the `MessageConverter` class. Using an instance of `MessageConverter` we can decode the column of encoded messages into a column of spark `StructType` and then expand the fields.
+
+```python
+from pyspark.sql.session import SparkSession
+from pbspark import MessageConverter
+from example.example_pb2 import SimpleMessage
+
+spark = SparkSession.builder.getOrCreate()
+
+example = SimpleMessage(name="hello", quantity=5, measure=12.3)
+data = [{"value": example.SerializeToString()}]
+df_encoded = spark.createDataFrame(data)
+
+mc = MessageConverter()
+df_decoded = df_encoded.select(mc.from_protobuf(df_encoded.value, SimpleMessage).alias("value"))
+df_expanded = df_decoded.select("value.*")
+df_expanded.show()
+
+# +-----+--------+-------+
+# | name|quantity|measure|
+# +-----+--------+-------+
+# |hello|       5|   12.3|
+# +-----+--------+-------+
+
+df_expanded.schema
+# StructType(List(StructField(name,StringType,true),StructField(quantity,IntegerType,true),StructField(measure,FloatType,true))
+```
+
+We can also re-encode them into protobuf.
+
+```python
+df_reencoded = df_decoded.select(mc.to_protobuf(df_decoded.value, SimpleMessage).alias("value"))
+```
+
+For expanded data, we can also encode after packing into a struct column:
+
+```python
+from pyspark.sql.functions import struct
+
+df_unexpanded = df_expanded.select(
+    struct([df_expanded[c] for c in df_expanded.columns]).alias("value")
+)
+df_reencoded = df_unexpanded.select(
+    mc.to_protobuf(df_unexpanded.value, SimpleMessage).alias("value")
+)
+```
+
+### Conversion details
+
+Internally, `pbspark` uses protobuf's `MessageToDict`, which deserializes everything into JSON compatible objects by default. The exceptions are
+* protobuf's bytes type, which `MessageToDict` would decode to a base64-encoded string; `pbspark` will decode any bytes fields directly to a spark `BinaryType`.
+* protobuf's well known type, Timestamp type, which `MessageToDict` would decode to a string; `pbspark` will decode any Timestamp messages directly to a spark `TimestampType` (via python datetime objects).
+* protobuf's int64 types, which `MessageToDict` would decode to a string for compatibility reasons; `pbspark` will decode these to `LongType`.
+
+### Custom conversion of message types
+
+Custom serde is also supported. Suppose we use our `NestedMessage` from the repository's example and we want to serialize the key and value together into a single string.
+
+```protobuf
+message NestedMessage {
+  string key = 1;
+  string value = 2;
+}
+```
+
+We can create and register a custom serializer with the `MessageConverter`.
+
+```python
+from pbspark import MessageConverter
+from example.example_pb2 import ExampleMessage
+from example.example_pb2 import NestedMessage
+from pyspark.sql.types import StringType
+
+mc = MessageConverter()
+
+# register a custom serializer
+# this will serialize the NestedMessages into a string rather than a
+# struct with `key` and `value` fields
+encode_nested = lambda message:  message.key + ":" + message.value
+
+mc.register_serializer(NestedMessage, encode_nested, StringType())
+
+# ...
+
+from pyspark.sql.session import SparkSession
+from pyspark import SparkContext
+from pyspark.serializers import CloudPickleSerializer
+
+sc = SparkContext(serializer=CloudPickleSerializer())
+spark = SparkSession(sc).builder.getOrCreate()
+
+message = ExampleMessage(nested=NestedMessage(key="hello", value="world"))
+data = [{"value": message.SerializeToString()}]
+df_encoded = spark.createDataFrame(data)
+
+df_decoded = df_encoded.select(mc.from_protobuf(df_encoded.value, ExampleMessage).alias("value"))
+# rather than a struct the value of `nested` is a string
+df_decoded.select("value.nested").show()
+
+# +-----------+
+# |     nested|
+# +-----------+
+# |hello:world|
+# +-----------+
+```
+
+### How to write conversion functions
+
+More generally, custom serde functions should be written in the following format.
+
+```python
+# Encoding takes a message instance and returns the result
+# of the custom transformation.
+def encode_nested(message: NestedMessage) -> str:
+    return message.key + ":" + message.value
+
+# Decoding takes the encoded value, a message instance, and path string
+# and populates the fields of the message instance. It returns `None`.
+# The path str is used in the protobuf parser to log parse error info.
+# Note that the first argument type should match the return type of the
+# encoder if using both.
+def decode_nested(s: str, message: NestedMessage, path: str):
+    key, value = s.split(":")
+    message.key = key
+    message.value = value
+```
+
+### Avoiding PicklingErrors
+
+A seemingly common issue with protobuf and distributed processing is when a `PicklingError` is encountered when transmitting (pickling) protobuf message types from a main process to a fork. To avoid this, you need to ensure that the fully qualified module name in your protoc-generated python file is the same as the module path from which the message type is imported. In other words, for the example here, the descriptor module passed to the builder is `example.example_pb2`
+
+```python
+# from example/example_pb2.py
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "example.example_pb2", globals())
+                                                     ^^^^^^^^^^^^^^^^^^^
+```
+
+And to import the message type we would call the same module path:
+
+```python
+from example.example_pb2 import ExampleMessage
+     ^^^^^^^^^^^^^^^^^^^
+```
+
+Note that the import module is the same as the one passed to the builder from the protoc-generated python. If these do not match, then you will encounter a `PicklingError`. From the pickle documentation: *pickle can save and restore class instances transparently, however the class definition must be importable and live in the same module as when the object was stored.*
+
+To ensure that the module path is correct, you should run `protoc` from the relative root path of your proto files. For example, in this project, in the `Makefile` under the `gen` command, we call `protoc` from the project root rather than from within the `example` directory.
+
+```makefile
+export PROTO_PATH=.
+
+gen:
+	poetry run protoc -I $$PROTO_PATH --python_out=$$PROTO_PATH --mypy_out=$$PROTO_PATH --proto_path=$$PROTO_PATH $$PROTO_PATH/example/*.proto
+```
+
+### Known issues
+
+`RecursionError` when using self-referencing protobuf messages. Spark schemas do not allow for arbitrary depth, so protobuf messages which are circular- or self-referencing will result in infinite recursion errors when inferring the schema. If you have message structures like this you should resort to creating custom conversion functions, which forcibly limit the structural depth when converting these messages.
+
+## Development
+
+Ensure that [asdf](https://asdf-vm.com/) is installed, then run `make setup`.
 
+* To format code `make fmt`
+* To test code `make test`
+* To run protoc `make gen`
 
-setup(**setup_kwargs)
```

