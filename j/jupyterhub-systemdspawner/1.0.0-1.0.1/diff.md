# Comparing `tmp/jupyterhub-systemdspawner-1.0.0.tar.gz` & `tmp/jupyterhub-systemdspawner-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-systemdspawner-1.0.0.tar", last modified: Thu Jun  1 21:28:48 2023, max compression
+gzip compressed data, was "jupyterhub-systemdspawner-1.0.1.tar", last modified: Thu Jun  8 13:12:35 2023, max compression
```

## Comparing `jupyterhub-systemdspawner-1.0.0.tar` & `jupyterhub-systemdspawner-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:28:48.950944 jupyterhub-systemdspawner-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-06-01 21:28:48.950944 jupyterhub-systemdspawner-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:28:48.946944 jupyterhub-systemdspawner-1.0.0/jupyterhub_systemdspawner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-06-01 21:28:48.000000 jupyterhub-systemdspawner-1.0.0/jupyterhub_systemdspawner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-01 21:28:48.000000 jupyterhub-systemdspawner-1.0.0/jupyterhub_systemdspawner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:28:48.000000 jupyterhub-systemdspawner-1.0.0/jupyterhub_systemdspawner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-01 21:28:48.000000 jupyterhub-systemdspawner-1.0.0/jupyterhub_systemdspawner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 21:28:48.000000 jupyterhub-systemdspawner-1.0.0/jupyterhub_systemdspawner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 21:28:48.000000 jupyterhub-systemdspawner-1.0.0/jupyterhub_systemdspawner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 21:28:48.950944 jupyterhub-systemdspawner-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:28:48.946944 jupyterhub-systemdspawner-1.0.0/systemdspawner/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/systemdspawner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/systemdspawner/systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/systemdspawner/systemdspawner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:28:48.946944 jupyterhub-systemdspawner-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/tests/test_systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-01 21:28:36.000000 jupyterhub-systemdspawner-1.0.0/tests/test_systemdspawner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:12:35.773663 jupyterhub-systemdspawner-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-08 13:12:20.000000 jupyterhub-systemdspawner-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 13:12:20.000000 jupyterhub-systemdspawner-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-06-08 13:12:35.773663 jupyterhub-systemdspawner-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15433 2023-06-08 13:12:20.000000 jupyterhub-systemdspawner-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:12:35.773663 jupyterhub-systemdspawner-1.0.1/jupyterhub_systemdspawner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-06-08 13:12:35.000000 jupyterhub-systemdspawner-1.0.1/jupyterhub_systemdspawner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-08 13:12:35.000000 jupyterhub-systemdspawner-1.0.1/jupyterhub_systemdspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:12:35.000000 jupyterhub-systemdspawner-1.0.1/jupyterhub_systemdspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 13:12:35.000000 jupyterhub-systemdspawner-1.0.1/jupyterhub_systemdspawner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 13:12:35.000000 jupyterhub-systemdspawner-1.0.1/jupyterhub_systemdspawner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 13:12:35.000000 jupyterhub-systemdspawner-1.0.1/jupyterhub_systemdspawner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-08 13:12:20.000000 jupyterhub-systemdspawner-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:12:35.773663 jupyterhub-systemdspawner-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-08 13:12:20.000000 jupyterhub-systemdspawner-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:12:35.773663 jupyterhub-systemdspawner-1.0.1/systemdspawner/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 13:12:20.000000 jupyterhub-systemdspawner-1.0.1/systemdspawner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-06-08 13:12:20.000000 jupyterhub-systemdspawner-1.0.1/systemdspawner/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-06-08 13:12:20.000000 jupyterhub-systemdspawner-1.0.1/systemdspawner/systemdspawner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:12:35.773663 jupyterhub-systemdspawner-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-06-08 13:12:20.000000 jupyterhub-systemdspawner-1.0.1/tests/test_systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-08 13:12:20.000000 jupyterhub-systemdspawner-1.0.1/tests/test_systemdspawner.py
```

### Comparing `jupyterhub-systemdspawner-1.0.0/LICENSE` & `jupyterhub-systemdspawner-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-systemdspawner-1.0.0/PKG-INFO` & `jupyterhub-systemdspawner-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-systemdspawner
-Version: 1.0.0
+Version: 1.0.1
 Summary: JupyterHub Spawner using systemd for resource isolation
 Home-page: https://github.com/jupyterhub/systemdspawner
 Author: Yuvi Panda
 Author-email: yuvipanda@gmail.com
 License: 3 Clause BSD
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `jupyterhub-systemdspawner-1.0.0/README.md` & `jupyterhub-systemdspawner-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-systemdspawner-1.0.0/jupyterhub_systemdspawner.egg-info/PKG-INFO` & `jupyterhub-systemdspawner-1.0.1/jupyterhub_systemdspawner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-systemdspawner
-Version: 1.0.0
+Version: 1.0.1
 Summary: JupyterHub Spawner using systemd for resource isolation
 Home-page: https://github.com/jupyterhub/systemdspawner
 Author: Yuvi Panda
 Author-email: yuvipanda@gmail.com
 License: 3 Clause BSD
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `jupyterhub-systemdspawner-1.0.0/pyproject.toml` & `jupyterhub-systemdspawner-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 #
 # ref: https://github.com/your-tools/tbump#readme
 #
 [tool.tbump]
 github_url = "https://github.com/jupyterhub/systemdspawner"
 
 [tool.tbump.version]
