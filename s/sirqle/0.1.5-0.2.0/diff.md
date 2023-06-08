# Comparing `tmp/sirqle-0.1.5.tar.gz` & `tmp/sirqle-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirqle-0.1.5.tar", last modified: Wed Apr 19 11:50:01 2023, max compression
+gzip compressed data, was "sirqle-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sirqle-0.1.5.tar` & `sirqle-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      683 2023-04-13 10:02:21.646915 sirqle-0.1.5/.github/workflows/bump.yml
--rw-r--r--   0        0        0     1917 2022-11-07 10:40:09.758048 sirqle-0.1.5/.gitignore
--rw-r--r--   0        0        0     1149 2023-04-12 17:02:21.974466 sirqle-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0    18092 2022-11-07 10:38:03.624761 sirqle-0.1.5/LICENSE
--rw-r--r--   0        0        0     1090 2023-04-19 11:49:41.577776 sirqle-0.1.5/Makefile
--rw-r--r--   0        0        0     3341 2023-04-12 17:02:21.974466 sirqle-0.1.5/README.md
--rw-r--r--   0        0        0      846 2022-10-22 22:08:14.497554 sirqle-0.1.5/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     1636 2023-04-12 17:02:21.974466 sirqle-0.1.5/docs/index.md
--rw-r--r--   0        0        0      153 2022-11-07 11:23:18.775395 sirqle-0.1.5/docs/reference.md
--rw-r--r--   0        0        0      155 2023-02-01 08:04:46.168879 sirqle-0.1.5/mkdocs.yml
--rw-r--r--   0        0        0     1337 2023-04-19 11:49:58.469769 sirqle-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      294 2023-02-01 08:04:46.164879 sirqle-0.1.5/requirements.txt
--rw-r--r--   0        0        0      884 2023-02-01 08:04:46.164879 sirqle-0.1.5/requirements_dev.txt
--rw-r--r--   0        0        0       38 2022-11-02 17:12:51.611854 sirqle-0.1.5/setup.py
--rw-r--r--   0        0        0      126 2023-04-12 17:01:06.634486 sirqle-0.1.5/src/sirqle/__init__.py
--rw-r--r--   0        0        0     9665 2023-04-19 11:48:59.717793 sirqle-0.1.5/src/sirqle/query.py
--rw-r--r--   0        0        0        0 2022-10-11 09:32:28.171344 sirqle-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     1208 2023-04-13 10:02:21.650915 sirqle-0.1.5/tests/test_create.py
--rw-r--r--   0        0        0     3447 2023-04-12 17:02:21.974466 sirqle-0.1.5/tests/test_insert.py
--rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 sirqle-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      683 2023-04-13 10:02:21.646915 sirqle-0.2.0/.github/workflows/bump.yml
+-rw-r--r--   0        0        0     1917 2022-11-07 10:40:09.758048 sirqle-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1149 2023-04-12 17:02:21.974466 sirqle-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2023-05-16 15:49:30.858005 sirqle-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1089 2023-06-06 09:14:00.389308 sirqle-0.2.0/Makefile
+-rw-r--r--   0        0        0     3341 2023-04-12 17:02:21.974466 sirqle-0.2.0/README.md
+-rw-r--r--   0        0        0      846 2022-10-22 22:08:14.497554 sirqle-0.2.0/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     1636 2023-04-12 17:02:21.974466 sirqle-0.2.0/docs/index.md
+-rw-r--r--   0        0        0      153 2022-11-07 11:23:18.775395 sirqle-0.2.0/docs/reference.md
+-rw-r--r--   0        0        0      155 2023-02-01 08:04:46.168879 sirqle-0.2.0/mkdocs.yml
+-rw-r--r--   0        0        0     1337 2023-06-08 12:40:19.488186 sirqle-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      294 2023-02-01 08:04:46.164879 sirqle-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      884 2023-02-01 08:04:46.164879 sirqle-0.2.0/requirements_dev.txt
+-rw-r--r--   0        0        0       38 2022-11-02 17:12:51.611854 sirqle-0.2.0/setup.py
+-rw-r--r--   0        0        0      126 2023-04-12 17:01:06.634486 sirqle-0.2.0/src/sirqle/__init__.py
+-rw-r--r--   0        0        0    10341 2023-06-08 12:39:25.820155 sirqle-0.2.0/src/sirqle/query.py
+-rw-r--r--   0        0        0        0 2022-10-11 09:32:28.171344 sirqle-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1208 2023-04-13 10:02:21.650915 sirqle-0.2.0/tests/test_create.py
+-rw-r--r--   0        0        0     3447 2023-04-12 17:02:21.974466 sirqle-0.2.0/tests/test_insert.py
+-rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 sirqle-0.2.0/PKG-INFO
```

### Comparing `sirqle-0.1.5/.github/workflows/bump.yml` & `sirqle-0.2.0/.github/workflows/bump.yml`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.5/.gitignore` & `sirqle-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.5/.pre-commit-config.yaml` & `sirqle-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.5/Makefile` & `sirqle-0.2.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 BIN = .venv_dev/bin/
 
 
 warn:
 	@echo "Use make for development only!"
 
 install: warn ## install dev venv
-	@python3 -m venv .venv_dev
+	@python -m venv .venv_dev
 	@$(BIN)pip install -e '.[dev]'
 
 startdb: ## start the database
 	@surreal start --bind 127.0.0.1:9120 --log trace --user test --pass test memory > /dev/null 2>db_log.txt &
 	@echo "SurrealDB started at 127.0.0.1:9120"
 
 test: startdb ## run the test suite
```

