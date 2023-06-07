# Comparing `tmp/databricks_sql_connector-2.5.2.tar.gz` & `tmp/databricks_sql_connector-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_sql_connector-2.5.2.tar", max compression
+gzip compressed data, was "databricks_sql_connector-2.6.0.tar", max compression
```

## Comparing `databricks_sql_connector-2.5.2.tar` & `databricks_sql_connector-2.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     4191 2023-05-09 03:34:38.854149 databricks_sql_connector-2.5.2/CHANGELOG.md
--rw-r--r--   0        0        0    11346 2023-05-09 03:34:38.854149 databricks_sql_connector-2.5.2/LICENSE
--rw-r--r--   0        0        0     2723 2023-05-09 03:34:38.854149 databricks_sql_connector-2.5.2/README.md
--rw-r--r--   0        0        0     1417 2023-05-09 03:35:04.634186 databricks_sql_connector-2.5.2/pyproject.toml
--rw-r--r--   0        0        0      295 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/__init__.py
--rw-r--r--   0        0        0     1269 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/sql/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/sql/auth/__init__.py
--rw-r--r--   0        0        0     3894 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/sql/auth/auth.py
--rw-r--r--   0        0        0     5493 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/sql/auth/authenticators.py
--rw-r--r--   0        0        0     9717 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/sql/auth/oauth.py
--rw-r--r--   0        0        0     1201 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/sql/auth/oauth_http_handler.py
--rw-r--r--   0        0        0     1269 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/sql/auth/thrift_http_client.py
--rw-r--r--   0        0        0    36862 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/sql/client.py
--rw-r--r--   0        0        0     2423 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/sql/exc.py
--rw-r--r--   0        0        0        0 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/sql/experimental/__init__.py
--rw-r--r--   0        0        0     2236 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/sql/experimental/oauth_persistence.py
--rwxr-xr-x   0        0        0     8062 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
--rw-r--r--   0        0        0   136849 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
--rw-r--r--   0        0        0       49 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/sql/thrift_api/TCLIService/__init__.py
--rw-r--r--   0        0        0     1307 2023-05-09 03:34:38.858149 databricks_sql_connector-2.5.2/src/databricks/sql/thrift_api/TCLIService/constants.py
--rw-r--r--   0        0        0  2077276 2023-05-09 03:34:38.866149 databricks_sql_connector-2.5.2/src/databricks/sql/thrift_api/TCLIService/ttypes.py
--rw-r--r--   0        0        0        0 2023-05-09 03:34:38.866149 databricks_sql_connector-2.5.2/src/databricks/sql/thrift_api/__init__.py
--rw-r--r--   0        0        0    41140 2023-05-09 03:34:38.866149 databricks_sql_connector-2.5.2/src/databricks/sql/thrift_backend.py
--rw-r--r--   0        0        0     6771 2023-05-09 03:34:38.866149 databricks_sql_connector-2.5.2/src/databricks/sql/types.py
--rw-r--r--   0        0        0     6646 2023-05-09 03:34:38.866149 databricks_sql_connector-2.5.2/src/databricks/sql/utils.py
--rw-r--r--   0        0        0       60 2023-05-09 03:34:38.866149 databricks_sql_connector-2.5.2/src/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     9761 2023-05-09 03:34:38.866149 databricks_sql_connector-2.5.2/src/databricks/sqlalchemy/dialect/__init__.py
--rw-r--r--   0        0        0      494 2023-05-09 03:34:38.866149 databricks_sql_connector-2.5.2/src/databricks/sqlalchemy/dialect/base.py
--rw-r--r--   0        0        0      792 2023-05-09 03:34:38.866149 databricks_sql_connector-2.5.2/src/databricks/sqlalchemy/dialect/compiler.py
--rw-r--r--   0        0        0     4107 1970-01-01 00:00:00.000000 databricks_sql_connector-2.5.2/PKG-INFO
+-rw-r--r--   0        0        0     4320 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11346 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/LICENSE
+-rw-r--r--   0        0        0     2723 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/README.md
+-rw-r--r--   0        0        0     1417 2023-06-07 22:25:18.463320 databricks_sql_connector-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0      295 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/__init__.py
+-rw-r--r--   0        0        0     1269 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/auth/__init__.py
+-rw-r--r--   0        0        0     3894 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/auth/auth.py
+-rw-r--r--   0        0        0     5493 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/auth/authenticators.py
+-rw-r--r--   0        0        0     9717 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/auth/oauth.py
+-rw-r--r--   0        0        0     1201 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/auth/oauth_http_handler.py
+-rw-r--r--   0        0        0     5900 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/auth/thrift_http_client.py
+-rw-r--r--   0        0        0    36862 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/client.py
+-rw-r--r--   0        0        0     2423 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/exc.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/experimental/__init__.py
+-rw-r--r--   0        0        0     2236 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/experimental/oauth_persistence.py
+-rwxr-xr-x   0        0        0     8062 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
+-rw-r--r--   0        0        0   136849 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
+-rw-r--r--   0        0        0       49 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/__init__.py
+-rw-r--r--   0        0        0     1307 2023-06-07 22:24:49.881864 databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/constants.py
+-rw-r--r--   0        0        0  2077276 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/ttypes.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/__init__.py
+-rw-r--r--   0        0        0    41308 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sql/thrift_backend.py
+-rw-r--r--   0        0        0     6771 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sql/types.py
+-rw-r--r--   0        0        0     6646 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sql/utils.py
+-rw-r--r--   0        0        0       60 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     9761 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sqlalchemy/dialect/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sqlalchemy/dialect/base.py
+-rw-r--r--   0        0        0      792 2023-06-07 22:24:49.889865 databricks_sql_connector-2.6.0/src/databricks/sqlalchemy/dialect/compiler.py
+-rw-r--r--   0        0        0     4107 1970-01-01 00:00:00.000000 databricks_sql_connector-2.6.0/PKG-INFO
```

### Comparing `databricks_sql_connector-2.5.2/CHANGELOG.md` & `databricks_sql_connector-2.6.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # Release History
 
