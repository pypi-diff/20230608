# Comparing `tmp/firmitas-0.1.1.tar.gz` & `tmp/firmitas-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firmitas-0.1.1.tar", max compression
+gzip compressed data, was "firmitas-0.1.2.tar", max compression
```

## Comparing `firmitas-0.1.1.tar` & `firmitas-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0    35148 2023-06-01 12:05:07.834486 firmitas-0.1.1/LICENSE
--rw-r--r--   0        0        0     9560 2023-06-01 12:03:07.446782 firmitas-0.1.1/README.md
--rw-r--r--   0        0        0     2037 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/base/__init__.py
--rw-r--r--   0        0        0     7304 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/base/maintool.py
--rw-r--r--   0        0        0        0 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/conf/__init__.py
--rw-r--r--   0        0        0    19059 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/conf/certlist.yml
--rw-r--r--   0        0        0      203 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/conf/logrdata.py
--rw-r--r--   0        0        0     1611 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/conf/standard.py
--rw-r--r--   0        0        0      617 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/main.py
--rw-r--r--   0        0        0     1147 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/unit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/unit/gogithub.py
--rw-r--r--   0        0        0     2096 2023-06-01 12:03:07.446782 firmitas-0.1.1/firmitas/unit/gopagure.py
--rw-r--r--   0        0        0     1780 2023-06-01 12:52:05.267866 firmitas-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    10605 2023-06-01 13:20:34.545662 firmitas-0.1.1/setup.py
--rw-r--r--   0        0        0    11052 2023-06-01 13:20:34.546119 firmitas-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-06 13:46:04.925465 firmitas-0.1.2/LICENSE
+-rw-r--r--   0        0        0     9560 2023-06-06 13:46:04.925465 firmitas-0.1.2/README.md
+-rw-r--r--   0        0        0     2037 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/base/__init__.py
+-rw-r--r--   0        0        0     7304 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/base/maintool.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/conf/__init__.py
+-rw-r--r--   0        0        0    19059 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/conf/certlist.yml
+-rw-r--r--   0        0        0      203 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/conf/logrdata.py
+-rw-r--r--   0        0        0     1611 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/conf/standard.py
+-rw-r--r--   0        0        0      617 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/main.py
+-rw-r--r--   0        0        0     1147 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/unit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/unit/gogithub.py
+-rw-r--r--   0        0        0     2096 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/unit/gopagure.py
+-rw-r--r--   0        0        0     1780 2023-06-08 05:48:14.087401 firmitas-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    11103 1970-01-01 00:00:00.000000 firmitas-0.1.2/PKG-INFO
```

### Comparing `firmitas-0.1.1/LICENSE` & `firmitas-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.1/README.md` & `firmitas-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.1/firmitas/__init__.py` & `firmitas-0.1.2/firmitas/__init__.py`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.1/firmitas/base/maintool.py` & `firmitas-0.1.2/firmitas/base/maintool.py`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.1/firmitas/conf/certlist.yml` & `firmitas-0.1.2/firmitas/conf/certlist.yml`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.1/firmitas/conf/standard.py` & `firmitas-0.1.2/firmitas/conf/standard.py`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.1/firmitas/main.py` & `firmitas-0.1.2/firmitas/main.py`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.1/firmitas/unit/__init__.py` & `firmitas-0.1.2/firmitas/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.1/firmitas/unit/gopagure.py` & `firmitas-0.1.2/firmitas/unit/gopagure.py`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.1/pyproject.toml` & `firmitas-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firmitas"
-version = "0.1.1"
+version = "0.1.2"
 description = "Simple notification service for X.509-standard TLS certificate statuses"
 authors = ["Akashdeep Dhar <akashdeep.dhar@gmail.com>"]
 license = "GPL-3.0-or-later"
 maintainers = ["Akashdeep Dhar <akashdeep.dhar@gmail.com>"]
 readme = "README.md"
 homepage = "https://gitlab.com/t0xic0der/firmitas/"
 repository = "https://gitlab.com/t0xic0der/firmitas/"
@@ -24,15 +24,15 @@
     "Topic :: System :: Networking",
     "Topic :: System :: Networking :: Monitoring",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 click = ">=8.0.0,<9"
-cryptography = ">=36.0.0,<40"
+cryptography = ">=36.0.0,<42"
 pyyaml = ">=5.0.0,<7"
 requests = ">=2.20.0,<3"
 
 [tool.poetry.dev-dependencies]
 black = "^23.0.0"
 isort = "^5.10.1"
 pytest = "^7.1.3"