### Comparing `sirqle-0.1.5/README.md` & `sirqle-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.5/docs/gen_ref_pages.py` & `sirqle-0.2.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.5/docs/index.md` & `sirqle-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.5/pyproject.toml` & `sirqle-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "sirqle"
-version = "0.1.5"
+version = "0.2.0"
 authors = [{ name = "Pythia Dev Team", email = "dev@pythia.social" }]
 description = "SurrealDB Query interface"
 readme = "README.md"
 requires-python = ">=3.10"
-dependencies = ["python-dotenv", "surrealdb==0.3.0"]
+dependencies = ["python-dotenv", "surrealdb>=0.3.0"]
 license = { file = "LICENSE" }
 [project.urls]
 Source = "https://github.com/PythiaSocialTech/sirqle"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["sirqle*"]
@@ -49,15 +49,15 @@
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.1.5"
+version = "0.2.0"
 version_files = ["pyproject.toml:version"]
 tag_format = "v$version"
 bump_message = "bump: $current_version → $new_version [skip ci]"
 
 
 [tool.pytest.ini_options]
 testpaths = 'tests'
```

### Comparing `sirqle-0.1.5/requirements_dev.txt` & `sirqle-0.2.0/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.5/src/sirqle/query.py` & `sirqle-0.2.0/src/sirqle/query.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 from __future__ import annotations
 
 from typing import List, Optional, Tuple
+from urllib.parse import urlparse
 from warnings import warn
 
 from dotenv import dotenv_values
 from surrealdb.http import SurrealHTTP
+from surrealdb.ws import Surreal
 
-HTTP_PARAMS = ["URL", "NAMESPACE", "USERNAME", "PASSWORD", "DATABASE"]
+PARAMS = ["URL", "NAMESPACE", "USERNAME", "PASSWORD", "DATABASE"]
+
+
+CLIENT = {
+    "ws": Surreal,
+    "wss": Surreal,
+    "http": SurrealHTTP,
+    "https": SurrealHTTP,
+}
 
 
 class Config:
     def __init__(
         self,
         env_file: str = ".db_conf",
         client: Optional[SurrealHTTP] = None,
@@ -35,27 +45,35 @@
                 file that has all the previous arguments set
 
         """
         if client:
             self.client = client
         elif env_file:
             conf = dotenv_values(env_file)
-            if set(HTTP_PARAMS).issubset(set(conf.keys())):
-                self.client = SurrealHTTP(
-                    **{param.lower(): conf[param] for param in HTTP_PARAMS}
+            if set(PARAMS).issubset(set(conf.keys())):
+                scheme = str(urlparse(conf["URL"]).scheme)
+                self.client = CLIENT[scheme](
+                    **{param.lower(): conf[param] for param in PARAMS}
                 )
-        elif all([username, database, password, namespace, url]):
-            self.client = SurrealHTTP(
+        elif username and database and password and namespace and url:
+            scheme = str(urlparse(url).scheme)
+            self.client = CLIENT[scheme](
                 url,
                 namespace=namespace,
                 database=database,
                 username=username,
                 password=password,
             )
 
+    async def signup(self, user: str, password: str) -> str:
+        return await self.client.signup({"user": user, "pass": password})
+
+    async def signin(self, user: str, password: str) -> str:
+        return await self.client.signin({"user": user, "pass": password})
+
 
 class Query:
     def __init__(self, config: Config | None = None):
         """Create a `Query` class
 
         The Query module aims to replace the standard SurrealQL and make it more Python
             friendly. Internally it constructs a SurrealQL string from method chaining
@@ -256,27 +274,14 @@
         else:
             warn(
                 "No arguments for RETURN statement. RETURN statement not \
                 added to the query."
             )
         return self
 
-    def use(self, args: str | list | dict | Query) -> Query:
-        """USE statement.
-
-        Args:
-            args: arguments for the statement
-
-        Returns:
-            Query: returns the same `Query` object
-        """
-        self.query += " USE "
-        self.query += self._parse_args(args)
-        return self
-
     def return_(self, args: str | list | dict | Query | None) -> Query:
         """RETURN statement.
 
         Args:
             args: arguments for the statement
 
         Returns:
@@ -324,14 +329,26 @@
 
         """
         if self.client is None:
             raise Exception("No client provided!")
         res = await self._execute_query()
         return res
 
+    async def use(self, ns: str, db: str) -> None:
+        if isinstance(self.client, Surreal):
+            await self.client.use(namespace=ns, database=db)
+        elif isinstance(self.client, SurrealHTTP):
+            self.client = SurrealHTTP(
+                url=self.client._url,
+                namespace=ns,
+                database=db,
+                username=self.client._username,
+                password=self.client._password,
+            )
+
     # HACK:
     def __repr__(self):
         self._end()
         return self.query
 
     def __getitem__(self, key):
         return self.query[key]
```

### Comparing `sirqle-0.1.5/tests/test_create.py` & `sirqle-0.2.0/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.5/tests/test_insert.py` & `sirqle-0.2.0/tests/test_insert.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.5/PKG-INFO` & `sirqle-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sirqle
-Version: 0.1.5
+Version: 0.2.0
 Summary: SurrealDB Query interface
 Author-email: Pythia Dev Team <dev@pythia.social>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
-Requires-Dist: surrealdb==0.3.0
+Requires-Dist: surrealdb>=0.3.0
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-asyncio ; extra == "dev"
 Requires-Dist: pytest-dependency ; extra == "dev"
 Requires-Dist: commitizen ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: mkdocs ; extra == "docs"
```

