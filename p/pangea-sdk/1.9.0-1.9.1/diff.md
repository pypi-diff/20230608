# Comparing `tmp/pangea_sdk-1.9.0.tar.gz` & `tmp/pangea_sdk-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangea_sdk-1.9.0.tar", max compression
+gzip compressed data, was "pangea_sdk-1.9.1.tar", max compression
```

## Comparing `pangea_sdk-1.9.0.tar` & `pangea_sdk-1.9.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     7767 2023-04-28 12:39:18.679772 pangea_sdk-1.9.0/README.md
--rw-r--r--   0        0        0      146 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/__init__.py
--rw-r--r--   0        0        0     3778 2023-04-28 12:39:18.679772 pangea_sdk-1.9.0/pangea/audit_logger.py
--rw-r--r--   0        0        0     1059 2023-05-25 19:57:45.767916 pangea_sdk-1.9.0/pangea/config.py
--rw-r--r--   0        0        0     8741 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/deep_verify.py
--rw-r--r--   0        0        0      604 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/deprecated.py
--rw-r--r--   0        0        0     6511 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/dump_audit.py
--rw-r--r--   0        0        0     4458 2023-05-25 19:57:45.767916 pangea_sdk-1.9.0/pangea/exceptions.py
--rw-r--r--   0        0        0    10052 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/request.py
--rw-r--r--   0        0        0     3891 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/response.py
--rw-r--r--   0        0        0      221 2023-05-25 19:57:45.767916 pangea_sdk-1.9.0/pangea/services/__init__.py
--rw-r--r--   0        0        0    24530 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/audit/audit.py
--rw-r--r--   0        0        0      451 2023-04-28 12:39:18.679772 pangea_sdk-1.9.0/pangea/services/audit/exceptions.py
--rw-r--r--   0        0        0    12093 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/audit/models.py
--rw-r--r--   0        0        0     5281 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/audit/signing.py
--rw-r--r--   0        0        0     7807 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/audit/util.py
--rw-r--r--   0        0        0    37055 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/authn/authn.py
--rw-r--r--   0        0        0    16758 2023-05-25 19:57:45.767916 pangea_sdk-1.9.0/pangea/services/authn/models.py
--rw-r--r--   0        0        0      956 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/base.py
--rw-r--r--   0        0        0     4034 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/embargo.py
--rw-r--r--   0        0        0    34640 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/intel.py
--rw-r--r--   0        0        0     7440 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/redact.py
--rw-r--r--   0        0        0     1450 2023-04-28 12:39:18.679772 pangea_sdk-1.9.0/pangea/services/vault/models/asymmetric.py
--rw-r--r--   0        0        0     8463 2023-04-28 18:21:39.489966 pangea_sdk-1.9.0/pangea/services/vault/models/common.py
--rw-r--r--   0        0        0      481 2023-04-28 12:39:18.679772 pangea_sdk-1.9.0/pangea/services/vault/models/secret.py
--rw-r--r--   0        0        0     1330 2023-04-28 18:21:39.489966 pangea_sdk-1.9.0/pangea/services/vault/models/symmetric.py
--rw-r--r--   0        0        0    44423 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/services/vault/vault.py
--rw-r--r--   0        0        0     5472 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/tools.py
--rw-r--r--   0        0        0      554 2023-05-23 13:45:34.331889 pangea_sdk-1.9.0/pangea/utils.py
--rw-r--r--   0        0        0    10616 2023-05-25 20:04:02.232288 pangea_sdk-1.9.0/pangea/verify_audit.py
--rw-r--r--   0        0        0      840 2023-05-25 20:04:02.236288 pangea_sdk-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     8760 1970-01-01 00:00:00.000000 pangea_sdk-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     7767 2023-04-28 12:40:26.182902 pangea_sdk-1.9.1/README.md
+-rw-r--r--   0        0        0      146 2023-06-08 12:11:20.163141 pangea_sdk-1.9.1/pangea/__init__.py
+-rw-r--r--   0        0        0     3778 2023-04-28 12:40:26.182902 pangea_sdk-1.9.1/pangea/audit_logger.py
+-rw-r--r--   0        0        0     1059 2023-06-06 18:59:31.171699 pangea_sdk-1.9.1/pangea/config.py
+-rw-r--r--   0        0        0     8343 2023-06-08 19:01:01.397510 pangea_sdk-1.9.1/pangea/deep_verify.py
+-rw-r--r--   0        0        0      604 2023-06-08 19:01:01.397510 pangea_sdk-1.9.1/pangea/deprecated.py
+-rw-r--r--   0        0        0     6511 2023-06-08 19:01:01.397510 pangea_sdk-1.9.1/pangea/dump_audit.py
+-rw-r--r--   0        0        0     4458 2023-06-06 18:59:31.171699 pangea_sdk-1.9.1/pangea/exceptions.py
+-rw-r--r--   0        0        0     9922 2023-06-08 19:01:01.397510 pangea_sdk-1.9.1/pangea/request.py
+-rw-r--r--   0        0        0     3891 2023-06-08 19:01:01.397510 pangea_sdk-1.9.1/pangea/response.py
+-rw-r--r--   0        0        0      221 2023-06-06 18:59:31.171699 pangea_sdk-1.9.1/pangea/services/__init__.py
+-rw-r--r--   0        0        0    24530 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/audit/audit.py
+-rw-r--r--   0        0        0      451 2023-04-28 12:40:26.182902 pangea_sdk-1.9.1/pangea/services/audit/exceptions.py
+-rw-r--r--   0        0        0    12093 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/audit/models.py
+-rw-r--r--   0        0        0     5265 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/audit/signing.py
+-rw-r--r--   0        0        0     7638 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/audit/util.py
+-rw-r--r--   0        0        0    37055 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/authn/authn.py
+-rw-r--r--   0        0        0    16758 2023-06-02 19:28:58.018357 pangea_sdk-1.9.1/pangea/services/authn/models.py
+-rw-r--r--   0        0        0      956 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/base.py
+-rw-r--r--   0        0        0     4034 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/embargo.py
+-rw-r--r--   0        0        0    35748 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/intel.py
+-rw-r--r--   0        0        0     7440 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/redact.py
+-rw-r--r--   0        0        0     1450 2023-04-28 12:40:26.182902 pangea_sdk-1.9.1/pangea/services/vault/models/asymmetric.py
+-rw-r--r--   0        0        0     8463 2023-06-06 18:59:31.171699 pangea_sdk-1.9.1/pangea/services/vault/models/common.py
+-rw-r--r--   0        0        0      481 2023-04-28 12:40:26.182902 pangea_sdk-1.9.1/pangea/services/vault/models/secret.py
+-rw-r--r--   0        0        0     1330 2023-05-04 12:20:49.539533 pangea_sdk-1.9.1/pangea/services/vault/models/symmetric.py
+-rw-r--r--   0        0        0    44423 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/vault/vault.py
+-rw-r--r--   0        0        0     5547 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/tools.py
+-rw-r--r--   0        0        0      974 2023-06-08 12:11:20.163141 pangea_sdk-1.9.1/pangea/utils.py
+-rw-r--r--   0        0        0    10616 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/verify_audit.py
+-rw-r--r--   0        0        0      840 2023-06-08 12:11:20.163141 pangea_sdk-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     8760 1970-01-01 00:00:00.000000 pangea_sdk-1.9.1/PKG-INFO
```

### Comparing `pangea_sdk-1.9.0/README.md` & `pangea_sdk-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/audit_logger.py` & `pangea_sdk-1.9.1/pangea/audit_logger.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/config.py` & `pangea_sdk-1.9.1/pangea/config.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/deep_verify.py` & `pangea_sdk-1.9.1/pangea/deep_verify.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,27 +82,14 @@
     return 2 ** (math.ceil(math.log2(tree_size)) - 1)
 
 
 def get_proof_path(proof: str) -> str:
     return "".join(elem[0] for elem in proof.split(","))
 
 