```

### Comparing `firmitas-0.1.1/setup.py` & `firmitas-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,125 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: firmitas
+Version: 0.1.2
+Summary: Simple notification service for X.509-standard TLS certificate statuses
+Home-page: https://gitlab.com/t0xic0der/firmitas/
+License: GPL-3.0-or-later
+Keywords: notification,security,certificate
+Author: Akashdeep Dhar
+Author-email: akashdeep.dhar@gmail.com
+Maintainer: Akashdeep Dhar
+Maintainer-email: akashdeep.dhar@gmail.com
+Requires-Python: >=3.8,<4
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Security
+Classifier: Topic :: Security :: Cryptography
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: System :: Networking :: Monitoring
+Classifier: Topic :: System :: Operating System
+Requires-Dist: click (>=8.0.0,<9)
+Requires-Dist: cryptography (>=36.0.0,<42)
+Requires-Dist: pyyaml (>=5.0.0,<7)
+Requires-Dist: requests (>=2.20.0,<3)
+Project-URL: Documentation, https://gitlab.com/t0xic0der/firmitas/-/blob/main/README.md
+Project-URL: Repository, https://gitlab.com/t0xic0der/firmitas/
+Description-Content-Type: text/markdown
+
+# firmitas
+
+Simple notification service for X.509-standard TLS certificate statuses
+
+## `__usage__`
+
+1. Clone the repository to your local storage and make it the present working directory.
+   ```
+   $ git clone https://gitlab.com/t0xic0der/firmitas.git
+   ```
+   ```
+   $ cd firmitas
+   ```
+2. Ensure that [`Poetry`](https://python-poetry.org/) and [Virtualenv](https://pypi.org/project/virtualenv/) are installed and up-to-date on the system.
+   ```
+   $ sudo dnf install --assumeyes poetry virtualenv
+   ```
+3. Create a virtual environment within the cloned local directory and enable it.
+   ```
+   $ virtualenv venv
+   ```
+   ```
+   $ source venv/bin/activate
+   ```
+4. Install the project and its dependencies in the enabled virtual environment.
+   ```
+   $ (venv) poetry install
+   ```
+5. Make a copy of the project configuration file and make your changes to it.
+   ```
+   $ (venv) cp firmitas/conf/standard.py firmitas/conf/myconfig.py
+   ```
+   The project configuration file houses the following variables that can be modified according to the requirements of the project user.  
+   - `gitforge` - The source code forge on which the issue tickets need to be created. The valid options for this configuration variable are `github`, `gitlab` and `pagure`. The support for `pagure` is implemented while that for `github` and `gitlab` is planned.
+   - `repoloca` - The location of the ticketing repository. This is required for source code forges that require the absolute location of the remote ticketing repository for the project to be able to access the API and create notification tickets.
+   - `reponame` - The name of the ticketing repository. This is required for source code forges that require the repository name with namespace of the remote ticketing repository for the project to be able to access the API and create notification tickets.
+   - `username` - The username to masquerade as in order to create notification tickets. This is required for source code forges that require the username with whom an API token is associated for the project to be authenticated on their behalf.
+   - `password` - The password or API token belonging to the aforementioned username. This is required for source code forges that require the password or API token associated with the ticketing repository to authenticate the project on the owner's behalf.
+   - `daysqant` - The minimum number of days remaining from the validity expiry date to make notifications for. As a sane default, it is set to open up a notification ticket when the TLS certificate is 30 days away from its validation expiry date.
+   - `tagslist` - The list of labels to the tag the notification tickets with. A minimum of one label is required to ensure that there is a way to filter out the automated notification tickets on a shared issue tracker from the manually created ones.
+   - `maxretry` - The maximum number of retries to make when the process of opening up a notification ticket fails. As a sane default, it is set to allow up to 5 retries, and it is a good practice to have a value greater than one to compensate for spotty connections.
+   - `certloca` - The location where the X.509 standard TLS certificates are stored. Note that this refers to a locally available storage location and not a remotely available storage location. The default is set as "/var/tmp/firmitas/certhere" directory.
+   - `hostloca` - The location where the mapping file of service hostnames, maintainers, certificate statistics and notification statistics are stored. As with the previous configuration variable, even this one refers to a locally available storage location.
+   - `logrconf` - The configuration variable that sets the logging behaviour for the project. As a sane default, the logging level has been set to "DEBUG" to allow for greater verbosity in details and a custom format to the console handler.
+   - `certdict` - The global variable used across the project to share the details of the certificates to be probed into, the statistics of issuing authority, serial number, dates information and much more. Do not change it as this gets overridden.
+6. Make a copy of the mapping configuration file and make your changes to it.
+   ```
+   $ (venv) cp firmitas/conf/certlist.yml firmitas/conf/mytlscts.yml
+   ```
+   The mapping configuration file houses a list of service hostnames having the following variables that can be either modified according to the requirements of the project user or computed by the project during its runtime.
+   - `path`: The location of the X.509 standard TLS certificate file relative to the "certloca" variable previously set in the project configuration file. This helps the project to locate the X.509 standard TLS certificate file is read and acted upon.
+   - `user`: The username on the source code forge that was previously set on the "gitforge" variable in the project configuration file. If the username is not available on the stated source code forge, the notification ticket making process will error out.
+   - `certstat`: This consists of a list of variables that must not be set manually as they would be overridden by the project during its runtime. Here is a list of those variables with their associated meanings and significance.
+     - `cstarted`: A variable of boolean type. This is computed as TRUE if the current datetime is greater than the "not valid before" datetime of the stated X.509 standard TLS certificate and FALSE if the current datetime is lesser than the "not valid before" datetime of the same.
+     - `cstopped`: A variable of boolean type. This is computed as TRUE if the current datetime is greater than the "not valid after" datetime of the stated X.509 standard TLS certificate and FALSE if the current datetime is less than the "not valid after" datetime of the same.
+     - `daystobt`: A variable of integer type. This is computed as the difference in the number of days from the current datetime to the datetime from when the stated X.509 standard TLS certificate becomes valid. This can either be a positive integer if the "not valid before" datetime has not been reached or a negative integer if the "not valid before" datetime has been passed.
+     - `daystodd`: A variable of integer type. This is computed as the difference in the number of days from the current datetime to the datetime to when the stated X.509 standard TLS certificate becomes expired. This can either be a positive integer if the "not valid after" datetime has not been reached or a negative integer if the "not valid after" datetime has been passed.
+     - `issuauth`: A variable of string type. This stores the found name of the issuing authority for the stated X.509 standard TLS certificate. This can be useful if the same issuing authority is planned to be used to regenerate a new one from.
+     - `serialno`: A variable of string type. This stores the found serial number of the stated X.509 standard TLS certificate. This can be useful to de-validate the existing certificate before opting in to regenerate a new one.
+     - `strtdate`: A variable of datetime type. This is computed as the datetime data consisting of the "not valid before" datetime value.
+     - `stopdate`: A variable of datetime type. This is computed as the datetime data consisting of the "not valid after" datetime value.
+   - `notistat`: This consists of a list of variables that must not be set manually as they would be overridden by the project during its runtime. Here is a list of those variables with their associated meanings and significance.
+     - `done`: A variable of boolean type. This stores the flag to state if the notification about the expiry of the stated X.509 standard TLS certificate has been made. The variable is set to TRUE if the notification has been created and FALSE otherwise.
+     - `link`: A variable of string type. This stores the location of the notification ticket on the selected source code forge that was previously set on the "gitforge" variable in the project configuration file.
+     - `time`: A variable of datetime type. This stores the datetime information of when the previously stated notification ticket was created. This can be useful to track down if there are any repeated notifications made.
+7. Make sure that the location of the custom mapping configuration file is pointed correctly at in the custom project configuration file.
+8. View the console help menu of the project service by running the following command.
+   ```
+   $ (venv) firmitas --help
+   ```
+   Output
+   ```
+   Usage: firmitas [OPTIONS]
+   
+   Options:
+     -c, --conffile PATH  Read configuration from the specified Python file
+     --version            Show the version and exit.
+     --help               Show this message and exit.
+   ```
+9. With the configuration variables set appropriately, run the project service by executing the following command.
+   ```
+   $ (venv) firmitas --conffile firmitas/conf/myconfig.py
+   ```
+   Refrain from making any changes in the existing entries of the mapping configuration file after the first successful run unless it is absolutely necessary to do so as the project service writes and references notification creation status from that file. Any unmonitored change to the existing entries in said file after the first successful run of the project service could lead to unintended consequences such as duplicate notification entries, untracked notification tickets pertaining to services etc.
 
-packages = \
-['firmitas', 'firmitas.base', 'firmitas.conf', 'firmitas.unit']
+## `__license__`
 
-package_data = \
-{'': ['*']}
+This project is licensed under GNU General Public License 3.0 or later.
 
-install_requires = \
-['click>=8.0.0,<9',
- 'cryptography>=36.0.0,<40',
- 'pyyaml>=5.0.0,<7',
- 'requests>=2.20.0,<3']
-
-entry_points = \
-{'console_scripts': ['firmitas = firmitas.main:main']}
-
-setup_kwargs = {
-    'name': 'firmitas',
-    'version': '0.1.1',
-    'description': 'Simple notification service for X.509-standard TLS certificate statuses',
-    'long_description': '# firmitas\n\nSimple notification service for X.509-standard TLS certificate statuses\n\n## `__usage__`\n\n1. Clone the repository to your local storage and make it the present working directory.\n   ```\n   $ git clone https://gitlab.com/t0xic0der/firmitas.git\n   ```\n   ```\n   $ cd firmitas\n   ```\n2. Ensure that [`Poetry`](https://python-poetry.org/) and [Virtualenv](https://pypi.org/project/virtualenv/) are installed and up-to-date on the system.\n   ```\n   $ sudo dnf install --assumeyes poetry virtualenv\n   ```\n3. Create a virtual environment within the cloned local directory and enable it.\n   ```\n   $ virtualenv venv\n   ```\n   ```\n   $ source venv/bin/activate\n   ```\n4. Install the project and its dependencies in the enabled virtual environment.\n   ```\n   $ (venv) poetry install\n   ```\n5. Make a copy of the project configuration file and make your changes to it.\n   ```\n   $ (venv) cp firmitas/conf/standard.py firmitas/conf/myconfig.py\n   ```\n   The project configuration file houses the following variables that can be modified according to the requirements of the project user.  \n   - `gitforge` - The source code forge on which the issue tickets need to be created. The valid options for this configuration variable are `github`, `gitlab` and `pagure`. The support for `pagure` is implemented while that for `github` and `gitlab` is planned.\n   - `repoloca` - The location of the ticketing repository. This is required for source code forges that require the absolute location of the remote ticketing repository for the project to be able to access the API and create notification tickets.\n   - `reponame` - The name of the ticketing repository. This is required for source code forges that require the repository name with namespace of the remote ticketing repository for the project to be able to access the API and create notification tickets.\n   - `username` - The username to masquerade as in order to create notification tickets. This is required for source code forges that require the username with whom an API token is associated for the project to be authenticated on their behalf.\n   - `password` - The password or API token belonging to the aforementioned username. This is required for source code forges that require the password or API token associated with the ticketing repository to authenticate the project on the owner\'s behalf.\n   - `daysqant` - The minimum number of days remaining from the validity expiry date to make notifications for. As a sane default, it is set to open up a notification ticket when the TLS certificate is 30 days away from its validation expiry date.\n   - `tagslist` - The list of labels to the tag the notification tickets with. A minimum of one label is required to ensure that there is a way to filter out the automated notification tickets on a shared issue tracker from the manually created ones.\n   - `maxretry` - The maximum number of retries to make when the process of opening up a notification ticket fails. As a sane default, it is set to allow up to 5 retries, and it is a good practice to have a value greater than one to compensate for spotty connections.\n   - `certloca` - The location where the X.509 standard TLS certificates are stored. Note that this refers to a locally available storage location and not a remotely available storage location. The default is set as "/var/tmp/firmitas/certhere" directory.\n   - `hostloca` - The location where the mapping file of service hostnames, maintainers, certificate statistics and notification statistics are stored. As with the previous configuration variable, even this one refers to a locally available storage location.\n   - `logrconf` - The configuration variable that sets the logging behaviour for the project. As a sane default, the logging level has been set to "DEBUG" to allow for greater verbosity in details and a custom format to the console handler.\n   - `certdict` - The global variable used across the project to share the details of the certificates to be probed into, the statistics of issuing authority, serial number, dates information and much more. Do not change it as this gets overridden.\n6. Make a copy of the mapping configuration file and make your changes to it.\n   ```\n   $ (venv) cp firmitas/conf/certlist.yml firmitas/conf/mytlscts.yml\n   ```\n   The mapping configuration file houses a list of service hostnames having the following variables that can be either modified according to the requirements of the project user or computed by the project during its runtime.\n   - `path`: The location of the X.509 standard TLS certificate file relative to the "certloca" variable previously set in the project configuration file. This helps the project to locate the X.509 standard TLS certificate file is read and acted upon.\n   - `user`: The username on the source code forge that was previously set on the "gitforge" variable in the project configuration file. If the username is not available on the stated source code forge, the notification ticket making process will error out.\n   - `certstat`: This consists of a list of variables that must not be set manually as they would be overridden by the project during its runtime. Here is a list of those variables with their associated meanings and significance.\n     - `cstarted`: A variable of boolean type. This is computed as TRUE if the current datetime is greater than the "not valid before" datetime of the stated X.509 standard TLS certificate and FALSE if the current datetime is lesser than the "not valid before" datetime of the same.\n     - `cstopped`: A variable of boolean type. This is computed as TRUE if the current datetime is greater than the "not valid after" datetime of the stated X.509 standard TLS certificate and FALSE if the current datetime is less than the "not valid after" datetime of the same.\n     - `daystobt`: A variable of integer type. This is computed as the difference in the number of days from the current datetime to the datetime from when the stated X.509 standard TLS certificate becomes valid. This can either be a positive integer if the "not valid before" datetime has not been reached or a negative integer if the "not valid before" datetime has been passed.\n     - `daystodd`: A variable of integer type. This is computed as the difference in the number of days from the current datetime to the datetime to when the stated X.509 standard TLS certificate becomes expired. This can either be a positive integer if the "not valid after" datetime has not been reached or a negative integer if the "not valid after" datetime has been passed.\n     - `issuauth`: A variable of string type. This stores the found name of the issuing authority for the stated X.509 standard TLS certificate. This can be useful if the same issuing authority is planned to be used to regenerate a new one from.\n     - `serialno`: A variable of string type. This stores the found serial number of the stated X.509 standard TLS certificate. This can be useful to de-validate the existing certificate before opting in to regenerate a new one.\n     - `strtdate`: A variable of datetime type. This is computed as the datetime data consisting of the "not valid before" datetime value.\n     - `stopdate`: A variable of datetime type. This is computed as the datetime data consisting of the "not valid after" datetime value.\n   - `notistat`: This consists of a list of variables that must not be set manually as they would be overridden by the project during its runtime. Here is a list of those variables with their associated meanings and significance.\n     - `done`: A variable of boolean type. This stores the flag to state if the notification about the expiry of the stated X.509 standard TLS certificate has been made. The variable is set to TRUE if the notification has been created and FALSE otherwise.\n     - `link`: A variable of string type. This stores the location of the notification ticket on the selected source code forge that was previously set on the "gitforge" variable in the project configuration file.\n     - `time`: A variable of datetime type. This stores the datetime information of when the previously stated notification ticket was created. This can be useful to track down if there are any repeated notifications made.\n7. Make sure that the location of the custom mapping configuration file is pointed correctly at in the custom project configuration file.\n8. View the console help menu of the project service by running the following command.\n   ```\n   $ (venv) firmitas --help\n   ```\n   Output\n   ```\n   Usage: firmitas [OPTIONS]\n   \n   Options:\n     -c, --conffile PATH  Read configuration from the specified Python file\n     --version            Show the version and exit.\n     --help               Show this message and exit.\n   ```\n9. With the configuration variables set appropriately, run the project service by executing the following command.\n   ```\n   $ (venv) firmitas --conffile firmitas/conf/myconfig.py\n   ```\n   Refrain from making any changes in the existing entries of the mapping configuration file after the first successful run unless it is absolutely necessary to do so as the project service writes and references notification creation status from that file. Any unmonitored change to the existing entries in said file after the first successful run of the project service could lead to unintended consequences such as duplicate notification entries, untracked notification tickets pertaining to services etc.\n\n## `__license__`\n\nThis project is licensed under GNU General Public License 3.0 or later.\n',
-    'author': 'Akashdeep Dhar',
-    'author_email': 'akashdeep.dhar@gmail.com',
-    'maintainer': 'Akashdeep Dhar',
-    'maintainer_email': 'akashdeep.dhar@gmail.com',
-    'url': 'https://gitlab.com/t0xic0der/firmitas/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4',
-}
-
-
-setup(**setup_kwargs)
```

