# Comparing `tmp/mindsdb_sdk-1.0.2.tar.gz` & `tmp/mindsdb_sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mindsdb_sdk-1.0.2.tar", last modified: Thu Apr 13 15:09:53 2023, max compression
+gzip compressed data, was "dist/mindsdb_sdk-1.0.3.tar", last modified: Thu Jun  8 11:11:12 2023, max compression
```

## Comparing `mindsdb_sdk-1.0.2.tar` & `mindsdb_sdk-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:09:53.000000 mindsdb_sdk-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-13 15:09:53.000000 mindsdb_sdk-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:09:53.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)      407 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:09:53.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/connectors/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15842 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/mindsdb_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:09:53.000000 mindsdb_sdk-1.0.2/mindsdb_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-13 15:09:52.000000 mindsdb_sdk-1.0.2/mindsdb_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-13 15:09:53.000000 mindsdb_sdk-1.0.2/mindsdb_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:09:52.000000 mindsdb_sdk-1.0.2/mindsdb_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 15:09:52.000000 mindsdb_sdk-1.0.2/mindsdb_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 15:09:52.000000 mindsdb_sdk-1.0.2/mindsdb_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:09:53.000000 mindsdb_sdk-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-13 15:09:39.000000 mindsdb_sdk-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:11:12.000000 mindsdb_sdk-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 11:10:59.000000 mindsdb_sdk-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-08 11:11:12.000000 mindsdb_sdk-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-08 11:10:59.000000 mindsdb_sdk-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:11:12.000000 mindsdb_sdk-1.0.3/mindsdb_sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      407 2023-06-08 11:10:59.000000 mindsdb_sdk-1.0.3/mindsdb_sdk/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-08 11:10:59.000000 mindsdb_sdk-1.0.3/mindsdb_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:11:12.000000 mindsdb_sdk-1.0.3/mindsdb_sdk/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:10:59.000000 mindsdb_sdk-1.0.3/mindsdb_sdk/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-08 11:10:59.000000 mindsdb_sdk-1.0.3/mindsdb_sdk/connectors/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-08 11:10:59.000000 mindsdb_sdk-1.0.3/mindsdb_sdk/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-06-08 11:10:59.000000 mindsdb_sdk-1.0.3/mindsdb_sdk/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-06-08 11:10:59.000000 mindsdb_sdk-1.0.3/mindsdb_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-08 11:10:59.000000 mindsdb_sdk-1.0.3/mindsdb_sdk/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-06-08 11:10:59.000000 mindsdb_sdk-1.0.3/mindsdb_sdk/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-08 11:10:59.000000 mindsdb_sdk-1.0.3/mindsdb_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:11:12.000000 mindsdb_sdk-1.0.3/mindsdb_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-08 11:11:12.000000 mindsdb_sdk-1.0.3/mindsdb_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-08 11:11:12.000000 mindsdb_sdk-1.0.3/mindsdb_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:11:12.000000 mindsdb_sdk-1.0.3/mindsdb_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 11:11:12.000000 mindsdb_sdk-1.0.3/mindsdb_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 11:11:12.000000 mindsdb_sdk-1.0.3/mindsdb_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 11:10:59.000000 mindsdb_sdk-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:11:12.000000 mindsdb_sdk-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-08 11:10:59.000000 mindsdb_sdk-1.0.3/setup.py
```

### Comparing `mindsdb_sdk-1.0.2/mindsdb_sdk/__init__.py` & `mindsdb_sdk-1.0.3/mindsdb_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-1.0.2/mindsdb_sdk/connectors/rest_api.py` & `mindsdb_sdk-1.0.3/mindsdb_sdk/connectors/rest_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,17 +54,15 @@
             json = {'password': self.password, 'username': self.username}
             url = self.url + managed_endpoint
             r = self.session.post(url, json=json)
 
         r.raise_for_status()
 
     @_try_relogin
-    def sql_query(self, sql, database=None, lowercase_columns=False):
-        if database is None:
-            database = 'mindsdb'
+    def sql_query(self, sql, database='mindsdb', lowercase_columns=False):
         url = self.url + '/api/sql/query'
         r = self.session.post(url, json={
             'query': sql,
             'context': {'db': database}
         })
         r.raise_for_status()
