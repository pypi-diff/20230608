# Comparing `tmp/salt-rewrite-2.4.2.tar.gz` & `tmp/salt-rewrite-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salt-rewrite-2.4.2.tar", max compression
+gzip compressed data, was "salt-rewrite-2.4.3.tar", max compression
```

## Comparing `salt-rewrite-2.4.2.tar` & `salt-rewrite-2.4.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2020-02-05 15:05:21.219175 salt-rewrite-2.4.2/LICENSE
--rw-r--r--   0        0        0      652 2023-06-07 16:31:25.236076 salt-rewrite-2.4.2/pyproject.toml
--rw-r--r--   0        0        0       43 2022-06-23 07:32:30.489445 salt-rewrite-2.4.2/src/saltrewrite/__init__.py
--rw-r--r--   0        0        0     1537 2023-06-07 06:44:56.636972 salt-rewrite-2.4.2/src/saltrewrite/__main__.py
--rw-r--r--   0        0        0     1570 2023-06-07 06:44:53.926961 salt-rewrite-2.4.2/src/saltrewrite/__main__.py~
--rw-r--r--   0        0        0     1416 2022-06-23 07:32:30.506111 salt-rewrite-2.4.2/src/saltrewrite/fixes.py
--rw-r--r--   0        0        0      305 2022-06-23 07:32:30.499445 salt-rewrite-2.4.2/src/saltrewrite/imports/__init__.py
--rw-r--r--   0        0        0     2767 2022-06-23 07:33:00.272886 salt-rewrite-2.4.2/src/saltrewrite/imports/fix_tornado_imports.py
--rw-r--r--   0        0        0      343 2022-06-23 07:46:36.072615 salt-rewrite-2.4.2/src/saltrewrite/salt/__init__.py
--rw-r--r--   0        0        0    26730 2023-06-07 16:30:49.162571 salt-rewrite-2.4.2/src/saltrewrite/salt/fix_docstrings.py
--rw-r--r--   0        0        0    27018 2023-06-07 16:29:54.122309 salt-rewrite-2.4.2/src/saltrewrite/salt/fix_docstrings.py~
--rw-r--r--   0        0        0     5219 2023-06-07 15:43:48.044732 salt-rewrite-2.4.2/src/saltrewrite/salt/fix_dunder_utils.py
--rw-r--r--   0        0        0     5255 2023-06-07 15:31:58.591735 salt-rewrite-2.4.2/src/saltrewrite/salt/fix_dunder_utils.py~
--rw-r--r--   0        0        0      827 2022-06-23 07:32:30.536111 salt-rewrite-2.4.2/src/saltrewrite/testsuite/__init__.py
--rw-r--r--   0        0        0    20763 2022-06-23 07:34:49.989951 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_asserts.py
--rw-r--r--   0        0        0     1224 2022-06-23 07:32:30.486111 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_destructive_test_decorator.py
--rw-r--r--   0        0        0     1210 2022-06-23 07:32:30.502778 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_expensive_test_decorator.py
--rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_requires_network_decorator.py
--rw-r--r--   0        0        0     1270 2022-06-23 07:32:30.499445 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py
--rw-r--r--   0        0        0     1263 2022-06-23 07:32:30.529445 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py
--rw-r--r--   0        0        0     1291 2022-06-23 07:32:30.479445 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py
--rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py
--rw-r--r--   0        0        0     1168 2022-06-23 07:32:30.492778 salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_slow_test_decorator.py
--rw-r--r--   0        0        0     6570 2022-06-23 07:32:30.532778 salt-rewrite-2.4.2/src/saltrewrite/utils.py
--rw-r--r--   0        0        0      903 2023-06-07 16:32:06.949920 salt-rewrite-2.4.2/setup.py
--rw-r--r--   0        0        0      543 2023-06-07 16:32:06.950241 salt-rewrite-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2020-02-05 15:05:21.219175 salt-rewrite-2.4.3/LICENSE
+-rw-r--r--   0        0        0      652 2023-06-08 05:53:09.580698 salt-rewrite-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0       43 2022-06-23 07:32:30.489445 salt-rewrite-2.4.3/src/saltrewrite/__init__.py
+-rw-r--r--   0        0        0     1537 2023-06-07 06:44:56.636972 salt-rewrite-2.4.3/src/saltrewrite/__main__.py
+-rw-r--r--   0        0        0     1570 2023-06-07 06:44:53.926961 salt-rewrite-2.4.3/src/saltrewrite/__main__.py~
+-rw-r--r--   0        0        0     1416 2022-06-23 07:32:30.506111 salt-rewrite-2.4.3/src/saltrewrite/fixes.py
+-rw-r--r--   0        0        0      305 2022-06-23 07:32:30.499445 salt-rewrite-2.4.3/src/saltrewrite/imports/__init__.py
+-rw-r--r--   0        0        0     2767 2022-06-23 07:33:00.272886 salt-rewrite-2.4.3/src/saltrewrite/imports/fix_tornado_imports.py
+-rw-r--r--   0        0        0      343 2022-06-23 07:46:36.072615 salt-rewrite-2.4.3/src/saltrewrite/salt/__init__.py
+-rw-r--r--   0        0        0    26877 2023-06-08 05:49:17.715767 salt-rewrite-2.4.3/src/saltrewrite/salt/fix_docstrings.py
+-rw-r--r--   0        0        0    26877 2023-06-08 05:48:41.215488 salt-rewrite-2.4.3/src/saltrewrite/salt/fix_docstrings.py~
+-rw-r--r--   0        0        0     5326 2023-06-08 04:49:23.504289 salt-rewrite-2.4.3/src/saltrewrite/salt/fix_dunder_utils.py
+-rw-r--r--   0        0        0     5524 2023-06-07 19:25:10.596718 salt-rewrite-2.4.3/src/saltrewrite/salt/fix_dunder_utils.py~
+-rw-r--r--   0        0        0      827 2022-06-23 07:32:30.536111 salt-rewrite-2.4.3/src/saltrewrite/testsuite/__init__.py
+-rw-r--r--   0        0        0    20763 2022-06-23 07:34:49.989951 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_asserts.py
+-rw-r--r--   0        0        0     1224 2022-06-23 07:32:30.486111 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_destructive_test_decorator.py
+-rw-r--r--   0        0        0     1210 2022-06-23 07:32:30.502778 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_expensive_test_decorator.py
+-rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_requires_network_decorator.py
+-rw-r--r--   0        0        0     1270 2022-06-23 07:32:30.499445 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py
+-rw-r--r--   0        0        0     1263 2022-06-23 07:32:30.529445 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py
+-rw-r--r--   0        0        0     1291 2022-06-23 07:32:30.479445 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py
+-rw-r--r--   0        0        0     1227 2022-06-23 07:32:30.496111 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py
+-rw-r--r--   0        0        0     1168 2022-06-23 07:32:30.492778 salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_slow_test_decorator.py
+-rw-r--r--   0        0        0     6570 2022-06-23 07:32:30.532778 salt-rewrite-2.4.3/src/saltrewrite/utils.py
+-rw-r--r--   0        0        0      903 2023-06-08 05:53:39.426485 salt-rewrite-2.4.3/setup.py
+-rw-r--r--   0        0        0      543 2023-06-08 05:53:39.426847 salt-rewrite-2.4.3/PKG-INFO
```

### Comparing `salt-rewrite-2.4.2/LICENSE` & `salt-rewrite-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/pyproject.toml` & `salt-rewrite-2.4.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "salt-rewrite"
-version = "2.4.2"
+version = "2.4.3"
 description = "A set of Bowler code to rewrite parts of Salt"
 authors = ["Pedro Algarvio <pedro@algarvio.me>"]
 license = "Apache-2.0"
 packages = [
   {include = "saltrewrite", from = "src" }
 ]
