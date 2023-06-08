# Comparing `tmp/drf_misc-0.0.1.tar.gz` & `tmp/drf_misc-1.4.0.tar.gz`

## Comparing `drf_misc-0.0.1.tar` & `drf_misc-1.4.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 drf_misc-0.0.1/.isort.cfg
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 drf_misc-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    20793 2020-02-02 00:00:00.000000 drf_misc-0.0.1/.pylintrc
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 drf_misc-0.0.1/ignore-spelling-words.txt
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 drf_misc-0.0.1/mypy.ini
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 drf_misc-0.0.1/requirements.txt
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 drf_misc-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/__init__.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/admin.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/apps.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/settings.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/core/__init__.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/core/api_exceptions.py
--rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/core/api_views.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/core/audit_service.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/core/cache.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/core/filter_backend.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/core/middlewares.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/core/models.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/core/paginations.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/core/parsers.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/core/permissions.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/core/serializers.py
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/core/services.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/core/throttling.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/utility/__init__.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/utility/decorators.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/utility/epoch_util.py
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/utility/misc.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 drf_misc-0.0.1/src/utility/validator.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 drf_misc-0.0.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 drf_misc-0.0.1/LICENSE
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 drf_misc-0.0.1/README.md
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 drf_misc-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 drf_misc-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 drf_misc-1.4.0/.isort.cfg
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 drf_misc-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    20793 2020-02-02 00:00:00.000000 drf_misc-1.4.0/.pylintrc
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 drf_misc-1.4.0/ignore-spelling-words.txt
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 drf_misc-1.4.0/mypy.ini
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 drf_misc-1.4.0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-1.4.0/setup.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 drf_misc-1.4.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 drf_misc-1.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/admin.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/apps.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/settings.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/core/__init__.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/core/api_exceptions.py
+-rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/core/api_views.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/core/audit_service.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/core/cache.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/core/filter_backend.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/core/middlewares.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/core/models.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/core/paginations.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/core/parsers.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/core/permissions.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/core/serializers.py
+-rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/core/services.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/core/throttling.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/utility/__init__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/utility/decorators.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/utility/epoch_util.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/utility/misc.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 drf_misc-1.4.0/src/utility/validator.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 drf_misc-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 drf_misc-1.4.0/LICENSE
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 drf_misc-1.4.0/README.md
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 drf_misc-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 drf_misc-1.4.0/PKG-INFO
```

### Comparing `drf_misc-0.0.1/.pre-commit-config.yaml` & `drf_misc-1.4.0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -7,72 +7,62 @@
       - id: check-case-conflict
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: fix-encoding-pragma
-      - id: name-tests-test
-        args: [ "--django" ]
       - id: trailing-whitespace
       - id: requirements-txt-fixer
 
-  - repo: https://github.com/ambv/black
-    rev: 23.1.0
-    hooks:
-      - id: black
-
   - repo: https://github.com/PyCQA/autoflake
-    rev:  v2.0.1
+    rev: v2.0.1
     hooks:
       - id: autoflake
         name: Remove unused variables and imports
         language: python
         args:
           [
             "--in-place",
             "--remove-all-unused-imports",
             "--remove-unused-variables",
             "--expand-star-imports",
             "--ignore-init-module-imports",
           ]
         files: \.py$
 
-
   - repo: https://github.com/pycqa/bandit
     rev: 1.7.4
     hooks:
       - id: bandit
-        args: [ '-iii', '-ll' ]
+        args: ["-iii", "-ll"]
 
   - repo: https://github.com/asottile/seed-isort-config
     rev: v2.2.0
     hooks:
       - id: seed-isort-config
 
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
 
-  - repo: https://github.com/pycqa/pylint
-    rev: "v2.16.0"
-    hooks:
-      - id: pylint
-        language: system
-        types: [python]
-        args: [
-          "-rn", # Only display messages
-          "--rcfile=./.pylintrc", # Link to your config file,
-        ]
-        exclude: "[a-zA-Z]*/(migrations)/(.)*"
-
-
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.2
     hooks:
