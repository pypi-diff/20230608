# Comparing `tmp/databudgie-2.7.5.tar.gz` & `tmp/databudgie-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databudgie-2.7.5.tar", max compression
+gzip compressed data, was "databudgie-2.8.1.tar", max compression
```

## Comparing `databudgie-2.7.5.tar` & `databudgie-2.8.1.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0     5139 2023-04-21 19:04:42.269454 databudgie-2.7.5/CHANGELOG.md
--rw-r--r--   0        0        0     1973 2023-04-21 19:04:42.269454 databudgie-2.7.5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1053 2023-04-21 19:04:42.269454 databudgie-2.7.5/LICENSE
--rw-r--r--   0        0        0     1292 2023-04-21 19:04:42.269454 databudgie-2.7.5/README.md
--rw-r--r--   0        0        0     2879 2023-04-21 19:04:42.269454 databudgie-2.7.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 19:04:42.269454 databudgie-2.7.5/src/databudgie/__init__.py
--rw-r--r--   0        0        0       69 2023-04-21 19:04:42.269454 databudgie-2.7.5/src/databudgie/__main__.py
--rw-r--r--   0        0        0       74 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/adapter/__init__.py
--rw-r--r--   0        0        0     7162 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/adapter/base.py
--rw-r--r--   0        0        0    10638 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/adapter/postgres.py
--rw-r--r--   0        0        0     7361 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/backup.py
--rw-r--r--   0        0        0      105 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/cli/__init__.py
--rw-r--r--   0        0        0     2896 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/cli/base.py
--rw-r--r--   0        0        0     6458 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/cli/commands.py
--rw-r--r--   0        0        0     1473 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/cli/config.py
--rw-r--r--   0        0        0      456 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/cli/setup.py
--rw-r--r--   0        0        0     1112 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/compression.py
--rw-r--r--   0        0        0    11862 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/config.py
--rw-r--r--   0        0        0      105 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/manifest/__init__.py
--rw-r--r--   0        0        0     2348 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/manifest/manager.py
--rw-r--r--   0        0        0     1602 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/manifest/sqlalchemy.py
--rw-r--r--   0        0        0      565 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/match.py
--rw-r--r--   0        0        0     1564 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/output.py
--rw-r--r--   0        0        0        0 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/py.typed
--rw-r--r--   0        0        0     8408 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/restore.py
--rw-r--r--   0        0        0     1948 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/s3.py
--rw-r--r--   0        0        0    11806 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/storage.py
--rw-r--r--   0        0        0     4586 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/table_op.py
--rw-r--r--   0        0        0     2462 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/utils.py
--rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 databudgie-2.7.5/setup.py
--rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 databudgie-2.7.5/PKG-INFO
+-rw-r--r--   0        0        0     5139 2023-06-08 20:35:22.217064 databudgie-2.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1973 2023-06-08 20:35:22.217064 databudgie-2.8.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1053 2023-06-08 20:35:22.217064 databudgie-2.8.1/LICENSE
+-rw-r--r--   0        0        0     1310 2023-06-08 20:35:22.217064 databudgie-2.8.1/README.md
+-rw-r--r--   0        0        0     2883 2023-06-08 20:35:22.221064 databudgie-2.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/__init__.py
+-rw-r--r--   0        0        0       69 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/__main__.py
+-rw-r--r--   0        0        0       74 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/adapter/__init__.py
+-rw-r--r--   0        0        0     7162 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/adapter/base.py
+-rw-r--r--   0        0        0    10638 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/adapter/postgres.py
+-rw-r--r--   0        0        0     7361 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/backup.py
+-rw-r--r--   0        0        0      105 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/cli/__init__.py
+-rw-r--r--   0        0        0     2896 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/cli/base.py
+-rw-r--r--   0        0        0     6733 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/cli/commands.py
+-rw-r--r--   0        0        0     4696 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/cli/config.py
+-rw-r--r--   0        0        0     1112 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/compression.py
+-rw-r--r--   0        0        0    11307 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/config.py
+-rw-r--r--   0        0        0      105 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/manifest/__init__.py
+-rw-r--r--   0        0        0     2348 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/manifest/manager.py
+-rw-r--r--   0        0        0     1602 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/manifest/sqlalchemy.py
+-rw-r--r--   0        0        0      565 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/match.py
+-rw-r--r--   0        0        0     1564 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/output.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/py.typed
+-rw-r--r--   0        0        0     8408 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/restore.py
+-rw-r--r--   0        0        0     1948 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/s3.py
+-rw-r--r--   0        0        0    11806 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/storage.py
+-rw-r--r--   0        0        0     4586 2023-06-08 20:35:22.221064 databudgie-2.8.1/src/databudgie/table_op.py
+-rw-r--r--   0        0        0     2462 2023-06-08 20:35:22.225065 databudgie-2.8.1/src/databudgie/utils.py
+-rw-r--r--   0        0        0     2580 1970-01-01 00:00:00.000000 databudgie-2.8.1/setup.py
+-rw-r--r--   0        0        0     2653 1970-01-01 00:00:00.000000 databudgie-2.8.1/PKG-INFO
```

### Comparing `databudgie-2.7.5/CHANGELOG.md` & `databudgie-2.8.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/CONTRIBUTING.md` & `databudgie-2.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/LICENSE` & `databudgie-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/README.md` & `databudgie-2.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 ![Github Actions Build](https://github.com/schireson/databudgie/actions/workflows/build.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/schireson/databudgie/badge.svg?branch=main&t=6I0aU6)](https://coveralls.io/github/schireson/databudgie?branch=main)
 [![Documentation
 Status](https://readthedocs.org/projects/databudgie/badge/?version=latest)](https://databudgie.readthedocs.io)
 
 ![](docs/source/_static/databudgie.png)
 
-Databudgie is a CLI & library for database performing targeted backup and restore
-of database tables or arbitrary queries against database tables.
+Databudgie is a CLI & library for database performing targeted backup and
+restore of database tables or arbitrary queries against database tables.
 
 # Usage
 
 A minimal config file might look like:
 
 ```yaml
-# config.databudgie.yml
+# databudgie.yml or config.databudgie.yml
 backup:
   url: postgresql://postgres:postgres@localhost:5432/postgres
   tables:
     - name: public.product
       query: "select * from {table} where store_id > 4"
       location: s3://my-s3-bucket/databudgie/public.product
 restore:
   url: postgresql://postgres:postgres@localhost:5432/postgres
   tables:
     - name: public.product
       location: s3://my-s3-bucket/databudgie/public.product
 ```
 
-With that config in place, backing up the defined tables (using the specified config)
-is as simple as `databudgie backup`; and restore `databudgie restore`.
+With that config in place, backing up the defined tables (using the specified
+config) is as simple as `databudgie backup`; and restore `databudgie restore`.
 
 ## Installation
 
 ```bash
 pip install databudgie
 ```
```

### Comparing `databudgie-2.7.5/pyproject.toml` & `databudgie-2.8.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databudgie"
-version = "2.7.5"
+version = "2.8.1"
 packages = [
     { include = "databudgie", from = "src" },
 ]
 
 authors = [
   "Andrew Sosa <andrewso@known.is>",
   "Dan Cardin <ddcardin@gmail.com>",
@@ -34,20 +34,18 @@
 sqlalchemy = ">=1.3"
 strapp = {version = ">=0.2.7", extras = ["click", "sqlalchemy"] }
 click = ">=7.0.0"
 typing-extensions = {version = ">=3.10.0", python = "<3.8"}
 importlib-metadata = {version = "*", python = "<3.8"}
 
 boto3 = { version = "*", optional = true }
-sentry-sdk = { version = "*", optional = true }
 psycopg2 = { version = ">=2.7", optional = true }
 psycopg2-binary = { version = ">=2.7", optional = true }
 
 [tool.poetry.extras]
-sentry = ["sentry-sdk"]
 s3 = ["boto3"]
 psycopg2 = ["psycopg2"]
 psycopg2-binary = ["psycopg2-binary"]
 
 [tool.poetry.dev-dependencies]
 boto3 = "^1.16.10,<1.17.72"
 black = "22.3.0"
@@ -79,14 +77,18 @@
 
 [tool.mypy]
 strict_optional = true
 ignore_missing_imports = true
 warn_unused_ignores = true
 incremental = true
 
+[[tool.mypy.overrides]]
+module = 'tests.mockmodels.*'
+ignore_errors = true
+
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 exclude_lines = [
   "pragma: no cover",
   "if TYPE_CHECKING:",
   "if __name__ == .__main__.:",
```

### Comparing `databudgie-2.7.5/src/databudgie/adapter/base.py` & `databudgie-2.8.1/src/databudgie/adapter/base.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/src/databudgie/adapter/postgres.py` & `databudgie-2.8.1/src/databudgie/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/src/databudgie/backup.py` & `databudgie-2.8.1/src/databudgie/backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
                 backup(
                     table_op=table_op,
                     storage=storage,
                     adapter=adapter,
                     console=console,
                 )
 
-    console.info("Finished Backing up tables")
+    console.info("Finished backing up tables")
 
 
 def backup(
     *,
     table_op: TableOp[BackupTableConfig],
     adapter: Adapter,
     storage: StorageBackend,
```

### Comparing `databudgie-2.7.5/src/databudgie/cli/base.py` & `databudgie-2.8.1/src/databudgie/cli/base.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/src/databudgie/cli/commands.py` & `databudgie-2.8.1/src/databudgie/cli/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 
 import click
 from sqlalchemy.orm import Session
 
 from databudgie.cli.base import resolver
 from databudgie.cli.config import (
     CliConfig,
-    DEFAULT_CONFIG_FILE,
-    load_configs,
+    collect_config,
+    loaders,
     pretty_print,
 )
 from databudgie.config import (
     BackupConfig,
     ConfigError,
-    ConfigStack,
     RestoreConfig,
     RootConfig,
 )
 from databudgie.manifest.manager import Manifest
 from databudgie.output import Console
 from databudgie.storage import StorageBackend
 
@@ -29,25 +28,25 @@
 @click.option(
     "-a",
     "--adapter",
     default=None,
     type=click.Choice(["postgres", "postgresql", "python"], case_sensitive=False),
     help="Override the automatic dialect detection.",
 )
-@click.option("-c", "--config", default=[DEFAULT_CONFIG_FILE], help="config file", multiple=True)
+@click.option("-c", "--config", default=None, help="config file", multiple=True)
 @click.option(
     "-C",
     "--conn",
     "--connection",
     default=None,
     help="The name of a named connection to use. Takes precedence over the 'url' field if present.",
 )
 @click.option("-v", "--verbose", count=True, default=0)
 @click.option(
-    "--ddl", default=None, is_flag=True, help="Whether to backup the DDL. Overrides the config option, if set"
+    "--ddl/--no-ddl", default=None, is_flag=True, help="Whether to backup the DDL. Overrides the config option, if set"
 )
 @click.option("-u", "--url", default=None, help="The url used to connect to the database.")
 @click.option("-l", "--location", default=None, help="The location to read/write backups from/to.")
 @click.option(
     "-t",
     "--table",
     default=None,
@@ -69,14 +68,25 @@
 )
 @click.option(
     "--dry-run/--no-dry-run",
     default=None,
     is_flag=True,
     help="Do not actually perform the write operations of the backup/restore. It **does**, however, execute the queries.",
 )
+@click.option(
+    "--raw-config",
+    default=None,
+    help="Accepts raw config as a string, rather than searching a file for it.",
+)
+@click.option(
+    "--raw-config-format",
+    default="json",
+    help="The assumed format of --raw-config. Defaults to `json`. Must be one of: `yml`, `yaml`, `json`, `toml`.",
+    type=click.Choice(loaders),
+)
 @click.version_option()
 def cli(
     strict: bool,
     config: Iterable[str],
     verbose: int = 0,
     color: bool = True,
     conn: Optional[str] = None,
@@ -84,14 +94,16 @@
     ddl: Optional[bool] = None,
     url: Optional[str] = None,
     table: Optional[Tuple[str, ...]] = None,
     exclude: Optional[Tuple[str, ...]] = None,
     location: Optional[str] = None,
     dry_run: bool = False,
     stats: bool = False,
+    raw_config: Optional[str] = None,
+    raw_config_format: str = "json",
 ):
     if color is False:
         os.environ["NO_COLOR"] = "true"
 
     if conn and url:
         raise click.UsageError("--url and --connection are mutually exclusive options")
 
@@ -101,19 +113,21 @@
         exclude=list(exclude) if exclude else None,
         url=url,
         location=location,
         adapter=adapter,
         strict=strict,
     )
 
-    configs = load_configs(config)
-    config_stack = ConfigStack(cli_config.to_dict(), *configs)
-
     try:
-        root_config = RootConfig.from_stack(config_stack)
+        root_config = collect_config(
+            cli_config=cli_config,
+            file_names=config,
+            raw_config=raw_config,
+            raw_config_format=raw_config_format,
+        )
     except ConfigError as e:
         raise click.UsageError(*e.args)
 
     resolver.register_values(
         root_config=root_config,
         verbosity=verbose,
         console=Console(verbosity=verbose),
@@ -132,17 +146,14 @@
     backup_manifest: Optional[Manifest] = None,
     backup_id: Optional[int] = None,
     stats: bool = False,
     dry_run: bool = False,
 ):
     """Perform backup."""
     from databudgie.backup import backup_all
-    from databudgie.cli.setup import setup
-
-    setup(backup_config.sentry)
 
     if backup_manifest and backup_id:
         backup_manifest.set_transaction_id(backup_id)
 
     storage = StorageBackend.from_config(
         backup_config,
         manifest=backup_manifest,
@@ -183,19 +194,16 @@
     restore_id: Optional[int] = None,
     clean: Optional[bool] = None,
     yes: bool = False,
     stats: bool = False,
     dry_run: bool = False,
 ):
     """Perform restore."""
-    from databudgie.cli.setup import setup
     from databudgie.restore import restore_all
 
-    setup(restore_config.sentry)
-
     if restore_manifest and restore_id:
         restore_manifest.set_transaction_id(restore_id)
 
     restore_config.ddl.clean = clean or restore_config.ddl.clean
 
     if not yes and restore_config.ddl.clean:
         message = "About to delete the database! input 'y' if that's what you want: "
```

### Comparing `databudgie-2.7.5/src/databudgie/compression.py` & `databudgie-2.8.1/src/databudgie/compression.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/src/databudgie/config.py` & `databudgie-2.8.1/src/databudgie/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,26 +78,29 @@
 class DDLConfig(Config):
     enabled: bool = False
     location: str = "backups/ddl"
     clean: bool = False
     strategy: str = "use_latest_filename"
 
     @classmethod
-    def from_dict(cls, ddl_config: dict | bool, root_location: str | None = None):
-        if isinstance(ddl_config, bool):
-            expanded_ddl_config: dict[str, Any] = {"enabled": ddl_config}
+    def from_dict(cls, ddl_config: dict | bool | str, root_location: str | None = None):
+        if isinstance(ddl_config, (bool, str)):
+            expanded_ddl_config: dict[str, Any] = {"enabled": bool(ddl_config)}
         else:
             expanded_ddl_config = ddl_config
 
         location = compose_root_location(root_location, expanded_ddl_config.get("location"), default="backups/ddl")
 
         # Splat into a new dict so we can override `location` without mutating
         # the original input (which may be re-read later in config parsing)
         final_ddl_config = {**expanded_ddl_config, "location": location}
 
+        if "clean" in final_ddl_config:
+            final_ddl_config["clean"] = bool(final_ddl_config["clean"])
+
         return from_partial(cls, **final_ddl_config)
 
 
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 # Core configuration models
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
@@ -128,15 +131,14 @@
     connections: dict[str, Connection]
     ddl: DDLConfig
 
     connection: Connection | None = None
     manifest: str | None = None
 
     s3: S3Config | None = None
-    sentry: SentryConfig | None = None
     root_location: str | None = None
     adapter: str | None = None
 
     @classmethod
     @abc.abstractmethod
     def get_child_class(cls):
         pass
@@ -153,26 +155,24 @@
         # manifest defauls to None
         manifest: str | None = stack.get("manifest")
 
         ddl = DDLConfig.from_dict(stack.get("ddl", {}), root_location)
 
         # Optional integration configs
         s3 = S3Config.from_dict(stack.get("s3"))
-        sentry = SentryConfig.from_dict(stack.get("sentry"))
 
         adapter = stack.get("adapter")
 
         connections = Connection.from_collection(stack.get("connections"))
 
         return cls(
             connection=connection,
             tables=tables,
             manifest=manifest,
             s3=s3,
-            sentry=sentry,
             ddl=ddl,
             root_location=root_location,
             adapter=adapter,
             connections=connections,
         )
 
 
@@ -247,19 +247,19 @@
         return from_partial(
             cls,
             name=stack.get("name"),
             location=location,
             query=stack.get("query"),
             compression=stack.get("compression"),
             exclude=stack.get("exclude"),
-            sequences=stack.get("sequences", True),
-            data=stack.get("data", True),
-            ddl=stack.get("ddl", True),
-            follow_foreign_keys=stack.get("follow_foreign_keys", False),
-            strict=stack.get("strict", False),
+            sequences=bool(stack.get("sequences", True)),
+            data=bool(stack.get("data", True)),
+            ddl=bool(ddl),
+            follow_foreign_keys=bool(stack.get("follow_foreign_keys", False)),
+            strict=bool(stack.get("strict", False)),
         )
 
 
 @dataclass
 class BackupConfig(TableParentConfig[BackupTableConfig]):
     @classmethod
     def get_child_class(cls):
@@ -292,19 +292,19 @@
             cls,
             name=stack.get("name"),
             location=location,
             strategy=stack.get("strategy"),
             truncate=stack.get("truncate"),
             compression=stack.get("compression"),
             exclude=stack.get("exclude"),
-            sequences=stack.get("sequences", True),
-            data=stack.get("data", True),
-            ddl=stack.get("ddl", True),
-            follow_foreign_keys=stack.get("follow_foreign_keys", False),
-            strict=stack.get("strict", False),
+            sequences=bool(stack.get("sequences", True)),
+            data=bool(stack.get("data", True)),
+            ddl=bool(ddl),
+            follow_foreign_keys=bool(stack.get("follow_foreign_keys", False)),
+            strict=bool(stack.get("strict", False)),
         )
 
 
 @dataclass
 class RestoreConfig(TableParentConfig[RestoreTableConfig]):
     @classmethod
     def get_child_class(cls):
@@ -332,37 +332,14 @@
 
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 # Optional Integration configs which do NOT have default values built-in
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 @dataclass
-class SentryConfig(Config):
-    """Configuration for Sentry integration.
-
-    SentryConfig does not inherit keys from the root config.
-    """
-
-    dsn: str | None = None
-    environment: str | None = None
-    version: str | None = None
-
-    @classmethod
-    def from_dict(cls, sentry_config: dict | None) -> SentryConfig | None:
-        if sentry_config is None:
-            return None
-
-        return cls(
-            dsn=sentry_config.get("dsn"),
-            environment=sentry_config.get("environment"),
-            version=sentry_config.get("version"),
-        )
-
-
-@dataclass
 class S3Config(Config):
     aws_access_key_id: str | None = None
     aws_secret_access_key: str | None = None
     region: str | None = None
     profile: str | None = None
 
     @classmethod
```

### Comparing `databudgie-2.7.5/src/databudgie/manifest/manager.py` & `databudgie-2.8.1/src/databudgie/manifest/manager.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/src/databudgie/manifest/sqlalchemy.py` & `databudgie-2.8.1/src/databudgie/manifest/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/src/databudgie/match.py` & `databudgie-2.8.1/src/databudgie/match.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/src/databudgie/output.py` & `databudgie-2.8.1/src/databudgie/output.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/src/databudgie/restore.py` & `databudgie-2.8.1/src/databudgie/restore.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/src/databudgie/s3.py` & `databudgie-2.8.1/src/databudgie/s3.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/src/databudgie/storage.py` & `databudgie-2.8.1/src/databudgie/storage.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/src/databudgie/table_op.py` & `databudgie-2.8.1/src/databudgie/table_op.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/src/databudgie/utils.py` & `databudgie-2.8.1/src/databudgie/utils.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.5/setup.py` & `databudgie-2.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,24 @@
  'sqlalchemy>=1.3',
  'strapp[click,sqlalchemy]>=0.2.7']
 
 extras_require = \
 {':python_version < "3.8"': ['typing-extensions>=3.10.0', 'importlib-metadata'],
  'psycopg2': ['psycopg2>=2.7'],
  'psycopg2-binary': ['psycopg2-binary>=2.7'],
- 's3': ['boto3'],
- 'sentry': ['sentry-sdk']}
+ 's3': ['boto3']}
 
 entry_points = \
 {'console_scripts': ['databudgie = databudgie.__main__:run']}
 
 setup_kwargs = {
     'name': 'databudgie',
-    'version': '2.7.5',
+    'version': '2.8.1',
     'description': 'Ergonomic and flexible tool for database backup and restore',
-    'long_description': '# Databudgie\n\n![Github Actions Build](https://github.com/schireson/databudgie/actions/workflows/build.yml/badge.svg)\n[![Coverage Status](https://coveralls.io/repos/github/schireson/databudgie/badge.svg?branch=main&t=6I0aU6)](https://coveralls.io/github/schireson/databudgie?branch=main)\n[![Documentation\nStatus](https://readthedocs.org/projects/databudgie/badge/?version=latest)](https://databudgie.readthedocs.io)\n\n![](docs/source/_static/databudgie.png)\n\nDatabudgie is a CLI & library for database performing targeted backup and restore\nof database tables or arbitrary queries against database tables.\n\n# Usage\n\nA minimal config file might look like:\n\n```yaml\n# config.databudgie.yml\nbackup:\n  url: postgresql://postgres:postgres@localhost:5432/postgres\n  tables:\n    - name: public.product\n      query: "select * from {table} where store_id > 4"\n      location: s3://my-s3-bucket/databudgie/public.product\nrestore:\n  url: postgresql://postgres:postgres@localhost:5432/postgres\n  tables:\n    - name: public.product\n      location: s3://my-s3-bucket/databudgie/public.product\n```\n\nWith that config in place, backing up the defined tables (using the specified config)\nis as simple as `databudgie backup`; and restore `databudgie restore`.\n\n## Installation\n\n```bash\npip install databudgie\n```\n',
+    'long_description': '# Databudgie\n\n![Github Actions Build](https://github.com/schireson/databudgie/actions/workflows/build.yml/badge.svg)\n[![Coverage Status](https://coveralls.io/repos/github/schireson/databudgie/badge.svg?branch=main&t=6I0aU6)](https://coveralls.io/github/schireson/databudgie?branch=main)\n[![Documentation\nStatus](https://readthedocs.org/projects/databudgie/badge/?version=latest)](https://databudgie.readthedocs.io)\n\n![](docs/source/_static/databudgie.png)\n\nDatabudgie is a CLI & library for database performing targeted backup and\nrestore of database tables or arbitrary queries against database tables.\n\n# Usage\n\nA minimal config file might look like:\n\n```yaml\n# databudgie.yml or config.databudgie.yml\nbackup:\n  url: postgresql://postgres:postgres@localhost:5432/postgres\n  tables:\n    - name: public.product\n      query: "select * from {table} where store_id > 4"\n      location: s3://my-s3-bucket/databudgie/public.product\nrestore:\n  url: postgresql://postgres:postgres@localhost:5432/postgres\n  tables:\n    - name: public.product\n      location: s3://my-s3-bucket/databudgie/public.product\n```\n\nWith that config in place, backing up the defined tables (using the specified\nconfig) is as simple as `databudgie backup`; and restore `databudgie restore`.\n\n## Installation\n\n```bash\npip install databudgie\n```\n',
     'author': 'Andrew Sosa',
     'author_email': 'andrewso@known.is',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/schireson/databudgie',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `databudgie-2.7.5/PKG-INFO` & `databudgie-2.8.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databudgie
-Version: 2.7.5
+Version: 2.8.1
 Summary: Ergonomic and flexible tool for database backup and restore
 Home-page: https://github.com/schireson/databudgie
 License: MIT
 Keywords: sqlalchemy,postgres,database,etl,s3
 Author: Andrew Sosa
 Author-email: andrewso@known.is
 Requires-Python: >=3.7,<4
@@ -15,23 +15,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Archiving :: Backup
 Provides-Extra: psycopg2
 Provides-Extra: psycopg2-binary
 Provides-Extra: s3
-Provides-Extra: sentry
 Requires-Dist: boto3; extra == "s3"
 Requires-Dist: click (>=7.0.0)
 Requires-Dist: configly[yaml]
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: psycopg2 (>=2.7); extra == "psycopg2"
 Requires-Dist: psycopg2-binary (>=2.7); extra == "psycopg2-binary"
 Requires-Dist: rich
-Requires-Dist: sentry-sdk; extra == "sentry"
 Requires-Dist: sqlalchemy (>=1.3)
 Requires-Dist: strapp[click,sqlalchemy] (>=0.2.7)
 Requires-Dist: typing-extensions (>=3.10.0); python_version < "3.8"
 Project-URL: Repository, https://github.com/schireson/databudgie
 Description-Content-Type: text/markdown
 
 # Databudgie
@@ -39,38 +37,38 @@
 ![Github Actions Build](https://github.com/schireson/databudgie/actions/workflows/build.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/schireson/databudgie/badge.svg?branch=main&t=6I0aU6)](https://coveralls.io/github/schireson/databudgie?branch=main)
 [![Documentation
 Status](https://readthedocs.org/projects/databudgie/badge/?version=latest)](https://databudgie.readthedocs.io)
 
 ![](docs/source/_static/databudgie.png)
 
-Databudgie is a CLI & library for database performing targeted backup and restore
-of database tables or arbitrary queries against database tables.
+Databudgie is a CLI & library for database performing targeted backup and
+restore of database tables or arbitrary queries against database tables.
 
 # Usage
 
 A minimal config file might look like:
 
 ```yaml
-# config.databudgie.yml
+# databudgie.yml or config.databudgie.yml
 backup:
   url: postgresql://postgres:postgres@localhost:5432/postgres
   tables:
     - name: public.product
       query: "select * from {table} where store_id > 4"
       location: s3://my-s3-bucket/databudgie/public.product
 restore:
   url: postgresql://postgres:postgres@localhost:5432/postgres
   tables:
     - name: public.product
       location: s3://my-s3-bucket/databudgie/public.product
 ```
 
-With that config in place, backing up the defined tables (using the specified config)
-is as simple as `databudgie backup`; and restore `databudgie restore`.
+With that config in place, backing up the defined tables (using the specified
+config) is as simple as `databudgie backup`; and restore `databudgie restore`.
 
 ## Installation
 
 ```bash
 pip install databudgie
 ```
```