```

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/__main__.py` & `salt-rewrite-2.4.3/src/saltrewrite/__main__.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/__main__.py~` & `salt-rewrite-2.4.3/src/saltrewrite/__main__.py~`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/fixes.py` & `salt-rewrite-2.4.3/src/saltrewrite/fixes.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/imports/fix_tornado_imports.py` & `salt-rewrite-2.4.3/src/saltrewrite/imports/fix_tornado_imports.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/salt/fix_docstrings.py` & `salt-rewrite-2.4.3/src/saltrewrite/salt/fix_docstrings.py~`

 * *Files 1% similar despite different names*

```diff
@@ -118,25 +118,25 @@
     splitters = (",", "/", " ")
     for splitter in splitters:
         for _vs in version.split(splitter):
             for _splitter in splitters:
                 if _splitter in _vs:
                     break
             else:
-                versions.add(_vs)
+                versions.add(_vs.strip())
     parsed_versions = []
     for version in versions:
         try:
-            version = SaltStackVersion.from_name(version)
+            parsed_versions.append(SaltStackVersion.from_name(version))
         except ValueError:
             try:
-                version = SaltStackVersion.parse(version)
-            except ValueError:
-                pass
-        parsed_versions.append(version)
+                parsed_versions.append(SaltStackVersion.parse(version))
+            except ValueError as exc:
+                raise RuntimeError(f"Unable to parse {version!r} as a SaltStackVersion") from exc
+
     replace_contents = ".. {}:: {}".format(
         vtype, ",".join([v.string for v in sorted(parsed_versions)])
     )
     return replace_contents
 
 
 def _convert_version_names_to_numbers(docstring, filename):
