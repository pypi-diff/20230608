# Comparing `tmp/vestapol-0.0.18.tar.gz` & `tmp/vestapol-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vestapol-0.0.18.tar", max compression
+gzip compressed data, was "vestapol-0.0.20.tar", max compression
```

## Comparing `vestapol-0.0.18.tar` & `vestapol-0.0.20.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0    11355 2022-10-24 16:51:51.126129 vestapol-0.0.18/LICENSE
--rw-r--r--   0        0        0     2910 2022-10-24 16:51:51.126129 vestapol-0.0.18/README.md
--rw-r--r--   0        0        0      909 2022-10-24 16:51:51.126129 vestapol-0.0.18/pyproject.toml
--rw-r--r--   0        0        0      209 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/__init__.py
--rw-r--r--   0        0        0        0 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/api/__init__.py
--rw-r--r--   0        0        0      798 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/api/api.py
--rw-r--r--   0        0        0        0 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/destinations/__init__.py
--rw-r--r--   0        0        0      579 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/destinations/base_destination.py
--rw-r--r--   0        0        0     3000 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/destinations/gcp_destination.py
--rw-r--r--   0        0        0      957 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/destinations/local_destination.py
--rw-r--r--   0        0        0     2231 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/external_tables.py
--rw-r--r--   0        0        0        0 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/py.typed
--rw-r--r--   0        0        0        0 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/web_resources/__init__.py
--rw-r--r--   0        0        0     2987 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/web_resources/base_resource.py
--rw-r--r--   0        0        0     1891 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/web_resources/csv_resource.py
--rw-r--r--   0        0        0      588 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/web_resources/github_resource.py
--rw-r--r--   0        0        0     2700 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/web_resources/json_resource.py
--rw-r--r--   0        0        0        0 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/writers/__init__.py
--rw-r--r--   0        0        0      542 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/writers/json_writer.py
--rw-r--r--   0        0        0      184 2022-10-24 16:51:51.130129 vestapol-0.0.18/vestapol/writers/text_writer.py
--rw-r--r--   0        0        0     3972 1970-01-01 00:00:00.000000 vestapol-0.0.18/setup.py
--rw-r--r--   0        0        0     3785 1970-01-01 00:00:00.000000 vestapol-0.0.18/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-06-08 19:56:21.858248 vestapol-0.0.20/LICENSE
+-rw-r--r--   0        0        0     3015 2023-06-08 19:56:21.858248 vestapol-0.0.20/README.md
+-rw-r--r--   0        0        0     1011 2023-06-08 19:56:21.862248 vestapol-0.0.20/pyproject.toml
+-rw-r--r--   0        0        0      209 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/api/__init__.py
+-rw-r--r--   0        0        0      798 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/api/api.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/destinations/__init__.py
+-rw-r--r--   0        0        0      579 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/destinations/base_destination.py
+-rw-r--r--   0        0        0     3013 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/destinations/gcp_destination.py
+-rw-r--r--   0        0        0      957 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/destinations/local_destination.py
+-rw-r--r--   0        0        0     2331 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/external_tables.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/py.typed
+-rw-r--r--   0        0        0        0 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/web_resources/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/web_resources/base_resource.py
+-rw-r--r--   0        0        0     1891 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/web_resources/csv_resource.py
+-rw-r--r--   0        0        0      588 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/web_resources/github_resource.py
+-rw-r--r--   0        0        0     2700 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/web_resources/json_resource.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/writers/__init__.py
+-rw-r--r--   0        0        0      542 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/writers/json_writer.py
+-rw-r--r--   0        0        0      184 2023-06-08 19:56:21.862248 vestapol-0.0.20/vestapol/writers/text_writer.py
+-rw-r--r--   0        0        0     3880 1970-01-01 00:00:00.000000 vestapol-0.0.20/PKG-INFO
```

### Comparing `vestapol-0.0.18/LICENSE` & `vestapol-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.18/README.md` & `vestapol-0.0.20/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -38,16 +38,21 @@
 for row in query_job.result():
     print(row)
 ```
 
 
 ## Prerequisites
 
-Installation of this project requires [Poetry](https://python-poetry.org/docs/) and Python version 3.8+.
+Installation of this project requires [Poetry](https://python-poetry.org/docs/) 1.2+ and Python version 3.9+.
 
+Older version of poetry can be updated by running:
+```shell
+poetry self update
+poetry --version
+```
 
 ## Installation
 
 Install vestapol and its dependencies by running:
 
 ```shell
 poetry install
