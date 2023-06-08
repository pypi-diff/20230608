# Comparing `tmp/mysqlx-1.1.9.tar.gz` & `tmp/mysqlx-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.1.9.tar", last modified: Wed Jun  7 04:22:04 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.2.1.tar", last modified: Thu Jun  8 14:33:08 2023, max compression
```

## Comparing `mysqlx-1.1.9.tar` & `mysqlx-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 04:22:04.000000 mysqlx-1.1.9/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.1.9/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-07 04:22:04.000000 mysqlx-1.1.9/mysqlx/
--rw-rw-rw-   0        0        0     4695 2023-06-07 02:19:08.000000 mysqlx-1.1.9/mysqlx/coder.py
--rw-rw-rw-   0        0        0    10185 2023-06-07 02:33:53.000000 mysqlx-1.1.9/mysqlx/db.py
--rw-rw-rw-   0        0        0     3370 2023-06-06 00:29:56.000000 mysqlx-1.1.9/mysqlx/dbx.py
--rw-rw-rw-   0        0        0     5295 2023-06-06 23:27:22.000000 mysqlx-1.1.9/mysqlx/helper.py
--rw-rw-rw-   0        0        0    10080 2023-06-07 04:19:02.000000 mysqlx-1.1.9/mysqlx/orm.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.1.9/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 04:22:04.000000 mysqlx-1.1.9/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-07 04:22:04.000000 mysqlx-1.1.9/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-06 08:06:39.000000 mysqlx-1.1.9/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      404 2023-06-07 04:22:04.000000 mysqlx-1.1.9/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-06-07 04:22:04.000000 mysqlx-1.1.9/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      297 2023-06-07 04:22:04.000000 mysqlx-1.1.9/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-06-07 04:22:04.000000 mysqlx-1.1.9/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      404 2023-06-07 04:22:04.000000 mysqlx-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2598 2023-06-06 12:09:45.000000 mysqlx-1.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 04:22:04.000000 mysqlx-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0      807 2023-06-07 04:21:46.000000 mysqlx-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 14:33:08.000000 mysqlx-1.2.1/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.2.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-08 14:33:08.000000 mysqlx-1.2.1/mysqlx/
+-rw-rw-rw-   0        0        0     5484 2023-06-08 14:29:56.000000 mysqlx-1.2.1/mysqlx/coder.py
+-rw-rw-rw-   0        0        0    10185 2023-06-07 12:34:06.000000 mysqlx-1.2.1/mysqlx/db.py
+-rw-rw-rw-   0        0        0     3370 2023-06-06 00:29:56.000000 mysqlx-1.2.1/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0     5295 2023-06-06 23:27:22.000000 mysqlx-1.2.1/mysqlx/helper.py
+-rw-rw-rw-   0        0        0    11033 2023-06-07 14:35:41.000000 mysqlx-1.2.1/mysqlx/orm.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.2.1/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 14:33:08.000000 mysqlx-1.2.1/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-08 14:33:08.000000 mysqlx-1.2.1/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-06 08:06:39.000000 mysqlx-1.2.1/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      404 2023-06-08 14:33:08.000000 mysqlx-1.2.1/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-06-08 14:33:08.000000 mysqlx-1.2.1/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      297 2023-06-08 14:33:08.000000 mysqlx-1.2.1/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-06-08 14:33:08.000000 mysqlx-1.2.1/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      404 2023-06-08 14:33:08.000000 mysqlx-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2598 2023-06-06 12:09:45.000000 mysqlx-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-08 14:33:08.000000 mysqlx-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-06-08 14:32:48.000000 mysqlx-1.2.1/setup.py
```

### Comparing `mysqlx-1.1.9/LICENSE` & `mysqlx-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.1.9/mysqlx/coder.py` & `mysqlx-1.2.1/mysqlx/coder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,82 +1,93 @@
+import os
 from . import db
-from jinja2 import Template
+from jinja2 import FileSystemLoader, Environment
 from typing import Union, Iterable
 