-def height(size: int) -> int:
-    return int(math.log2(size)) + 1
-
-
-def index_number(tree_height: int, membership_proof: str) -> int:
-    decoded_proof = audit_util.decode_membership_proof(membership_proof)
-    idx_number: int = 0
-    for idx, proof in enumerate(decoded_proof):
-        if proof.side == "left":
-            idx_number += round(2 ** (tree_height - idx - 1))
-    return idx_number
-
-
 def verify_hash(data: dict, data_hash: str) -> bool:
     """Verify the hash of an event"""
     succeeded = False
     try:
         if not audit_util.verify_envelope_hash(EventEnvelope(**data), data_hash):
             print("Hash failed: ", data)
             raise ValueError("Hash does not match")
```

### Comparing `pangea_sdk-1.9.0/pangea/deprecated.py` & `pangea_sdk-1.9.1/pangea/deprecated.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/dump_audit.py` & `pangea_sdk-1.9.1/pangea/dump_audit.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/exceptions.py` & `pangea_sdk-1.9.1/pangea/exceptions.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/request.py` & `pangea_sdk-1.9.1/pangea/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,16 +235,14 @@
             raise exceptions.ServiceNotEnabledException(self.service, response)
         elif status == ResponseStatus.PROVIDER_ERR.value:
             raise exceptions.ProviderErrorException(summary, response)
         elif status in (ResponseStatus.MISSING_CONFIG_ID_SCOPE.value, ResponseStatus.MISSING_CONFIG_ID.value):
             raise exceptions.MissingConfigID(self.service, response)
         elif status == ResponseStatus.SERVICE_NOT_AVAILABLE.value:
             raise exceptions.ServiceNotAvailableException(summary, response)