@@ -145,15 +145,15 @@
     """
     return CONVERT_VERSION_NAMES_TO_NUMBERS_RE.sub(
         _handle_convert_version_names_to_numbers_match, docstring
     )
 
 
 CLI_EXAMPLE_CASE_AND_SPACING_RE = re.compile(
-    r"(?:[\n]+)([ ]+)CLI Example(?P<plural>s)?(?:[\s]+)?:(?:[^\n]+)?(?:[\n]+)",
+    r"(?:[\n\r]+)([ ]+)CLI Example(?P<plural>s)?(?:[\s]+)?:(?:[^\n\r]+)?(?:[\n]\r+)",
     flags=re.I | re.MULTILINE,
 )
 CLI_EXAMPLE_MISSING_CODE_BLOCK_RE = re.compile(
     r"\n([ ]+)CLI Example(?P<plural>s)?:\n\n([\s]+)salt ", flags=re.I | re.MULTILINE
 )
 
 
@@ -223,30 +223,30 @@
 # pylint: disable=missing-function-docstring,missing-class-docstring
 
 MAX_SIZE = sys.maxsize
 VERSION_LIMIT = MAX_SIZE - 200
 
 
 @total_ordering
-class SaltVersion(namedtuple("SaltVersion", "name, info, released")):
+class SaltVersion(namedtuple("SaltVersion", "name, info, released")):  # pragma: no cover
     __slots__ = ()
 
     def __new__(cls, name, info, released=False):
         if isinstance(info, int):
             info = (info,)
         return super().__new__(cls, name, info, released)
 
     def __eq__(self, other):
         return self.info == other.info
 
     def __gt__(self, other):
         return self.info > other.info
 
 
-class SaltVersionsInfo(type):
+class SaltVersionsInfo(type):  # pragma: no cover
 
     _sorted_versions = ()
     _current_release = None
     _previous_release = None
     _next_release = None
 
     # ----- Please refrain from fixing whitespace ---------------------------------->
@@ -414,15 +414,15 @@
                 if version == cls.current_release():
                     break
                 previous = version
             cls._previous_release = previous
         return cls._previous_release
 
 
-class SaltStackVersion:
+class SaltStackVersion:  # pragma: no cover
     """
     Handle SaltStack versions class.
 
     Knows how to parse ``git describe`` output, knows about release candidates
     and also supports version comparison.
     """
```

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/salt/fix_docstrings.py~` & `salt-rewrite-2.4.3/src/saltrewrite/salt/fix_docstrings.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,44 +118,42 @@
     splitters = (",", "/", " ")
     for splitter in splitters:
         for _vs in version.split(splitter):
             for _splitter in splitters:
                 if _splitter in _vs:
                     break
             else:
-                versions.add(_vs)
+                versions.add(_vs.strip())
     parsed_versions = []
     for version in versions:
         try:
-            version = SaltStackVersion.from_name(version)
+            parsed_versions.append(SaltStackVersion.from_name(version))
         except ValueError:
             try:
-                version = SaltStackVersion.parse(version)
-            except ValueError:
-                pass
-        parsed_versions.append(version)
-    import click
-    click.echo(f"V1: {parsed_versions}")
-    click.echo(f"V2: {sorted(parsed_versions)}")
-    click.echo(f"V2.1: {sorted(parsed_versions, key=lambda v: v.full_info_all_versions)}")
-    replace_contents = ".. {}:: {}".format(vtype, ",".join([v.string for v in sorted(parsed_versions)]))
+                parsed_versions.append(SaltStackVersion.parse(version))
+            except ValueError as exc:
+                raise RuntimeError(f"Unable to parse {version!r} as a SaltStackVersion") from exc
+
+    replace_contents = ".. {}:: {}".format(
+        vtype, ",".join([v.string for v in sorted(parsed_versions)])
+    )
     return replace_contents
 
 
 def _convert_version_names_to_numbers(docstring, filename):
     """
     Convert Salt version names to their version numbers counterpart
     """
     return CONVERT_VERSION_NAMES_TO_NUMBERS_RE.sub(
         _handle_convert_version_names_to_numbers_match, docstring
     )
 
 
 CLI_EXAMPLE_CASE_AND_SPACING_RE = re.compile(
-    r"(?:[\n]+)([ ]+)CLI Example(?P<plural>s)?(?:[\s]+)?:(?:[^\n]+)?(?:[\n]+)",
+    r"(?:[\n\r]+)([ ]+)CLI Example(?P<plural>s)?(?:[\s]+)?:(?:[^\n\r]+)?(?:[\n\r]+)",
     flags=re.I | re.MULTILINE,
 )
 CLI_EXAMPLE_MISSING_CODE_BLOCK_RE = re.compile(
     r"\n([ ]+)CLI Example(?P<plural>s)?:\n\n([\s]+)salt ", flags=re.I | re.MULTILINE
 )
 
 
@@ -225,30 +223,30 @@
 # pylint: disable=missing-function-docstring,missing-class-docstring
 
 MAX_SIZE = sys.maxsize
 VERSION_LIMIT = MAX_SIZE - 200
 
 
 @total_ordering
-class SaltVersion(namedtuple("SaltVersion", "name, info, released")):
+class SaltVersion(namedtuple("SaltVersion", "name, info, released")):  # pragma: no cover
     __slots__ = ()
 
     def __new__(cls, name, info, released=False):
         if isinstance(info, int):
             info = (info,)
         return super().__new__(cls, name, info, released)
 
     def __eq__(self, other):
         return self.info == other.info
 
     def __gt__(self, other):
         return self.info > other.info
 
 
-class SaltVersionsInfo(type):
+class SaltVersionsInfo(type):  # pragma: no cover
 
     _sorted_versions = ()
     _current_release = None
     _previous_release = None
     _next_release = None
 
     # ----- Please refrain from fixing whitespace ---------------------------------->
@@ -416,15 +414,15 @@
                 if version == cls.current_release():
                     break
                 previous = version
             cls._previous_release = previous
         return cls._previous_release
 
 
-class SaltStackVersion:
+class SaltStackVersion:  # pragma: no cover
     """
     Handle SaltStack versions class.
 
     Knows how to parse ``git describe`` output, knows about release candidates
     and also supports version comparison.
     """
 
@@ -697,17 +695,14 @@
             # We have pre-release information, the other side doesn't
             other_noc_info[other_pre_type] = "zzzzz"
 
         if not self.pre_type and other.pre_type:
             # The other side has pre-release information, we don't
             noc_info[pre_type] = "zzzzz"
 
-        import click
-        click.echo(f"V3: {method} - {tuple(noc_info)} , {tuple(other_noc_info)}")
-
         return method(tuple(noc_info), tuple(other_noc_info))
 
     def __lt__(self, other):
         return self.__compare__(other, lambda _self, _other: _self < _other)
 
     def __le__(self, other):
         return self.__compare__(other, lambda _self, _other: _self <= _other)
```

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/salt/fix_dunder_utils.py` & `salt-rewrite-2.4.3/src/saltrewrite/salt/fix_dunder_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,66 +16,73 @@
 from bowler.types import Leaf
 from bowler.types import Node
 from fissix.fixer_util import Call
 from fissix.fixer_util import Dot
 from fissix.fixer_util import touch_import
 
 
+SALT_DUNDERS = (
+    "__active_provider_name__",
+    "__context__",
+    "__env__",
+    "__events__",
+    "__executors__",
+    "__grains__",
+    "__instance_id__",
+    "__jid_event__",
+    "__low__",
+    "__lowstate__",
+    "__master_opts__",
+    "__opts__",
+    "__pillar__",
+    "__proxy__",
+    "__reg__",
+    "__ret__",
+    "__runner__",
+    "__running__",
+    "__salt__",
+    "__salt_system_encoding__",
+    "__serializers__",
+    "__states__",
+    "__utils__",
+)
+
+
 class DunderParser(ast.NodeTransformer):  # pylint: disable=missing-class-docstring
     # pylint: disable=missing-function-docstring,invalid-name
     def __init__(self):
         self.virtualname = None
         self.uses_salt_dunders = False
 
     def visit_Name(self, node):
-        salt_dunders = (
-            "__active_provider_name__",
-            "__context__",
-            "__env__",
-            "__events__",
-            "__executors__",
-            "__grains__",
-            "__instance_id__",
-            "__jid_event__",
-            "__low__",
-            "__lowstate__",
-            "__master_opts__",
-            "__opts__",
-            "__pillar__",
-            "__proxy__",
-            "__reg__",
-            "__ret__",
-            "__runner__",
-            "__running__",
-            "__salt__",
-            "__salt_system_encoding__",
-            "__serializers__",
-            "__states__",
-            "__utils__",
-        )
-        if node.id in salt_dunders:
+        if node.id in SALT_DUNDERS:
             self.uses_salt_dunders = True
 
     def visit_Assign(self, node):
         for target in node.targets:
             if not isinstance(target, ast.Name):
                 continue
             if target.id == "__virtualname__":
                 self.virtualname = node.value.s
 
     # pylint: enable=missing-function-docstring,invalid-name
 
 
+def _get_salt_code_root():
+    return pathlib.Path.cwd()
+
+
 @lru_cache
 def get_utils_module_info():
     """
     Collect utils modules dunder information.
     """
     mapping = {}
-    for path in pathlib.Path("salt", "utils").rglob("*.py"):
+    salt_utils_package_path = _get_salt_code_root().joinpath("salt", "utils")
+    for path in salt_utils_package_path.rglob("*.py"):
         transformer = DunderParser()
         tree = ast.parse(path.read_text())
         transformer.visit(tree)
         mapping[path.resolve()] = {
             "modname": path.stem,
             "virtualname": transformer.virtualname or path.stem,
             "uses_salt_dunders": transformer.uses_salt_dunders,
@@ -85,21 +92,25 @@
 
 @lru_cache
 def get_utils_module_details(name):
     """
     Return utils module details.
     """
     full_module_name = f"salt.utils.{name}"
-    full_module_path = pathlib.Path(full_module_name.replace(".", os.sep))
+    full_module_path = pathlib.Path(f"{full_module_name.replace('.', os.sep)}.py")
+    utils_module_info = get_utils_module_info()
     if full_module_path.exists():
-        return get_utils_module_info()[full_module_path]
+        return utils_module_info[full_module_path]
     modname = name.split(".")[0]
-    for entry in get_utils_module_info().values():
+    for entry in utils_module_info.values():
         if entry["virtualname"] == modname:
             return entry
+    raise RuntimeError(
+        f"Could not find the python module for {name!r} and '{full_module_path}' " "does not exist"
+    )
 
 
 def rewrite(paths, interactive=False, silent=False):
     """
     Rewrite the passed in paths
     """
     (
```

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/salt/fix_dunder_utils.py~` & `salt-rewrite-2.4.3/src/saltrewrite/salt/fix_dunder_utils.py~`

 * *Files 11% similar despite different names*

```diff
@@ -61,21 +61,26 @@
                 continue
             if target.id == "__virtualname__":
                 self.virtualname = node.value.s
 
     # pylint: enable=missing-function-docstring,invalid-name
 
 
+def _get_salt_code_root():
+    return pathlib.Path.cwd()
+
+
 @lru_cache
 def get_utils_module_info():
     """
     Collect utils modules dunder information.
     """
     mapping = {}
-    for path in pathlib.Path("salt", "utils").rglob("*.py"):
+    salt_utils_package_path = _get_salt_code_root().joinpath("salt", "utils")
+    for path in salt_utils_package_path.rglob("*.py"):
         transformer = DunderParser()
         tree = ast.parse(path.read_text())
         transformer.visit(tree)
         mapping[path.resolve()] = {
             "modname": path.stem,
             "virtualname": transformer.virtualname or path.stem,
             "uses_salt_dunders": transformer.uses_salt_dunders,
@@ -85,28 +90,31 @@
 
 @lru_cache
 def get_utils_module_details(name):
     """
     Return utils module details.
     """
     full_module_name = f"salt.utils.{name}"
-    full_module_path = pathlib.Path(full_module_name.replace(".", os.sep))
+    full_module_path = pathlib.Path(f"{full_module_name.replace('.', os.sep)}.py")
+    utils_module_info = get_utils_module_info()
     if full_module_path.exists():
-        return get_utils_module_info()[full_module_path]
+        return utils_module_info[full_module_path]
     modname = name.split(".")[0]
-    for entry in get_utils_module_info().values():
+    for entry in utils_module_info.values():
         if entry["virtualname"] == modname:
             return entry
+    raise RuntimeError(
+        f"Could not find the python module for {name!r} and '{full_module_path}' " "does not exist"
+    )
 
 
 def rewrite(paths, interactive=False, silent=False):
     """
     Rewrite the passed in paths
     """
-    click.echo(f"PATHS: {paths!r}")
     (
         Query(paths)
         .select(
             """
             (
                 dunder_call=power<
                     '__utils__'
```

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/testsuite/__init__.py` & `salt-rewrite-2.4.3/src/saltrewrite/testsuite/__init__.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_asserts.py` & `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_asserts.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_destructive_test_decorator.py` & `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_destructive_test_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_expensive_test_decorator.py` & `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_expensive_test_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_requires_network_decorator.py` & `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_requires_network_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py` & `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_requires_salt_modules_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py` & `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_requires_salt_states_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py` & `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_skip_if_binaries_missing_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py` & `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_skip_if_not_root_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/testsuite/fix_slow_test_decorator.py` & `salt-rewrite-2.4.3/src/saltrewrite/testsuite/fix_slow_test_decorator.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/src/saltrewrite/utils.py` & `salt-rewrite-2.4.3/src/saltrewrite/utils.py`

 * *Files identical despite different names*

### Comparing `salt-rewrite-2.4.2/setup.py` & `salt-rewrite-2.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ['bowler>=0.9.0', 'fissix>=21.6,<22.0']
 
 entry_points = \
 {'console_scripts': ['salt-rewrite = saltrewrite.__main__:rewrite']}
 
 setup_kwargs = {
     'name': 'salt-rewrite',
-    'version': '2.4.2',
+    'version': '2.4.3',
     'description': 'A set of Bowler code to rewrite parts of Salt',
     'long_description': None,
     'author': 'Pedro Algarvio',
     'author_email': 'pedro@algarvio.me',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `salt-rewrite-2.4.2/PKG-INFO` & `salt-rewrite-2.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-rewrite
-Version: 2.4.2
+Version: 2.4.3
 Summary: A set of Bowler code to rewrite parts of Salt
 License: Apache-2.0
 Author: Pedro Algarvio
 Author-email: pedro@algarvio.me
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