-COMMON_COLS = ['id', 'create_by', 'update_by', 'create_time', 'update_time', 'del_flag']
-
 
 class Coder:
     comma1 = ','
     comma2 = '，'
     sql = '''
     SELECT column_name, data_type, character_maximum_length, NUMERIC_precision, NUMERIC_scale, column_key FROM information_schema.columns
      WHERE table_schema = (SELECT DATABASE())
        AND table_name = ? 
     '''
-    template = '''from mysqlx.orm import Model
-from decimal import Decimal
-from datetime import date, datetime
-  
-{% for meta in metas %}
-class {{meta.class_name}}(Model):
-    __pk__ = '{{meta.pk}}'
-    __table__ = '{{meta.table}}'
-    
-    def __init__(self,{% for item in meta.columns %}{% if loop.last %} {{item.COLUMN_NAME}}: {{item.DATA_TYPE}} = None{% else %} {{item.COLUMN_NAME}}: {{item.DATA_TYPE}} = None,{% endif %}{% endfor %}): 
-        super().__init__({% for super_column in meta.super_columns %}{% if loop.first %}{{super_column}}={{super_column}}{% else %}, {{super_column}}={{super_column}}{% endif %}{% endfor %}) {% for item in meta.self_columns %}
-        self.{{item.COLUMN_NAME}} = {{item.COLUMN_NAME}} {% endfor %}
-        
-{% endfor %}
-'''
 
     def __init__(self, user: str, password: str, database: str, host='127.0.0.1', port=3306, use_unicode=True, pool_size=1, show_sql=True, **kwargs):
         db.init_db(user, password, database, host, port, pool_size, use_unicode, show_sql, **kwargs)
 
-    def generate_with_schema(self, schema: str = None, path: str = None):
+    def generate_with_schema(self, schema: str = None, path: str = None, common_cols=['create_by', 'create_time'],
+                             attributes={'__pk__': 'id', '__update_by__': 'update_by', '__update_time__': 'update_time', '__del_flag__': 'del_flag'}):
         if schema:
             db.execute('use %s' % schema)
         tables = db.select('show tables')
         tables = [table['Tables_in_investment'] for table in tables]
-        self.generate_with_tables(tables=tables, path=path)
+        self.generate_with_tables(tables=tables, path=path, common_cols=common_cols, attributes=attributes)
 
-    def generate_with_tables(self, tables: Union[str, Iterable[str]], path: str = None):
+    def generate_with_tables(self, tables: Union[str, Iterable[str]], path: str = None, common_cols=['create_by', 'create_time'],
+                             attributes={'__pk__': 'id', '__update_by__': 'update_by', '__update_time__': 'update_time', '__del_flag__': 'del_flag'}):
         metas = None
         only_one_table = False
+
+        columns = [v for v in attributes.values()]
+        common_cols.reverse()
+        for i in range(0, 2):
+            columns.insert(1, common_cols[i])
+
+        # 去重
+        base_columns = list(set(columns))
+        # 保持原有顺序
+        base_columns.sort(key=columns.index)
+
         if isinstance(tables, str):
             if self.comma1 in tables:
                 tables = tables.split(self.comma1)
             elif self.comma2 in tables:
                 tables = tables.split(self.comma2)
             else:
                 only_one_table = True
-                metas = [self._get_table_meta(tables)]
+                metas = [self._get_table_meta(tables, base_columns)]
 
         if not only_one_table:
             if not isinstance(tables, set):
                 tables = set(tables)
-            metas = [self._get_table_meta(table.strip()) for table in tables]
+            metas = [self._get_table_meta(table.strip(), base_columns) for table in tables]
 
         no_pk_tables = [meta for meta in metas if isinstance(meta, str)]
         if len(no_pk_tables) > 0:
             print("There isn't primary key in the tables %s, it will not generate model class." % no_pk_tables)
 
         metas = [meta for meta in metas if isinstance(meta, dict)]
         if len(metas) > 0:
