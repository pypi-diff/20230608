# Comparing `tmp/caep-0.1.8.tar.gz` & `tmp/caep-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caep-0.1.8.tar", last modified: Thu May  4 16:45:13 2023, max compression
+gzip compressed data, was "caep-0.1.9.tar", last modified: Thu Jun  8 06:03:50 2023, max compression
```

## Comparing `caep-0.1.8.tar` & `caep-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-05-04 16:45:13.847711 caep-0.1.8/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      773 2020-03-11 11:42:29.000000 caep-0.1.8/LICENSE
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-05-04 16:45:13.847711 caep-0.1.8/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9157 2023-03-28 14:28:15.000000 caep-0.1.8/README.md
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-05-04 16:45:13.844377 caep-0.1.8/caep/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      369 2023-03-28 05:50:28.000000 caep-0.1.8/caep/__init__.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     8171 2023-04-21 06:55:27.000000 caep-0.1.8/caep/config.py
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)      922 2023-01-30 06:37:56.000000 caep-0.1.8/caep/example.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1396 2023-03-28 05:50:28.000000 caep-0.1.8/caep/helpers.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        0 2023-01-02 09:23:36.000000 caep-0.1.8/caep/py.typed
--rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    11081 2023-01-30 11:31:45.000000 caep-0.1.8/caep/schema.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1548 2023-01-02 09:23:36.000000 caep-0.1.8/caep/xdg.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-05-04 16:45:13.847711 caep-0.1.8/caep.egg-info/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-05-04 16:45:13.000000 caep-0.1.8/caep.egg-info/PKG-INFO
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      357 2023-05-04 16:45:13.000000 caep-0.1.8/caep.egg-info/SOURCES.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2023-05-04 16:45:13.000000 caep-0.1.8/caep.egg-info/dependency_links.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       23 2023-05-04 16:45:13.000000 caep-0.1.8/caep.egg-info/requires.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        5 2023-05-04 16:45:13.000000 caep-0.1.8/caep.egg-info/top_level.txt
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-03-11 11:43:17.000000 caep-0.1.8/caep.egg-info/zip-safe
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       38 2023-05-04 16:45:13.847711 caep-0.1.8/setup.cfg
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      994 2023-05-04 16:45:10.000000 caep-0.1.8/setup.py
-drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-05-04 16:45:13.847711 caep-0.1.8/tests/
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2420 2023-01-02 09:23:36.000000 caep-0.1.8/tests/test_config.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1455 2023-03-28 05:50:28.000000 caep-0.1.8/tests/test_helpers.py
--rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    10271 2023-04-21 06:55:27.000000 caep-0.1.8/tests/test_schema.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-06-08 06:03:50.793479 caep-0.1.9/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      773 2020-03-11 11:42:29.000000 caep-0.1.9/LICENSE
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-06-08 06:03:50.793479 caep-0.1.9/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9157 2023-03-28 14:28:15.000000 caep-0.1.9/README.md
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-06-08 06:03:50.793479 caep-0.1.9/caep/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      369 2023-03-28 05:50:28.000000 caep-0.1.9/caep/__init__.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)     8348 2023-06-08 06:03:48.000000 caep-0.1.9/caep/config.py
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)      922 2023-01-30 06:37:56.000000 caep-0.1.9/caep/example.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1875 2023-06-08 06:03:48.000000 caep-0.1.9/caep/helpers.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        0 2023-01-02 09:23:36.000000 caep-0.1.9/caep/py.typed
+-rwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)    11081 2023-01-30 11:31:45.000000 caep-0.1.9/caep/schema.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     1548 2023-01-02 09:23:36.000000 caep-0.1.9/caep/xdg.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-06-08 06:03:50.793479 caep-0.1.9/caep.egg-info/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     9606 2023-06-08 06:03:50.000000 caep-0.1.9/caep.egg-info/PKG-INFO
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      357 2023-06-08 06:03:50.000000 caep-0.1.9/caep.egg-info/SOURCES.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2023-06-08 06:03:50.000000 caep-0.1.9/caep.egg-info/dependency_links.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       23 2023-06-08 06:03:50.000000 caep-0.1.9/caep.egg-info/requires.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        5 2023-06-08 06:03:50.000000 caep-0.1.9/caep.egg-info/top_level.txt
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)        1 2020-03-11 11:43:17.000000 caep-0.1.9/caep.egg-info/zip-safe
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)       38 2023-06-08 06:03:50.793479 caep-0.1.9/setup.cfg
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)      994 2023-06-08 06:03:48.000000 caep-0.1.9/setup.py
+drwxr-xr-x   0 fredrikb  (1000) fredrikb  (1000)        0 2023-06-08 06:03:50.793479 caep-0.1.9/tests/
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2420 2023-01-02 09:23:36.000000 caep-0.1.9/tests/test_config.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)     2217 2023-06-08 06:03:48.000000 caep-0.1.9/tests/test_helpers.py
+-rw-r--r--   0 fredrikb  (1000) fredrikb  (1000)    10271 2023-04-21 06:55:27.000000 caep-0.1.9/tests/test_schema.py
```

### Comparing `caep-0.1.8/LICENSE` & `caep-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `caep-0.1.8/PKG-INFO` & `caep-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caep
-Version: 0.1.8
+Version: 0.1.9
 Summary: Config Argument Env Parser (CAEP)
 Home-page: https://github.com/mnemonic-no/caep
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: ISC
 Keywords: mnemonic
 Classifier: Development Status :: 4 - Beta
```

