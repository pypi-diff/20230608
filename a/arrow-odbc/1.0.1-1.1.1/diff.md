# Comparing `tmp/arrow_odbc-1.0.1.tar.gz` & `tmp/arrow_odbc-1.1.1.tar.gz`

## Comparing `arrow_odbc-1.0.1.tar` & `arrow_odbc-1.1.1.tar`

### file list

```diff
@@ -1,43 +1,45 @@
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 arrow_odbc-1.0.1/Cargo.toml
--rw-r--r--   0      501       20      136 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/.gitattributes
--rw-r--r--   0      501       20      131 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/.github/dependabot.yml
--rw-r--r--   0      501       20     1522 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/.github/workflows/test.yml
--rw-r--r--   0      501       20     1807 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/.github/workflows/wheel.yml
--rw-r--r--   0      501       20      286 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/.gitignore
--rw-r--r--   0      501       20      841 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/.readthedocs.yaml
--rw-r--r--   0      501       20     4861 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/Changelog.md
--rw-r--r--   0      501       20     1954 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/Contributing.md
--rw-r--r--   0      501       20     1069 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/LICENSE
--rw-r--r--   0      501       20     7727 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/README.md
--rw-r--r--   0      501       20       14 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/cbindgen.toml
--rw-r--r--   0      501       20      639 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/conftest.py
--rw-r--r--   0      501       20      638 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/doc/Makefile
--rw-r--r--   0      501       20      804 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/doc/make.bat
--rw-r--r--   0      501       20       16 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/doc/requirements.txt
--rw-r--r--   0      501       20      155 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/doc/source/arrow_odbc.rst
--rw-r--r--   0      501       20     1965 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/doc/source/conf.py
--rw-r--r--   0      501       20      458 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/doc/source/index.rst
--rw-r--r--   0      501       20       67 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/doc/source/modules.rst
--rw-r--r--   0      501       20      348 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/docker-compose.yml
--rw-r--r--   0      501       20      564 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/manylinux/Dockerfile
--rw-r--r--   0      501       20      121 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/manylinux/Readme.md
--rw-r--r--   0      501       20      148 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/manylinux/WHEEL
--rw-r--r--   0      501       20     1256 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/manylinux/build_wheel.sh
--rw-r--r--   0      501       20      617 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/pyproject.toml
--rw-r--r--   0      501       20      307 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/python/arrow_odbc/__init__.py
--rw-r--r--   0      501       20     1645 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/python/arrow_odbc/connect.py
--rw-r--r--   0      501       20      672 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/python/arrow_odbc/error.py
--rw-r--r--   0      501       20    15067 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/python/arrow_odbc/reader.py
--rw-r--r--   0      501       20     9164 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/python/arrow_odbc/writer.py
--rw-r--r--   0      501       20     2322 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/src/error.rs
--rw-r--r--   0      501       20     2841 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/src/lib.rs
--rw-r--r--   0      501       20     1239 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/src/parameter.rs
--rw-r--r--   0      501       20     3033 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/src/reader/arrow_odbc_reader.rs
--rw-r--r--   0      501       20     6484 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/src/reader.rs
--rw-r--r--   0      501       20     3613 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/src/writer.rs
--rw-r--r--   0      501       20        0 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/tests/__init__.py
--rw-r--r--   0      501       20     4115 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/tests/iris.csv
--rw-r--r--   0      501       20     2413 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/tests/iris.parquet
--rw-r--r--   0      501       20    19183 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/tests/test_arrow_odbc.py
--rw-r--r--   0      501       20    35304 2023-04-10 12:34:39.000000 arrow_odbc-1.0.1/Cargo.lock
--rw-r--r--   0        0        0     8251 1970-01-01 00:00:00.000000 arrow_odbc-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 arrow_odbc-1.1.1/Cargo.toml
+-rw-r--r--   0        0        0      136 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/.gitattributes
+-rw-r--r--   0        0        0      131 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1522 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1807 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/.github/workflows/wheel.yml
+-rw-r--r--   0        0        0      286 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/.gitignore
+-rw-r--r--   0        0        0      841 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     5026 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/Changelog.md
+-rw-r--r--   0        0        0     1954 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/Contributing.md
+-rw-r--r--   0        0        0     1069 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/LICENSE
+-rw-r--r--   0        0        0     7727 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/README.md
+-rw-r--r--   0        0        0       14 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/cbindgen.toml
+-rw-r--r--   0        0        0      639 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/conftest.py
+-rw-r--r--   0        0        0      638 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/doc/Makefile
+-rw-r--r--   0        0        0      804 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/doc/make.bat
+-rw-r--r--   0        0        0       16 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/doc/requirements.txt
+-rw-r--r--   0        0        0      155 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/doc/source/arrow_odbc.rst
+-rw-r--r--   0        0        0     1965 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/doc/source/conf.py
+-rw-r--r--   0        0        0      458 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/doc/source/index.rst
+-rw-r--r--   0        0        0       67 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/doc/source/modules.rst
+-rw-r--r--   0        0        0      348 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/docker-compose.yml
+-rw-r--r--   0        0        0      564 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/manylinux/Dockerfile
+-rw-r--r--   0        0        0      121 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/manylinux/Readme.md
+-rw-r--r--   0        0        0      148 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/manylinux/WHEEL
+-rw-r--r--   0        0        0     1256 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/manylinux/build_wheel.sh
+-rw-r--r--   0        0        0      640 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      358 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/python/arrow_odbc/__init__.py
+-rw-r--r--   0        0        0     1645 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/python/arrow_odbc/connect.py
+-rw-r--r--   0        0        0      672 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/python/arrow_odbc/error.py
+-rw-r--r--   0        0        0      791 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/python/arrow_odbc/log.py
+-rw-r--r--   0        0        0    15067 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/python/arrow_odbc/reader.py
+-rw-r--r--   0        0        0     9164 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/python/arrow_odbc/writer.py
+-rw-r--r--   0        0        0     2322 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/src/error.rs
+-rw-r--r--   0        0        0     2897 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/src/lib.rs
+-rw-r--r--   0        0        0      685 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/src/logging.rs
+-rw-r--r--   0        0        0     1239 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/src/parameter.rs
+-rw-r--r--   0        0        0     3030 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/src/reader/arrow_odbc_reader.rs
+-rw-r--r--   0        0        0     6484 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/src/reader.rs
+-rw-r--r--   0        0        0     3613 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/src/writer.rs
+-rw-r--r--   0        0        0        0 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     4115 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/tests/iris.csv
+-rw-r--r--   0        0        0     2413 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/tests/iris.parquet
+-rw-r--r--   0        0        0    19491 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/tests/test_arrow_odbc.py
+-rw-r--r--   0        0        0    34251 2023-06-08 18:27:26.000000 arrow_odbc-1.1.1/Cargo.lock
+-rw-r--r--   0        0        0     8251 1970-01-01 00:00:00.000000 arrow_odbc-1.1.1/PKG-INFO
```