-            self._generate({'metas': metas}, path)
+            def get_type(col):
+                if col == attributes.get('__pk__') or col == attributes.get('__update_by__') or col == attributes.get('__del_flag__'):
+                    return 'int'
+                elif col == attributes.get('__update_time__'):
+                    return 'datetime'
+                elif col.endswith("_time"):
+                    return 'datetime'
+                elif col.endswith("_date"):
+                    return 'date'
+                else:
+                    return 'None'
+
+            attributes['metas'] = metas
+            attributes['base_columns'] = [{'COLUMN_NAME': col, 'DATA_TYPE': get_type(col)} for col in base_columns]
+            self._generate(attributes, path)
 
-    def _get_table_meta(self, table: str):
+    def _get_table_meta(self, table: str, base_columns):
         pk = None
         super_columns = []
         columns = db.do_select(self.sql, table)
         for col in columns:
             if col['COLUMN_KEY'] == 'PRI':
                 pk = col['COLUMN_NAME']
 
-            if col['COLUMN_NAME'] in COMMON_COLS:
+            if col['COLUMN_NAME'] in base_columns:
                 super_columns.append(col['COLUMN_NAME'])
 
             if col['DATA_TYPE'] in ('tinyint', 'bigint'):
                 col['DATA_TYPE'] = 'int'
             elif col['DATA_TYPE'] == 'double':
                 col['DATA_TYPE'] = 'float'
             elif col['DATA_TYPE'] == 'decimal':
@@ -89,29 +100,32 @@
 
         class_name = self._get_class_name(table)
         return {
             'pk': pk,
             'table': table,
             'class_name': class_name,
             'columns': columns,
-            'self_columns': [col for col in columns if col['COLUMN_NAME'] not in COMMON_COLS],
+            'self_columns': [col for col in columns if col['COLUMN_NAME'] not in base_columns],
             'super_columns': super_columns
         }
 
-    def _generate(self, metas: dict, path: str):
-        tpl = Template(self.template)
-        r = tpl.render(**metas)
+    @staticmethod
+    def _generate(metas: dict, path: str):
+        loader = FileSystemLoader(searchpath=os.path.dirname(__file__))
+        environment = Environment(loader=loader)
+        tpl = environment.get_template('coder.tpl')
+        output = tpl.render(**metas)
         if path:
             suffix = '.py'
             path = path if path.endswith(suffix) else path + suffix
             with open(path, 'w', encoding='utf-8') as f:
-                f.write(r)
+                f.write(output)
             print('Model文件已生成：%s' % path)
         else:
-            print(r)
+            print(output)
 
     @staticmethod
     def _get_class_name(table):
         if '_' not in table:
             return table.capitalize()
 
         names = table.split('_')
```

### Comparing `mysqlx-1.1.9/mysqlx/db.py` & `mysqlx-1.2.1/mysqlx/db.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.1.9/mysqlx/dbx.py` & `mysqlx-1.2.1/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.1.9/mysqlx/helper.py` & `mysqlx-1.2.1/mysqlx/helper.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.1.9/mysqlx/orm.py` & `mysqlx-1.2.1/mysqlx/orm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from . import db
 from typing import Iterable
-from datetime import datetime
 
-PK, TABLE, UPDATE_TIME = '__pk__', '__table__', 'update_time'
+PK, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG = '__pk__', '__table__', '__update_by__', '__update_time__', '__del_flag__'
 SYMBOLS = ['=', '>', '<']
 BETWEEN, LIKE, IN = 'between', 'like', 'in'
 
 
 def _get_condition_arg(k, v):
     if not isinstance(v, str):
         return "`%s`=?" % k, v
@@ -16,248 +15,269 @@
     elif BETWEEN in v_lower or LIKE in v_lower or IN in v_lower:
         return "`%s` %s" % (k, v), None
     else:
         return "`%s`=?" % k, v
 
 
 def _get_where_args(**kwargs):
-    where, args = '', []
     if kwargs:
         conditions, args = zip(*[_get_condition_arg(k, v) for k, v in kwargs.items()])
         args = [arg for arg in args if arg is not None]
         where = 'WHERE %s' % ' and '.join(conditions)
