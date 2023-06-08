# Comparing `tmp/quiltplus-0.9.2.tar.gz` & `tmp/quiltplus-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quiltplus-0.9.2.tar", max compression
+gzip compressed data, was "quiltplus-0.9.3.tar", max compression
```

## Comparing `quiltplus-0.9.2.tar` & `quiltplus-0.9.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-03-01 19:37:11.440551 quiltplus-0.9.2/LICENSE.md
--rw-r--r--   0        0        0      668 2023-05-31 14:03:42.566191 quiltplus-0.9.2/README.md
--rw-r--r--   0        0        0      908 2023-06-06 02:31:19.767034 quiltplus-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      468 2023-06-05 00:41:34.765649 quiltplus-0.9.2/quiltplus/__init__.py
--rw-r--r--   0        0        0      716 2023-03-01 19:37:11.446051 quiltplus-0.9.2/quiltplus/ignore.py
--rw-r--r--   0        0        0     3697 2023-06-06 02:31:19.767775 quiltplus-0.9.2/quiltplus/local.py
--rw-r--r--   0        0        0     3960 2023-06-06 02:31:19.768805 quiltplus-0.9.2/quiltplus/package.py
--rw-r--r--   0        0        0      518 2023-06-06 02:31:19.769900 quiltplus-0.9.2/quiltplus/path.py
--rw-r--r--   0        0        0       80 2023-05-31 14:03:42.576780 quiltplus-0.9.2/quiltplus/property.py
--rw-r--r--   0        0        0        0 2023-06-03 15:46:39.663802 quiltplus-0.9.2/quiltplus/py.typed
--rw-r--r--   0        0        0      609 2023-06-03 15:46:39.664625 quiltplus-0.9.2/quiltplus/registry.py
--rw-r--r--   0        0        0      708 2023-06-03 15:46:39.666292 quiltplus-0.9.2/quiltplus/resource.py
--rw-r--r--   0        0        0      366 2023-05-31 14:03:42.579049 quiltplus-0.9.2/quiltplus/root.py
--rw-r--r--   0        0        0     1220 2023-06-06 02:31:19.770765 quiltplus-0.9.2/quiltplus/type.py
--rw-r--r--   0        0        0     1708 2023-06-06 02:31:19.771443 quiltplus-0.9.2/quiltplus/uri.py
--rw-r--r--   0        0        0      589 2023-06-03 15:46:39.669427 quiltplus-0.9.2/quiltplus/versions.py
--rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 quiltplus-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-01 19:37:11.440551 quiltplus-0.9.3/LICENSE.md
+-rw-r--r--   0        0        0      668 2023-05-31 14:03:42.566191 quiltplus-0.9.3/README.md
+-rw-r--r--   0        0        0      916 2023-06-08 06:20:36.366383 quiltplus-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      468 2023-06-05 00:41:34.765649 quiltplus-0.9.3/quiltplus/__init__.py
+-rw-r--r--   0        0        0      716 2023-03-01 19:37:11.446051 quiltplus-0.9.3/quiltplus/ignore.py
+-rw-r--r--   0        0        0     3794 2023-06-08 06:20:36.366907 quiltplus-0.9.3/quiltplus/local.py
+-rw-r--r--   0        0        0     4287 2023-06-08 06:20:36.367537 quiltplus-0.9.3/quiltplus/package.py
+-rw-r--r--   0        0        0      495 2023-06-08 06:20:36.368491 quiltplus-0.9.3/quiltplus/path.py
+-rw-r--r--   0        0        0       80 2023-05-31 14:03:42.576780 quiltplus-0.9.3/quiltplus/property.py
+-rw-r--r--   0        0        0        0 2023-06-03 15:46:39.663802 quiltplus-0.9.3/quiltplus/py.typed
+-rw-r--r--   0        0        0      609 2023-06-03 15:46:39.664625 quiltplus-0.9.3/quiltplus/registry.py
+-rw-r--r--   0        0        0      708 2023-06-03 15:46:39.666292 quiltplus-0.9.3/quiltplus/resource.py
+-rw-r--r--   0        0        0      376 2023-06-07 23:40:53.197044 quiltplus-0.9.3/quiltplus/root.py
+-rw-r--r--   0        0        0     1298 2023-06-08 06:20:36.368989 quiltplus-0.9.3/quiltplus/type.py
+-rw-r--r--   0        0        0     1724 2023-06-07 23:40:53.198698 quiltplus-0.9.3/quiltplus/uri.py
+-rw-r--r--   0        0        0      589 2023-06-03 15:46:39.669427 quiltplus-0.9.3/quiltplus/versions.py
+-rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 quiltplus-0.9.3/PKG-INFO
```

### Comparing `quiltplus-0.9.2/LICENSE.md` & `quiltplus-0.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.2/README.md` & `quiltplus-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.2/pyproject.toml` & `quiltplus-0.9.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quiltplus"
-version = "0.9.2"
+version = "0.9.3"
 description = "Resource-oriented Python API/CLI for Quilt's decentralized social knowledge platform"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["yaml", "api", "resource", "quilt"]
 packages = [
    { include = "quiltplus" }
@@ -16,16 +16,16 @@
 quilt3 = "^5.1.0"
 trio = "^0.22.0"
 isort = "^5.12.0"
 asyncclick = "^8.1.3.4"
 pytest-cov = "^4.0.0"
 anyio = "^3.7.0"
 typing-extensions = "^4.6.3"
-un-yaml = ">=0.2.0"
-# udc = {git = "https://github.com/data-yaml/udc.git", rev = "main"}
+un-yaml = ">=0.3.1"
+# un-yaml = {git = "https://github.com/data-yaml/un-yaml.git", rev = "main"}
 tzlocal = "^5.0.1"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 pytest-trio = "^0.8.0"
 pytest-watcher = "^0.3.1"
 mypy = "^1.3.0"
```

### Comparing `quiltplus-0.9.2/quiltplus/ignore.py` & `quiltplus-0.9.3/quiltplus/ignore.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.2/quiltplus/local.py` & `quiltplus-0.9.3/quiltplus/local.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,61 +37,59 @@
         else:
             subprocess.Popen(["xdg-open", dest])
         return dest
 
     def __init__(self, attrs: dict):
         super().__init__(attrs)
         self.local_registry = get_package_registry()
+        logging.debug(f"get_package_registry(): {self.local_registry}")
         for tmp in QuiltLocal.TempDir():
             logging.info(f"Package using QuiltLocal.TempDir: {tmp}")
             self.last_path = tmp
 
-    def check_dir(self, path: Path | None = None):
-        if not path:
+    def check_dir(self, local_dir: Path | None = None):
+        if not local_dir:
             return self.last_path
 
-        self.last_path = path
-        if not path.exists():
-            logging.warning(f"Path does not exist: {path}")
-            path.mkdir(parents=True, exist_ok=True)
-        elif not path.is_dir():
-            raise ValueError(f"Path is not a directory: {path}")
-        return path
-
-    def check_path(self, opts: dict):
-        path = opts.get(QuiltLocal.K_PTH)
-        return self.check_dir(path)
+        self.last_path = local_dir
+        if not local_dir.exists():
+            logging.warning(f"Path does not exist: {local_dir}")
+            local_dir.mkdir(parents=True, exist_ok=True)
+        elif not local_dir.is_dir():
+            raise ValueError(f"Path is not a directory: {local_dir}")
+        return local_dir
+
+    def check_dir_arg(self, opts: dict):
+        local_dir = opts.get(QuiltLocal.K_DIR)
+        return self.check_dir(local_dir)
 
-    def local_path(self, *paths: str):
+    def local_path(self, *paths: str) -> Path:
         p = self.check_dir()
         for path in paths:
             p = p / path
 
         p.mkdir(parents=True, exist_ok=True)
         return p
 
-    def local_files(self):
+    def local_files(self) -> list[Path]:
         root = self.local_path()
-        return [
-            os.path.relpath(os.path.join(dir, file), root)
-            for (dir, dirs, files) in os.walk(root)
-            for file in files
-        ]
+        return [f for f in root.rglob("*") if f.is_file()]
 
     def dest(self):
-        return str(self.local_path())  # + "/"
+        return str(self.local_path())
 
     def local_cache(self) -> Path:
         base_path = Path(self.local_registry.base.path)
+        logging.debug(f"local_registry.base.path: {base_path}")
         if not base_path.exists():
             logging.warning(f"local_cache does not exist: {base_path}")
         return base_path / self.package
 
     def _diff(self) -> dict[str, str]:
-        """Compare files in local_path to local cache"""
+        """Compare files in local_dir to local cache"""
         cache = self.local_cache()
         if not cache.exists():
             logging.warning(f"_diff: local_cache[{cache}] does not exist")
             return {}
         diff = dircmp(str(cache), self.dest())
         # logging.debug(f"_diff.diff: {diff}")
         results = {
```

### Comparing `quiltplus-0.9.2/quiltplus/package.py` & `quiltplus-0.9.3/quiltplus/package.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 from .local import QuiltLocal
 from .uri import QuiltUri
 
 
 class QuiltPackage(QuiltLocal):
     K_STAGE = "stage"
     K_MSG = "message"
-    ERR_MOD = "Local files have been modified. Use --force to overwrite."
+    ERR_MOD = (
+        f"Local files have been modified. Unset --{QuiltLocal.K_FAIL} to overwrite."
+    )
 
     @classmethod
     def FromURI(cls: Type[Self], uri: str):
         attrs = QuiltUri.AttrsFromUri(uri)
         return cls(attrs)
 
     def __init__(self, attrs: dict):
@@ -26,17 +28,19 @@
 
     def path_uri(self, sub_path: str):
         return self.pkg_uri() + f"&{QuiltPackage.K_PTH}=" + sub_path
 
     async def browse(self):
         logging.debug(f"browse {self.package} {self.registry} {self.hash}")
         try:
-            q = Package.browse(
-                self.package, self.registry, top_hash=self.hash
-            ) if self.hash else Package.browse(self.package, self.registry)
+            q = (
+                Package.browse(self.package, self.registry, top_hash=self.hash)
+                if self.hash
+                else Package.browse(self.package, self.registry)
+            )
             return q
         except Exception as err:
             logging.error(err)
         return None
 
     async def local_pkg(self):
         q = Package().set_dir(".", path=self.dest())
@@ -55,60 +59,63 @@
     def stage_uri(self, stage: str, sub_path: str):
         return self.path_uri(sub_path).replace(
             QuiltPackage.PREFIX, f"{QuiltPackage.PREFIX}{QuiltPackage.K_STAGE}+{stage}+"
         )
 
     async def diff(self, opts: dict = {}):
         """List files that differ from local_cache()"""
-        self.check_path(opts)
+        self.check_dir_arg(opts)
         diffs = self._diff()
         return [self.stage_uri(stage, filename) for filename, stage in diffs.items()]
 
     def unexpected_loss(self, opts, get=True) -> bool:
-        """Check if _diff and not force"""
-        modified = [k for k,v in self._diff().items() if v == "touch"]
-        force = opts.get(QuiltPackage.K_FORCE, False)
-        return len(modified) > 0 and not force
+        """Check if _diff and fallible"""
+        modified = [k for k, v in self._diff().items() if v == "touch"]
+        fallible = opts.get(QuiltPackage.K_FAIL, False)
+        return len(modified) > 0 and fallible
 
     async def get(self, opts: dict = {}):
         """Download package to dest()"""
-        dest = self.check_path(opts)
+        dest = self.check_dir_arg(opts)
+        logging.debug(f"get dest={dest}: {opts}")
         if self.unexpected_loss(opts):
             raise ValueError(f"{dest}: {QuiltPackage.ERR_MOD}\n{self._diff()}")
         q = await self.remote_pkg()
         q.fetch(dest=dest)
-        result = self.local_files()
-        return result
+        files = self.local_files()
+        return [f"file://{fn}" for fn in files]
 
     async def commit(self, opts: dict = {}):
         """Create package in the local registry"""
         pass
 
     async def push(self, q: Package, opts: dict):
         """Generic handler for all push methods"""
+        dest = self.check_dir_arg(opts)
         kwargs = {
             QuiltPackage.K_REG: self.registry,
-            QuiltPackage.K_FORCE: True,
+            QuiltPackage.K_FORCE: not opts.get(QuiltPackage.K_FAIL, False),
             QuiltPackage.K_MSG: opts.get(
                 QuiltPackage.K_MSG, f"{__name__} {QuiltPackage.Now()} @ {opts}"
             ),
         }
-        q.set_dir(".", self.check_path(opts))
+        logging.debug(f"push dest={dest}: {opts}\n{kwargs}")
+        q.set_dir(".", dest)
         q.build(self.package)
         q.push(self.package, **kwargs)
-        self.hash = None
-        await self.browse() # reset to latest
+        self.hash = None  # TODO: get, and return URI with, new hash
+        await self.browse()  # reset local registry to latest
         return [self.uri]
 
     async def put(self, opts: dict = {}):
         """Create a new remote version that exactly matches the local folder"""
         q = Package()
         return await self.push(q, opts)
 
-    # TODO: fail if remote package is newer (unless --force)
+    # TODO: fail if remote package is newer AND --fallible
     async def patch(self, opts: dict = {}):
         """Use contents of directory to (merge) update the remote package"""
         q = await self.remote_pkg()  # reset to latest
         return await self.push(q, opts)
 
     def delete(self):  # remove local cache
         return shutil.rmtree(self.last_path)
```

### Comparing `quiltplus-0.9.2/quiltplus/registry.py` & `quiltplus-0.9.3/quiltplus/registry.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.2/quiltplus/resource.py` & `quiltplus-0.9.3/quiltplus/resource.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.2/quiltplus/type.py` & `quiltplus-0.9.3/quiltplus/type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from datetime import datetime
 
 from tzlocal import get_localzone
-from un_yaml import UnUri
+from un_yaml import UnUri  # type: ignore
 
 
 class QuiltType:
     PREFIX = "quilt+"
     K_BKT = UnUri.K_HOST
+    K_DIR = "dir"
+    K_FILE = "file"
     K_FORCE = "force"
+    K_FAIL = "fallible"
     K_REG = "registry"
 
     # Fragments
     K_PKG = "package"
     K_PTH = "path"
     K_PRP = "property"
     K_CAT = "catalog"
```

### Comparing `quiltplus-0.9.2/quiltplus/uri.py` & `quiltplus-0.9.3/quiltplus/uri.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Create Quilt URI from UnURI attributes
 
-from un_yaml import UnUri
+from un_yaml import UnUri  # type: ignore
 
 from .type import QuiltType
 
 
 class QuiltUri(QuiltType):
     @classmethod
     def FromUnUri(cls, un: UnUri) -> "QuiltUri":
```

### Comparing `quiltplus-0.9.2/quiltplus/versions.py` & `quiltplus-0.9.3/quiltplus/versions.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.2/PKG-INFO` & `quiltplus-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quiltplus
-Version: 0.9.2
+Version: 0.9.3
 Summary: Resource-oriented Python API/CLI for Quilt's decentralized social knowledge platform
 License: MIT
 Keywords: yaml,api,resource,quilt
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Requires-Dist: asyncclick (>=8.1.3.4,<9.0.0.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: quilt3 (>=5.1.0,<6.0.0)
 Requires-Dist: trio (>=0.22.0,<0.23.0)
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Requires-Dist: tzlocal (>=5.0.1,<6.0.0)
-Requires-Dist: un-yaml (>=0.2.0)
+Requires-Dist: un-yaml (>=0.3.1)
 Requires-Dist: urllib3 (<2)
 Description-Content-Type: text/markdown
 
 # QuiltPlus
 
 ## Next-generation API for Quilt Universal Data Collections
```

