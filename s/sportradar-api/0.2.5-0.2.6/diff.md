# Comparing `tmp/sportradar-api-0.2.5.tar.gz` & `tmp/sportradar_api-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sportradar-api-0.2.5.tar", last modified: Thu Mar 16 18:03:35 2023, max compression
+gzip compressed data, was "sportradar_api-0.2.6.tar", max compression
```

## Comparing `sportradar-api-0.2.5.tar` & `sportradar_api-0.2.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2023-03-16 18:03:16.991533 sportradar-api-0.2.5/LICENSE
--rw-r--r--   0        0        0      414 2023-03-16 18:03:16.991533 sportradar-api-0.2.5/README.md
--rw-r--r--   0        0        0     1253 2023-03-16 18:03:16.995533 sportradar-api-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      187 2023-03-16 18:03:16.995533 sportradar-api-0.2.5/sportradar_api/__init__.py
--rw-r--r--   0        0        0     3968 2023-03-16 18:03:16.995533 sportradar-api-0.2.5/sportradar_api/main.py
--rw-r--r--   0        0        0        0 2023-03-16 18:03:16.995533 sportradar-api-0.2.5/sportradar_api/soccer_extended/__init__.py
--rw-r--r--   0        0        0     2325 2023-03-16 18:03:16.995533 sportradar-api-0.2.5/sportradar_api/soccer_extended/soccer_extended.py
--rw-r--r--   0        0        0     7904 2023-03-16 18:03:16.995533 sportradar-api-0.2.5/sportradar_api/soccer_extended/soccer_extended_pandas.py
--rw-r--r--   0        0        0        0 2023-03-16 18:03:16.995533 sportradar-api-0.2.5/sportradar_api/utils/__init__.py
--rw-r--r--   0        0        0     1055 2023-03-16 18:03:16.995533 sportradar-api-0.2.5/sportradar_api/utils/utils.py
--rw-r--r--   0        0        0     1206 2023-03-16 18:03:35.911610 sportradar-api-0.2.5/setup.py
--rw-r--r--   0        0        0     1137 2023-03-16 18:03:35.911903 sportradar-api-0.2.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1095 2023-02-25 14:54:00.129997 sportradar_api-0.2.6/LICENSE
+-rwxr-xr-x   0        0        0      432 2023-03-12 14:12:52.685758 sportradar_api-0.2.6/README.md
+-rwxr-xr-x   0        0        0     1303 2023-06-08 17:10:13.029428 sportradar_api-0.2.6/pyproject.toml
+-rwxr-xr-x   0        0        0      191 2023-02-25 14:54:38.670548 sportradar_api-0.2.6/sportradar_api/__init__.py
+-rwxr-xr-x   0        0        0     4076 2023-03-01 03:25:20.802436 sportradar_api-0.2.6/sportradar_api/main.py
+-rwxr-xr-x   0        0        0        0 2023-02-25 14:54:38.591783 sportradar_api-0.2.6/sportradar_api/soccer_extended/__init__.py
+-rwxr-xr-x   0        0        0     2767 2023-06-08 17:07:59.707843 sportradar_api-0.2.6/sportradar_api/soccer_extended/soccer_extended.py
+-rwxr-xr-x   0        0        0     9374 2023-06-08 17:06:51.241701 sportradar_api-0.2.6/sportradar_api/soccer_extended/soccer_extended_pandas.py
+-rwxr-xr-x   0        0        0        0 2023-02-28 18:34:53.524396 sportradar_api-0.2.6/sportradar_api/utils/__init__.py
+-rwxr-xr-x   0        0        0     1094 2023-03-12 14:12:01.545012 sportradar_api-0.2.6/sportradar_api/utils/utils.py
+-rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 sportradar_api-0.2.6/setup.py
+-rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 sportradar_api-0.2.6/PKG-INFO
```

### Comparing `sportradar-api-0.2.5/pyproject.toml` & `sportradar_api-0.2.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-[tool.poetry]
-name = "sportradar-api"
-version = "0.2.5"
-description = "Lightweight wrapper for Sportradar API"
-authors = ["Felipe Allegretti <felipe@allegretti.me>"]
-readme = "README.md"
-license = "MIT"
-homepage = "https://felipeall.github.io/sportradar-api"
-repository = "https://github.com/felipeall/sportradar-api"
-classifiers = [
-    "Topic :: Software Development :: Libraries",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-]
-packages = [{include = "sportradar_api"}]
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.poetry.dependencies]
-python = "^3.9"
-requests = "2.28.2"
-pandas = "1.5.3"
-flatten-json = "0.1.13"
-
-[tool.poetry.group.dev.dependencies]
-black = "23.1.0"
-isort = "5.12.0"
-pyproject-flake8 = "6.0.0.post1"
-jupyter = "1.0.0"
-
-[tool.poetry.group.docs.dependencies]
-mkdocs = "1.4.2"
-mkdocstrings = {extras = ["python"], version = "0.20.0"}
-mkdocs-material = "9.0.14"
-mkdocs-minify-plugin = "0.6.2"
-mkdocs-git-revision-date-localized-plugin = "1.1.0"
-mkdocs-git-authors-plugin = "0.7.0"
-
-[tool.black]
-line-length = 120
-verbose = true
-preview = true
-
-[tool.isort]
-profile = "black"
-
-[tool.flake8]
+[tool.poetry]
+name = "sportradar-api"
+version = "0.2.6"
+description = "Lightweight wrapper for Sportradar API"
+authors = ["Felipe Allegretti <felipe@allegretti.me>"]
+readme = "README.md"
+license = "MIT"
+homepage = "https://felipeall.github.io/sportradar-api"
+repository = "https://github.com/felipeall/sportradar-api"
+classifiers = [
+    "Topic :: Software Development :: Libraries",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+]
+packages = [{include = "sportradar_api"}]
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.dependencies]
+python = "^3.9"
+requests = "2.28.2"
+pandas = "1.5.3"
+flatten-json = "0.1.13"
+
+[tool.poetry.group.dev.dependencies]
+black = "23.1.0"
+isort = "5.12.0"
+pyproject-flake8 = "6.0.0.post1"
+jupyter = "1.0.0"
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "1.4.2"
+mkdocstrings = {extras = ["python"], version = "0.20.0"}
+mkdocs-material = "9.0.14"
+mkdocs-minify-plugin = "0.6.2"
+mkdocs-git-revision-date-localized-plugin = "1.1.0"
+mkdocs-git-authors-plugin = "0.7.0"
+
+[tool.black]
+line-length = 120
+verbose = true
+preview = true
+
+[tool.isort]
+profile = "black"
+
+[tool.flake8]
 max-line-length = 120