-        elif status == ResponseStatus.NOT_FOUND.value:
-            raise exceptions.NotFound(response.raw_response.url, response)
         elif status == ResponseStatus.TREE_NOT_FOUND.value:
             raise exceptions.TreeNotFoundException(summary, response)
         elif status == ResponseStatus.IP_NOT_FOUND.value:
             raise exceptions.IPNotFoundException(summary)
         elif status == ResponseStatus.BAD_OFFSET.value:
             raise exceptions.BadOffsetException(summary, response)
         elif status == ResponseStatus.FORBIDDEN_VAULT_OPERATION.value:
```

### Comparing `pangea_sdk-1.9.0/pangea/response.py` & `pangea_sdk-1.9.1/pangea/response.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/services/audit/audit.py` & `pangea_sdk-1.9.1/pangea/services/audit/audit.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/services/audit/models.py` & `pangea_sdk-1.9.1/pangea/services/audit/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,16 +166,16 @@
     action: List[str] = []
     source: List[str] = []
     status: List[str] = []
     target: List[str] = []
 
 
 class SearchOrder(str, enum.Enum):
-    ASC = "desc"
-    DESC = "asc"
+    ASC = "asc"
+    DESC = "desc"
 
     def __str__(self):
         return str(self.value)
 
     def __repr__(self):
         return str(self.value)
```

### Comparing `pangea_sdk-1.9.0/pangea/services/audit/signing.py` & `pangea_sdk-1.9.1/pangea/services/audit/signing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
 from abc import ABC, abstractmethod
-from base64 import b64decode, b64encode
 from typing import Optional
 
 from cryptography import exceptions
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import ed25519
 from cryptography.hazmat.primitives.asymmetric.types import PRIVATE_KEY_TYPES
 from pangea.exceptions import PangeaException
-from pangea.services.audit.util import b64decode_ascii
+from pangea.services.audit.util import b64decode, b64decode_ascii, b64encode_ascii
 from pangea.services.vault.models.common import AsymmetricAlgorithm
 
 
 class AlgorithmSigner(ABC):
     def __init__(self, private_key):
         self.private_key: PRIVATE_KEY_TYPES = private_key
 
@@ -29,15 +28,15 @@
     def get_algorithm(self) -> str:
         pass
 
 
 class ED25519Signer(AlgorithmSigner):
     def sign(self, message: bytes) -> str:
         signature = self.private_key.sign(message)
-        return b64encode(signature).decode("ascii")
+        return b64encode_ascii(signature)
 
     def get_public_key_PEM(self) -> str:
         return (
             self.private_key.public_key()
             .public_bytes(encoding=serialization.Encoding.PEM, format=serialization.PublicFormat.SubjectPublicKeyInfo)
             .decode("utf-8")
         )
@@ -134,15 +133,15 @@
         self, signature_b64: str, message_bytes: bytes, public_key_input: str = None
     ) -> Optional[bool]:
         if self._has_header(public_key_input):
             pubkey = self._decode_public_key(bytes(public_key_input, "utf-8"))
         else:
             # To make backward compatible with original public keys send encoded bytes in base64
             public_key_bytes = b64decode_ascii(public_key_input)
