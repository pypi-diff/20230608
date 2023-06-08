# Comparing `tmp/MelodieTable-0.2.0-py3-none-any.whl.zip` & `tmp/MelodieTable-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10042 bytes, number of entries: 12
+Zip file size: 10116 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      163 b- defN 23-May-30 12:51 MelodieTable/__init__.py
 -rw-rw-rw-  2.0 fat     6128 b- defN 23-May-09 14:56 MelodieTable/reader_writer.py
--rw-rw-rw-  2.0 fat     2800 b- defN 23-May-30 13:33 MelodieTable/table_base.py
+-rw-rw-rw-  2.0 fat     2802 b- defN 23-Jun-02 03:01 MelodieTable/table_base.py
 -rw-rw-rw-  2.0 fat     3104 b- defN 23-May-30 12:01 MelodieTable/table_general.py
--rw-rw-rw-  2.0 fat     6645 b- defN 23-May-31 11:04 MelodieTable/table_objects.py
+-rw-rw-rw-  2.0 fat     6967 b- defN 23-Jun-02 03:25 MelodieTable/table_objects.py
 -rw-rw-rw-  2.0 fat     4077 b- defN 23-May-30 12:19 MelodieTable/table_pyam.py
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Jun-02 02:28 MelodieTable-0.2.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      160 b- defN 23-Jun-02 02:28 MelodieTable-0.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-02 02:28 MelodieTable-0.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       66 b- defN 23-Jun-02 02:28 MelodieTable-0.2.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-02 02:28 MelodieTable-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1014 b- defN 23-Jun-02 02:28 MelodieTable-0.2.0.dist-info/RECORD
-12 files, 25354 bytes uncompressed, 8324 bytes compressed:  67.2%
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Jun-08 01:49 MelodieTable-0.3.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      160 b- defN 23-Jun-08 01:49 MelodieTable-0.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-08 01:49 MelodieTable-0.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       66 b- defN 23-Jun-08 01:49 MelodieTable-0.3.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-08 01:49 MelodieTable-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1014 b- defN 23-Jun-08 01:49 MelodieTable-0.3.0.dist-info/RECORD
+12 files, 25678 bytes uncompressed, 8398 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: MelodieTable/table_objects.py
 Comment: 
 
 Filename: MelodieTable/table_pyam.py
 Comment: 
 
-Filename: MelodieTable-0.2.0.dist-info/LICENSE
+Filename: MelodieTable-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: MelodieTable-0.2.0.dist-info/METADATA
+Filename: MelodieTable-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: MelodieTable-0.2.0.dist-info/WHEEL
+Filename: MelodieTable-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: MelodieTable-0.2.0.dist-info/entry_points.txt
+Filename: MelodieTable-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: MelodieTable-0.2.0.dist-info/top_level.txt
+Filename: MelodieTable-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: MelodieTable-0.2.0.dist-info/RECORD
+Filename: MelodieTable-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## MelodieTable/table_base.py

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from sqlalchemy.types import BigInteger, Text, TypeEngine, Float, Boolean
 from typing import Callable, Dict, List, Optional, Tuple, TypeVar, Type, Any
 
