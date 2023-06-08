# Comparing `tmp/tapisservice-1.4.0a3.tar.gz` & `tmp/tapisservice-1.4.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapisservice-1.4.0a3.tar", max compression
+gzip compressed data, was "tapisservice-1.4.0a4.tar", max compression
```

## Comparing `tapisservice-1.4.0a3.tar` & `tapisservice-1.4.0a4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1086 2023-02-20 20:37:25.853989 tapisservice-1.4.0a3/README.md
--rw-r--r--   0        0        0      853 2023-06-02 21:17:25.907716 tapisservice-1.4.0a3/pyproject.toml
--rw-r--r--   0        0        0     2682 2023-03-02 05:07:52.208778 tapisservice-1.4.0a3/tapisservice/__init__.py
--rw-r--r--   0        0        0    35545 2023-06-02 19:25:04.454134 tapisservice-1.4.0a3/tapisservice/auth.py
--rw-r--r--   0        0        0     6379 2022-04-08 19:00:25.736057 tapisservice-1.4.0a3/tapisservice/config.py
--rw-r--r--   0        0        0     6311 2023-02-20 20:38:01.165617 tapisservice-1.4.0a3/tapisservice/configschema.json
--rw-r--r--   0        0        0     1040 2022-04-08 19:00:25.736057 tapisservice-1.4.0a3/tapisservice/errors.py
--rw-r--r--   0        0        0     1455 2022-04-08 19:00:25.736057 tapisservice-1.4.0a3/tapisservice/logs.py
--rw-r--r--   0        0        0      174 2022-04-08 19:00:25.736057 tapisservice-1.4.0a3/tapisservice/tapisdjango/__init__.py
--rw-r--r--   0        0        0       71 2022-10-28 20:28:11.884719 tapisservice-1.4.0a3/tapisservice/tapisfastapi/__init__.py
--rw-r--r--   0        0        0     3851 2022-05-03 16:51:03.395898 tapisservice-1.4.0a3/tapisservice/tapisfastapi/auth.py
--rw-r--r--   0        0        0     3090 2022-05-03 16:18:04.431729 tapisservice-1.4.0a3/tapisservice/tapisfastapi/utils.py
--rw-r--r--   0        0        0       45 2022-04-08 19:00:25.736057 tapisservice-1.4.0a3/tapisservice/tapisflask/__init__.py
--rw-r--r--   0        0        0     2826 2023-03-02 01:08:58.073370 tapisservice-1.4.0a3/tapisservice/tapisflask/auth.py
--rw-r--r--   0        0        0     1396 2022-04-08 19:00:25.736057 tapisservice-1.4.0a3/tapisservice/tapisflask/resources.py
--rw-r--r--   0        0        0     4133 2023-06-02 21:16:32.544231 tapisservice-1.4.0a3/tapisservice/tapisflask/utils.py
--rw-r--r--   0        0        0    15526 2023-02-20 20:38:01.165617 tapisservice-1.4.0a3/tapisservice/tenants.py
--rw-r--r--   0        0        0        0 2022-04-08 19:00:25.736057 tapisservice-1.4.0a3/tapisservice/utils.py
--rw-r--r--   0        0        0     1979 1970-01-01 00:00:00.000000 tapisservice-1.4.0a3/setup.py
--rw-r--r--   0        0        0     2072 1970-01-01 00:00:00.000000 tapisservice-1.4.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-02-20 20:37:25.853989 tapisservice-1.4.0a4/README.md
+-rw-r--r--   0        0        0      853 2023-06-08 16:19:03.647858 tapisservice-1.4.0a4/pyproject.toml
+-rw-r--r--   0        0        0     2682 2023-03-02 05:07:52.208778 tapisservice-1.4.0a4/tapisservice/__init__.py
+-rw-r--r--   0        0        0    35545 2023-06-02 19:25:04.454134 tapisservice-1.4.0a4/tapisservice/auth.py
+-rw-r--r--   0        0        0     6379 2022-04-08 19:00:25.736057 tapisservice-1.4.0a4/tapisservice/config.py
+-rw-r--r--   0        0        0     6311 2023-02-20 20:38:01.165617 tapisservice-1.4.0a4/tapisservice/configschema.json
+-rw-r--r--   0        0        0     1040 2022-04-08 19:00:25.736057 tapisservice-1.4.0a4/tapisservice/errors.py
+-rw-r--r--   0        0        0     1455 2022-04-08 19:00:25.736057 tapisservice-1.4.0a4/tapisservice/logs.py
+-rw-r--r--   0        0        0      174 2022-04-08 19:00:25.736057 tapisservice-1.4.0a4/tapisservice/tapisdjango/__init__.py
+-rw-r--r--   0        0        0       71 2022-10-28 20:28:11.884719 tapisservice-1.4.0a4/tapisservice/tapisfastapi/__init__.py
+-rw-r--r--   0        0        0     3851 2022-05-03 16:51:03.395898 tapisservice-1.4.0a4/tapisservice/tapisfastapi/auth.py
+-rw-r--r--   0        0        0     3090 2022-05-03 16:18:04.431729 tapisservice-1.4.0a4/tapisservice/tapisfastapi/utils.py
+-rw-r--r--   0        0        0       45 2022-04-08 19:00:25.736057 tapisservice-1.4.0a4/tapisservice/tapisflask/__init__.py
+-rw-r--r--   0        0        0     2826 2023-03-02 01:08:58.073370 tapisservice-1.4.0a4/tapisservice/tapisflask/auth.py
+-rw-r--r--   0        0        0     1396 2022-04-08 19:00:25.736057 tapisservice-1.4.0a4/tapisservice/tapisflask/resources.py
+-rw-r--r--   0        0        0     4234 2023-06-08 15:54:20.717752 tapisservice-1.4.0a4/tapisservice/tapisflask/utils.py
+-rw-r--r--   0        0        0    15526 2023-02-20 20:38:01.165617 tapisservice-1.4.0a4/tapisservice/tenants.py
+-rw-r--r--   0        0        0        0 2022-04-08 19:00:25.736057 tapisservice-1.4.0a4/tapisservice/utils.py
+-rw-r--r--   0        0        0     1979 1970-01-01 00:00:00.000000 tapisservice-1.4.0a4/setup.py
+-rw-r--r--   0        0        0     2072 1970-01-01 00:00:00.000000 tapisservice-1.4.0a4/PKG-INFO
```

### Comparing `tapisservice-1.4.0a3/README.md` & `tapisservice-1.4.0a4/README.md`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a3/pyproject.toml` & `tapisservice-1.4.0a4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tapisservice"
-version = "1.4.0a3"
+version = "1.4.0a4"
 description = "Python lib for interacting with an instance of the Tapis API Framework's tapisservice plugin."
 license = "BSD-4-Clause"
 authors = ["Joe Stubbs <jstubbs@tacc.utexas.edu>"]
 maintainers = ["Joe Stubbs <jstubbs@tacc.utexas.edu>",
 			   "Christian Garcia <cgarcia@tacc.utexas.edu>"]
 readme = "README.md"
 repository = "https://github.com/tapis-project/tapipy-tapisservice"
```

