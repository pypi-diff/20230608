# Comparing `tmp/pysettings-validator-0.2.0.tar.gz` & `tmp/pysettings-validator-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysettings-validator-0.2.0.tar", last modified: Sun Oct  2 17:58:44 2022, max compression
+gzip compressed data, was "pysettings-validator-0.3.0.tar", last modified: Thu Jun  8 17:46:29 2023, max compression
```

## Comparing `pysettings-validator-0.2.0.tar` & `pysettings-validator-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxr-xr-x   0 palazzem  (1000) palazzem  (1000)        0 2022-10-02 17:58:44.083415 pysettings-validator-0.2.0/
--rw-r--r--   0 palazzem  (1000) palazzem  (1000)     1527 2022-10-02 16:59:55.000000 pysettings-validator-0.2.0/LICENSE
--rw-r--r--   0 palazzem  (1000) palazzem  (1000)     5159 2022-10-02 17:58:44.083415 pysettings-validator-0.2.0/PKG-INFO
--rw-r--r--   0 palazzem  (1000) palazzem  (1000)     4347 2022-10-02 17:22:50.000000 pysettings-validator-0.2.0/README.md
-drwxr-xr-x   0 palazzem  (1000) palazzem  (1000)        0 2022-10-02 17:58:44.082415 pysettings-validator-0.2.0/pysettings/
--rw-r--r--   0 palazzem  (1000) palazzem  (1000)        0 2022-10-02 16:59:55.000000 pysettings-validator-0.2.0/pysettings/__init__.py
--rw-r--r--   0 palazzem  (1000) palazzem  (1000)     4104 2022-10-02 16:59:55.000000 pysettings-validator-0.2.0/pysettings/base.py
--rw-r--r--   0 palazzem  (1000) palazzem  (1000)      330 2022-10-02 16:59:55.000000 pysettings-validator-0.2.0/pysettings/exceptions.py
--rw-r--r--   0 palazzem  (1000) palazzem  (1000)     1542 2022-10-02 16:59:55.000000 pysettings-validator-0.2.0/pysettings/options.py
--rw-r--r--   0 palazzem  (1000) palazzem  (1000)      843 2022-10-02 16:59:55.000000 pysettings-validator-0.2.0/pysettings/validators.py
-drwxr-xr-x   0 palazzem  (1000) palazzem  (1000)        0 2022-10-02 17:58:44.083415 pysettings-validator-0.2.0/pysettings_validator.egg-info/
--rw-r--r--   0 palazzem  (1000) palazzem  (1000)     5159 2022-10-02 17:58:44.000000 pysettings-validator-0.2.0/pysettings_validator.egg-info/PKG-INFO
--rw-r--r--   0 palazzem  (1000) palazzem  (1000)      316 2022-10-02 17:58:44.000000 pysettings-validator-0.2.0/pysettings_validator.egg-info/SOURCES.txt
--rw-r--r--   0 palazzem  (1000) palazzem  (1000)        1 2022-10-02 17:58:44.000000 pysettings-validator-0.2.0/pysettings_validator.egg-info/dependency_links.txt
--rw-r--r--   0 palazzem  (1000) palazzem  (1000)       11 2022-10-02 17:58:44.000000 pysettings-validator-0.2.0/pysettings_validator.egg-info/top_level.txt
--rw-r--r--   0 palazzem  (1000) palazzem  (1000)       38 2022-10-02 17:58:44.083415 pysettings-validator-0.2.0/setup.cfg
--rw-r--r--   0 palazzem  (1000) palazzem  (1000)     3317 2022-10-02 17:57:27.000000 pysettings-validator-0.2.0/setup.py
+drwxr-xr-x   0 palazzem  (1051) palazzem  (1051)        0 2023-06-08 17:46:29.703604 pysettings-validator-0.3.0/
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     1527 2023-06-08 15:50:52.000000 pysettings-validator-0.3.0/LICENSE
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     6405 2023-06-08 17:46:29.703604 pysettings-validator-0.3.0/PKG-INFO
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     5593 2023-06-08 17:42:49.000000 pysettings-validator-0.3.0/README.md
+drwxr-xr-x   0 palazzem  (1051) palazzem  (1051)        0 2023-06-08 17:46:29.703604 pysettings-validator-0.3.0/pysettings/
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)        0 2023-06-08 15:50:52.000000 pysettings-validator-0.3.0/pysettings/__init__.py
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     4642 2023-06-08 17:42:49.000000 pysettings-validator-0.3.0/pysettings/base.py
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)      330 2023-06-08 15:50:52.000000 pysettings-validator-0.3.0/pysettings/exceptions.py
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     1542 2023-06-08 17:30:19.000000 pysettings-validator-0.3.0/pysettings/options.py
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)      843 2023-06-08 15:50:52.000000 pysettings-validator-0.3.0/pysettings/validators.py
+drwxr-xr-x   0 palazzem  (1051) palazzem  (1051)        0 2023-06-08 17:46:29.703604 pysettings-validator-0.3.0/pysettings_validator.egg-info/
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     6405 2023-06-08 17:46:29.000000 pysettings-validator-0.3.0/pysettings_validator.egg-info/PKG-INFO
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)      409 2023-06-08 17:46:29.000000 pysettings-validator-0.3.0/pysettings_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)        1 2023-06-08 17:46:29.000000 pysettings-validator-0.3.0/pysettings_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)       11 2023-06-08 17:46:29.000000 pysettings-validator-0.3.0/pysettings_validator.egg-info/top_level.txt
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)       38 2023-06-08 17:46:29.703604 pysettings-validator-0.3.0/setup.cfg
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     3317 2023-06-08 17:43:16.000000 pysettings-validator-0.3.0/setup.py
+drwxr-xr-x   0 palazzem  (1051) palazzem  (1051)        0 2023-06-08 17:46:29.703604 pysettings-validator-0.3.0/tests/
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)      348 2023-06-08 17:42:49.000000 pysettings-validator-0.3.0/tests/test_fixtures.py
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     2355 2023-06-08 15:50:52.000000 pysettings-validator-0.3.0/tests/test_options.py
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     4713 2023-06-08 17:42:49.000000 pysettings-validator-0.3.0/tests/test_settings.py
+-rw-r--r--   0 palazzem  (1051) palazzem  (1051)     1562 2023-06-08 15:50:52.000000 pysettings-validator-0.3.0/tests/test_validators.py
```

### Comparing `pysettings-validator-0.2.0/LICENSE` & `pysettings-validator-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysettings-validator-0.2.0/PKG-INFO` & `pysettings-validator-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: pysettings-validator
-Version: 0.2.0
-Summary: Python package to store your application settings. Validators are built-in!
-Home-page: https://github.com/palazzem/pysettings
-Author: Emanuele Palazzetti
-Author-email: emanuele.palazzetti@gmail.com
-License: BSD 3-Clause
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # pysettings
 
 [![PyPI version](https://badge.fury.io/py/pysettings-validator.svg)](https://badge.fury.io/py/pysettings-validator)
 [![Linting](https://github.com/palazzem/pysettings/actions/workflows/linting.yaml/badge.svg?branch=master)](https://github.com/palazzem/pysettings/actions/workflows/linting.yaml)
 [![Testing](https://github.com/palazzem/pysettings/actions/workflows/testing.yaml/badge.svg?branch=master)](https://github.com/palazzem/pysettings/actions/workflows/testing.yaml)
 
 Pysettings is a Python package to store your application settings. Compared to some
@@ -123,14 +101,62 @@
 # app/main.py
 settings = Settings()
 settings.dry_run = "Yes"
 settings.description = "Dry run mode!"
 settings.is_valid()  # raises ConfigNotValid exception
 ```
 
+### Test your Settings (pytest)
+
+If you need to change some of your settings during tests, you can use the following snippet
+to restore the previous settings after each test:
+
+```python
+# tests/fixtures/settings.py
+from pysettings.base import BaseSettings
+from pysettings.options import Option
+from pysettings.validators import is_https_url
+
+# Class definition
+class TestSettings(BaseSettings):
+    url = Option(validators=[is_https_url])
+    description = Option()
+
+# Use settings in your application
+settings = TestSettings()
+settings.url = "https://example.com"
+settings.description = "A shiny Website!"
+settings.is_valid()
+
+# tests/conftest.py
+import copy
+import pytest
+
+from .fixtures import settings as config
+
+
+@pytest.fixture
+def settings():
+    previous_config = copy.deepcopy(config.settings)
+    yield config.settings
+    config.settings = previous_config
+
+# tests/test_settings.py
+def test_settings_changes_1(settings):
+    assert settings.description == "A shiny Website!"
+    settings.description = "Test 1"
+    assert settings.description == "Test 1"
+
+
+def test_settings_changes_2(settings):
+    assert settings.description == "A shiny Website!"
+    settings.description = "Test 2"
+    assert settings.description == "Test 2"
+```
+
 ## Development
 
 We accept external contributions even though the project is mostly designed for personal
 needs. If you think some parts can be exposed with a more generic interface, feel free
 to open a GitHub issue and to discuss your suggestion.
 
 ### Coding Guidelines
@@ -142,15 +168,14 @@
 [1]: https://pypi.org/project/flake8/
 [2]: https://github.com/ambv/black
 
 ### Testing
 
 `tox` is used to execute the following test matrix:
 * `lint`: launches `flake8` and `black --check` to be sure the code honors our style guideline
-* `py{35,36,37,38}`: launches `py.test` to execute all tests under Python 3.5, 3.6,
-  3.7 and 3.8.
+* `py{3.7,3.8,3.9,3.10,3.11}`: launches `py.test` to execute tests with different Python versions.
 
 To launch the full test matrix, just:
 
 ```bash
 $ tox
 ```
```

### Comparing `pysettings-validator-0.2.0/README.md` & `pysettings-validator-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: pysettings-validator
+Version: 0.3.0
+Summary: Python package to store your application settings. Validators are built-in!
+Home-page: https://github.com/palazzem/pysettings
+Author: Emanuele Palazzetti
+Author-email: emanuele.palazzetti@gmail.com
+License: BSD 3-Clause
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 # pysettings
 
 [![PyPI version](https://badge.fury.io/py/pysettings-validator.svg)](https://badge.fury.io/py/pysettings-validator)
 [![Linting](https://github.com/palazzem/pysettings/actions/workflows/linting.yaml/badge.svg?branch=master)](https://github.com/palazzem/pysettings/actions/workflows/linting.yaml)
 [![Testing](https://github.com/palazzem/pysettings/actions/workflows/testing.yaml/badge.svg?branch=master)](https://github.com/palazzem/pysettings/actions/workflows/testing.yaml)
 
 Pysettings is a Python package to store your application settings. Compared to some
@@ -101,14 +123,62 @@
 # app/main.py
 settings = Settings()
 settings.dry_run = "Yes"
 settings.description = "Dry run mode!"
 settings.is_valid()  # raises ConfigNotValid exception
 ```
 
+### Test your Settings (pytest)
+
+If you need to change some of your settings during tests, you can use the following snippet
+to restore the previous settings after each test:
+
+```python
+# tests/fixtures/settings.py
+from pysettings.base import BaseSettings
+from pysettings.options import Option
+from pysettings.validators import is_https_url
+
+# Class definition
+class TestSettings(BaseSettings):
+    url = Option(validators=[is_https_url])
+    description = Option()
+
+# Use settings in your application
+settings = TestSettings()
+settings.url = "https://example.com"
+settings.description = "A shiny Website!"
+settings.is_valid()
+
+# tests/conftest.py
+import copy
+import pytest
+
+from .fixtures import settings as config
+
+
+@pytest.fixture
+def settings():
+    previous_config = copy.deepcopy(config.settings)
+    yield config.settings
+    config.settings = previous_config
+
+# tests/test_settings.py
+def test_settings_changes_1(settings):
+    assert settings.description == "A shiny Website!"
+    settings.description = "Test 1"
+    assert settings.description == "Test 1"
+
+
+def test_settings_changes_2(settings):
+    assert settings.description == "A shiny Website!"
+    settings.description = "Test 2"
+    assert settings.description == "Test 2"
+```
+
 ## Development
 
 We accept external contributions even though the project is mostly designed for personal
 needs. If you think some parts can be exposed with a more generic interface, feel free
 to open a GitHub issue and to discuss your suggestion.
 
 ### Coding Guidelines
@@ -120,15 +190,14 @@
 [1]: https://pypi.org/project/flake8/
 [2]: https://github.com/ambv/black
 
 ### Testing
 
 `tox` is used to execute the following test matrix:
 * `lint`: launches `flake8` and `black --check` to be sure the code honors our style guideline
-* `py{35,36,37,38}`: launches `py.test` to execute all tests under Python 3.5, 3.6,
-  3.7 and 3.8.
+* `py{3.7,3.8,3.9,3.10,3.11}`: launches `py.test` to execute tests with different Python versions.
 
 To launch the full test matrix, just:
 
 ```bash
 $ tox
 ```
```

### Comparing `pysettings-validator-0.2.0/pysettings/base.py` & `pysettings-validator-0.3.0/pysettings/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import copy
+
 from .options import Option
 from .exceptions import OptionNotAvailable, ConfigNotValid
 
 
 class BaseSettings(object):
     """Configuration base class that must be extended to define application settings.
     Every setting must be of type ``Option`` otherwise it's not taken in consideration
@@ -21,15 +23,19 @@
 
     def __init__(self):
         """Store options defined as class attributes in a local registry."""
         self._options = []
         for attr, value in self.__class__.__dict__.items():
             option = self._get_option(attr)
             if isinstance(option, Option):
+                # Store the attribute name in the options list and copy the
+                # Option object to avoid sharing the same instance across
+                # settings instances
                 self._options.append(attr)
+                object.__setattr__(self, attr, copy.deepcopy(option))
 
     def __setattr__(self, name, value):
         """Config attributes must be of type Option. This setattr() ensures that the
         Option.value is properly set.
 
         Args:
             name: the name of the attribute.
@@ -64,20 +70,26 @@
             return object.__getattribute__(self, name)
 
     def __getattr__(self, name):
         """``__getattr__`` is called whenever the ``__getattribute__()`` didn't
         find the attribute. In that case it means the given attribute is not
         a configuration option that was defined as class attributes.
 
+        Internal attributes are still accessible.
+
         Args:
             name: the attribute name to retrieve.
         Raise:
             OptionNotAvailable: the configuration option is not present.
         """
-        raise OptionNotAvailable("the option is not present in the current config")
+        if name.startswith("__") and name.endswith("__"):
+            # Providing access to internal attributes is required for pickle and copy
+            return object.__getattribute__(self, name)
+        else:
+            raise OptionNotAvailable("the option is not present in the current config")
 
     def _get_option(self, name):
         """Retrieve the Option instance instead of proxying the call to retrieve
         the ``Option.value``.
 
         Args:
             name: the ``Option`` name.
```

### Comparing `pysettings-validator-0.2.0/pysettings/options.py` & `pysettings-validator-0.3.0/pysettings/options.py`

 * *Files identical despite different names*

### Comparing `pysettings-validator-0.2.0/pysettings/validators.py` & `pysettings-validator-0.3.0/pysettings/validators.py`

 * *Files identical despite different names*

### Comparing `pysettings-validator-0.2.0/pysettings_validator.egg-info/PKG-INFO` & `pysettings-validator-0.3.0/pysettings_validator.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysettings-validator
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python package to store your application settings. Validators are built-in!
 Home-page: https://github.com/palazzem/pysettings
 Author: Emanuele Palazzetti
 Author-email: emanuele.palazzetti@gmail.com
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -123,14 +123,62 @@
 # app/main.py
 settings = Settings()
 settings.dry_run = "Yes"
 settings.description = "Dry run mode!"
 settings.is_valid()  # raises ConfigNotValid exception
 ```
 
+### Test your Settings (pytest)
+
+If you need to change some of your settings during tests, you can use the following snippet
+to restore the previous settings after each test:
+
+```python
+# tests/fixtures/settings.py
+from pysettings.base import BaseSettings
+from pysettings.options import Option
+from pysettings.validators import is_https_url
+
+# Class definition
+class TestSettings(BaseSettings):
+    url = Option(validators=[is_https_url])
+    description = Option()
+
+# Use settings in your application
+settings = TestSettings()
+settings.url = "https://example.com"
+settings.description = "A shiny Website!"
+settings.is_valid()
+
+# tests/conftest.py
+import copy
+import pytest
+
+from .fixtures import settings as config
+
+
+@pytest.fixture
+def settings():
+    previous_config = copy.deepcopy(config.settings)
+    yield config.settings
+    config.settings = previous_config
+
+# tests/test_settings.py
+def test_settings_changes_1(settings):
+    assert settings.description == "A shiny Website!"
+    settings.description = "Test 1"
+    assert settings.description == "Test 1"
+
+
+def test_settings_changes_2(settings):
+    assert settings.description == "A shiny Website!"
+    settings.description = "Test 2"
+    assert settings.description == "Test 2"
+```
+
 ## Development
 
 We accept external contributions even though the project is mostly designed for personal
 needs. If you think some parts can be exposed with a more generic interface, feel free
 to open a GitHub issue and to discuss your suggestion.
 
 ### Coding Guidelines
@@ -142,15 +190,14 @@
 [1]: https://pypi.org/project/flake8/
 [2]: https://github.com/ambv/black
 
 ### Testing
 
 `tox` is used to execute the following test matrix:
 * `lint`: launches `flake8` and `black --check` to be sure the code honors our style guideline
-* `py{35,36,37,38}`: launches `py.test` to execute all tests under Python 3.5, 3.6,
-  3.7 and 3.8.
+* `py{3.7,3.8,3.9,3.10,3.11}`: launches `py.test` to execute tests with different Python versions.
 
 To launch the full test matrix, just:
 
 ```bash
 $ tox
 ```
```

### Comparing `pysettings-validator-0.2.0/setup.py` & `pysettings-validator-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
-VERSION = "0.2.0"
+VERSION = "0.3.0"
 
 # What packages are required for this module to be executed?
 REQUIRES_PYTHON = ">=3.7.0"
 REQUIRED = []
 
 # What packages are optional?
 EXTRAS = {}
```