-    -   id: codespell
+      - id: codespell
         name: codespell
         description: Checks for common misspellings in text files.
-        entry: codespell --ignore-words ignore-spelling-words.txt readme.md
+        entry: codespell --ignore-words ignore-spelling-words.txt
         language: python
         types: [text]
+
+  - repo: https://github.com/dhruvmanila/remove-print-statements
+    rev: "v0.5.0"
+    hooks:
+      - id: remove-print-statements
+        args: ["--verbose"]
+
+  - repo: https://github.com/ambv/black
+    rev: 23.1.0
+    hooks:
+      - id: black
```

### Comparing `drf_misc-0.0.1/.pylintrc` & `drf_misc-1.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.1/src/admin.py` & `drf_misc-1.4.0/src/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 if app_settings.ADD_ALL_MODELS_IN_ADMIN:
     models = apps.get_models()
     for i in models:
         AdminClass = type("AdminClass", (ListAdminMixin, admin.ModelAdmin), {})
         try:
             admin.site.register(i, AdminClass)
         except admin.sites.AlreadyRegistered as e:
-            print(e)
+            pass
```

### Comparing `drf_misc-0.0.1/src/settings.py` & `drf_misc-1.4.0/src/settings.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.1/src/core/api_exceptions.py` & `drf_misc-1.4.0/src/core/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.1/src/core/api_views.py` & `drf_misc-1.4.0/src/core/api_views.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.1/src/core/audit_service.py` & `drf_misc-1.4.0/src/core/audit_service.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.1/src/core/filter_backend.py` & `drf_misc-1.4.0/src/core/filter_backend.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.1/src/core/middlewares.py` & `drf_misc-1.4.0/src/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.1/src/core/models.py` & `drf_misc-1.4.0/src/core/models.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.1/src/core/paginations.py` & `drf_misc-1.4.0/src/core/paginations.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.1/src/core/serializers.py` & `drf_misc-1.4.0/src/core/serializers.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.1/src/core/services.py` & `drf_misc-1.4.0/src/core/services.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.1/src/core/throttling.py` & `drf_misc-1.4.0/src/core/throttling.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.1/src/utility/epoch_util.py` & `drf_misc-1.4.0/src/utility/epoch_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,12 +25,9 @@
     for _ in range(count):
         date_iter.append((temp.zero.epoch(), eod(temp.epoch())))
         if asc:
             temp = temp.add(**{period: 1})
         else:
             temp = temp.subtract(**{period: 1})
     for a in date_iter:
-        print(
-            moment.unix(a[0]).timezone("Asia/Kolkata"),
-            moment.unix(a[1]).timezone("Asia/Kolkata"),
-        )
+        pass
     return date_iter
```

### Comparing `drf_misc-0.0.1/src/utility/misc.py` & `drf_misc-1.4.0/src/utility/misc.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.1/src/utility/validator.py` & `drf_misc-1.4.0/src/utility/validator.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.1/.gitignore` & `drf_misc-1.4.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -164,7 +164,10 @@
 *.log
 db.sqlite3
 db.sqlite3-journal
 .pybuilder/
 Pipfile.lock
 poetry.lock
 pdm.lock
+
+
+.pypirc
```

### Comparing `drf_misc-0.0.1/LICENSE` & `drf_misc-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_misc-0.0.1/pyproject.toml` & `drf_misc-1.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "drf-misc"
-version = "0.0.1"
+version = "v1.4.0"
 authors = [
   { name="Abhishek Sharma", email="abhishm20@gmail.com" },
 ]
 description = "A small Django DRF extension library which includes some useful utilities, APIs, Serializers and Services."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `drf_misc-0.0.1/PKG-INFO` & `drf_misc-1.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-misc
-Version: 0.0.1
+Version: 1.4.0
 Summary: A small Django DRF extension library which includes some useful utilities, APIs, Serializers and Services.
 Project-URL: Homepage, https://github.com/abhishm20/drf-misc
 Project-URL: Bug Tracker, https://github.com/abhishm20/drf-misc/issues
 Author-email: Abhishek Sharma <abhishm20@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