-            pubkey = ed25519.Ed25519PublicKey.from_public_bytes(public_key_bytes)
+            pubkey = ed25519.Ed25519PublicKey.from_public_bytes(public_key_bytes[-32:])
 
         signature_bytes = b64decode(signature_b64)
         for cls, verifier in verifiers.items():
             if isinstance(pubkey, cls):
                 return verifier(pubkey).verify(message_bytes, signature_bytes)
         else:
             raise PangeaException(f"Not supported public key type: {type(pubkey)}")
```

### Comparing `pangea_sdk-1.9.0/pangea/services/audit/util.py` & `pangea_sdk-1.9.1/pangea/services/audit/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,18 +68,18 @@
 
 
 def canonicalize_event(event: Event) -> bytes:
     tpm_event = event.get_stringified_copy()
     return canonicalize_json(normalize_log(tpm_event.dict(exclude_none=True)))
 
 
-def b64encode(data: bytes) -> bytes:
+def b64encode(data: bytes) -> str:
     ret = None
     if data is not None:
-        ret = base64.b64encode(data)
+        ret = base64.b64encode(data).decode("utf-8")
     return ret
 
 
 def b64encode_ascii(data: bytes) -> str:
     ret = None
     if data is not None:
         ret = base64.b64encode(data).decode("ascii")
@@ -89,15 +89,15 @@
 def b64decode_ascii(data: str) -> bytes:
     ret = None
     if data is not None:
         ret = base64.b64decode(data.encode("ascii"))
     return ret
 
 
-def b64decode(data) -> bytes:
+def b64decode(data: str) -> bytes:
     ret = None
     if data is not None:
         ret = base64.b64decode(data)
     return ret
 
 
 def decode_membership_proof(data: str) -> MembershipProof:
@@ -182,21 +182,14 @@
     return sha256(bytes(data, "utf8")).hexdigest()
 
 
 def hash_dict(data: dict) -> str:
     return sha256(canonicalize_json(data)).hexdigest()
 
 
-def base64url_decode(input_parameter):
-    rem = len(input_parameter) % 4
-    if rem > 0:
-        input_parameter += "=" * (4 - rem)
-    return base64.urlsafe_b64decode(input_parameter)
-
-
 def arweave_transaction_url(trans_id: str):
     return f"{ARWEAVE_BASE_URL}/{trans_id}/"
 
 
 def arweave_graphql_url():
     return f"{ARWEAVE_BASE_URL}/graphql"
```

### Comparing `pangea_sdk-1.9.0/pangea/services/authn/authn.py` & `pangea_sdk-1.9.1/pangea/services/authn/authn.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/services/authn/models.py` & `pangea_sdk-1.9.1/pangea/services/authn/models.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/services/base.py` & `pangea_sdk-1.9.1/pangea/services/base.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/services/embargo.py` & `pangea_sdk-1.9.1/pangea/services/embargo.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/services/intel.py` & `pangea_sdk-1.9.1/pangea/services/intel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
 import enum
 import hashlib
 from typing import Dict, List, Optional
 
 from pangea.deprecated import pangea_deprecated
+from pangea.exceptions import PangeaException
 from pangea.response import APIRequestModel, APIResponseModel, PangeaResponse, PangeaResponseResult
 
 from .base import ServiceBase
 
 
 class IntelCommonRequest(APIRequestModel):
     """
@@ -1026,15 +1027,15 @@
         return response
 
     def password_breached(
         self,
         hash_type: HashType,
         hash_prefix: str,
         verbose: Optional[bool] = None,
-        raw: Optional[bool] = None,
+        raw: Optional[bool] = True,
         provider: Optional[str] = None,
     ) -> PangeaResponse[UserPasswordBreachedResult]:
         """
         Look up breached passwords
 
         Find out if a password has been exposed in security breaches by providing a 5 character prefix of the password hash.
 
@@ -1064,7 +1065,30 @@
 
         input = UserPasswordBreachedRequest(
             hash_type=hash_type, hash_prefix=hash_prefix, provider=provider, verbose=verbose, raw=raw
         )
         response = self.request.post("v1/password/breached", data=input.dict(exclude_none=True))
         response.result = UserPasswordBreachedResult(**response.raw_result)
         return response
