# Comparing `tmp/keegcpass-0.2.0.tar.gz` & `tmp/keegcpass-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keegcpass-0.2.0.tar", max compression
+gzip compressed data, was "keegcpass-0.3.0.tar", max compression
```

## Comparing `keegcpass-0.2.0.tar` & `keegcpass-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1180 2023-06-08 08:09:32.686333 keegcpass-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     9881 2023-06-08 08:09:32.686333 keegcpass-0.2.0/LICENSES_3RD_PARTY.md
--rw-r--r--   0        0        0        0 2023-06-07 11:37:50.075552 keegcpass-0.2.0/README.md
--rw-r--r--   0        0        0      636 2023-06-08 08:09:32.690333 keegcpass-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 11:33:25.399637 keegcpass-0.2.0/src/__init__.py
--rw-r--r--   0        0        0     2503 2023-06-08 08:09:32.690333 keegcpass-0.2.0/src/secrets_readers.py
--rw-r--r--   0        0        0     2382 2023-06-08 08:09:32.690333 keegcpass-0.2.0/src/secrets_writers.py
--rw-r--r--   0        0        0      700 2023-06-08 08:09:32.690333 keegcpass-0.2.0/src/validation_models.py
--rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 keegcpass-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1180 2023-06-08 08:09:32.686333 keegcpass-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     9881 2023-06-08 08:09:32.686333 keegcpass-0.3.0/LICENSES_3RD_PARTY.md
+-rw-r--r--   0        0        0        0 2023-06-07 11:37:50.075552 keegcpass-0.3.0/README.md
+-rw-r--r--   0        0        0      636 2023-06-08 09:10:20.566425 keegcpass-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-07 11:33:25.399637 keegcpass-0.3.0/src/__init__.py
+-rw-r--r--   0        0        0     2503 2023-06-08 09:07:53.450532 keegcpass-0.3.0/src/secrets_readers.py
+-rw-r--r--   0        0        0     2383 2023-06-08 09:07:53.470532 keegcpass-0.3.0/src/secrets_writers.py
+-rw-r--r--   0        0        0      700 2023-06-08 08:09:32.690333 keegcpass-0.3.0/src/validation_models.py
+-rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 keegcpass-0.3.0/PKG-INFO
```

### Comparing `keegcpass-0.2.0/LICENSE.md` & `keegcpass-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `keegcpass-0.2.0/LICENSES_3RD_PARTY.md` & `keegcpass-0.3.0/LICENSES_3RD_PARTY.md`

 * *Files identical despite different names*

### Comparing `keegcpass-0.2.0/pyproject.toml` & `keegcpass-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keegcpass"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
     "Andy Koch <andyvk85@gmail.com>",
 ]
 description = ""
 classifiers = ["Programming Language :: Python :: 3"]
 readme = "README.md"
 packages = [{ include = "src" }]
```

### Comparing `keegcpass-0.2.0/src/secrets_readers.py` & `keegcpass-0.3.0/src/secrets_readers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from abc import ABC, abstractmethod
 
 from google.cloud import secretmanager_v1 as sm
 from pykeepass import PyKeePass
 
-from validation_models import SecretsModel, GcpSecretsModel, SecretModel, KeePassSecretsModel
-
+from .validation_models import SecretsModel, GcpSecretsModel, SecretModel, KeePassSecretsModel
 
 class SecretsReader(ABC):
     @abstractmethod
     def read_secrets(self) -> SecretsModel:
         pass
```

### Comparing `keegcpass-0.2.0/src/secrets_writers.py` & `keegcpass-0.3.0/src/secrets_writers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import abstractmethod, ABC
 from typing import List
 
 from google.cloud import secretmanager_v1 as sm
 from google.cloud.secretmanager_v1 import SecretVersion
 from pykeepass import PyKeePass
 
-from validation_models import KeePassSecretsModel, GcpSecretsModel, SecretsModel
+from .validation_models import KeePassSecretsModel, GcpSecretsModel, SecretsModel
 
 
 class SecretsWriter(ABC):
     @abstractmethod
     def write_secrets(self, data: SecretsModel):
         pass
```

### Comparing `keegcpass-0.2.0/src/validation_models.py` & `keegcpass-0.3.0/src/validation_models.py`

 * *Files identical despite different names*

### Comparing `keegcpass-0.2.0/PKG-INFO` & `keegcpass-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keegcpass
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Home-page: https://github.com/andyvk85/KeeGCPass
 License: MIT
 Author: Andy Koch
 Author-email: andyvk85@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

