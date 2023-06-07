# Comparing `tmp/sqbased-0.1.0.tar.gz` & `tmp/sqbased-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqbased-0.1.0.tar", max compression
+gzip compressed data, was "sqbased-0.1.2.tar", max compression
```

## Comparing `sqbased-0.1.0.tar` & `sqbased-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       73 2023-06-07 18:49:35.588559 sqbased-0.1.0/README.md
--rw-r--r--   0        0        0      397 2023-06-07 20:25:13.260467 sqbased-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8121 2023-06-07 21:03:08.590463 sqbased-0.1.0/sqbased/__main__.py
--rw-r--r--   0        0        0      611 1970-01-01 00:00:00.000000 sqbased-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      261 2023-06-07 21:04:28.756811 sqbased-0.1.2/README.md
+-rw-r--r--   0        0        0      397 2023-06-07 22:47:35.563336 sqbased-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     8555 2023-06-07 22:47:22.340048 sqbased-0.1.2/sqbased/__main__.py
+-rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 sqbased-0.1.2/PKG-INFO
```

### Comparing `sqbased-0.1.0/sqbased/__main__.py` & `sqbased-0.1.2/sqbased/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,18 @@
         cursor.execute(f"SELECT COUNT(*) FROM {table[0]};")
         row_count = cursor.fetchone()[0]
         logger.info(f"    rows: {row_count}")
 
         # get the size of just this table using dbstat
         cursor.execute(f"SELECT SUM(pgsize) FROM dbstat WHERE name='{table[0]}';")
         table_size = cursor.fetchone()[0]
-        logger.info(f"    size: {friendly_size(table_size)}")
+        if table_size:
+            logger.info(f"    size: {friendly_size(table_size)}")
+        else:
+            logger.info(f"    size: unknown")
 
 
 @app.command("vacuum", help="vacuum a database for optimal layout")
 def vacuum(
     db_file_in: str = typer.Argument(..., help="Input database file to use"),
     db_file_out: str = typer.Argument(..., help="Output database file to use"),
 ):
@@ -108,14 +111,19 @@
         help="Columns to create fts5 index on. Defaults to all text columns.",
     ),
     drop_original: bool = typer.Option(
         False,
         "--drop-original",
         help="Drop the original table after creating the fts5 table.",
     ),
+    vacuum: bool = typer.Option(
+        False,
+        "--vacuum",
+        help="Vacuum the database after creating the fts5 table.",
+    ),
 ):
     if db_file_in != db_file_out:
         logger.info(f"copying database: {db_file_in} -> {db_file_out}")
         shutil.copyfile(db_file_in, db_file_out)
 
     logger.info(f"opening database: {db_file_out}")
     conn = sqlite3.connect(db_file_out)
@@ -163,37 +171,39 @@
             column
             for column, column_type in zip(table_columns, table_column_types)
             if (column_type == "text" or "VARCHAR" in column_type)
         ]
 
     logger.info(f"  fts columns: {fts_columns}")
 
-    # create the fts5 table
+    # create the fts5 table, with external content
     fts_columns_str = ", ".join(fts_columns)
     conn.execute(
-        f"CREATE VIRTUAL TABLE {fts_table_name} USING fts5({fts_columns_str});"
+        f"CREATE VIRTUAL TABLE {fts_table_name} USING fts5({fts_columns_str}, content={table_name});"
     )
+    # this can be queried as such:
+    # SELECT * FROM mytable WHERE ROWID IN (SELECT ROWID FROM mytable_fts5 WHERE mytable_fts5 MATCH 'some query') LIMIT 10;
     conn.commit()
 
     # insert the data from the input table into the fts5 table
     logger.info(f"coping data from {table_name} -> {fts_table_name}")
     conn.execute(
         f"INSERT INTO {fts_table_name}({fts_columns_str}) SELECT {fts_columns_str} FROM {table_name};"
     )
     conn.commit()
 
     if drop_original:
         logger.warn(f"dropping original table: {table_name}")
         conn.execute(f"DROP TABLE {table_name};")
         conn.commit()
 
-    # vacuum the database
-    logger.info("vacuuming database")
-    conn.execute("VACUUM;")
-    conn.commit()
+    if vacuum:
+        logger.info("vacuuming database")
+        conn.execute("VACUUM;")
+        conn.commit()
 
 
 @app.command("copytables", help="copy tables from one database to another")
 def copytables(
     db_file_in: str = typer.Argument(..., help="Input database file to use"),
     db_file_out: str = typer.Argument(..., help="Output database file to use"),
     tables: List[str] = typer.Argument(..., help="Tables to copy"),
```

