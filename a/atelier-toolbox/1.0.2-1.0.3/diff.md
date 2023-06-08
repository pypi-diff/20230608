# Comparing `tmp/atelier_toolbox-1.0.2.tar.gz` & `tmp/atelier_toolbox-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atelier_toolbox-1.0.2.tar", max compression
+gzip compressed data, was "atelier_toolbox-1.0.3.tar", max compression
```

## Comparing `atelier_toolbox-1.0.2.tar` & `atelier_toolbox-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1070 2023-02-08 11:10:21.722435 atelier_toolbox-1.0.2/LICENSE
--rw-r--r--   0        0        0     5170 2023-02-08 11:10:21.722435 atelier_toolbox-1.0.2/README.md
--rw-r--r--   0        0        0      766 2023-02-08 11:10:21.722435 atelier_toolbox-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-08 11:10:21.722435 atelier_toolbox-1.0.2/src/toolbox/__init__.py
--rw-r--r--   0        0        0      547 2023-02-08 11:10:21.722435 atelier_toolbox-1.0.2/src/toolbox/cli.py
--rw-r--r--   0        0        0      829 2023-02-08 11:10:21.722435 atelier_toolbox-1.0.2/src/toolbox/common/calendar.py
--rw-r--r--   0        0        0      461 2023-02-08 11:10:21.722435 atelier_toolbox-1.0.2/src/toolbox/common/exceptions.py
--rw-r--r--   0        0        0      410 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/common/file.py
--rw-r--r--   0        0        0      868 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/common/output.py
--rw-r--r--   0        0        0      836 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/common/work.py
--rw-r--r--   0        0        0      263 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/scripts.py
--rw-r--r--   0        0        0      112 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/sets/business/__init__.py
--rw-r--r--   0        0        0       64 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/sets/business/__version__.py
--rw-r--r--   0        0        0     1721 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/sets/business/cli.py
--rw-r--r--   0        0        0       94 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/sets/dw/__init__.py
--rw-r--r--   0        0        0       64 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/sets/dw/__version__.py
--rw-r--r--   0        0        0     2058 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/sets/dw/cli.py
--rw-r--r--   0        0        0    12979 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/sets/dw/download.py
--rw-r--r--   0        0        0       96 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/sets/hash/__init__.py
--rw-r--r--   0        0        0       64 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/sets/hash/__version__.py
--rw-r--r--   0        0        0     1730 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/sets/hash/cli.py
--rw-r--r--   0        0        0      334 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/sets/hash/hash_algoritms_enum.py
--rw-r--r--   0        0        0       99 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/sets/pdf/__init__.py
--rw-r--r--   0        0        0       64 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/sets/pdf/__version__.py
--rw-r--r--   0        0        0     1605 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/sets/pdf/cli.py
--rw-r--r--   0        0        0     1431 2023-02-08 11:10:21.726435 atelier_toolbox-1.0.2/src/toolbox/sets/pdf/converter.py
--rw-r--r--   0        0        0     6370 1970-01-01 00:00:00.000000 atelier_toolbox-1.0.2/setup.py
--rw-r--r--   0        0        0     6053 1970-01-01 00:00:00.000000 atelier_toolbox-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/LICENSE
+-rw-r--r--   0        0        0     5170 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/README.md
+-rw-r--r--   0        0        0      766 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/src/toolbox/__init__.py
+-rw-r--r--   0        0        0      547 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/src/toolbox/cli.py
+-rw-r--r--   0        0        0      829 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/src/toolbox/common/calendar.py
+-rw-r--r--   0        0        0      461 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/src/toolbox/common/exceptions.py
+-rw-r--r--   0        0        0      410 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/src/toolbox/common/file.py
+-rw-r--r--   0        0        0      868 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/src/toolbox/common/output.py
+-rw-r--r--   0        0        0      836 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/src/toolbox/common/work.py
+-rw-r--r--   0        0        0      263 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/scripts.py
+-rw-r--r--   0        0        0      112 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/business/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/business/__version__.py
+-rw-r--r--   0        0        0     1721 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/business/cli.py
+-rw-r--r--   0        0        0       94 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/dw/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/dw/__version__.py
+-rw-r--r--   0        0        0     2058 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/dw/cli.py
+-rw-r--r--   0        0        0    12979 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/dw/download.py
+-rw-r--r--   0        0        0       96 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/hash/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/hash/__version__.py
+-rw-r--r--   0        0        0     1730 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/hash/cli.py
+-rw-r--r--   0        0        0      334 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/hash/hash_algoritms_enum.py
+-rw-r--r--   0        0        0       99 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/pdf/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/pdf/__version__.py
+-rw-r--r--   0        0        0     1605 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/pdf/cli.py
+-rw-r--r--   0        0        0     1431 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/pdf/converter.py
+-rw-r--r--   0        0        0     6053 1970-01-01 00:00:00.000000 atelier_toolbox-1.0.3/PKG-INFO
```

### Comparing `atelier_toolbox-1.0.2/LICENSE` & `atelier_toolbox-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.2/README.md` & `atelier_toolbox-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.2/pyproject.toml` & `atelier_toolbox-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atelier-toolbox"
-version = "1.0.2"
+version = "1.0.3"
 description = "Tools for various automations 🧰"
 authors = ["Mihai"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/mihaichris/atelier-toolbox"
 keywords = ["toolbox", "automation", "poetry"]
 packages = [{ include = "toolbox", from="src"}]
```

### Comparing `atelier_toolbox-1.0.2/src/toolbox/cli.py` & `atelier_toolbox-1.0.3/src/toolbox/cli.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.2/src/toolbox/common/calendar.py` & `atelier_toolbox-1.0.3/src/toolbox/common/calendar.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.2/src/toolbox/common/output.py` & `atelier_toolbox-1.0.3/src/toolbox/common/output.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.2/src/toolbox/common/work.py` & `atelier_toolbox-1.0.3/src/toolbox/common/work.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.2/src/toolbox/sets/business/cli.py` & `atelier_toolbox-1.0.3/src/toolbox/sets/business/cli.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.2/src/toolbox/sets/dw/cli.py` & `atelier_toolbox-1.0.3/src/toolbox/sets/dw/cli.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.2/src/toolbox/sets/dw/download.py` & `atelier_toolbox-1.0.3/src/toolbox/sets/dw/download.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.2/src/toolbox/sets/hash/cli.py` & `atelier_toolbox-1.0.3/src/toolbox/sets/hash/cli.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.2/src/toolbox/sets/pdf/cli.py` & `atelier_toolbox-1.0.3/src/toolbox/sets/pdf/cli.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.2/src/toolbox/sets/pdf/converter.py` & `atelier_toolbox-1.0.3/src/toolbox/sets/pdf/converter.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.2/setup.py` & `atelier_toolbox-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,71 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: atelier-toolbox
+Version: 1.0.3
+Summary: Tools for various automations 🧰
+Home-page: https://github.com/mihaichris/atelier-toolbox
+License: MIT
+Keywords: toolbox,automation,poetry
+Author: Mihai
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: ocrmypdf (>=14.0.1,<15.0.0)
+Requires-Dist: pdf2docx (>=0.5.6,<0.6.0)
+Requires-Dist: pylint (>=2.15.5,<3.0.0)
+Requires-Dist: pytest (>=7.2,<8.0)
+Requires-Dist: rich (>=12.6.0,<13.0.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: typer[all] (>=0.6.1,<0.7.0)
+Project-URL: Repository, https://github.com/mihaichris/atelier-toolbox
+Description-Content-Type: text/markdown
+
+# atelier-toolbox
+
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mihaichris/atelier-toolbox/build.yml)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mihaichris/atelier-toolbox/test.yml?label=test)
+[![Issues](https://img.shields.io/github/issues/mihaichris/atelier-toolbox)](https://github.com/mihaichris/atelier-toolbox/issues)
+[![License](https://img.shields.io/github/license/mihaichris/atelier-toolbox)](https://github.com/mihaichris/atelier-toolbox/blob/main/LICENSE)
+[![Version](https://img.shields.io/github/v/tag/mihaichris/atelier-toolbox)](https://github.com/mihaichris/atelier-toolbox/blob/main/LICENSE)
+[![Python Version](https://img.shields.io/pypi/pyversions/atelier-toolbox)](https://pypi.org/project/atelier-toolbox/)
+
+## Description
+
+Tools for various automations 🧰.
+
+## Installation
+
+You can install the Toolbox from [PyPI](https://pypi.org/):
+
+```python
+python -m pip install atelier-toolbox
+```
+The package is supported on Python 3.10 and above.
+
+
+## How to use
+
+```python
+Usage: toolbox [OPTIONS] COMMAND [ARGS]...
+
+╭─ Options ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --install-completion          Install completion for the current shell.                                                                                                                                   │
+│ --show-completion             Show completion for the current shell, to copy it or customize the installation.                                                                                            │
+│ --help                        Show this message and exit.                                                                                                                                                 │
+╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Commands ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ business                                                  Business CLI Tool                                                                                                                               │
+│ dw                                                        Download CLI Tool                                                                                                                               │
+│ hash                                                      Hashing Files CLI Tool                                                                                                                          │
+│ pdf                                                       PDF CLI Tool                                                                                                                                    │
+╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
 
-package_dir = \
-{'': 'src'}
+## CHANGELOG
+ Please refer to [CHANGELOG.md](https://github.com/mihaichris/toolbox/blob/main/CHANGELOG.md)
 
-packages = \
-['toolbox',
- 'toolbox.common',
- 'toolbox.sets.business',
- 'toolbox.sets.dw',
- 'toolbox.sets.hash',
- 'toolbox.sets.pdf']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8.1.3,<9.0.0',
- 'ocrmypdf>=14.0.1,<15.0.0',
- 'pdf2docx>=0.5.6,<0.6.0',
- 'pylint>=2.15.5,<3.0.0',
- 'pytest>=7.2,<8.0',
- 'rich>=12.6.0,<13.0.0',
- 'tomli>=2.0.1,<3.0.0',
- 'typer[all]>=0.6.1,<0.7.0']
-
-entry_points = \
-{'console_scripts': ['test = toolbox.scripts:test',
-                     'toolbox = toolbox.cli:main']}
-
-setup_kwargs = {
-    'name': 'atelier-toolbox',
-    'version': '1.0.2',
-    'description': 'Tools for various automations 🧰',
-    'long_description': '# atelier-toolbox\n\n![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mihaichris/atelier-toolbox/build.yml)\n![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mihaichris/atelier-toolbox/test.yml?label=test)\n[![Issues](https://img.shields.io/github/issues/mihaichris/atelier-toolbox)](https://github.com/mihaichris/atelier-toolbox/issues)\n[![License](https://img.shields.io/github/license/mihaichris/atelier-toolbox)](https://github.com/mihaichris/atelier-toolbox/blob/main/LICENSE)\n[![Version](https://img.shields.io/github/v/tag/mihaichris/atelier-toolbox)](https://github.com/mihaichris/atelier-toolbox/blob/main/LICENSE)\n[![Python Version](https://img.shields.io/pypi/pyversions/atelier-toolbox)](https://pypi.org/project/atelier-toolbox/)\n\n## Description\n\nTools for various automations 🧰.\n\n## Installation\n\nYou can install the Toolbox from [PyPI](https://pypi.org/):\n\n```python\npython -m pip install atelier-toolbox\n```\nThe package is supported on Python 3.10 and above.\n\n\n## How to use\n\n```python\nUsage: toolbox [OPTIONS] COMMAND [ARGS]...\n\n╭─ Options ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --install-completion          Install completion for the current shell.                                                                                                                                   │\n│ --show-completion             Show completion for the current shell, to copy it or customize the installation.                                                                                            │\n│ --help                        Show this message and exit.                                                                                                                                                 │\n╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│ business                                                  Business CLI Tool                                                                                                                               │\n│ dw                                                        Download CLI Tool                                                                                                                               │\n│ hash                                                      Hashing Files CLI Tool                                                                                                                          │\n│ pdf                                                       PDF CLI Tool                                                                                                                                    │\n╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n## CHANGELOG\n Please refer to [CHANGELOG.md](https://github.com/mihaichris/toolbox/blob/main/CHANGELOG.md)\n\n## License\n[MIT](https://opensource.org/licenses/MIT)\n',
-    'author': 'Mihai',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/mihaichris/atelier-toolbox',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+## License
+[MIT](https://opensource.org/licenses/MIT)
 
-
-setup(**setup_kwargs)
```

