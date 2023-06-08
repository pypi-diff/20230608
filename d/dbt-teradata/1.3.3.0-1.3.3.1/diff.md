# Comparing `tmp/dbt-teradata-1.3.3.0.tar.gz` & `tmp/dbt-teradata-1.3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-teradata-1.3.3.0.tar", last modified: Tue Apr 18 07:37:56 2023, max compression
+gzip compressed data, was "dbt-teradata-1.3.3.1.tar", last modified: Thu Jun  8 09:09:24 2023, max compression
```

## Comparing `dbt-teradata-1.3.3.0.tar` & `dbt-teradata-1.3.3.1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21235 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20969 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/adapters/teradata/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/adapters/teradata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 07:37:54.000000 dbt-teradata-1.3.3.0/dbt/adapters/teradata/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/adapters/teradata/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/adapters/teradata/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/adapters/teradata/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/adapters/teradata/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/teradata/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/incremental/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/seed/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/seed/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/snapshot/
--rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/test/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/test/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt_teradata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21235 2023-04-18 07:37:56.000000 dbt-teradata-1.3.3.0/dbt_teradata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-18 07:37:56.000000 dbt-teradata-1.3.3.0/dbt_teradata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:37:56.000000 dbt-teradata-1.3.3.0/dbt_teradata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 07:37:56.000000 dbt-teradata-1.3.3.0/dbt_teradata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-18 07:37:56.000000 dbt-teradata-1.3.3.0/dbt_teradata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-18 07:37:54.000000 dbt-teradata-1.3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20980 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.792976 dbt-teradata-1.3.3.1/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.792976 dbt-teradata-1.3.3.1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt/adapters/teradata/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/adapters/teradata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 09:09:21.000000 dbt-teradata-1.3.3.1/dbt/adapters/teradata/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/adapters/teradata/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/adapters/teradata/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/adapters/teradata/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/adapters/teradata/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.792976 dbt-teradata-1.3.3.1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt/include/teradata/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/columns.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.792976 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/incremental/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/seed/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/seed/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/test/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-08 09:08:44.000000 dbt-teradata-1.3.3.1/dbt/include/teradata/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/dbt_teradata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-06-08 09:09:24.000000 dbt-teradata-1.3.3.1/dbt_teradata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-08 09:09:24.000000 dbt-teradata-1.3.3.1/dbt_teradata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:09:24.000000 dbt-teradata-1.3.3.1/dbt_teradata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 09:09:24.000000 dbt-teradata-1.3.3.1/dbt_teradata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 09:09:24.000000 dbt-teradata-1.3.3.1/dbt_teradata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:09:24.796976 dbt-teradata-1.3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-08 09:09:21.000000 dbt-teradata-1.3.3.1/setup.py
```

### Comparing `dbt-teradata-1.3.3.0/LICENSE` & `dbt-teradata-1.3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.0/PKG-INFO` & `dbt-teradata-1.3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-teradata
-Version: 1.3.3.0
+Version: 1.3.3.1
 Summary: The Teradata adapter plugin for dbt (data build tool)
 Home-page: https://github.com/Teradata/dbt-teradata
 Author: Teradata Corporation
 Author-email: developers@teradata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -216,14 +216,15 @@
 * `ephemeral`
 * `incremental`
 
 #### Incremental Materialization
 The following incremental materialization strategies are supported:
 * `append` (default)
 * `delete+insert`