```

### Comparing `sportradar-api-0.2.5/sportradar_api/main.py` & `sportradar_api-0.2.6/sportradar_api/main.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-import logging
-import os
-from dataclasses import dataclass
-from time import sleep
-from typing import Optional
-
-import requests
-from requests import HTTPError, Response
-
-
-@dataclass
-class SportradarAPI:
-    api: str
-    api_key: Optional[str] = None
-    api_access_level: str = "trial"
-    api_version: str = "v4"
-    api_language_code: str = "en"
-    api_format: str = "json"
-    timeout: int = 120
-    sleep_time: int = 1.2
-    verbose: bool = True
-
-    def __post_init__(self):
-        self._set_logger()
-        self._set_api_key()
-
-    def _set_logger(self):
-        if self.verbose:
-            logging.basicConfig(
-                level=logging.INFO,
-                format="[%(asctime)s] [SportradarAPI] %(message)s",
-                datefmt="%Y-%m-%d %H:%M:%S",
-            )
-        self.log = logging.getLogger()
-
-    def _set_api_key(self):
-        if not self.api_key:
-            self.api_key = os.getenv("SPORTRADAR_API_KEY")
-            assert self.api_key, "Please provide `api_key` parameter or set SPORTRADAR_API_KEY environment variable"
-            self.log.info(f'Loaded SPORTRADAR_API_KEY: {self.api_key[:4].ljust(len(self.api_key), "*")}')
-        else:
-            self.log.info(f'Loaded `api_key` parameter: {self.api_key[:4].ljust(len(self.api_key),"*")}')
-
-    def _call_endpoint(self, endpoint: str, key: Optional[str] = None) -> dict:
-        response = self._make_request(endpoint=endpoint)
-        content = response.json()
-
-        request_results = response.headers.get("X-Result")
-        request_max_results = response.headers.get("X-Max-Results")
-        self.log.info(f"[{endpoint}] Headers: {response.headers}")
-
-        if request_results is None or request_max_results is None:
-            self.log.info(f"[{endpoint}] Fetching complete!")
-            return content
-
-        request_results = int(request_results)
-        request_max_results = int(request_max_results)
-
-        if request_max_results - request_results <= 0:
-            self.log.info(f"[{endpoint}] Total records: {len(content.get(key))}")
-            self.log.info(f"[{endpoint}] Fetching complete!")
-            return content
-
-        for offset in range(request_results, request_max_results, request_results):
-            response = self._make_request(endpoint=endpoint, offset=offset, limit=request_results)
-            content[key].extend(response.json().get(key))
-
-        self.log.info(f"[{endpoint}] Parsed records: {len(content.get(key))}")
-        self.log.info(f"[{endpoint}] Fetching complete!")
-        return content
-
-    def _make_request(self, endpoint: str, offset: Optional[int] = None, limit: Optional[int] = None) -> Response:
-        sleep(self.sleep_time)
-
-        url = (
-            "https://api.sportradar.us"
-            f"/{self.api}"
-            f"/{self.api_access_level}"
-            f"/{self.api_version}"
-            f"/{self.api_language_code}"
-            f"/{endpoint}"
-            f".{self.api_format}"
-        )
-
-        self.log.info(f"[{endpoint}] Calling endpoint...")
-        self.log.info(f"[{endpoint}] Parameters: {offset=} {limit=}")
-
-        response = requests.get(
-            url,
-            timeout=self.timeout,
-            params={"api_key": self.api_key, "offset": offset, "limit": limit},
-        )
-
-        self.log.info(f"[{endpoint}] Response Status Code: {response.status_code}")
-        self.log.info(
-            f"[{endpoint}] Updated API Key Quota: "
-            f"{response.headers.get('X-Plan-Quota-Current')}"
-            f"/{response.headers.get('X-Plan-Quota-Allotted')}"
-        )
-
-        if response.status_code == 200:
-            return response
-
-        elif 400 <= response.status_code < 500:
-            raise HTTPError(f"{response.status_code} Client Error: {response.reason} for url: {url}", response=response)
-
-        elif 500 <= response.status_code < 600:
-            raise HTTPError(f"{response.status_code} Server Error: {response.reason} for url: {url}", response=response)
+import logging
+import os
+from dataclasses import dataclass
+from time import sleep
+from typing import Optional
+
+import requests
+from requests import HTTPError, Response
+
+
+@dataclass
+class SportradarAPI:
+    api: str
+    api_key: Optional[str] = None
+    api_access_level: str = "trial"
+    api_version: str = "v4"
+    api_language_code: str = "en"
+    api_format: str = "json"
+    timeout: int = 120
+    sleep_time: int = 1.2
+    verbose: bool = True
+
+    def __post_init__(self):
+        self._set_logger()
+        self._set_api_key()
+
+    def _set_logger(self):
+        if self.verbose:
+            logging.basicConfig(
+                level=logging.INFO,
+                format="[%(asctime)s] [SportradarAPI] %(message)s",
+                datefmt="%Y-%m-%d %H:%M:%S",
+            )
+        self.log = logging.getLogger()
+
+    def _set_api_key(self):
+        if not self.api_key:
+            self.api_key = os.getenv("SPORTRADAR_API_KEY")
+            assert self.api_key, "Please provide `api_key` parameter or set SPORTRADAR_API_KEY environment variable"
+            self.log.info(f'Loaded SPORTRADAR_API_KEY: {self.api_key[:4].ljust(len(self.api_key), "*")}')
+        else:
+            self.log.info(f'Loaded `api_key` parameter: {self.api_key[:4].ljust(len(self.api_key),"*")}')
+
+    def _call_endpoint(self, endpoint: str, key: Optional[str] = None) -> dict:
+        response = self._make_request(endpoint=endpoint)
+        content = response.json()
+
+        request_results = response.headers.get("X-Result")
+        request_max_results = response.headers.get("X-Max-Results")
+        self.log.info(f"[{endpoint}] Headers: {response.headers}")
+
+        if request_results is None or request_max_results is None:
+            self.log.info(f"[{endpoint}] Fetching complete!")
+            return content
+
+        request_results = int(request_results)
+        request_max_results = int(request_max_results)
+
+        if request_max_results - request_results <= 0:
+            self.log.info(f"[{endpoint}] Total records: {len(content.get(key))}")
+            self.log.info(f"[{endpoint}] Fetching complete!")
+            return content
+
+        for offset in range(request_results, request_max_results, request_results):
+            response = self._make_request(endpoint=endpoint, offset=offset, limit=request_results)
+            content[key].extend(response.json().get(key))
+
+        self.log.info(f"[{endpoint}] Parsed records: {len(content.get(key))}")
+        self.log.info(f"[{endpoint}] Fetching complete!")
+        return content
+
+    def _make_request(self, endpoint: str, offset: Optional[int] = None, limit: Optional[int] = None) -> Response:
+        sleep(self.sleep_time)
+
+        url = (
+            "https://api.sportradar.us"
+            f"/{self.api}"
+            f"/{self.api_access_level}"
+            f"/{self.api_version}"
+            f"/{self.api_language_code}"
+            f"/{endpoint}"
+            f".{self.api_format}"
+        )
+
+        self.log.info(f"[{endpoint}] Calling endpoint...")
+        self.log.info(f"[{endpoint}] Parameters: {offset=} {limit=}")
+
+        response = requests.get(
+            url,
+            timeout=self.timeout,
+            params={"api_key": self.api_key, "offset": offset, "limit": limit},
+        )
+
+        self.log.info(f"[{endpoint}] Response Status Code: {response.status_code}")
+        self.log.info(
+            f"[{endpoint}] Updated API Key Quota: "
+            f"{response.headers.get('X-Plan-Quota-Current')}"
+            f"/{response.headers.get('X-Plan-Quota-Allotted')}"
+        )
+
+        if response.status_code == 200:
+            return response
+
+        elif 400 <= response.status_code < 500:
+            raise HTTPError(f"{response.status_code} Client Error: {response.reason} for url: {url}", response=response)
+
+        elif 500 <= response.status_code < 600:
+            raise HTTPError(f"{response.status_code} Server Error: {response.reason} for url: {url}", response=response)
```

### Comparing `sportradar-api-0.2.5/sportradar_api/utils/utils.py` & `sportradar_api-0.2.6/sportradar_api/utils/utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from typing import Optional
-
-import pandas as pd
-
-
-def remove_str(text: str, strings_to_remove: list) -> str:
-    for string in strings_to_remove:
-        text = text.replace(string, "")
-
-    return text
-
-
-def explode_column(
-    df_to_explode: pd.DataFrame, col_to_explode: str, cols_to_keep: Optional[list] = None
-) -> pd.DataFrame:
-    df = df_to_explode.copy()
-    if cols_to_keep:
-        df = df.loc[:, cols_to_keep + [col_to_explode]]
-
-    df = df.explode(col_to_explode)
-
-    normalized = pd.json_normalize(df[col_to_explode]).add_prefix(f"{col_to_explode}.")
-    normalized.index = df.index
-
-    df = pd.concat([df, normalized], axis=1)
-    df = df.drop(columns=col_to_explode)
-
-    return df
-
-
-def remove_cols_str(df: pd.DataFrame, str_list: list) -> pd.DataFrame:
-    df.columns = [remove_str(col, str_list) for col in df.columns]
-    return df
-
-
-def replace_cols_str(df: pd.DataFrame, replace_map: dict) -> pd.DataFrame:
-    for old, new in replace_map.items():
-        df.columns = [col.replace(old, new) for col in df.columns]
-    return df
+from typing import Optional
+
+import pandas as pd
+
+
+def remove_str(text: str, strings_to_remove: list) -> str:
+    for string in strings_to_remove:
+        text = text.replace(string, "")
+
+    return text
+
+
+def explode_column(
+    df_to_explode: pd.DataFrame, col_to_explode: str, cols_to_keep: Optional[list] = None
+) -> pd.DataFrame:
+    df = df_to_explode.copy()
+    if cols_to_keep:
+        df = df.loc[:, cols_to_keep + [col_to_explode]]
+
+    df = df.explode(col_to_explode)
+
+    normalized = pd.json_normalize(df[col_to_explode]).add_prefix(f"{col_to_explode}.")
+    normalized.index = df.index
+
+    df = pd.concat([df, normalized], axis=1)
+    df = df.drop(columns=col_to_explode)
+
+    return df
+
+
+def remove_cols_str(df: pd.DataFrame, str_list: list) -> pd.DataFrame:
+    df.columns = [remove_str(col, str_list) for col in df.columns]
+    return df
+
+
+def replace_cols_str(df: pd.DataFrame, replace_map: dict) -> pd.DataFrame:
+    for old, new in replace_map.items():
+        df.columns = [col.replace(old, new) for col in df.columns]
+    return df
```

### Comparing `sportradar-api-0.2.5/setup.py` & `sportradar_api-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 {'': ['*']}
 
 install_requires = \
 ['flatten-json==0.1.13', 'pandas==1.5.3', 'requests==2.28.2']
 
 setup_kwargs = {
     'name': 'sportradar-api',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'Lightweight wrapper for Sportradar API',
     'long_description': "# Sportradar API\nLightweight wrapper for [Sportradar API](https://developer.sportradar.com/docs/read/Home)\n\n## Set up\n1. Register on [Sportradar Developer](https://developer.sportradar.com/member/register)\n2. Generate an API Key\n\n## Installation\n````bash\npip install sportradar-api\n````\n\n## Usage\n\n````python\nfrom sportradar_api import SoccerExtended\n\nsportradar = SoccerExtended(api_key='SPORTRADAR_API_KEY')\n````",
     'author': 'Felipe Allegretti',
     'author_email': 'felipe@allegretti.me',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://felipeall.github.io/sportradar-api',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
```

### Comparing `sportradar-api-0.2.5/PKG-INFO` & `sportradar_api-0.2.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: sportradar-api
-Version: 0.2.5
+Version: 0.2.6
 Summary: Lightweight wrapper for Sportradar API
 Home-page: https://felipeall.github.io/sportradar-api
 License: MIT
 Author: Felipe Allegretti
 Author-email: felipe@allegretti.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: flatten-json (==0.1.13)
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: requests (==2.28.2)
 Project-URL: Repository, https://github.com/felipeall/sportradar-api
 Description-Content-Type: text/markdown
```