```

### Comparing `mindsdb_sdk-1.0.2/mindsdb_sdk/database.py` & `mindsdb_sdk-1.0.3/mindsdb_sdk/database.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-1.0.2/mindsdb_sdk/model.py` & `mindsdb_sdk-1.0.3/mindsdb_sdk/model.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-1.0.2/mindsdb_sdk/project.py` & `mindsdb_sdk-1.0.3/mindsdb_sdk/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,34 +25,42 @@
         self.next_run_at = data['next_run_at']
         self.schedule_str = data['schedule_str']
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.name}, query='{self.query_str}')"
 
     def refresh(self):
+        """
+        Retrieve job data from mindsdb server
+        """
         job = self.project.get_job(self.name)
         self._update(job.data)
 
-    def get_history(self):
+    def get_history(self) -> pd.DataFrame:
+        """
+        Get history of job execution
+
+        :return: dataframe with job executions
+        """
         ast_query = Select(
             targets=[Star()],
             from_table=Identifier('jobs_history'),
             where=dict_to_binary_op({
                 'name': self.name
             })
         )
         return self.project.api.sql_query(ast_query.to_string(), database=self.project.name)
 
 
 class Project:
     """
     Allows to work with project: to manage models and views inside of it or call raw queries inside of project
 
-    Queries
-    ----------
+    **Queries**
+
     Making prediciton using sql:
 
     >>> query = project.query('select * from database.table join model1')
     >>> df = query.fetch()
 
     Making time series prediction:
 
@@ -61,16 +69,16 @@
     ...     FROM mindsdb.house_sales_model as m
     ...     JOIN example_db.demo_data.house_sales as t
     ...     WHERE t.saledate > LATEST AND t.type = 'house'
     ...     AND t.bedrooms=2
     ...     LIMIT 4;
     ...    ''').fetch()
 
-    Views
-    ----------
+    **Views**
+
     Get:
 
     >>> views = project.list_views()
     >>> view = views[0]
 
     By name:
 
@@ -98,16 +106,15 @@
     >>> df = view.fetch()
 
     Drop view:
 
     >>> project.drop_view('view1')
 
 
-    Models
-    ----------
+    **Models**
 
     Get:
 
     >>> models = project.list_models()
     >>> model = models[0]
 
     Get version:
@@ -189,15 +196,15 @@
     ...   JOIN example_db.demo_data.house_sales as t
     ...  WHERE t.saledate > LATEST AND t.type = 'house'
     ...   AND t.bedrooms=2
     ...  LIMIT 4;
     ...''').fetch()
 
 
-    Model managing
+    **Model managing**
 
     Fine-tuning
 
     >>> model.finetune(query)
     >>> model.finetune('select * from demo_data.house_sales', database='example_db')
     >>> model.finetune(query, params={'x': 2})
```

### Comparing `mindsdb_sdk-1.0.2/mindsdb_sdk/query.py` & `mindsdb_sdk-1.0.3/mindsdb_sdk/query.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-1.0.2/mindsdb_sdk/server.py` & `mindsdb_sdk-1.0.3/mindsdb_sdk/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
 from mindsdb_sql.parser.dialects.mindsdb import CreateDatabase
-from mindsdb_sql.parser.ast import DropDatabase
+from mindsdb_sql.parser.ast import DropDatabase, Identifier
 
 from mindsdb_sdk.connectors.rest_api import RestAPI
 from .database import Database
 from .project import Project
 
 
 class Server:
@@ -84,15 +84,15 @@
 
         :param name: Identifier for the integration to be created
         :param engine: Engine to be selected depending on the database connection.
         :param connection_args: {"key": "value"} object with the connection parameters specific for each engine
         :return: created Database object
         """
         ast_query = CreateDatabase(
-            name=name,
+            name=Identifier(name),
             engine=engine,
             parameters=connection_args,
         )
         self.api.sql_query(ast_query.to_string())
         return Database(self, name)
 
     def drop_database(self, name: str):
@@ -133,15 +133,15 @@
         Create new project and return it
 
         :param name: name of the project
         :return: Project object
         """
 
         ast_query = CreateDatabase(
-            name=name,
+            name=Identifier(name),
             engine='mindsdb',
             parameters={}
         )
 
         self.api.sql_query(ast_query.to_string())
         return Project(self, name)
 
@@ -158,9 +158,9 @@
         """
         Get Project by name
 
         :param name: name of project
         :return: Project object
         """
         if name not in self._list_projects():
-            raise AttributeError("Database doesn't exist")
+            raise AttributeError("Project doesn't exist")
         return Project(self, name)
```

### Comparing `mindsdb_sdk-1.0.2/setup.py` & `mindsdb_sdk-1.0.3/setup.py`

 * *Files identical despite different names*

