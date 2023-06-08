# Comparing `tmp/sirqle-0.2.0.tar.gz` & `tmp/sirqle-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirqle-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sirqle-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sirqle-0.2.0.tar` & `sirqle-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      683 2023-04-13 10:02:21.646915 sirqle-0.2.0/.github/workflows/bump.yml
--rw-r--r--   0        0        0     1917 2022-11-07 10:40:09.758048 sirqle-0.2.0/.gitignore
--rw-r--r--   0        0        0     1149 2023-04-12 17:02:21.974466 sirqle-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2023-05-16 15:49:30.858005 sirqle-0.2.0/LICENSE
--rw-r--r--   0        0        0     1089 2023-06-06 09:14:00.389308 sirqle-0.2.0/Makefile
--rw-r--r--   0        0        0     3341 2023-04-12 17:02:21.974466 sirqle-0.2.0/README.md
--rw-r--r--   0        0        0      846 2022-10-22 22:08:14.497554 sirqle-0.2.0/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     1636 2023-04-12 17:02:21.974466 sirqle-0.2.0/docs/index.md
--rw-r--r--   0        0        0      153 2022-11-07 11:23:18.775395 sirqle-0.2.0/docs/reference.md
--rw-r--r--   0        0        0      155 2023-02-01 08:04:46.168879 sirqle-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0     1337 2023-06-08 12:40:19.488186 sirqle-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      294 2023-02-01 08:04:46.164879 sirqle-0.2.0/requirements.txt
--rw-r--r--   0        0        0      884 2023-02-01 08:04:46.164879 sirqle-0.2.0/requirements_dev.txt
--rw-r--r--   0        0        0       38 2022-11-02 17:12:51.611854 sirqle-0.2.0/setup.py
--rw-r--r--   0        0        0      126 2023-04-12 17:01:06.634486 sirqle-0.2.0/src/sirqle/__init__.py
--rw-r--r--   0        0        0    10341 2023-06-08 12:39:25.820155 sirqle-0.2.0/src/sirqle/query.py
--rw-r--r--   0        0        0        0 2022-10-11 09:32:28.171344 sirqle-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1208 2023-04-13 10:02:21.650915 sirqle-0.2.0/tests/test_create.py
--rw-r--r--   0        0        0     3447 2023-04-12 17:02:21.974466 sirqle-0.2.0/tests/test_insert.py
--rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 sirqle-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      683 2023-04-13 10:02:21.646915 sirqle-0.2.1/.github/workflows/bump.yml
+-rw-r--r--   0        0        0     1917 2022-11-07 10:40:09.758048 sirqle-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1149 2023-04-12 17:02:21.974466 sirqle-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      636 2023-06-08 13:37:27.496997 sirqle-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-05-16 15:49:30.858005 sirqle-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1089 2023-06-06 09:14:00.389308 sirqle-0.2.1/Makefile
+-rw-r--r--   0        0        0     3341 2023-04-12 17:02:21.974466 sirqle-0.2.1/README.md
+-rw-r--r--   0        0        0      846 2022-10-22 22:08:14.497554 sirqle-0.2.1/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     1636 2023-04-12 17:02:21.974466 sirqle-0.2.1/docs/index.md
+-rw-r--r--   0        0        0      153 2022-11-07 11:23:18.775395 sirqle-0.2.1/docs/reference.md
+-rw-r--r--   0        0        0      155 2023-02-01 08:04:46.168879 sirqle-0.2.1/mkdocs.yml
+-rw-r--r--   0        0        0     1337 2023-06-08 13:37:24.972997 sirqle-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      294 2023-02-01 08:04:46.164879 sirqle-0.2.1/requirements.txt
+-rw-r--r--   0        0        0      884 2023-02-01 08:04:46.164879 sirqle-0.2.1/requirements_dev.txt
+-rw-r--r--   0        0        0       38 2022-11-02 17:12:51.611854 sirqle-0.2.1/setup.py
+-rw-r--r--   0        0        0      126 2023-04-12 17:01:06.634486 sirqle-0.2.1/src/sirqle/__init__.py
+-rw-r--r--   0        0        0    10500 2023-06-08 13:36:49.908990 sirqle-0.2.1/src/sirqle/query.py
+-rw-r--r--   0        0        0        0 2022-10-11 09:32:28.171344 sirqle-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1208 2023-04-13 10:02:21.650915 sirqle-0.2.1/tests/test_create.py
+-rw-r--r--   0        0        0     3447 2023-04-12 17:02:21.974466 sirqle-0.2.1/tests/test_insert.py
+-rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 sirqle-0.2.1/PKG-INFO
```

### Comparing `sirqle-0.2.0/.github/workflows/bump.yml` & `sirqle-0.2.1/.github/workflows/bump.yml`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.0/.gitignore` & `sirqle-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.0/.pre-commit-config.yaml` & `sirqle-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.0/LICENSE` & `sirqle-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.0/Makefile` & `sirqle-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.0/README.md` & `sirqle-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.0/docs/gen_ref_pages.py` & `sirqle-0.2.1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.0/docs/index.md` & `sirqle-0.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.0/pyproject.toml` & `sirqle-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sirqle"
-version = "0.2.0"
+version = "0.2.1"
 authors = [{ name = "Pythia Dev Team", email = "dev@pythia.social" }]
 description = "SurrealDB Query interface"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = ["python-dotenv", "surrealdb>=0.3.0"]
 license = { file = "LICENSE" }
 [project.urls]
@@ -49,15 +49,15 @@
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.0"
+version = "0.2.1"
 version_files = ["pyproject.toml:version"]
 tag_format = "v$version"
 bump_message = "bump: $current_version → $new_version [skip ci]"
 
 
 [tool.pytest.ini_options]
 testpaths = 'tests'
```

### Comparing `sirqle-0.2.0/requirements_dev.txt` & `sirqle-0.2.1/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.0/src/sirqle/query.py` & `sirqle-0.2.1/src/sirqle/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,18 @@
             self.client = CLIENT[scheme](
                 url,
                 namespace=namespace,
                 database=database,
                 username=username,
                 password=password,
             )
+        elif url:
+            scheme = str(urlparse(url).scheme)
+            if scheme in ["wss", "ws"]:
+                self.client = CLIENT[scheme](url=url)
 
     async def signup(self, user: str, password: str) -> str:
         return await self.client.signup({"user": user, "pass": password})
 
     async def signin(self, user: str, password: str) -> str:
         return await self.client.signin({"user": user, "pass": password})
```

### Comparing `sirqle-0.2.0/tests/test_create.py` & `sirqle-0.2.1/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.0/tests/test_insert.py` & `sirqle-0.2.1/tests/test_insert.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.2.0/PKG-INFO` & `sirqle-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirqle
-Version: 0.2.0
+Version: 0.2.1
 Summary: SurrealDB Query interface
 Author-email: Pythia Dev Team <dev@pythia.social>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
 Requires-Dist: surrealdb>=0.3.0
 Requires-Dist: pre-commit ; extra == "dev"
```

