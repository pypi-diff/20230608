# Comparing `tmp/onecompiler-0.1.11.tar.gz` & `tmp/onecompiler-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onecompiler-0.1.11.tar", max compression
+gzip compressed data, was "onecompiler-1.1.0.tar", max compression
```

## Comparing `onecompiler-0.1.11.tar` & `onecompiler-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-06-06 14:12:34.685634 onecompiler-0.1.11/LICENSE
--rw-r--r--   0        0        0       37 2023-06-06 14:12:34.685634 onecompiler-0.1.11/README.md
--rw-r--r--   0        0        0      148 2023-06-07 19:21:32.574182 onecompiler-0.1.11/onecompiler/__init__.py
--rw-r--r--   0        0        0      143 2023-06-06 21:20:15.290434 onecompiler-0.1.11/onecompiler/api/__init__.py
--rw-r--r--   0        0        0      868 2023-06-06 21:19:36.366434 onecompiler-0.1.11/onecompiler/api/async_compiler.py
--rw-r--r--   0        0        0      889 2023-06-07 19:31:09.838182 onecompiler-0.1.11/onecompiler/api/compiler.py
--rw-r--r--   0        0        0      228 2023-06-06 18:35:35.538435 onecompiler-0.1.11/onecompiler/base_errors/LangNotFound.py
--rw-r--r--   0        0        0       89 2023-06-06 18:30:01.850435 onecompiler-0.1.11/onecompiler/base_errors/__init__.py
--rw-r--r--   0        0        0       90 2023-06-06 19:02:01.546434 onecompiler-0.1.11/onecompiler/base_models/__init__.py
--rw-r--r--   0        0        0      767 2023-06-07 14:46:49.652433 onecompiler-0.1.11/onecompiler/base_models/base_compiler.py
--rw-r--r--   0        0        0    39084 2023-06-07 19:35:29.334182 onecompiler-0.1.11/onecompiler/data.py
--rw-r--r--   0        0        0      175 2023-06-06 22:14:05.578435 onecompiler-0.1.11/onecompiler/pydantic_models/__init__.py
--rw-r--r--   0        0        0      602 2023-06-07 14:45:16.256433 onecompiler-0.1.11/onecompiler/pydantic_models/lang.py
--rw-r--r--   0        0        0      792 2023-06-07 19:19:53.794182 onecompiler-0.1.11/onecompiler/pydantic_models/response.py
--rw-r--r--   0        0        0       14 2023-06-06 18:12:06.070434 onecompiler-0.1.11/onecompiler/requirements.txt
--rw-r--r--   0        0        0      326 2023-06-07 19:36:18.218182 onecompiler-0.1.11/pyproject.toml
--rw-r--r--   0        0        0      622 1970-01-01 00:00:00.000000 onecompiler-0.1.11/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-06 14:12:34.685634 onecompiler-1.1.0/LICENSE
+-rw-r--r--   0        0        0       37 2023-06-06 14:12:34.685634 onecompiler-1.1.0/README.md
+-rw-r--r--   0        0        0      134 2023-06-08 17:50:43.546355 onecompiler-1.1.0/onecompiler/__init__.py
+-rw-r--r--   0        0        0      143 2023-06-06 21:20:15.290434 onecompiler-1.1.0/onecompiler/api/__init__.py
+-rw-r--r--   0        0        0     1212 2023-06-08 18:02:34.590355 onecompiler-1.1.0/onecompiler/api/async_compiler.py
+-rw-r--r--   0        0        0     1173 2023-06-08 18:01:59.642355 onecompiler-1.1.0/onecompiler/api/compiler.py
+-rw-r--r--   0        0        0      228 2023-06-06 18:35:35.538435 onecompiler-1.1.0/onecompiler/base_errors/LangNotFound.py
+-rw-r--r--   0        0        0       89 2023-06-06 18:30:01.850435 onecompiler-1.1.0/onecompiler/base_errors/__init__.py
+-rw-r--r--   0        0        0       90 2023-06-06 19:02:01.546434 onecompiler-1.1.0/onecompiler/base_models/__init__.py
+-rw-r--r--   0        0        0     1773 2023-06-08 18:06:47.770355 onecompiler-1.1.0/onecompiler/base_models/base_compiler.py
+-rw-r--r--   0        0        0     2493 2023-06-08 17:47:40.234355 onecompiler-1.1.0/onecompiler/data.py
+-rw-r--r--   0        0        0      175 2023-06-06 22:14:05.578435 onecompiler-1.1.0/onecompiler/pydantic_models/__init__.py
+-rw-r--r--   0        0        0      602 2023-06-07 14:45:16.256433 onecompiler-1.1.0/onecompiler/pydantic_models/lang.py
+-rw-r--r--   0        0        0      791 2023-06-08 16:18:50.561637 onecompiler-1.1.0/onecompiler/pydantic_models/response.py
+-rw-r--r--   0        0        0       14 2023-06-06 18:12:06.070434 onecompiler-1.1.0/onecompiler/requirements.txt
+-rw-r--r--   0        0        0      325 2023-06-08 18:07:37.554355 onecompiler-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 onecompiler-1.1.0/PKG-INFO
```

### Comparing `onecompiler-0.1.11/LICENSE` & `onecompiler-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onecompiler-0.1.11/onecompiler/api/async_compiler.py` & `onecompiler-1.1.0/onecompiler/api/async_compiler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 from httpx import AsyncClient
 from onecompiler.base_models import BaseCompiler
 from onecompiler.pydantic_models import Response
-import asyncio, time
+
 
 class ToLang:
-	def __init__(self, compiler):
-			self.compiler = compiler
+    def __init__(self, compiler):
+        self.compiler = compiler
+
+    def __getattr__(self, lang: str):
+        async def func(code: str):
+            return await self.compiler.compiler(lang, code) 
+        return func
+	
+class QueryLang:
+    def __init__(self, compiler):
+        self.compiler = compiler
 
-	def __getattr__(self, lang: str):
-		async def func(code: str):
-			return await self.compiler.compiler(lang, code) 
-		return func
+    def __getattr__(self, lang: str):
+        async def func(code: str):
+            if lang in self.compiler.query_langs:
+                return await self.compiler.compiler(lang, code) 
+        return func
 
 class AsyncCompiler(BaseCompiler):
     def __init__(self) -> None:
         super().__init__()
         self._client = AsyncClient()
         self.to = ToLang(self)
+        self.query = QueryLang(self)
 	
     async def compiler(self, lang: str, code: str) -> Response:
         """ compiles your code """
         lang_data = self._get_lang_data(lang, code)
         lang_data.properties.files[0].content = code
         res = await self._client.post(self._url, json=lang_data.dict(), headers=self._headers)
         return Response.parse_obj(res.json())
```

### Comparing `onecompiler-0.1.11/onecompiler/pydantic_models/lang.py` & `onecompiler-1.1.0/onecompiler/pydantic_models/lang.py`

 * *Files identical despite different names*

### Comparing `onecompiler-0.1.11/onecompiler/pydantic_models/response.py` & `onecompiler-1.1.0/onecompiler/pydantic_models/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 from typing import Any, List, Optional
-
 from pydantic import BaseModel
 
 
 class File(BaseModel):
     name: str
     content: str
```

### Comparing `onecompiler-0.1.11/PKG-INFO` & `onecompiler-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onecompiler
-Version: 0.1.11
+Version: 1.1.0
 Summary: 
 License: Apache
 Author: pokedim13
 Author-email: skinxedovich@vk.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