-
-    return where, args
+        return where, args
+    return '', []
 
 
 class Model:
-
-    def __init__(self, id: int = None, create_by: int = None, create_time: datetime = None, update_time: datetime = None, update_by: int = None,
-                 del_flag: int = None):
-        self.id = id
-        self.create_by = create_by
-        self.create_time = create_time
-        self.update_by = update_by
-        self.update_by = update_time
-        self.del_flag = del_flag
-
     def __str__(self):
-        kv = {k: v for k, v in self.__dict__.items() if k not in (PK, TABLE)}
+        kv = {k: v for k, v in self.__dict__.items() if not k.startswith("__")}
         return str(kv)
 
     def __getattr__(self, name):
         if PK == name:
             return 'id'
         elif TABLE == name:
             return self.__class__.__name__.lower()
+        elif UPDATE_BY == name:
+            return 'update_by'
+        elif UPDATE_TIME == name:
+            return 'update_time'
         else:
             return None
 
     def persist(self):
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
-        self.id = db.save(self.__table__, **kv)
+        self.id = db.save(self._get_table(), **kv)
         return self.id
 
     def update(self):
-        pk = self.__pk__
+        pk, table = self._get_pk_and_table()
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
-        if pk in kv:
-            update_kv = {k: v for k, v in kv.items() if k != pk}
+        if pk not in kv:
+            raise KeyError("Not primary key.")
+
+        update_kv = {k: v for k, v in kv.items() if k != pk}
+        if update_kv:
             cols, args = zip(*update_kv.items())
             args = [*args, kv[pk]]
-            if UPDATE_TIME in update_kv:
-                sql = 'UPDATE `%s` SET %s WHERE `%s`=? limit 1' % (self.__table__, ','.join(['`%s`=?' % col for col in cols]), pk)
+            update_time_col = self._get_update_time_col()
+            if update_time_col is None or update_time_col in update_kv:
+                sql = 'UPDATE `%s` SET %s WHERE `%s`=? limit 1' % (table, ','.join(['`%s`=?' % col for col in cols]), pk)
             else:
-                sql = 'UPDATE `%s` SET %s, %s=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (self.__table__, ','.join(['`%s`=?' % col for col in cols]), UPDATE_TIME, pk)
+                sql = 'UPDATE `%s` SET %s, %s=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (table, ','.join(['`%s`=?' % col for col in cols]), update_time_col, pk)
             db.do_execute(sql, *args)
-        else:
-            raise KeyError("Not primary key.")
 
     def load(self):
-        pk = self.__pk__
+        pk, table = self._get_pk_and_table()
         kv = self.__dict__
         _id = kv.get(pk)
         if _id is not None:
             cols, _ = zip(*kv.items())
-            sql = 'SELECT %s FROM `%s` WHERE `%s`=? limit 1' % (','.join(['`%s`' % col for col in cols]), self.__table__, pk)
+            sql = 'SELECT %s FROM `%s` WHERE `%s`=? limit 1' % (','.join(['`%s`' % col for col in cols]), table, pk)
             self.__dict__.update(db.do_select_one(sql, _id))
             return self
         else:
             raise KeyError("Not primary key.")
 
     def delete(self):
-        pk = self.__pk__
+        pk, table = self._get_pk_and_table()
         _id = self.__dict__.get(pk)
-        if _id is not None:
-            sql = 'DELETE FROM `%s` WHERE `%s`=? limit 1' % (self.__table__, pk)
-            return db.do_execute(sql, _id)
-        else:
+        if _id is None:
             raise KeyError("Not primary key.")
 
+        sql = 'DELETE FROM `%s` WHERE `%s`=? limit 1' % (table, pk)
+        return db.do_execute(sql, _id)
+
     def logic_delete(self, update_by: int = None):
-        pk = self.__pk__
+        pk, table = self._get_pk_and_table()
         _id = self.__dict__.get(pk)