-current = "1.0.0"
+current = "1.0.1"
 regex = '''
     (?P<major>\d+)
     \.
     (?P<minor>\d+)
     \.
     (?P<patch>\d+)
     (?P<pre>((a|b|rc)\d+)|)
```

### Comparing `jupyterhub-systemdspawner-1.0.0/setup.py` & `jupyterhub-systemdspawner-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="jupyterhub-systemdspawner",
-    version="1.0.0",
+    version="1.0.1",
     description="JupyterHub Spawner using systemd for resource isolation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jupyterhub/systemdspawner",
     author="Yuvi Panda",
     author_email="yuvipanda@gmail.com",
     license="3 Clause BSD",
```

### Comparing `jupyterhub-systemdspawner-1.0.0/systemdspawner/systemd.py` & `jupyterhub-systemdspawner-1.0.1/systemdspawner/systemd.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 Systemd service utilities.
 
 Contains functions to start, stop & poll systemd services.
 Probably not very useful outside this spawner.
 """
 
 import asyncio
+import functools
 import os
 import re
 import shlex
+import shutil
 import subprocess
 import warnings
 
 # light validation of environment variable keys
 env_pat = re.compile("[A-Za-z_]+")
 
 RUN_ROOT = "/run"
@@ -139,14 +141,32 @@
     if environment_variables:
         runtime_dir = os.path.join(RUN_ROOT, properties["RuntimeDirectory"].split()[0])
         environment_file = make_environment_file(
             runtime_dir, unit_name, environment_variables
         )
         run_cmd.append(f"--property=EnvironmentFile={environment_file}")
 
+    # make sure cmd[0] is absolute, taking $PATH into account.
+    # systemd-run does not use the unit's $PATH environment
+    # to resolve relative paths.
+    if not os.path.isabs(cmd[0]):
+        if environment_variables and "PATH" in environment_variables:
+            # if unit specifies a $PATH, use it
+            path = environment_variables["PATH"]
+        else:
+            # search current process $PATH by default.
+            # this is the default behavior of shutil.which(path=None)
+            # but we still need the value for the error message
+            path = os.getenv("PATH", os.defpath)
+        exe = cmd[0]
+        abs_exe = shutil.which(exe, path=path)
+        if not abs_exe:
+            raise FileNotFoundError(f"{exe} not found on {path}")
+        cmd[0] = abs_exe
+
     # Append typical Spawner "cmd" and "args" on how to start the user server
     run_cmd += cmd + args
 
     proc = await asyncio.create_subprocess_exec(*run_cmd)
 
     return await proc.wait()
 
@@ -199,22 +219,36 @@
 
     Throws CalledProcessError if resetting fails
     """
     proc = await asyncio.create_subprocess_exec("systemctl", "reset-failed", unit_name)
     await proc.wait()
 
 
+@functools.lru_cache
 def get_systemd_version():
     """
     Returns systemd's major version, or None if failing to do so.
     """
     try:
         version_response = subprocess.check_output(["systemctl", "--version"])
+    except Exception as e:
+        warnings.warn(
+            f"Failed to run `systemctl --version` to get systemd version: {e}",
+            RuntimeWarning,
+            stacklevel=2,
+        )
+
+    try:
         # Example response from Ubuntu 22.04:
         #
         # systemd 249 (249.11-0ubuntu3.9)
         # +PAM +AUDIT +SELINUX +APPARMOR +IMA +SMACK +SECCOMP +GCRYPT +GNUTLS +OPENSSL +ACL +BLKID +CURL +ELFUTILS +FIDO2 +IDN2 -IDN +IPTC +KMOD +LIBCRYPTSETUP +LIBFDISK +PCRE2 -PWQUALITY -P11KIT -QRENCODE +BZIP2 +LZ4 +XZ +ZLIB +ZSTD -XKBCOMMON +UTMP +SYSVINIT default-hierarchy=unified
         #
         version = int(float(version_response.split()[1]))
         return version
-    except:
+    except Exception as e:
+        warnings.warn(
+            f"Failed to parse systemd version from `systemctl --version`: {e}. output={version_response}",
+            RuntimeWarning,
+            stacklevel=2,
+        )
         return None
```

### Comparing `jupyterhub-systemdspawner-1.0.0/systemdspawner/systemdspawner.py` & `jupyterhub-systemdspawner-1.0.1/systemdspawner/systemdspawner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import os
 import pwd
 import sys
+import warnings
 
 from jupyterhub.spawner import Spawner
 from jupyterhub.utils import random_port
 from traitlets import Bool, Dict, List, Unicode
 
 from systemdspawner import systemd
 
@@ -153,24 +154,24 @@
 
         self.log.debug(
             "user:%s Initialized spawner with unit %s", self.user.name, self.unit_name
         )
 
         systemd_version = systemd.get_systemd_version()
         if systemd_version is None:
-            self.log.warning(
-                "Failed to parse systemd version from 'systemctl --version'"
-            )
+            # not found, nothing to check
+            # already warned about this in get_systemd_version
+            pass
         elif systemd_version < SYSTEMD_REQUIRED_VERSION:
             self.log.critical(
                 f"systemd version {SYSTEMD_REQUIRED_VERSION} or higher is required, version {systemd_version} is used"
             )
             sys.exit(1)
         elif systemd_version < SYSTEMD_LOWEST_RECOMMENDED_VERSION:
-            self.log.warning(
+            warnings.warn(
                 f"systemd version {SYSTEMD_LOWEST_RECOMMENDED_VERSION} or higher is recommended, version {systemd_version} is used"
             )
 
     def _expand_user_vars(self, string):
         """
         Expand user related variables in a given string
```

### Comparing `jupyterhub-systemdspawner-1.0.0/tests/test_systemd.py` & `jupyterhub-systemdspawner-1.0.1/tests/test_systemd.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,34 @@
         await asyncio.sleep(0.1)
 
         with open(os.path.join(d, "pwd")) as f:
             text = f.read().strip()
             assert text == d
 
 
+async def test_executable_path():
+    unit_name = "systemdspawner-unittest-" + str(time.time())
+    _, env_filename = tempfile.mkstemp()
+    with tempfile.TemporaryDirectory() as d:
+        await systemd.start_transient_service(
+            unit_name,
+            ["bash"],
+            ["-c", f"pwd > {d}/pwd"],
+            working_dir=d,
+            environment_variables={"PATH": os.environ["PATH"]},
+        )
+
+        # Wait a tiny bit for the systemd unit to complete running
+        await asyncio.sleep(0.1)
+
+        with open(os.path.join(d, "pwd")) as f:
+            text = f.read().strip()
+            assert text == d
+
+
 async def test_slice():
     unit_name = "systemdspawner-unittest-" + str(time.time())
     _, env_filename = tempfile.mkstemp()
     with tempfile.TemporaryDirectory() as d:
         await systemd.start_transient_service(
             unit_name,
             ["/bin/bash"],
```

### Comparing `jupyterhub-systemdspawner-1.0.0/tests/test_systemdspawner.py` & `jupyterhub-systemdspawner-1.0.1/tests/test_systemdspawner.py`

 * *Files identical despite different names*