```

### Comparing `vestapol-0.0.18/pyproject.toml` & `vestapol-0.0.20/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 [tool.poetry]
 name = "vestapol"
-version = "0.0.18"
+version = "0.0.20"
 description = "Python package that loads data from the web and deploys a corresponding external table definition, so that the data can be queried using standard SQL."
 authors = ["Brian Waligorski <bwaligorski@inquirer.com>"]
 license = "Apache License 2.0"
 readme = "README.md"  # Markdown files are supported
 repository = "https://github.com/phillymedia/vestapol"
 homepage = "https://github.com/phillymedia/vestapol"
 
 [tool.poetry.dependencies]
 python = ">=3.8.12,<3.11"
 requests = "^2.26"
-google-cloud-storage = "^1.43"
-google-cloud-bigquery = "^2.31"
+google-cloud-storage = ">=1.43"
+google-cloud-bigquery = ">=2.31"
 pendulum = "^2.1"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 python-dotenv = "^0.19.2"
 pytest = "^6.2.5"
 tox = "^3.25.0"
 mypy = "^0.982"
 types-requests = "^2.28.11"
 flake8 = "^5.0.4"
 black = "^22.8.0"
 pre-commit = "^2.20.0"
 
+[tool.poetry.group.tox]
+optional = true
+
+[tool.poetry.group.tox.dependencies]
+tox = "3.27.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `vestapol-0.0.18/vestapol/api/api.py` & `vestapol-0.0.20/vestapol/api/api.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.18/vestapol/destinations/base_destination.py` & `vestapol-0.0.20/vestapol/destinations/base_destination.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.18/vestapol/destinations/gcp_destination.py` & `vestapol-0.0.20/vestapol/destinations/gcp_destination.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import logging
 import os
 import pathlib
 from typing import TYPE_CHECKING
 
-from google.cloud import bigquery
-from google.cloud import storage
+import google.cloud.bigquery as bigquery
+import google.cloud.storage as storage
 
 from vestapol import external_tables
 from vestapol.destinations import base_destination
 
 
 if TYPE_CHECKING:
     from vestapol.web_resources.base_resource import BaseResource
```

### Comparing `vestapol-0.0.18/vestapol/destinations/local_destination.py` & `vestapol-0.0.20/vestapol/destinations/local_destination.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.18/vestapol/external_tables.py` & `vestapol-0.0.20/vestapol/external_tables.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     hive_partitioning_opts.source_uri_prefix = source_uri_prefix_fq
 
     external_config.hive_partitioning = hive_partitioning_opts
 
     external_config.source_uris = source_uris
 
     if bq_source_format == "CSV":
