# Comparing `tmp/choosy-0.0.2.tar.gz` & `tmp/choosy-0.0.3.tar.gz`

## Comparing `choosy-0.0.2.tar` & `choosy-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 choosy-0.0.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 choosy-0.0.2/src/choosy/__about__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 choosy-0.0.2/src/choosy/__init__.py
--rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 choosy-0.0.2/src/choosy/base.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 choosy-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 choosy-0.0.2/tests/test_base.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 choosy-0.0.2/.gitignore
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 choosy-0.0.2/LICENSE
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 choosy-0.0.2/README.md
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 choosy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 choosy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 choosy-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 choosy-0.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 choosy-0.0.3/src/choosy/__about__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 choosy-0.0.3/src/choosy/__init__.py
+-rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 choosy-0.0.3/src/choosy/base.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 choosy-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 choosy-0.0.3/tests/test_base.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 choosy-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 choosy-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 choosy-0.0.3/README.md
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 choosy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 choosy-0.0.3/PKG-INFO
```

### Comparing `choosy-0.0.2/.github/workflows/python-package.yml` & `choosy-0.0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `choosy-0.0.2/src/choosy/base.py` & `choosy-0.0.3/src/choosy/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,25 +186,25 @@
                     bin_column=bin_column,
                     weight_column=weight_column,
                     replace=replace,
                     seed=seed,
                     column_name=f"{ii}",
                 ).T
             )
-        out = pd.concat(dfs, axis=0)
+        out = pd.concat(dfs, axis=0).fillna(0)
         out.index = out.index.astype(int)
         return out
 
     def _aggregate_results(self, dfs, count_column, name):
         "Format the results into a single dataframe."
         df = pd.concat(dfs, ignore_index=True)
         if count_column is None:
             return df
         else:
-            return df.groupby(count_column).agg(**{name: pd.NamedAgg(column=count_column, aggfunc="count")}).fillna(0)
+            return df.groupby(count_column).agg(**{name: pd.NamedAgg(column=count_column, aggfunc="count")})
 
     def _format_filter(self, columns, values):
         "Format the filter for the query method."
         filters = []
         for col, val in zip(np.atleast_1d(columns), np.atleast_1d(values)):
             if isinstance(val, str):
                 filters.append(f'{col}=="{val}"')
```

### Comparing `choosy-0.0.2/tests/test_base.py` & `choosy-0.0.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `choosy-0.0.2/.gitignore` & `choosy-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `choosy-0.0.2/LICENSE` & `choosy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `choosy-0.0.2/README.md` & `choosy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `choosy-0.0.2/pyproject.toml` & `choosy-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 [tool.hatch.version]
 path = "src/choosy/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
+  "numpy",
+  "pandas",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
@@ -145,16 +147,16 @@
 branch = true
 parallel = true
 omit = [
   "src/choosy/__about__.py",
 ]
 
 [tool.coverage.paths]
-choosy = ["src/choosy", "*/structured-sampler/src/choosy"]
-tests = ["tests", "*/structured-sampler/tests"]
+choosy = ["src/choosy", "*/choosy/src/choosy"]
+tests = ["tests", "*/choosy/tests"]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
```

### Comparing `choosy-0.0.2/PKG-INFO` & `choosy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: choosy
-Version: 0.0.2
+Version: 0.0.3
 Project-URL: Documentation, https://github.com/ceesem/choosy#readme
 Project-URL: Issues, https://github.com/ceesem/choosy/issues
 Project-URL: Source, https://github.com/ceesem/choosy
 Author-email: Casey Schneider-Mizell <caseysm@gmail.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