-        if _id is not None:
-            if update_by is None:
-                sql = 'UPDATE `%s` SET `del_flag`=1, `%s`=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (self.__table__, UPDATE_TIME, pk)
-                return db.do_execute(sql, _id)
-            else:
-                sql = 'UPDATE `%s` SET `del_flag`=1, `update_by`=?, `%s`=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (self.__table__, UPDATE_TIME, pk)
-                return db.do_execute(sql, update_by, _id)
-        else:
+        if _id is None:
             raise KeyError("Not primary key.")
 
+        return self.logic_delete_by_id(_id, update_by)
+
     @classmethod
     def insert(cls, **kwargs):
-        table = cls._get_table(cls)
+        table = cls._get_table()
         return db.insert(table, **kwargs)
 
     @classmethod
     def save(cls, **kwargs):
-        table = cls._get_table(cls)
+        table = cls._get_table()
         return db.save(table, **kwargs)
 
     @classmethod
     def find_by_id(cls, id: int, *selection):
         """
         Return one object or None if no result.
         """
-        pk, table = cls._get_pk_and_table(cls)
         result = cls.select_by_id(id, *selection)
-        return cls.dict2obj(result, cls, pk, table) if result else None
+        return cls._dict2obj(result) if result else None
 
     @classmethod
     def find_by_ids(cls, ids: Iterable[int], *selection):
         """
         Return list(object) or empty list if no result.
         """
-        pk, table = cls._get_pk_and_table(cls)
-        return [cls.dict2obj(d, cls, pk, table) for d in cls.select_by_ids(ids, *selection)]
+        return [cls._dict2obj(d) for d in cls.select_by_ids(ids, *selection)]
 
     @classmethod
     def select_by_id(cls, id: int, *selection):
         """
         Return one row(dict) or None if no result.
         """
-        pk, table = cls._get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table()
         if len(selection) == 0:
             sql = 'SELECT * FROM `%s` WHERE `%s`=? limit 1' % (table, pk)
         else:
             sql = 'SELECT %s FROM `%s` WHERE `%s`=? limit 1' % (','.join(['`%s`' % col for col in selection]), table, pk)
         return db.do_select_one(sql, id)
 
     @classmethod
     def select_by_ids(cls, ids: Iterable[int], *selection):
         """
         Return list(dict) or empty list if no result.
         """
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
-        pk, table = cls._get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table()
         ids_str = ','.join(list(map(str, ids)))
         if len(selection) == 0:
             sql = 'SELECT * FROM `%s` WHERE `%s` in (%s) limit %d' % (table, pk, ids_str, ids_size)
         else:
             sql = 'SELECT %s FROM `%s` WHERE `%s` in (%s) limit %d' % (','.join(['`%s`' % col for col in selection]), table, pk, ids_str, ids_size)
         return db.do_select(sql)
 
     @classmethod
     def update_by_id(cls, id: int, **kwargs):
-        pk, table = cls._get_pk_and_table(cls)
+        assert kwargs, 'Must set update kv'
+        pk, table = cls._get_pk_and_table()
         cols, args = zip(*kwargs.items())
         args = [*args, id]
-        if UPDATE_TIME in kwargs:
-            sql = 'UPDATE `%s` SET %s WHERE `%s`=? limit 1' % (table, ','.join(['`%s`=?' % col for col in cols]), UPDATE_TIME, pk)
+        update_time_col = cls._get_update_time_col()
+        if update_time_col is None or update_time_col in kwargs:
+            sql = 'UPDATE `%s` SET %s WHERE `%s`=? limit 1' % (table, ','.join(['`%s`=?' % col for col in cols]), pk)
         else:
-            sql = 'UPDATE `%s` SET %s, `%s`=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (table, ','.join(['`%s`=?' % col for col in cols]), UPDATE_TIME, pk)
+            sql = 'UPDATE `%s` SET %s, `%s`=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (table, ','.join(['`%s`=?' % col for col in cols]), update_time_col, pk)
         db.do_execute(sql, *args)
 
     @classmethod
     def delete_by_id(cls, id: int):