### Comparing `arrow_odbc-1.0.1/Cargo.toml` & `arrow_odbc-1.1.1/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -10,24 +10,20 @@
 
 [lib]
 # Name needs to be identical to python package name
 name = "arrow_odbc"
 crate-type = ["cdylib"]
 
 [dependencies]
-arrow-odbc = "0.27.0"
+arrow-odbc = "0.28.5"
 # arrow would be included indirectly using arrow-odbc, but we need to explicitly specify the ffi
 # feature.
-arrow = { version = "36.0.0", default-features = false, features = ["ffi"] }
+arrow = { version = "41.0.0", default-features = false, features = ["ffi"] }
 lazy_static = "1.4.0"
-# We only depend indirectly on log, but we include it directly here to disable logging at compile
-# time.
-log = { version = "0.4.17", features = ["release_max_level_off"] }
+stderrlog = "0.5.4"
+log = "0.4.18"
 
 [profile.release]
 # Panics should only be caused by logic errors and are considered bugs
 panic = 'abort'
 # Link time Optimization
 lto = true
-
-[package.metadata.maturin]
-python-source = "python"
```

### Comparing `arrow_odbc-1.0.1/.github/workflows/test.yml` & `arrow_odbc-1.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/.github/workflows/wheel.yml` & `arrow_odbc-1.1.1/.github/workflows/wheel.yml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/.readthedocs.yaml` & `arrow_odbc-1.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/Changelog.md` & `arrow_odbc-1.1.1/Changelog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changelog
 
