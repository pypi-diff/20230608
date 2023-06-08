# Comparing `tmp/tor-python-easy-0.1.5.tar.gz` & `tmp/tor_python_easy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tor-python-easy-0.1.5.tar", max compression
+gzip compressed data, was "tor_python_easy-0.1.6.tar", max compression
```

## Comparing `tor-python-easy-0.1.5.tar` & `tor_python_easy-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1071 2022-08-12 15:58:04.458584 tor-python-easy-0.1.5/LICENSE.md
--rw-r--r--   0        0        0     2336 2022-08-12 15:58:04.458584 tor-python-easy-0.1.5/README.md
--rw-r--r--   0        0        0      471 2022-08-12 15:58:04.458584 tor-python-easy-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-12 15:58:04.458584 tor-python-easy-0.1.5/tor_python_easy/__init__.py
--rw-r--r--   0        0        0     1340 2022-08-12 15:58:04.458584 tor-python-easy-0.1.5/tor_python_easy/tor_control_port_client.py
--rw-r--r--   0        0        0      359 2022-08-12 15:58:04.458584 tor-python-easy-0.1.5/tor_python_easy/tor_socks_get_ip_client.py
--rw-r--r--   0        0        0     3130 2022-08-12 15:58:29.457132 tor-python-easy-0.1.5/setup.py
--rw-r--r--   0        0        0     2921 2022-08-12 15:58:29.457421 tor-python-easy-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-08 17:20:00.891541 tor_python_easy-0.1.6/LICENSE.md
+-rw-r--r--   0        0        0     2336 2023-06-08 17:20:00.891541 tor_python_easy-0.1.6/README.md
+-rw-r--r--   0        0        0      471 2023-06-08 17:20:00.895541 tor_python_easy-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 17:20:00.895541 tor_python_easy-0.1.6/tor_python_easy/__init__.py
+-rw-r--r--   0        0        0     1340 2023-06-08 17:20:00.895541 tor_python_easy-0.1.6/tor_python_easy/tor_control_port_client.py
+-rw-r--r--   0        0        0      359 2023-06-08 17:20:00.895541 tor_python_easy-0.1.6/tor_python_easy/tor_socks_get_ip_client.py
+-rw-r--r--   0        0        0     2972 1970-01-01 00:00:00.000000 tor_python_easy-0.1.6/PKG-INFO
```

### Comparing `tor-python-easy-0.1.5/LICENSE.md` & `tor_python_easy-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tor-python-easy-0.1.5/README.md` & `tor_python_easy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tor-python-easy-0.1.5/tor_python_easy/tor_control_port_client.py` & `tor_python_easy-0.1.6/tor_python_easy/tor_control_port_client.py`

 * *Files identical despite different names*

### Comparing `tor-python-easy-0.1.5/setup.py` & `tor_python_easy-0.1.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,91 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tor-python-easy
+Version: 0.1.6
+Summary: Simple library to manage tor proxy and IP changes
+Home-page: https://github.com/markowanga/tor-python-easy
+Author: Marcin Wątroba
+Author-email: markowanga@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PySocks (>=1.7.1,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Description-Content-Type: text/markdown
+
+# tor-python-easy
+
+[![Open Source Love](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
+[![CI Main](https://github.com/markowanga/tor-python-easy/actions/workflows/python-master.yml/badge.svg)](https://github.com/markowanga/tor-python-easy/actions/workflows/python-master.yml)
+[![PyPI version](https://badge.fury.io/py/tor-python-easy.svg)](https://badge.fury.io/py/tor-python-easy)
+[![MIT Licence](https://badges.frapsoft.com/os/mit/mit.svg?v=103)](https://opensource.org/licenses/mit-license.php)
+
+
+**tor-python-easy** was developed for use tor proxy in python with easy interface, which allow for
+changing ip address whenever you want.
+
+Repo is very simple but if you want you can **add new feature request**.
+
+## Donate
+
+If you want to sponsor me, in thanks for the project, please send me some crypto 😁:
+
+|Coin|Wallet address|
+|---|---|
+|Bitcoin|`3EajE9DbLvEmBHLRzjDfG86LyZB4jzsZyg`|
+|Etherum|`0xE43d8C2c7a9af286bc2fc0568e2812151AF9b1FD`|
+
+## Installation
+
+Library is only one file, so you can copy it to project.
+
+However, if you want you can install it with pip:
+
+```bash
+pip3 install tor-python-easy
+```
+
+## Run tor proxy
+
+There are two simple ways to run tor proxy.
+
+1. First one is using docker and docker-compose from this repo. You can manipulate with mapping
+   ports and password.
+   ```shell
+   docker-compose up
+   ```
+2. Second one uses tor installed in OS
+   ```shell
+   tor --controlport 9051 
+   ```
+
+## Use lib with python
+
+1. In terminal
+   ```shell
+   docker-compose up
+   ```
+2. In Python
+   ```python
+   from tor_python_easy.tor_control_port_client import TorControlPortClient
+   from tor_python_easy.tor_socks_get_ip_client import TorSocksGetIpClient
+   
+   if __name__ == '__main__':
+       proxy_config = {
+           'http': 'socks5://localhost:9050',
+           'https': 'socks5://localhost:9050',
+       }
+       ip_client = TorSocksGetIpClient(proxy_config)
+       tor_control_port_client = TorControlPortClient('localhost', 9051, 'test1234')
+   
+       for it in range(10):
+           old_ip = ip_client.get_ip()
+           tor_control_port_client.change_connection_ip(seconds_wait=10)
+           new_ip = ip_client.get_ip()
+           print(f'iteration {it + 1} ::  {old_ip} -> {new_ip}')
+   ```
+   
+   Output will give 10 IP migrations.
 
-packages = \
-['tor_python_easy']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PySocks>=1.7.1,<2.0.0', 'requests>=2.26.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'tor-python-easy',
-    'version': '0.1.5',
-    'description': 'Simple library to manage tor proxy and IP changes',
-    'long_description': "# tor-python-easy\n\n[![Open Source Love](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)\n[![CI Main](https://github.com/markowanga/tor-python-easy/actions/workflows/python-master.yml/badge.svg)](https://github.com/markowanga/tor-python-easy/actions/workflows/python-master.yml)\n[![PyPI version](https://badge.fury.io/py/tor-python-easy.svg)](https://badge.fury.io/py/tor-python-easy)\n[![MIT Licence](https://badges.frapsoft.com/os/mit/mit.svg?v=103)](https://opensource.org/licenses/mit-license.php)\n\n\n**tor-python-easy** was developed for use tor proxy in python with easy interface, which allow for\nchanging ip address whenever you want.\n\nRepo is very simple but if you want you can **add new feature request**.\n\n## Donate\n\nIf you want to sponsor me, in thanks for the project, please send me some crypto 😁:\n\n|Coin|Wallet address|\n|---|---|\n|Bitcoin|`3EajE9DbLvEmBHLRzjDfG86LyZB4jzsZyg`|\n|Etherum|`0xE43d8C2c7a9af286bc2fc0568e2812151AF9b1FD`|\n\n## Installation\n\nLibrary is only one file, so you can copy it to project.\n\nHowever, if you want you can install it with pip:\n\n```bash\npip3 install tor-python-easy\n```\n\n## Run tor proxy\n\nThere are two simple ways to run tor proxy.\n\n1. First one is using docker and docker-compose from this repo. You can manipulate with mapping\n   ports and password.\n   ```shell\n   docker-compose up\n   ```\n2. Second one uses tor installed in OS\n   ```shell\n   tor --controlport 9051 \n   ```\n\n## Use lib with python\n\n1. In terminal\n   ```shell\n   docker-compose up\n   ```\n2. In Python\n   ```python\n   from tor_python_easy.tor_control_port_client import TorControlPortClient\n   from tor_python_easy.tor_socks_get_ip_client import TorSocksGetIpClient\n   \n   if __name__ == '__main__':\n       proxy_config = {\n           'http': 'socks5://localhost:9050',\n           'https': 'socks5://localhost:9050',\n       }\n       ip_client = TorSocksGetIpClient(proxy_config)\n       tor_control_port_client = TorControlPortClient('localhost', 9051, 'test1234')\n   \n       for it in range(10):\n           old_ip = ip_client.get_ip()\n           tor_control_port_client.change_connection_ip(seconds_wait=10)\n           new_ip = ip_client.get_ip()\n           print(f'iteration {it + 1} ::  {old_ip} -> {new_ip}')\n   ```\n   \n   Output will give 10 IP migrations.\n",
-    'author': 'Marcin Wątroba',
-    'author_email': 'markowanga@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/markowanga/tor-python-easy',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