### Comparing `tapisservice-1.4.0a3/tapisservice/__init__.py` & `tapisservice-1.4.0a4/tapisservice/__init__.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a3/tapisservice/auth.py` & `tapisservice-1.4.0a4/tapisservice/auth.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a3/tapisservice/config.py` & `tapisservice-1.4.0a4/tapisservice/config.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a3/tapisservice/configschema.json` & `tapisservice-1.4.0a4/tapisservice/configschema.json`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a3/tapisservice/errors.py` & `tapisservice-1.4.0a4/tapisservice/errors.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a3/tapisservice/logs.py` & `tapisservice-1.4.0a4/tapisservice/logs.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a3/tapisservice/tapisfastapi/auth.py` & `tapisservice-1.4.0a4/tapisservice/tapisfastapi/auth.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a3/tapisservice/tapisfastapi/utils.py` & `tapisservice-1.4.0a4/tapisservice/tapisfastapi/utils.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a3/tapisservice/tapisflask/auth.py` & `tapisservice-1.4.0a4/tapisservice/tapisflask/auth.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a3/tapisservice/tapisflask/resources.py` & `tapisservice-1.4.0a4/tapisservice/tapisflask/resources.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a3/tapisservice/tapisflask/utils.py` & `tapisservice-1.4.0a4/tapisservice/tapisflask/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 # import flask.ext.restful.reqparse as reqparse
 from flask import jsonify, request
 from werkzeug.exceptions import ClientDisconnected
 from flask_restful import Api, reqparse
 import sqlalchemy
 import yaml
 
