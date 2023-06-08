# Comparing `tmp/grabngro-0.0.8.tar.gz` & `tmp/grabngro-0.0.9.tar.gz`

## Comparing `grabngro-0.0.8.tar` & `grabngro-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 grabngro-0.0.8/LICENSE
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 grabngro-0.0.8/README.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 grabngro-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 grabngro-0.0.8/src/grabngro/__init__.py
--rw-r--r--   0        0        0     4804 2020-02-02 00:00:00.000000 grabngro-0.0.8/src/grabngro/client.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 grabngro-0.0.8/.gitignore
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 grabngro-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 grabngro-0.0.9/LICENSE
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 grabngro-0.0.9/README.md
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 grabngro-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 grabngro-0.0.9/src/grabngro/__init__.py
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 grabngro-0.0.9/src/grabngro/client.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 grabngro-0.0.9/.gitignore
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 grabngro-0.0.9/PKG-INFO
```

### Comparing `grabngro-0.0.8/LICENSE` & `grabngro-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `grabngro-0.0.8/pyproject.toml` & `grabngro-0.0.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "grabngro"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Andrew Yatzkan", email="andrew.yatzkan@gro-intelligence.com" },
 ]
 description = "Python client library grabngro"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.7"
```

### Comparing `grabngro-0.0.8/src/grabngro/client.py` & `grabngro-0.0.9/src/grabngro/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -131,12 +131,21 @@
 		return self.simple_get_request('futures/'+querystring)
 
 	# Get futures data using a specific contract code
 	def get_by_code(self, code: str):
 		querystring: str = f"?code={code}"
 		return self.simple_get_request('futures_by_code/'+querystring)
 
+	# Get all futures contracts for a specific month for a given product
+	# For example, if product_code="C" and month_code="Z", return all data for December
+	# contracts for CME corn.
+	def get_all_contracts_by_month(self, product_code: str, month_code: str):
+		querystring: str = f"?product_code={product_code}&month_code={month_code}"
+		# Here we're returning the "values" format, so include a column parameters
+		# so the output can easily cast into pandas with ** operator
+		return {'data': self.simple_get_request('futures_by_month/'+querystring), 'columns': ['start_date', 'reporting_date', 'value']}
+
 	# Get futures curve for specific product/date
 	def get_curve(self, product_code: str, reporting_date: str):
 		querystring: str = f"?product_code={product_code}&reporting_date={reporting_date}"
 		return self.simple_get_request('futures_curve/'+querystring)
```