-pytypes_to_satypes: Dict[Type, Type[TypeEngine]] = {
+py_types_to_sa_types: Dict[Type, Type[TypeEngine]] = {
     int: BigInteger,
     str: Text,
     float: Float,
     bool: Boolean
 }
```

## MelodieTable/table_objects.py

```diff
@@ -1,31 +1,34 @@
-from typing import Callable, Generic, List, Optional, Tuple, Type, Union, Dict, TypeVar
+from typing import Any, Callable, Generic, List, Optional, Tuple, Type, Union, Dict, TypeVar
 from sqlalchemy import Column
 from sqlalchemy.types import TypeEngine
 from sqlalchemy.orm import declarative_base
 from .reader_writer import TableReader, TableWriter, DatabaseConnector
-from .table_base import TableBase, RowBase, pytypes_to_satypes, ColumnMeta
+from .table_base import TableBase, RowBase, py_types_to_sa_types, ColumnMeta
 
 Base = declarative_base()
 
 VEC_TEMPLATE = """
 def vectorize_template(obj):
     return [{exprs}]
 """
 
 
 class TableRow(RowBase):
-    def __init__(self, **kwargs) -> None:
+    __table__: "Table"
+
+    def __init__(self, table: "Table", **kwargs) -> None:
+        self.__table__ = table
         if kwargs is not None:
             for k, v in kwargs.items():
                 setattr(self, k, v)
 
     @classmethod
-    def from_dict(cls, d: Dict, aliases: Dict[str, str]):
-        r = TableRow()
+    def from_dict(cls, table: "Table", d: Dict, aliases: Dict[str, str]) -> "TableRow":
+        r = TableRow(table)
         for k, v in d.items():
             setattr(r, aliases[k], v)
         return r
 
     @classmethod
     def get_annotations(cls) -> Dict[str, Union[Type[int], Type[str], Type[float]]]:
         return cls.__annotations__
@@ -53,88 +56,92 @@
         attr_names = [attr_name for attr_name in list(
             set(attr_names)) if not attr_name.startswith("__")]
         dtypes = {}
         for attr_name in attr_names:
             assert attr_name in cls.get_annotations(
             ), f"Attribute \"{attr_name}\" of class {cls.__name__} must be annotated!"
             if not hasattr(cls, attr_name):
-                dtype = pytypes_to_satypes[cls.get_annotations()[attr_name]]()
+                dtype = py_types_to_sa_types[cls.get_annotations()[
+                    attr_name]]()
             else:
                 meta = getattr(cls, attr_name)
                 assert isinstance(meta, ColumnMeta)
                 if meta.dtype is not None:
                     dtype = meta.dtype
                 else:
-                    dtype = pytypes_to_satypes[cls.get_annotations()[
+                    dtype = py_types_to_sa_types[cls.get_annotations()[
                         attr_name]]()
             dtypes[attr_name] = dtype
         return dtypes
 
     @staticmethod
     def vectorizer(attrs: List[str]) -> Callable[[object], List[Union[bool, int, float, str]]]:
-        exprs = ",".join(['obj.'+attr for attr in attrs])
+        exprs = ",".join(['obj.' + attr for attr in attrs])
         code = VEC_TEMPLATE.format(exprs=exprs)
         vars = {}
         exec(code, None, vars)
         return vars["vectorize_template"]
 
+    def __setattr__(self, __name: str, __value: Any) -> None:
+        return super().__setattr__(__name, __value)
+
+
+class TR(TableRow):
+    pass
+
 
 RowType = Union[Type, Dict[str, TypeEngine]]
 
 TableRowGeneric = TypeVar("TableRowGeneric")
 
 
 class Table(TableBase, Generic[TableRowGeneric]):
     data: List[TableRowGeneric]
 
-    def __init__(self, row_type: RowType) -> None:
+    def __init__(self, row_type: Type[TableRowGeneric]) -> None:
         super().__init__()
-        self.row_cls: Type[TableRowGeneric] = None
+        self.row_cls: Type[TableRow] = row_type
         self._db_model_cls: Type = None
         self.row_types: Dict[str, Column] = {}
 
         if callable(row_type) and issubclass(row_type, TableRow):
-            self.row_cls = row_type
             self.row_types = row_type.get_datatypes()
-        elif isinstance(row_type, dict):
-            self.row_cls = TableRow
-            for prop_name, prop_value in row_type.items():
-                self.row_types[prop_name] = Column(prop_value)
+        # elif isinstance(row_type, dict):
+        #     self.row_cls = TableRow
+        #     for prop_name, prop_value in row_type.items():
+        #         self.row_types[prop_name] = Column(prop_value)
         else:
             raise NotImplementedError(
                 f"Cannot recognize table row type {type(row_type)}")
 
     def clear(self):
         self.data = []
 
-    def new_row(self):
-        return self.row_cls()
-
     @staticmethod
     def parse_header(header_colnames_list: List[str]):
         """
         Parse the header row.
         """
         cols: List[str] = []
         for col_index, col_name in enumerate(header_colnames_list):
             cols.append(col_name)
             assert col_name.isidentifier, f"Column name '{col_name}' should be an identifier!"
         return cols
 
     @staticmethod
-    def from_file(file_name: str, row_types: RowType, encoding='utf-8'):
+    def from_file(file_name: str, row_types: Type[TableRowGeneric], encoding='utf-8'):
         table = Table(row_type=row_types)
         reader = TableReader(file_name,
                              text_encoding=encoding)
         header, rows_iter = reader.read()
         columns = Table.parse_header(header)
-
+        aliases = table.row_cls.get_aliases()
         for row_data in rows_iter:
-            table_row_obj = table.row_cls(
-                **{col: row_data[i] for i, col in enumerate(columns)})
+            table_row_obj: TableRow = table.row_cls.from_dict(
+                table, {col: row_data[i] for i, col in enumerate(columns)}, aliases)
             table.data.append(table_row_obj)
         return table
 
     def to_file(self, file_name: str, encoding="utf-8"):
         writer = TableWriter(file_name,
                              text_encoding=encoding).write()
         headers = [row for row in self.row_types.keys()]
@@ -159,15 +166,15 @@
         writer.close()
 
     @staticmethod
     def from_dicts(row_type: RowType, dicts: List[dict]):
         table = Table(row_type)
         aliases = table.row_cls.get_aliases()
         for dic in dicts:
-            table.data.append(table.row_cls.from_dict(dic, aliases))
+            table.data.append(table.row_cls.from_dict(table, dic, aliases))
         return table
 
     def apply(self, ufunc: Callable[[TableRowGeneric], None]) -> None:
         for row in self.data:
             ufunc(row)
 
     def find_one(self, query: Callable[[TableRowGeneric], bool]) -> Optional[TableRowGeneric]:
```

## Comparing `MelodieTable-0.2.0.dist-info/LICENSE` & `MelodieTable-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