+* `merge`
 
 To learn more about dbt incremental strategies please check [the dbt incremental strategy documentation](https://docs.getdbt.com/docs/build/incremental-models#about-incremental_strategy).
 
 ### Commands
 
 All dbt commands are supported.
```

### Comparing `dbt-teradata-1.3.3.0/README.md` & `dbt-teradata-1.3.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -194,14 +194,15 @@
 * `ephemeral`
 * `incremental`
 
 #### Incremental Materialization
 The following incremental materialization strategies are supported:
 * `append` (default)
 * `delete+insert`
+* `merge`
 
 To learn more about dbt incremental strategies please check [the dbt incremental strategy documentation](https://docs.getdbt.com/docs/build/incremental-models#about-incremental_strategy).
 
 ### Commands
 
 All dbt commands are supported.
```

### Comparing `dbt-teradata-1.3.3.0/dbt/adapters/teradata/__init__.py` & `dbt-teradata-1.3.3.1/dbt/adapters/teradata/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.0/dbt/adapters/teradata/column.py` & `dbt-teradata-1.3.3.1/dbt/adapters/teradata/column.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.0/dbt/adapters/teradata/connections.py` & `dbt-teradata-1.3.3.1/dbt/adapters/teradata/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.0/dbt/adapters/teradata/impl.py` & `dbt-teradata-1.3.3.1/dbt/adapters/teradata/impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,8 +316,8 @@
                 grants_dict.update({privilege: [grantee]})
         return grants_dict
     
     def valid_incremental_strategies(self):
         """The set of standard builtin strategies which this adapter supports out-of-the-box.
         Not used to validate custom strategies defined by end users.
         """
-        return ["delete+insert","append"]
+        return ["delete+insert","append","merge"]
```

### Comparing `dbt-teradata-1.3.3.0/dbt/adapters/teradata/relation.py` & `dbt-teradata-1.3.3.1/dbt/adapters/teradata/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/adapters.sql` & `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/apply_grants.sql` & `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/catalog.sql` & `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/incremental/helpers.sql` & `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/incremental/helpers.sql`

 * *Files 10% similar despite different names*

```diff
@@ -3,26 +3,28 @@
   {%- set strategy = config.get("incremental_strategy") -%}
   {% if strategy == none %}
     {% set strategy = "append" %}
   {% endif %}
 
   {% set invalid_strategy_msg -%}
     Invalid incremental strategy provided: {{ strategy }}
-    Expected one of:  'append','delete+insert'
+    Expected one of:  'append','delete+insert','merge'
   {%- endset %}
-  {%- if strategy not in ['append','delete+insert'] %}
+  {%- if strategy not in ['append','delete+insert','merge'] %}
     {% do exceptions.raise_compiler_error(invalid_strategy_msg) %}
   {%- endif %}
 
   {% do return(strategy) %}
 {%- endmacro %}
 
 
-{% macro teradata__get_incremental_sql(strategy, target_relation, tmp_relation, unique_key, dest_columns) %}
+{% macro teradata__get_incremental_sql(strategy, target_relation, tmp_relation, unique_key, dest_columns,incremental_predicates) %}
   {% if strategy == 'delete+insert' %}
     {% do return(teradata__get_delete_insert_merge_sql(target_relation, tmp_relation, unique_key, dest_columns)) %}
   {% elif strategy == 'append' %}
     {% do return(teradata__get_incremental_append_sql(target_relation, tmp_relation,  dest_columns)) %}
+  {% elif strategy == 'merge' %}
+    {% do return(teradata__get_merge_sql(target_relation, tmp_relation, unique_key, dest_columns,incremental_predicates)) %}
   {% else %}
     {% do exceptions.raise_compiler_error("Invalid Strategy") %}
   {% endif %}
 {% endmacro %}
```

### Comparing `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/incremental/incremental.sql` & `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/incremental/incremental.sql`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,21 @@
 {% set target_relation = this.incorporate(type='table') %}
 {% set existing_relation = load_relation(this) %}
 {% set tmp_relation = make_temp_relation(this) %}
 
 -- {#-- Validate early so we don't run SQL if the strategy is invalid --#}
 {% set strategy = teradata__validate_get_incremental_strategy(config) %}
 
+{% set incremental_predicates = config.get('incremental_predicates', none) %}
+
 {% set on_schema_change = incremental_validate_on_schema_change(config.get('on_schema_change'), default='ignore') %}
 
+{%- set preexisting_tmp_relation = load_cached_relation(tmp_relation) -%}
+{{ drop_relation_if_exists(preexisting_tmp_relation) }}
+
 {{ run_hooks(pre_hooks, inside_transaction=False) }}
 
 -- `BEGIN` happens here:
 {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
 {% set to_drop = [] %}
 {% if existing_relation is none %}
@@ -40,15 +45,15 @@
 
    {% set dest_columns = process_schema_changes(on_schema_change, tmp_relation, existing_relation) %}
     {% if not dest_columns %}
         {%- set dest_columns = adapter.get_columns_in_relation(target_relation) -%}
     {% endif %}
 	
 	
-   {% set build_sql = teradata__get_incremental_sql(strategy, target_relation, tmp_relation, unique_key, dest_columns) %}
+   {% set build_sql = teradata__get_incremental_sql(strategy, target_relation, tmp_relation, unique_key, dest_columns,incremental_predicates) %}
 
 
    {% do to_drop.append(tmp_relation) %}
 {% endif %}
 
 {% call statement("main") %}
    {{ build_sql }}
```

### Comparing `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/seed/seed.sql` & `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql` & `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/test/test.sql` & `dbt-teradata-1.3.3.1/dbt/include/teradata/macros/materializations/test/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.3.0/dbt_teradata.egg-info/PKG-INFO` & `dbt-teradata-1.3.3.1/dbt_teradata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-teradata
-Version: 1.3.3.0
+Version: 1.3.3.1
 Summary: The Teradata adapter plugin for dbt (data build tool)
 Home-page: https://github.com/Teradata/dbt-teradata
 Author: Teradata Corporation
 Author-email: developers@teradata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -216,14 +216,15 @@
 * `ephemeral`
 * `incremental`
 
 #### Incremental Materialization
 The following incremental materialization strategies are supported:
 * `append` (default)
 * `delete+insert`
+* `merge`
 
 To learn more about dbt incremental strategies please check [the dbt incremental strategy documentation](https://docs.getdbt.com/docs/build/incremental-models#about-incremental_strategy).
 
 ### Commands
 
 All dbt commands are supported.
```

### Comparing `dbt-teradata-1.3.3.0/dbt_teradata.egg-info/SOURCES.txt` & `dbt-teradata-1.3.3.1/dbt_teradata.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 dbt/adapters/teradata/relation.py
 dbt/include/teradata/__init__.py
 dbt/include/teradata/dbt_project.yml
 dbt/include/teradata/sample_profiles.yml
 dbt/include/teradata/macros/adapters.sql
 dbt/include/teradata/macros/apply_grants.sql
 dbt/include/teradata/macros/catalog.sql
+dbt/include/teradata/macros/columns.sql
 dbt/include/teradata/macros/materializations/incremental/helpers.sql
 dbt/include/teradata/macros/materializations/incremental/incremental.sql
 dbt/include/teradata/macros/materializations/incremental/strategies.sql
 dbt/include/teradata/macros/materializations/seed/seed.sql
 dbt/include/teradata/macros/materializations/snapshot/snapshot.sql
 dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql
 dbt/include/teradata/macros/materializations/snapshot/strategies.sql
```

### Comparing `dbt-teradata-1.3.3.0/setup.py` & `dbt-teradata-1.3.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 package_name = "dbt-teradata"
-package_version = "1.3.3.0"
+package_version = "1.3.3.1"
 description = """The Teradata adapter plugin for dbt (data build tool)"""
 
 
 setup(
     name=package_name,
     version=package_version,
```