-        pk, table = cls._get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table()
         sql = 'DELETE FROM `%s` WHERE `%s`=? limit 1' % (table, pk)
         return db.do_execute(sql, id)
 
     @classmethod
     def delete_by_ids(cls, ids: Iterable[int]):
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
-        pk, table = cls._get_pk_and_table(cls)
+        pk, table = cls._get_pk_and_table()
         sql = 'DELETE FROM `%s` WHERE `%s` in (%s) limit %d' % (table, pk, ','.join(list(map(str, ids))), ids_size)
         return db.do_execute(sql)
 
     @classmethod
     def logic_delete_by_id(cls, id: int, update_by: int = None):
-        pk, table = cls._get_pk_and_table(cls)
-        if update_by is None:
-            sql = 'UPDATE `%s` SET `del_flag`=1, `%s`=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (table, UPDATE_TIME, pk)
-            return db.do_execute(sql, id)
+        pk, table = cls._get_pk_and_table()
+        del_flag_col = cls._get_del_flag_col()
+        update_by_col = cls._get_update_by_col()
+        update_time_col = cls._get_update_time_col()
+
+        if update_by is None or update_by_col is None:
+            if update_time_col:
+                sql = 'UPDATE `%s` SET `%s`=?, `%s`=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (table, del_flag_col, update_time_col, pk)
+            else:
+                sql = 'UPDATE `%s` SET `%s`=? WHERE `%s`=? limit 1' % (table, del_flag_col, pk)
+            return db.do_execute(sql, 1, id)
         else:
-            sql = 'UPDATE `%s` SET `del_flag`=1, `update_by`=?, `%s`=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (table, UPDATE_TIME, pk)
-            return db.do_execute(sql, update_by, id)
+            if update_time_col:
+                sql = 'UPDATE `%s` SET `%s`=?, `%s`=?, `%s`=CURRENT_TIMESTAMP WHERE `%s`=? limit 1' % (table, del_flag_col, update_by_col, update_time_col, pk)
+            else:
+                sql = 'UPDATE `%s` SET `%s`=?, `%s`=? WHERE `%s`=? limit 1' % (table, del_flag_col, update_by_col, pk)
+            return db.do_execute(sql, 1, update_by, id)
 
     @classmethod
     def logic_delete_by_ids(cls, ids: Iterable[int], update_by: int = None):
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
-        pk, table = cls._get_pk_and_table(cls)
+
+        pk, table = cls._get_pk_and_table()
         ids_str = ','.join(list(map(str, ids)))
-        if update_by is None:
-            sql = 'UPDATE `%s` SET `del_flag`=1, `%s`=CURRENT_TIMESTAMP WHERE `%s` in (%s) limit %d' % (table, UPDATE_TIME, pk, ids_str, ids_size)
-            return db.execute(sql)
+        del_flag_col = cls._get_del_flag_col()
+        update_by_col = cls._get_update_by_col()
+        update_time_col = cls._get_update_time_col()
+
+        if update_by is None or update_by_col is None:
+            if update_time_col:
+                sql = 'UPDATE `%s` SET `%s`=?, `%s`=CURRENT_TIMESTAMP WHERE `%s` in (%s) limit %d' % (table, del_flag_col, update_time_col, pk, ids_str, ids_size)
+            else:
+                sql = 'UPDATE `%s` SET `%s`=?, WHERE `%s` in (%s) limit %d' % (table, del_flag_col, pk, ids_str, ids_size)
+            return db.execute(sql, 1)
         else:
-            sql = 'UPDATE `%s` SET `del_flag`=1, `update_by`=?, `%s`=CURRENT_TIMESTAMP WHERE `%s` in (%s) limit %d' % (table, UPDATE_TIME, pk, ids_str, ids_size)
-            return db.do_execute(sql, update_by)
+            if update_time_col:
+                sql = 'UPDATE `%s` SET `%s`=?, `%s`=?, `%s`=CURRENT_TIMESTAMP WHERE `%s` in (%s) limit %d' % (table, del_flag_col, update_by_col, update_time_col, pk, ids_str, ids_size)
+            else:
+                sql = 'UPDATE `%s` SET `%s`=?, `%s`=?, WHERE `%s` in (%s) limit %d' % (table, del_flag_col, update_by_col, pk, ids_str, ids_size)
+            return db.do_execute(sql, 1, update_by)
 
     @classmethod
     def find(cls, *selection, **kwargs):
         """
         Return list(object) or empty list if no result.
         """