-from tapipy.tapis import Spec
 from tapisservice.config import conf
 from tapisservice.errors import BaseTapisError
 from tapisservice.logs import get_logger
 logger = get_logger(__name__)
 
 TAG = conf.version
 
 spec_path = os.environ.get("TAPIS_API_SPEC_PATH", '/home/tapis/service/resources/openapi_v3.yml')
 try:
-    spec = Spec.from_file_path(spec_path)
+    # import here because it's a slow import
+    from openapi_core import create_spec
+    spec_dict = yaml.safe_load(open(spec_path, 'r'))
+    spec = create_spec(spec_dict)
 except Exception as e:
     msg = f"Could not find/parse API spec file at path: {spec_path}; additional information: {e}"
     print(msg)
     raise BaseTapisError(msg)
 
 flask_errors_dict = {
     'MethodNotAllowed': {
```

### Comparing `tapisservice-1.4.0a3/tapisservice/tenants.py` & `tapisservice-1.4.0a4/tapisservice/tenants.py`

 * *Files identical despite different names*

### Comparing `tapisservice-1.4.0a3/setup.py` & `tapisservice-1.4.0a4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pycryptodome>=3.6.0', 'tapipy>=1.1.1']
 
 setup_kwargs = {
     'name': 'tapisservice',
-    'version': '1.4.0a3',
+    'version': '1.4.0a4',
     'description': "Python lib for interacting with an instance of the Tapis API Framework's tapisservice plugin.",
     'long_description': 'Tapipy plugin granting Tapis service functionality using `import tapisservice`.\n\n\n## Automated Builds with Make and Poetry\nThis repository includes a Makefile to automate tasks such as building the images and running tests.\nIt depends on Poetry; see the docs for installing on your platform: https://python-poetry.org/docs/\n\nNote: On Ubunut 20 LTS (and maybe other platforms?) you might hit an issue trying to run the `poetry build` \ncommand with your version of virtualenv; see this issue: https://github.com/python-poetry/poetry/issues/2972\n\nThe workaround, as described in the issue, is to remove the version of virtualenv bundled with Ubuntu and install\nit with pip:\n\n```\n $ sudo apt remove --purge python3-virtualenv virtualenv\n $ sudo apt install python3-pip   # if necessary \n $ pip3 install -U virtualenv\n```\n\n## Running the Tests\n\nIn order to run the tests, you will need to populate the `config-dev-develop.json` file within the `tests` with the service password for `abaco` in develop. If you do not know how to get that password, ask for help on the tacc-cloud slack team.\n\n',
     'author': 'Joe Stubbs',
     'author_email': 'jstubbs@tacc.utexas.edu',
     'maintainer': 'Joe Stubbs',
     'maintainer_email': 'jstubbs@tacc.utexas.edu',
     'url': 'https://github.com/tapis-project/tapipy-tapisservice',
```

### Comparing `tapisservice-1.4.0a3/PKG-INFO` & `tapisservice-1.4.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapisservice
-Version: 1.4.0a3
+Version: 1.4.0a4
 Summary: Python lib for interacting with an instance of the Tapis API Framework's tapisservice plugin.
 Home-page: https://github.com/tapis-project/tapipy-tapisservice
 License: BSD-4-Clause
 Author: Joe Stubbs
 Author-email: jstubbs@tacc.utexas.edu
 Maintainer: Joe Stubbs
 Maintainer-email: jstubbs@tacc.utexas.edu
```