+
+    class PasswordStatus(enum.Enum):
+        BREACHED = 0
+        UNBREACHED = 1
+        INCONCLUSIVE = 2
+
+    @staticmethod
+    def is_password_breached(response: PangeaResponse[UserBreachedResult], hash: str) -> PasswordStatus:
+        if response.result.raw_data is None:
+            raise PangeaException("Need raw data to check if hash is breached. Send request with raw=true")
+
+        hash_data = response.result.raw_data.pop(hash, None)
+        if hash_data is not None:
+            # If hash is present in raw data, it's because it was breached
+            return UserIntel.PasswordStatus.BREACHED
+        else:
+            # If it's not present, should check if I have all breached hash
+            # Server will return a maximum of 1000 hash, so if breached count is greater than that,
+            # I can't conclude is password is or is not breached
+            if len(response.result.raw_data.keys()) >= 1000:
+                return UserIntel.PasswordStatus.INCONCLUSIVE
+            else:
+                return UserIntel.PasswordStatus.UNBREACHED
```

### Comparing `pangea_sdk-1.9.0/pangea/services/redact.py` & `pangea_sdk-1.9.1/pangea/services/redact.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/services/vault/models/asymmetric.py` & `pangea_sdk-1.9.1/pangea/services/vault/models/asymmetric.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/services/vault/models/common.py` & `pangea_sdk-1.9.1/pangea/services/vault/models/common.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/services/vault/models/symmetric.py` & `pangea_sdk-1.9.1/pangea/services/vault/models/symmetric.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/services/vault/vault.py` & `pangea_sdk-1.9.1/pangea/services/vault/vault.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pangea/tools.py` & `pangea_sdk-1.9.1/pangea/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import enum
 import io
 import json
 import logging
 import os
 import sys
 import typing as t
-from datetime import date, datetime, timezone
+from datetime import datetime, timezone
 from logging.handlers import TimedRotatingFileHandler
 
 from pangea.config import PangeaConfig
 from pangea.exceptions import PangeaException
 from pangea.services import Audit
 
 
@@ -96,15 +96,16 @@
                 raise ValueError("invalid data")
         except (json.JSONDecodeError, ValueError, KeyError) as e:
             exit_with_error(f"failed to parse line {idx}: {str(e)}")
 
 
 def init_audit(token: str, domain: str) -> Audit:
     config = PangeaConfig(domain=domain)
-    audit = Audit(token, config=config)
+    audit = Audit(token, config=config, logger_name="audit")
+    logger_set_pangea_config(logger_name=audit.logger.name)
     return audit
 
 
 def make_aware_datetime(d: datetime) -> datetime:
     if d.tzinfo is None or d.tzinfo.utcoffset(d) is None:
         return d.replace(tzinfo=timezone.utc)
     else:
```

### Comparing `pangea_sdk-1.9.0/pangea/verify_audit.py` & `pangea_sdk-1.9.1/pangea/verify_audit.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.0/pyproject.toml` & `pangea_sdk-1.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pangea-sdk"
-version = "1.9.0"
+version = "1.9.1"
 description = "Pangea API SDK"
 authors = ["Glenn Gallien <glenn.gallien@pangea.cloud>"]
 license = "MIT"
 readme = "README.md"
 homepage = ""
 repository = ""
 keywords = ["Pangea", "SDK", "Audit"]
@@ -14,15 +14,15 @@
 ]
 packages = [
     { include = "pangea" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
-requests = "^2.27.1"
+requests = "^2.31.0"
 cryptography = "39.0.1"
 schema = "^0.7.5"
 python-dateutil = "^2.8.2"
 alive-progress = "^2.4.1"
 pydantic = "^1.10.2"
 pytest = "^7.2.0"
 deprecated = "^1.2.13"
```

### Comparing `pangea_sdk-1.9.0/PKG-INFO` & `pangea_sdk-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangea-sdk
-Version: 1.9.0
+Version: 1.9.1
 Summary: Pangea API SDK
 License: MIT
 Keywords: Pangea,SDK,Audit
 Author: Glenn Gallien
 Author-email: glenn.gallien@pangea.cloud
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: alive-progress (>=2.4.1,<3.0.0)
 Requires-Dist: cryptography (==39.0.1)
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pytest (>=7.2.0,<8.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: schema (>=0.7.5,<0.8.0)
 Description-Content-Type: text/markdown
 
 <p>
   <br />
   <a href="https://pangea.cloud?utm_source=github&utm_medium=node-sdk" target="_blank" rel="noopener noreferrer">
     <img src="https://pangea-marketing.s3.us-west-2.amazonaws.com/pangea-color.svg" alt="Pangea Logo" height="40" />
```