-## 2.5.x (Unreleased)
+## 2.6.x (Unreleased)
+
+## 2.6.0 (2023-06-07)
+
+- Add support for HTTP 1.1 connections (connection pools)
+- Add a default socket timeout for thrift RPCs
 
 ## 2.5.2 (2023-05-08)
 
 - Fix: SQLAlchemy adapter could not reflect TIMESTAMP or DATETIME columns
 - Other: Relax pandas and alembic dependency specifications
 
 ## 2.5.1 (2023-04-28)
```

### Comparing `databricks_sql_connector-2.5.2/LICENSE` & `databricks_sql_connector-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/README.md` & `databricks_sql_connector-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/pyproject.toml` & `databricks_sql_connector-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-sql-connector"
-version = "2.5.2"
+version = "2.6.0"
 description = "Databricks SQL Connector for Python"
 authors = ["Databricks <databricks-sql-connector-maintainers@databricks.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "databricks", from = "src"}]
 include = ["CHANGELOG.md"]
```

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sql/__init__.py` & `databricks_sql_connector-2.6.0/src/databricks/sql/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 NUMBER = DBAPITypeObject(
     "boolean", "tinyint", "smallint", "int", "bigint", "float", "double", "decimal"
 )
 DATETIME = DBAPITypeObject("timestamp")
 DATE = DBAPITypeObject("date")
 ROWID = DBAPITypeObject()
 
-__version__ = "2.5.2"
+__version__ = "2.6.0"
 USER_AGENT_NAME = "PyDatabricksSqlConnector"
 
 # These two functions are pyhive legacy
 Date = datetime.date
 Timestamp = datetime.datetime
```

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sql/auth/auth.py` & `databricks_sql_connector-2.6.0/src/databricks/sql/auth/auth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sql/auth/authenticators.py` & `databricks_sql_connector-2.6.0/src/databricks/sql/auth/authenticators.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sql/auth/oauth.py` & `databricks_sql_connector-2.6.0/src/databricks/sql/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sql/auth/oauth_http_handler.py` & `databricks_sql_connector-2.6.0/src/databricks/sql/auth/oauth_http_handler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sql/client.py` & `databricks_sql_connector-2.6.0/src/databricks/sql/client.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sql/exc.py` & `databricks_sql_connector-2.6.0/src/databricks/sql/exc.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sql/experimental/oauth_persistence.py` & `databricks_sql_connector-2.6.0/src/databricks/sql/experimental/oauth_persistence.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote` & `databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sql/thrift_api/TCLIService/TCLIService.py` & `databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sql/thrift_api/TCLIService/constants.py` & `databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sql/thrift_api/TCLIService/ttypes.py` & `databricks_sql_connector-2.6.0/src/databricks/sql/thrift_api/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sql/thrift_backend.py` & `databricks_sql_connector-2.6.0/src/databricks/sql/thrift_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 logger = logging.getLogger(__name__)
 
 THRIFT_ERROR_MESSAGE_HEADER = "x-thriftserver-error-message"
 DATABRICKS_ERROR_OR_REDIRECT_HEADER = "x-databricks-error-or-redirect-message"
 DATABRICKS_REASON_HEADER = "x-databricks-reason-phrase"
 
 TIMESTAMP_AS_STRING_CONFIG = "spark.thriftserver.arrowBasedRowSet.timestampAsString"
+DEFAULT_SOCKET_TIMEOUT = float(900)
 
 # see Connection.__init__ for parameter descriptions.
 # - Min/Max avoids unsustainable configs (sane values are far more constrained)
 # - 900s attempts-duration lines up w ODBC/JDBC drivers (for cluster startup > 10 mins)
 _retry_policy = {  # (type, default, min, max)
     "_retry_delay_min": (float, 1, 0.1, 60),
     "_retry_delay_max": (float, 60, 5, 3600),
@@ -95,16 +96,16 @@
         #   (Note this will stop _before_ intentionally exceeding; thus if the
         #   next calculated pre-retry delay would go past
         #   _retry_stop_after_attempts_duration, stop now.)
         #
         # _retry_stop_after_attempts_count
         #  The maximum number of times we should retry retryable requests (defaults to 24)
         # _socket_timeout
-        #  The timeout in seconds for socket send, recv and connect operations. Defaults to None for
-        #  no timeout. Should be a positive float or integer.
+        #  The timeout in seconds for socket send, recv and connect operations. Should be a positive float or integer.
+        #  (defaults to 900)
 
         port = port or 443
         if kwargs.get("_connection_uri"):
             uri = kwargs.get("_connection_uri")
         elif server_hostname and http_path:
             uri = "https://{host}:{port}/{path}".format(
                 host=server_hostname, port=port, path=http_path.lstrip("/")
@@ -148,16 +149,16 @@
 
         self._transport = databricks.sql.auth.thrift_http_client.THttpClient(
             auth_provider=self._auth_provider,
             uri_or_host=uri,
             ssl_context=ssl_context,
         )
 
-        timeout = kwargs.get("_socket_timeout")
-        # setTimeout defaults to None (i.e. no timeout), and is expected in ms
+        timeout = kwargs.get("_socket_timeout", DEFAULT_SOCKET_TIMEOUT)
+        # setTimeout defaults to 15 minutes and is expected in ms
         self._transport.setTimeout(timeout and (float(timeout) * 1000.0))
 
         self._transport.setCustomHeaders(dict(http_headers))
         protocol = thrift.protocol.TBinaryProtocol.TBinaryProtocol(self._transport)
         self._client = TCLIService.Client(protocol)
 
         try:
@@ -313,14 +314,18 @@
             # - non-None retry_delay -> sleep delay before retry
             # - error, error_message always set when available
 
             error, error_message, retry_delay = None, None, None
             try:
                 logger.debug("Sending request: {}".format(request))
                 response = method(request)
+
+                # Calling `close()` here releases the active HTTP connection back to the pool
+                self._transport.close()
+
                 logger.debug("Received response: {}".format(response))
                 return response
             except OSError as err:
                 error = err
                 error_message = str(err)
                 # fmt: off
                 # The built-in errno package encapsulates OSError codes, which are OS-specific.
```

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sql/types.py` & `databricks_sql_connector-2.6.0/src/databricks/sql/types.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sql/utils.py` & `databricks_sql_connector-2.6.0/src/databricks/sql/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sqlalchemy/dialect/__init__.py` & `databricks_sql_connector-2.6.0/src/databricks/sqlalchemy/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/src/databricks/sqlalchemy/dialect/compiler.py` & `databricks_sql_connector-2.6.0/src/databricks/sqlalchemy/dialect/compiler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.5.2/PKG-INFO` & `databricks_sql_connector-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sql-connector
-Version: 2.5.2
+Version: 2.6.0
 Summary: Databricks SQL Connector for Python
 License: Apache-2.0
 Author: Databricks
 Author-email: databricks-sql-connector-maintainers@databricks.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