+## 1.1.1
+
+- Fix version number in documentation.
+
+## 1.1.0
+
+- Update Rust dependencies
+- Adds `log_to_stderr` for emitting diagnostics directly to standard output.
+
 ## 1.0.1
 
 - More code examples in Docstrings
 
 ## 1.0.0
 
 - Breaking change: `read_arrow_batches_from_odbc` now also returns a batch reader instead of `None`, even if the SQL statement did not produce a result set. The resulting reader will be empty, i.e. iterating over batches stops immediatly. The assaciated schema attribute will contain no columns.
```

### Comparing `arrow_odbc-1.0.1/Contributing.md` & `arrow_odbc-1.1.1/Contributing.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/LICENSE` & `arrow_odbc-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/README.md` & `arrow_odbc-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/conftest.py` & `arrow_odbc-1.1.1/conftest.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/doc/Makefile` & `arrow_odbc-1.1.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/doc/make.bat` & `arrow_odbc-1.1.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/doc/source/conf.py` & `arrow_odbc-1.1.1/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "arrow-odbc"
 copyright = "2021, Markus Klein"
 author = "Markus Klein"
 
 # The full version, including alpha/beta/rc tags
-release = "1.0.1"
+release = "1.1.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `arrow_odbc-1.0.1/manylinux/Dockerfile` & `arrow_odbc-1.1.1/manylinux/Dockerfile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/manylinux/build_wheel.sh` & `arrow_odbc-1.1.1/manylinux/build_wheel.sh`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/pyproject.toml` & `arrow_odbc-1.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
-requires = ["cffi", "maturin>=0.13,<0.14"]
+requires = ["cffi", "maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "arrow-odbc"
 authors = [{name = "Markus Klein"}]
 description="Read the data of an ODBC data source as sequence of Apache Arrow record batches."
 readme = "README.md"
-version = "1.0.1"
+version = "1.1.1"
 dependencies = ["cffi", "pyarrow"]
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = ["pytest < 8.0.0"]
@@ -19,7 +19,8 @@
 [project.urls]
 repository = "https://github.com/pacman82/arrow-odbc-py"
 changelog = "https://github.com/pacman82/arrow-odbc-py/blob/main/Changelog.md"
 
 [tool.maturin]
 # Bindings type
 bindings = "cffi"
+python-source = "python"
```

### Comparing `arrow_odbc-1.0.1/python/arrow_odbc/connect.py` & `arrow_odbc-1.1.1/python/arrow_odbc/connect.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/python/arrow_odbc/error.py` & `arrow_odbc-1.1.1/python/arrow_odbc/error.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/python/arrow_odbc/reader.py` & `arrow_odbc-1.1.1/python/arrow_odbc/reader.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/python/arrow_odbc/writer.py` & `arrow_odbc-1.1.1/python/arrow_odbc/writer.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/src/error.rs` & `arrow_odbc-1.1.1/src/error.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/src/lib.rs` & `arrow_odbc-1.1.1/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 //! Defines C bindings for `arrow-odbc` to enable using it from Python.
 mod error;
 mod parameter;
 mod reader;
 mod writer;
+mod logging;
 
 use std::{borrow::Cow, ptr::null_mut, slice, str};
 
 use arrow_odbc::odbc_api::{escape_attribute_value, Connection, ConnectionOptions, Environment};
 use lazy_static::lazy_static;
 
 pub use error::{arrow_odbc_error_free, arrow_odbc_error_message, ArrowOdbcError};
 pub use reader::{
     arrow_odbc_reader_free, arrow_odbc_reader_make, arrow_odbc_reader_next, ArrowOdbcReader,
 };
 pub use writer::{
     arrow_odbc_writer_free, arrow_odbc_writer_make, arrow_odbc_writer_write_batch, ArrowOdbcWriter,
 };
+pub use logging::arrow_odbc_log_to_stderr;
 
 lazy_static! {
     static ref ENV: Environment = Environment::new().unwrap();
 }
 
 /// Opaque type to transport connection to an ODBC Datasource over language boundry
 pub struct OdbcConnection(Connection<'static>);
```

### Comparing `arrow_odbc-1.0.1/src/parameter.rs` & `arrow_odbc-1.1.1/src/parameter.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/src/reader/arrow_odbc_reader.rs` & `arrow_odbc-1.1.1/src/reader/arrow_odbc_reader.rs`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     pub fn next_batch(
         &mut self,
     ) -> Result<Option<(FFI_ArrowArray, FFI_ArrowSchema)>, ArrowOdbcError> {
         let next = self.0.as_mut().and_then(OdbcReader::next).transpose()?;
         let next = if let Some(batch) = next {
             let struct_array: StructArray = batch.into();
-            let arrow_array = ArrowArray::try_new(struct_array.data().clone())?;
+            let arrow_array = ArrowArray::try_new(struct_array.into_data())?;
             let array_data = arrow_array.to_data().unwrap();
             let ffi_array = FFI_ArrowArray::new(&array_data);
             let ffi_schema = FFI_ArrowSchema::try_from(array_data.data_type()).unwrap();
             Some((ffi_array, ffi_schema))
         } else {
             None
         };
```

### Comparing `arrow_odbc-1.0.1/src/reader.rs` & `arrow_odbc-1.1.1/src/reader.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/src/writer.rs` & `arrow_odbc-1.1.1/src/writer.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/tests/iris.csv` & `arrow_odbc-1.1.1/tests/iris.csv`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/tests/iris.parquet` & `arrow_odbc-1.1.1/tests/iris.parquet`

 * *Files identical despite different names*

### Comparing `arrow_odbc-1.0.1/tests/test_arrow_odbc.py` & `arrow_odbc-1.1.1/tests/test_arrow_odbc.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,22 @@
 
 from pytest import raises
 
 from arrow_odbc import (
     insert_into_table,
     from_table_to_db,
     read_arrow_batches_from_odbc,
+    log_to_stderr,
     Error,
 )
 
 MSSQL = "Driver={ODBC Driver 17 for SQL Server};Server=localhost;UID=SA;PWD=My@Test@Password1;"
 
+log_to_stderr()
+
 
 def test_should_report_error_on_invalid_connection_string_reading():
     """
     We want to forward the original ODBC errors to the end user. Of course foo
     is not a valid connection string. Therefore we want to see the creation of
     this connection fail, but with a nice error.
     """
@@ -99,15 +102,15 @@
     """
     # This statement produces two result sets
     query = f"SELECT 1 AS a; SELECT 2 AS b;"
 
     reader = read_arrow_batches_from_odbc(
         query=query, batch_size=100, connection_string=MSSQL
     )
-    
+
     assert reader.more_results(batch_size=100)
     assert not reader.more_results(batch_size=100)
 
 
 def test_advancing_past_last_result_set_leaves_empty_reader():
     """
     Moving past the last result set, leaves a reader returning a schema with no columns and no
@@ -605,14 +608,26 @@
     # Then
     actual = check_output(
         ["odbcsv", "fetch", "-c", MSSQL, "-q", f"SELECT a FROM {table}"]
     )
     assert "a\nHello\n" == actual.decode("utf8")
 
 
+def test_reinitalizing_logger_should_raise():
+    """
+    Reinitializin logger should raise
+    """
+    # When / Then
+    with raises(
+        Error,
+        match=r"attempted to set a logger after the logging system was already initialized",
+    ):
+        log_to_stderr()
+
+
 @pytest.mark.slow
 def test_should_not_leak_memory_for_each_batch():
     """
     Read a bunch of arrow batches and see if total memory usage went over a
     threshold after running GC. Currently I let this run manually and see if
     the process takes more memory over time as an assertion.
     """
```

### Comparing `arrow_odbc-1.0.1/Cargo.lock` & `arrow_odbc-1.1.1/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,17 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "android-activity"
 version = "0.4.1"
@@ -45,27 +45,33 @@
 [[package]]
 name = "android-properties"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc7eb209b1518d6bb87b283c20095f5228ecda460da70b44f0802523dea6da04"
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "arrow"
-version = "36.0.0"
+version = "41.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "990dfa1a9328504aa135820da1c95066537b69ad94c04881b785f64328e0fa6b"
+checksum = "4a46441ae78c0c5915f62aa32cad9910647c19241456dd24039646dd96d494a5"
 dependencies = [
  "ahash",
  "arrow-arith",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
@@ -74,86 +80,86 @@
  "arrow-schema",
  "arrow-select",
  "arrow-string",
 ]
 
 [[package]]
 name = "arrow-arith"
-version = "36.0.0"
+version = "41.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f2b2e52de0ab54173f9b08232b7184c26af82ee7ab4ac77c83396633c90199fa"
+checksum = "350c5067470aeeb38dcfcc1f7e9c397098116409c9087e43ca99c231020635d9"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-array"
-version = "36.0.0"
+version = "41.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e10849b60c17dbabb334be1f4ef7550701aa58082b71335ce1ed586601b2f423"
+checksum = "6049e031521c4e7789b7530ea5991112c0a375430094191f3b74bdf37517c9a9"
 dependencies = [
  "ahash",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
  "hashbrown 0.13.2",
  "num",
 ]
 
 [[package]]
 name = "arrow-buffer"
-version = "36.0.0"
+version = "41.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0746ae991b186be39933147117f8339eb1c4bbbea1c8ad37e7bf5851a1a06ba"
+checksum = "a83450b94b9fe018b65ba268415aaab78757636f68b7f37b6bc1f2a3888af0a0"
 dependencies = [
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-cast"
-version = "36.0.0"
+version = "41.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b88897802515d7b193e38b27ddd9d9e43923d410a9e46307582d756959ee9595"
+checksum = "249198411254530414805f77e88e1587b0914735ea180f906506905721f7a44a"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "chrono",
  "lexical-core",
  "num",
 ]
 
 [[package]]
 name = "arrow-data"
-version = "36.0.0"
+version = "41.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "533f937efa1aaad9dc86f6a0e382c2fa736a4943e2090c946138079bdf060cef"
+checksum = "4d48dcbed83d741d4af712af17f6d952972b8f6491b24ee2415243a7e37c6438"
 dependencies = [
  "arrow-buffer",
  "arrow-schema",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-odbc"
-version = "0.27.0"
+version = "0.28.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f67c97fff393388a0e128d584a71372ac1d27222ab321e44ff031b2ccd66ffe6"
+checksum = "6fbd7f6c1eee67c852b26ce9dfdaa931fe61954e59613dcb7fa9cb094bb513a2"
 dependencies = [
  "arrow",
  "atoi",
  "chrono",
  "odbc-api",
  "thiserror",
 ]
@@ -162,73 +168,74 @@
 name = "arrow-odbc-py"
 version = "0.1.0"
 dependencies = [
  "arrow",
  "arrow-odbc",
  "lazy_static",
  "log",
+ "stderrlog",
 ]
 
 [[package]]
 name = "arrow-ord"
-version = "36.0.0"
+version = "41.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33d2671eb3793f9410230ac3efb0e6d36307be8a2dac5fad58ac9abde8e9f01e"
+checksum = "29be2d5fadaab29e4fa6a7e527ceaa1c2cddc57dc6d86c062f7a05adcd8df71e"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-row"
-version = "36.0.0"
+version = "41.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc11fa039338cebbf4e29cf709c8ac1d6a65c7540063d4a25f991ab255ca85c8"
+checksum = "b6e0bd6ad24d56679b3317b499b0de61bca16d3142896908cce1aa943e56e981"
 dependencies = [
  "ahash",
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "half",
  "hashbrown 0.13.2",
 ]
 
 [[package]]
 name = "arrow-schema"
-version = "36.0.0"
+version = "41.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d04f17f7b86ded0b5baf98fe6123391c4343e031acc3ccc5fa604cc180bff220"
+checksum = "2b71d8d68d0bc2e648e4e395896dc518be8b90c5f0f763c59083187c3d46184b"
 dependencies = [
- "bitflags 2.1.0",
+ "bitflags 2.3.1",
 ]
 
 [[package]]
 name = "arrow-select"
-version = "36.0.0"
+version = "41.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "163e35de698098ff5f5f672ada9dc1f82533f10407c7a11e2cd09f3bcf31d18a"
+checksum = "470cb8610bdfda56554a436febd4e457e506f3c42e01e545a1ea7ecf2a4c8823"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "num",
 ]
 
 [[package]]
 name = "arrow-string"
-version = "36.0.0"
+version = "41.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfdfbed1b10209f0dc68e6aa4c43dc76079af65880965c7c3b73f641f23d4aba"
+checksum = "70f8a2e4ff9dbbd51adbabf92098b71e3eb2ef0cfcb75236ca7c3ce087cce038"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "regex",
@@ -241,30 +248,41 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "atty"
+version = "0.2.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
+dependencies = [
+ "hermit-abi",
+ "libc",
+ "winapi",
+]
+
+[[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.1.0"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c70beb79cbb5ce9c4f8e20849978f34225931f665bb49efa6982875a4d5facb3"
+checksum = "6776fc96284a0bb647b615056fc496d1fe1644a7ab01829818a6d91cae888b84"
 
 [[package]]
 name = "block-sys"
 version = "0.1.0-beta.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa55741ee90902547802152aaf3f8e5248aab7e21468089560d4c8840561146"
 dependencies = [
@@ -279,17 +297,17 @@
 dependencies = [
  "block-sys",
  "objc2-encode",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 dependencies = [
@@ -306,38 +324,28 @@
 name = "cfg_aliases"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd16c4719339c4530435d38e511904438d07cce7950afa3718a84ac36c10e89e"
 
 [[package]]
 name = "chrono"
-version = "0.4.24"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
+ "android-tzdata",
  "iana-time-zone",
  "js-sys",
- "num-integer",
  "num-traits",
  "time",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
-name = "codespan-reporting"
-version = "0.11.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
-dependencies = [
- "termcolor",
- "unicode-width",
-]
-
-[[package]]
 name = "const-random"
 version = "0.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "368a7a772ead6ce7e1de82bfb04c485f3db8ec744f72925af5735e29a22cc18e"
 dependencies = [
  "const-random-macro",
  "proc-macro-hack",
@@ -399,58 +407,14 @@
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
-name = "cxx"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
-dependencies = [
- "cc",
- "cxxbridge-flags",
- "cxxbridge-macro",
- "link-cplusplus",
-]
-
-[[package]]
-name = "cxx-build"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12cee708e8962df2aeb38f594aae5d827c022b6460ac71a7a3e2c3c2aae5a07b"
-dependencies = [
- "cc",
- "codespan-reporting",
- "once_cell",
- "proc-macro2",
- "quote",
- "scratch",
- "syn 2.0.13",
-]
-
-[[package]]
-name = "cxxbridge-flags"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
-
-[[package]]
-name = "cxxbridge-macro"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.13",
-]
-
-[[package]]
 name = "dispatch"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd0c93bb4b0c6d9b77f4435b0ae98c24d17f1c45b2ff844c6151a07256ca923b"
 
 [[package]]
 name = "force-send-sync"
@@ -471,17 +435,17 @@
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
 name = "getrandom"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
@@ -503,35 +467,43 @@
 [[package]]
 name = "hashbrown"
 version = "0.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
 
 [[package]]
+name = "hermit-abi"
+version = "0.1.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "iana-time-zone"
-version = "0.1.56"
+version = "0.1.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
- "cxx",
- "cxx-build",
+ "cc",
 ]
 
 [[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
@@ -565,17 +537,17 @@
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.61"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
+checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
@@ -644,41 +616,29 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.141"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "libm"
-version = "0.2.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
-
-[[package]]
-name = "link-cplusplus"
-version = "1.0.8"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
-dependencies = [
- "cc",
-]
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
@@ -833,17 +793,17 @@
 checksum = "abfcac41015b00a120608fdaa6938c44cb983fee294351cc4bac7638b4e50512"
 dependencies = [
  "objc-sys",
 ]
 
 [[package]]
 name = "odbc-api"
-version = "0.56.1"
+version = "0.57.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c6bf11bd6f82a755c9ab4df0723401ab4f45a0bac9c034466e6e9d2f5c162c8e"
+checksum = "24f67900e105061dac15759103b393022d06c491aed041864dccab0b1d820dad"
 dependencies = [
  "force-send-sync",
  "log",
  "odbc-sys",
  "thiserror",
  "widestring",
  "winit",
@@ -853,28 +813,25 @@
 name = "odbc-sys"
 version = "0.21.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "592c5c4ce58f47dde428c52b39904252191d25436b410cc232fae0813ff58f08"
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "orbclient"
-version = "0.3.44"
+version = "0.3.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0e9829e16c5e112e94efb5e2ad1fe17f8c1c99bb0fcdc8c65c44e935d904767d"
+checksum = "221d488cd70617f1bd599ed8ceb659df2147d9393717954d82a0f5e8032a6ab1"
 dependencies = [
- "cfg-if",
- "redox_syscall 0.2.16",
- "wasm-bindgen",
- "web-sys",
+ "redox_syscall",
 ]
 
 [[package]]
 name = "proc-macro-crate"
 version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f4c021e1093a56626774e81216a4ce732a735e5bad4868a03f3ed65ca0c3919"
@@ -887,110 +844,108 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "raw-window-handle"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f2ff9a1f06a88b01621b7ae906ef0211290d1c8a168a15542486a8f61c0833b9"
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
-dependencies = [
- "bitflags 1.3.2",
-]
-
-[[package]]
-name = "redox_syscall"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.29"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
-
-[[package]]
-name = "scratch"
-version = "1.0.5"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1792db035ce95be60c3f8853017b3999209281c24e2ba5bc8e59bf97a0c590c1"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
+name = "stderrlog"
+version = "0.5.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "69a26bbf6de627d389164afa9783739b56746c6c72c4ed16539f4ff54170327b"
+dependencies = [
+ "atty",
+ "chrono",
+ "log",
+ "termcolor",
+ "thread_local",
+]
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.13"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "termcolor"
-version = "1.2.0"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
+checksum = "bab24d30b911b2376f3a13cc2cd443142f0c81dda04c118693e35b3835757755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
 version = "1.0.40"
@@ -1004,15 +959,25 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.18",
+]
+
+[[package]]
+name = "thread_local"
+version = "1.1.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
+dependencies = [
+ "cfg-if",
+ "once_cell",
 ]
 
 [[package]]
 name = "time"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
@@ -1029,40 +994,34 @@
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
 dependencies = [
  "crunchy",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ab8ed2edee10b50132aed5f331333428b011c99402b5a534154ed15746f9622"
+checksum = "5a76a9312f5ba4c2dec6b9161fdf25d87ad8a09256ccea5a556fef03c706a10f"
 
 [[package]]
 name = "toml_edit"
-version = "0.19.8"
+version = "0.19.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "239410c8609e8125456927e6707163a3b1fdb40561e4b803bc041f466ccfdc13"
+checksum = "2380d56e8670370eee6566b0bfd4265f65b3f432e8c6d85623f728d4fa31f739"
 dependencies = [
  "indexmap",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
-
-[[package]]
-name = "unicode-width"
-version = "0.1.10"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
@@ -1076,82 +1035,82 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
+checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
+checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
+checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
+checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
+checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
 
 [[package]]
 name = "wayland-scanner"
 version = "0.29.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f4303d8fa22ab852f789e75a967f0a2cdc430a607751c0499bada3e451cbd53"
 dependencies = [
  "proc-macro2",
  "quote",
  "xml-rs",
 ]
 
 [[package]]
 name = "web-sys"
-version = "0.3.61"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
+checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "widestring"
@@ -1320,17 +1279,17 @@
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winit"
-version = "0.28.3"
+version = "0.28.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f504e8c117b9015f618774f8d58cd4781f5a479bc41079c064f974cbb253874"
+checksum = "866db3f712fffba75d31bf0cdecf357c8aeafd158c5b7ab51dba2a2b2d47f196"
 dependencies = [
  "android-activity",
  "bitflags 1.3.2",
  "cfg_aliases",
  "core-foundation",
  "core-graphics",
  "dispatch",
@@ -1338,28 +1297,28 @@
  "libc",
  "log",
  "ndk",
  "objc2",
  "once_cell",
  "orbclient",
  "raw-window-handle",
- "redox_syscall 0.3.5",
+ "redox_syscall",
  "wasm-bindgen",
  "wayland-scanner",
  "web-sys",
  "windows-sys",
 ]
 
 [[package]]
 name = "winnow"
-version = "0.4.1"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae8970b36c66498d8ff1d66685dc86b91b29db0c7739899012f63a63814b4b28"
+checksum = "61de7bac303dc551fe038e2b3cef0f571087a47571ea6e79a87692ac99b99699"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "xml-rs"
-version = "0.8.4"
+version = "0.8.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2d7d3948613f75c98fd9328cfdcc45acc4d360655289d0a7d4ec931392200a3"
+checksum = "52839dc911083a8ef63efa4d039d1f58b5e409f923e44c80828f206f66e5541c"
```

### Comparing `arrow_odbc-1.0.1/PKG-INFO` & `arrow_odbc-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: arrow-odbc
-Version: 1.0.1
+Version: 1.1.1
 Requires-Dist: cffi
 Requires-Dist: pyarrow
-Requires-Dist: pytest < 8.0.0; extra == 'test'
+Requires-Dist: pytest <8.0.0 ; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
 Summary: Read the data of an ODBC data source as sequence of Apache Arrow record batches.
 Author: Markus Klein
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: changelog, https://github.com/pacman82/arrow-odbc-py/blob/main/Changelog.md
 Project-URL: repository, https://github.com/pacman82/arrow-odbc-py
+Project-URL: changelog, https://github.com/pacman82/arrow-odbc-py/blob/main/Changelog.md
 
 # arrow-odbc-py
 
 [![Licence](https://img.shields.io/crates/l/arrow-odbc)](https://github.com/pacman82/arrow-odbc-py/blob/master/License)
 [![PyPI version](https://badge.fury.io/py/arrow-odbc.svg)](https://pypi.org/project/arrow-odbc/)
 [![Documentation Status](https://readthedocs.org/projects/arrow-odbc/badge/?version=latest)](https://arrow-odbc.readthedocs.io/en/latest/?badge=latest)
```