### Comparing `caep-0.1.8/README.md` & `caep-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `caep-0.1.8/caep/config.py` & `caep-0.1.9/caep/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,40 +95,48 @@
     if not ini_files:
         return None
 
     with open(ini_files[0]) as f:
         return f.read()
 
 
-def load_ini(
-    config_id: Optional[str],
-    config_name: Optional[str],
-    opts: Optional[List[str]] = None,
-) -> Tuple[Optional[configparser.ConfigParser], List[str]]:
+def get_early_parser() -> argparse.ArgumentParser:
     """
-    return config, remainder_argv
-
-    config_id and config_name will be used to locate the default config like this,
-    if they are specified:
-        - ~/.config/<CONFIG_ID>/<CONFIG_FILE_NAME>
-        - /etc/<CONFIG_FILE_NAME>
+    return ArgumentParser for early arguments
     """
-
     early_parser = argparse.ArgumentParser(
         description="configfile parser", add_help=False
     )
     early_parser.add_argument(
         "--config",
         dest="config",
         type=argparse.FileType("r", encoding="UTF-8"),
         default=None,
         nargs="+",
         help="change default configuration location",
     )
 
+    return early_parser
+
+
+def load_ini(
+    config_id: Optional[str],
+    config_name: Optional[str],
+    opts: Optional[List[str]] = None,
+) -> Tuple[Optional[configparser.ConfigParser], List[str]]:
+    """
+    return config, remainder_argv
+
+    config_id and config_name will be used to locate the default config like this,
+    if they are specified:
+        - ~/.config/<CONFIG_ID>/<CONFIG_FILE_NAME>
+        - /etc/<CONFIG_FILE_NAME>
+    """
+
+    early_parser = get_early_parser()
     args, remainder_argv = early_parser.parse_known_args(opts)
 
     config = []
 
     if args.config:
         config = [cfg_file.read() for cfg_file in args.config]
```

### Comparing `caep-0.1.8/caep/example.py` & `caep-0.1.9/caep/example.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.8/caep/schema.py` & `caep-0.1.9/caep/schema.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.8/caep/xdg.py` & `caep-0.1.9/caep/xdg.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.8/caep.egg-info/PKG-INFO` & `caep-0.1.9/caep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caep
-Version: 0.1.8
+Version: 0.1.9
 Summary: Config Argument Env Parser (CAEP)
 Home-page: https://github.com/mnemonic-no/caep
 Author: mnemonic AS
 Author-email: opensource@mnemonic.no
 License: ISC
 Keywords: mnemonic
 Classifier: Development Status :: 4 - Beta
```

### Comparing `caep-0.1.8/setup.py` & `caep-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), "rb") as f:
     long_description = f.read().decode("utf-8")
 
 setup(
     name="caep",
-    version="0.1.8",
+    version="0.1.9",
     author="mnemonic AS",
     zip_safe=True,
     author_email="opensource@mnemonic.no",
     description="Config Argument Env Parser (CAEP)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="ISC",
```

### Comparing `caep-0.1.8/tests/test_config.py` & `caep-0.1.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `caep-0.1.8/tests/test_helpers.py` & `caep-0.1.9/tests/test_helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-from typing import Any, Dict, Optional
+import shlex
+from pathlib import Path
+from typing import Any, Dict, List, Optional
 
 import pytest
 from pydantic import BaseModel  # noqa: E0611
 from pydantic import Field, root_validator
 from test_schema import parse_args
 
 import caep
 
+TEST_DATA_DIR = Path(__file__).parent / "data"
+INI_TEST_FILE = TEST_DATA_DIR / "config_testdata.ini"
+SECOND_INI_TEST_FILE = TEST_DATA_DIR / "config_testdata2.ini"
+
 
 class ExampleConfig(BaseModel):
     username: Optional[str] = Field(description="Username")
     password: Optional[str] = Field(description="Password")
     parent_id: Optional[str] = Field(description="Parent ID")
 
     @root_validator
@@ -18,14 +24,33 @@
         """If one argument is set, they should all be set"""
 
         caep.raise_if_some_and_not_all(values, ["username", "password", "parent_id"])
 
         return values
 
 
+def test_config_files() -> None:
+    """raise if config files are not returned correctly"""
+    files = [INI_TEST_FILE.as_posix(), SECOND_INI_TEST_FILE.as_posix()]
+
+    commandline = shlex.split(f"--config {' '.join(files)}")
+    config_files = caep.helpers.config_files(commandline)
+
+    for file in files:
+        assert file in config_files
+
+
+def test_config_files_empty() -> None:
+    """raise if config files are not empty"""
+    commandline: List[str] = []
+    config_files = caep.helpers.config_files(commandline)
+
+    assert config_files == []
+
+
 def test_raise_if_some_and_not_all() -> None:
     """raise_if_some_and_not_all success test"""
     commandline = "--username pytest --password supersecret --parent-id testing".split()
 
     config = parse_args(ExampleConfig, commandline)
 
     assert config.username == "pytest"
```

### Comparing `caep-0.1.8/tests/test_schema.py` & `caep-0.1.9/tests/test_schema.py`

 * *Files identical despite different names*