-        pk, table = cls._get_pk_and_table(cls)
-        return [cls.dict2obj(d, cls, pk, table) for d in cls.select(*selection, **kwargs)]
+        pk, table = cls._get_pk_and_table()
+        return [cls._dict2obj(d) for d in cls.select(*selection, **kwargs)]
 
     @classmethod
     def select(cls, *selection, **kwargs):
         """
         Return list(dict) or empty list if no result.
         """
-        limit = kwargs.get('limit')
-        if limit:
-            del kwargs['limit']
+        where, args = '', []
+        if kwargs:
+            limit = kwargs.get('limit')
+            if limit:
+                del kwargs['limit']
+            where, args = _get_where_args(**kwargs)
         else:
             limit = 1000
 
-        where, args = _get_where_args(**kwargs)
-        pk, table = cls._get_pk_and_table(cls)
+        limit_str = 'limit %d' % limit if limit else ''
+        pk, table = cls._get_pk_and_table()
         if len(selection) == 0:
-            sql = 'SELECT * FROM `%s` %s limit %d' % (table, where, limit)
+            sql = 'SELECT * FROM `%s` %s %s' % (table, where, limit_str)
         else:
-            sql = 'SELECT %s FROM `%s` %s limit %d' % (','.join(['`%s`' % col for col in selection]), table, where, limit)
+            sql = 'SELECT %s FROM `%s` %s %s' % (','.join(['`%s`' % col for col in selection]), table, where, limit_str)
         return db.do_select(sql, *args)
 
-    @staticmethod
+    @classmethod
     def _get_pk_and_table(cls):
-        pk = cls._get_pk(cls)
-        table = cls._get_table(cls)
-        return pk, table
-
-    @staticmethod
-    def _get_pk(cls):
-        pk = cls.__dict__.get(PK)
-        return pk if pk else 'id'
+        assert hasattr(cls, PK), "%s not set attribute '%s'" % (cls.__name__, PK)
+        return cls.__pk__, cls._get_table()
 
-    @staticmethod
+    @classmethod
     def _get_table(cls):
-        table = cls.__dict__.get(TABLE)
-        return table if table else cls.__name__.lower()
+        assert hasattr(cls, TABLE), "%s not set attribute '%s'" % (cls.__name__, TABLE)
+        return cls.__table__
 
-    @staticmethod
-    def dict2obj(dictionary, cls, pk, table):
+    @classmethod
+    def _dict2obj(cls, dictionary):
         m = Model()
         m.__dict__.update(dictionary)
         m.__class__ = cls
-        if cls.__dict__.get(PK) is not None:
-            m.__pk__ = pk
-        if cls.__dict__.get(TABLE) is not None:
-            m. __table__ = table
         return m
+
+    @classmethod
+    def _get_update_by_col(cls):
+        if hasattr(cls, UPDATE_BY):
+            return cls.__update_by__
+        return None
+
+    @classmethod
+    def _get_update_time_col(cls):
+        if hasattr(cls, UPDATE_TIME):
+            return cls.__update_time__
+        return None
+
+    @classmethod
+    def _get_del_flag_col(cls):
+        assert hasattr(cls, DEL_FLAG), "%s not set attribute '%s'" % (cls.__name__, DEL_FLAG)
+        return cls.__del_flag__
```

### Comparing `mysqlx-1.1.9/README.md` & `mysqlx-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mysqlx-1.1.9/setup.py` & `mysqlx-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     packages=find_packages(),
     description="mysqlx is a simple python sql executor for MySQL like iBatis.",
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=3.0.3',
         'mysql-connector-python>=8.0.20',
     ],
-    version='1.1.9',
+    version='1.2.1',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'iBatis', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.txt'],
```