-        external_config.csv_options.skip_leading_rows = skip_leading_rows
+        # skips mypy since Google does not give CSVOptions a signature
+        external_config.csv_options.skip_leading_rows = skip_leading_rows  # type: ignore # noqa: E501
 
     return external_config
 
 
 def create_gcp_table(
     source_format: str,
     project_id: str,
```

### Comparing `vestapol-0.0.18/vestapol/web_resources/base_resource.py` & `vestapol-0.0.20/vestapol/web_resources/base_resource.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.18/vestapol/web_resources/csv_resource.py` & `vestapol-0.0.20/vestapol/web_resources/csv_resource.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.18/vestapol/web_resources/github_resource.py` & `vestapol-0.0.20/vestapol/web_resources/github_resource.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.18/vestapol/web_resources/json_resource.py` & `vestapol-0.0.20/vestapol/web_resources/json_resource.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.18/vestapol/writers/json_writer.py` & `vestapol-0.0.20/vestapol/writers/json_writer.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.18/setup.py` & `vestapol-0.0.20/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,112 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: vestapol
+Version: 0.0.20
+Summary: Python package that loads data from the web and deploys a corresponding external table definition, so that the data can be queried using standard SQL.
+Home-page: https://github.com/phillymedia/vestapol
+License: Apache-2.0
+Author: Brian Waligorski
+Author-email: bwaligorski@inquirer.com
+Requires-Python: >=3.8.12,<3.11
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: google-cloud-bigquery (>=2.31)
+Requires-Dist: google-cloud-storage (>=1.43)
+Requires-Dist: pendulum (>=2.1,<3.0)
+Requires-Dist: requests (>=2.26,<3.0)
+Project-URL: Repository, https://github.com/phillymedia/vestapol
+Description-Content-Type: text/markdown
 
-packages = \
-['vestapol',
- 'vestapol.api',
- 'vestapol.destinations',
- 'vestapol.web_resources',
- 'vestapol.writers']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['google-cloud-bigquery>=2.31,<3.0',
- 'google-cloud-storage>=1.43,<2.0',
- 'pendulum>=2.1,<3.0',
- 'requests>=2.26,<3.0']
-
-setup_kwargs = {
-    'name': 'vestapol',
-    'version': '0.0.18',
-    'description': 'Python package that loads data from the web and deploys a corresponding external table definition, so that the data can be queried using standard SQL.',
-    'long_description': '# vestapol\n\nvestapol is a Python package that loads data from the web and deploys a corresponding external table definition, so that the data can be queried using standard SQL.\n\n["Vestapol"](https://www.youtube.com/watch?v=SKQG-JGyn7U) is an open D Major tuning for the guitar. It is named after a 19th-century composition distributed in some of the earliest instructional guides for guitar.\n\n## Usage\n\n```python\nfrom vestapol.web_resources.csv_resource import CSVResource\nfrom vestapol.destinations.gcp_destination import GoogleCloudPlatform\n\n\nnyt_covid_data_2022 = CSVResource(\n    name="nyt_covid19_us_counties_2022",\n    base_url="https://raw.githubusercontent.com/",\n    endpoint="nytimes/covid-19-data/master/rolling-averages/us-counties-2022.csv",\n    version="v0",\n    skip_leading_rows=1,\n)\n\ndestination = GoogleCloudPlatform()\n\nnyt_covid_data_2022.load(destination)\ntablename = destination.create_table(nyt_covid_data_2022)\n\n\nfrom google.cloud import bigquery\n\nclient = bigquery.Client()\nquery = f"""\n    select date, state, county, cases_avg_per_100k\n    from `{tablename}`\n    where requested_at = \'{nyt_covid_data_2022.requested_at}\'\n    limit 5\n"""\nquery_job = client.query(query)\nfor row in query_job.result():\n    print(row)\n```\n\n\n## Prerequisites\n\nInstallation of this project requires [Poetry](https://python-poetry.org/docs/) and Python version 3.8+.\n\n\n## Installation\n\nInstall vestapol and its dependencies by running:\n\n```shell\npoetry install\n```\n\n## Testing\n\nRun tests with the following command:\n\n```shell\npoetry run pytest\n```\n\n## Environment Variables\n\n- `GCS_BUCKET_NAME`: the Google Cloud Storage bucket where data is loaded (e.g. `inq-warehouse-waligob`)\n- `GCS_ROOT_PREFIX`: the GCS prefix where data is loaded (e.g. `data_catalog`)\n- `GBQ_PROJECT_ID`: the BigQuery project identifier (e.g. `inq-warehouse`)\n- `GBQ_DATASET_ID`: the BigQuery dataset where external tables will be created (e.g. `data_catalog_waligob`)\n- `GBQ_DATASET_LOCATION`: the BigQuery dataset location (e.g. `US`)\n- `GOOGLE_APPLICATION_CREDENTIALS=`: location of the GCS service account keyfile (e.g. `~/inq-warehouse-f0962a57089e-inf.json`)\n\n\n## Publishing to PyPI\n\nInstructions for pushing new versions of `vestapol` to PyPI:\n\n1. Update `CHANGELOG.md`. Include Additions, Fixes, and Changes.\n\n2. Update project version using either a valid [PEP 440 string](https://peps.python.org/pep-0440/) or a [valid bump rule](https://python-poetry.org/docs/master/cli/#version) following [Semantic Versioning](http://semver.org/).\n\n```shell\n    poetry version <version string or bump rule>\n```\n\n3. Create a [release](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository#creating-a-release) and check the CD Pipeline [action](https://github.com/phillymedia/vestapol/actions/workflows/release.yml) to ensure that the project was built and published to PyPI successfully.\n',
-    'author': 'Brian Waligorski',
-    'author_email': 'bwaligorski@inquirer.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/phillymedia/vestapol',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8.12,<3.11',
-}
+# vestapol
 
+vestapol is a Python package that loads data from the web and deploys a corresponding external table definition, so that the data can be queried using standard SQL.
+
+["Vestapol"](https://www.youtube.com/watch?v=SKQG-JGyn7U) is an open D Major tuning for the guitar. It is named after a 19th-century composition distributed in some of the earliest instructional guides for guitar.
+
+## Usage
+
+```python
+from vestapol.web_resources.csv_resource import CSVResource
+from vestapol.destinations.gcp_destination import GoogleCloudPlatform
+
+
+nyt_covid_data_2022 = CSVResource(
+    name="nyt_covid19_us_counties_2022",
+    base_url="https://raw.githubusercontent.com/",
+    endpoint="nytimes/covid-19-data/master/rolling-averages/us-counties-2022.csv",
+    version="v0",
+    skip_leading_rows=1,
+)
+
+destination = GoogleCloudPlatform()
+
+nyt_covid_data_2022.load(destination)
+tablename = destination.create_table(nyt_covid_data_2022)
+
+
+from google.cloud import bigquery
+
+client = bigquery.Client()
+query = f"""
+    select date, state, county, cases_avg_per_100k
+    from `{tablename}`
+    where requested_at = '{nyt_covid_data_2022.requested_at}'
+    limit 5
+"""
+query_job = client.query(query)
+for row in query_job.result():
+    print(row)
+```
+
+
+## Prerequisites
+
+Installation of this project requires [Poetry](https://python-poetry.org/docs/) 1.2+ and Python version 3.9+.
+
+Older version of poetry can be updated by running:
+```shell
+poetry self update
+poetry --version
+```
+
+## Installation
+
+Install vestapol and its dependencies by running:
+
+```shell
+poetry install
+```
+
+## Testing
+
+Run tests with the following command:
+
+```shell
+poetry run pytest
+```
+
+## Environment Variables
+
+- `GCS_BUCKET_NAME`: the Google Cloud Storage bucket where data is loaded (e.g. `inq-warehouse-waligob`)
+- `GCS_ROOT_PREFIX`: the GCS prefix where data is loaded (e.g. `data_catalog`)
+- `GBQ_PROJECT_ID`: the BigQuery project identifier (e.g. `inq-warehouse`)
+- `GBQ_DATASET_ID`: the BigQuery dataset where external tables will be created (e.g. `data_catalog_waligob`)
+- `GBQ_DATASET_LOCATION`: the BigQuery dataset location (e.g. `US`)
+- `GOOGLE_APPLICATION_CREDENTIALS=`: location of the GCS service account keyfile (e.g. `~/inq-warehouse-f0962a57089e-inf.json`)
+
+
+## Publishing to PyPI
+
+Instructions for pushing new versions of `vestapol` to PyPI:
+
+1. Update `CHANGELOG.md`. Include Additions, Fixes, and Changes.
+
+2. Update project version using either a valid [PEP 440 string](https://peps.python.org/pep-0440/) or a [valid bump rule](https://python-poetry.org/docs/master/cli/#version) following [Semantic Versioning](http://semver.org/).
+
+```shell
+    poetry version <version string or bump rule>
+```
+
+3. Create a [release](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository#creating-a-release) and check the CD Pipeline [action](https://github.com/phillymedia/vestapol/actions/workflows/release.yml) to ensure that the project was built and published to PyPI successfully.
 
-setup(**setup_kwargs)
```

