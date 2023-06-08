# Comparing `tmp/fastapi_restful-0.4.4.tar.gz` & `tmp/fastapi_restful-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_restful-0.4.4.tar", max compression
+gzip compressed data, was "fastapi_restful-0.4.5.tar", max compression
```

## Comparing `fastapi_restful-0.4.4.tar` & `fastapi_restful-0.4.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1081 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/LICENSE
--rw-r--r--   0        0        0     3597 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/README.md
--rw-r--r--   0        0        0      196 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/__init__.py
--rw-r--r--   0        0        0      881 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/api_model.py
--rw-r--r--   0        0        0     2518 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/api_settings.py
--rw-r--r--   0        0        0      882 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/camelcase.py
--rw-r--r--   0        0        0     6990 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/cbv.py
--rw-r--r--   0        0        0     1045 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/cbv_base.py
--rw-r--r--   0        0        0     1226 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/enums.py
--rw-r--r--   0        0        0     2251 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/guid_type.py
--rw-r--r--   0        0        0      245 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/inferring_router.py
--rw-r--r--   0        0        0      367 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/openapi.py
--rw-r--r--   0        0        0        0 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/py.typed
--rw-r--r--   0        0        0     5205 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/session.py
--rw-r--r--   0        0        0     3519 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/tasks.py
--rw-r--r--   0        0        0     7113 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/fastapi_restful/timing.py
--rw-r--r--   0        0        0     3272 2023-06-07 00:11:26.982122 fastapi_restful-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     5435 1970-01-01 00:00:00.000000 fastapi_restful-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-08 20:36:09.656974 fastapi_restful-0.4.5/LICENSE
+-rw-r--r--   0        0        0     3597 2023-06-08 20:36:09.656974 fastapi_restful-0.4.5/README.md
+-rw-r--r--   0        0        0      196 2023-06-08 20:36:09.656974 fastapi_restful-0.4.5/fastapi_restful/__init__.py
+-rw-r--r--   0        0        0      881 2023-06-08 20:36:09.656974 fastapi_restful-0.4.5/fastapi_restful/api_model.py
+-rw-r--r--   0        0        0     2518 2023-06-08 20:36:09.656974 fastapi_restful-0.4.5/fastapi_restful/api_settings.py
+-rw-r--r--   0        0        0      882 2023-06-08 20:36:09.656974 fastapi_restful-0.4.5/fastapi_restful/camelcase.py
+-rw-r--r--   0        0        0     6990 2023-06-08 20:36:09.656974 fastapi_restful-0.4.5/fastapi_restful/cbv.py
+-rw-r--r--   0        0        0     1045 2023-06-08 20:36:09.656974 fastapi_restful-0.4.5/fastapi_restful/cbv_base.py
+-rw-r--r--   0        0        0     1226 2023-06-08 20:36:09.656974 fastapi_restful-0.4.5/fastapi_restful/enums.py
+-rw-r--r--   0        0        0     2251 2023-06-08 20:36:09.656974 fastapi_restful-0.4.5/fastapi_restful/guid_type.py
+-rw-r--r--   0        0        0      245 2023-06-08 20:36:09.656974 fastapi_restful-0.4.5/fastapi_restful/inferring_router.py
+-rw-r--r--   0        0        0      367 2023-06-08 20:36:09.656974 fastapi_restful-0.4.5/fastapi_restful/openapi.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:36:09.656974 fastapi_restful-0.4.5/fastapi_restful/py.typed
+-rw-r--r--   0        0        0     5205 2023-06-08 20:36:09.660974 fastapi_restful-0.4.5/fastapi_restful/session.py
+-rw-r--r--   0        0        0     3519 2023-06-08 20:36:09.660974 fastapi_restful-0.4.5/fastapi_restful/tasks.py
+-rw-r--r--   0        0        0     7113 2023-06-08 20:36:09.660974 fastapi_restful-0.4.5/fastapi_restful/timing.py
+-rw-r--r--   0        0        0     3278 2023-06-08 20:36:09.660974 fastapi_restful-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     5434 1970-01-01 00:00:00.000000 fastapi_restful-0.4.5/PKG-INFO
```

### Comparing `fastapi_restful-0.4.4/LICENSE` & `fastapi_restful-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.4.4/README.md` & `fastapi_restful-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.4.4/fastapi_restful/api_model.py` & `fastapi_restful-0.4.5/fastapi_restful/api_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.4.4/fastapi_restful/api_settings.py` & `fastapi_restful-0.4.5/fastapi_restful/api_settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.4.4/fastapi_restful/camelcase.py` & `fastapi_restful-0.4.5/fastapi_restful/camelcase.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.4.4/fastapi_restful/cbv.py` & `fastapi_restful-0.4.5/fastapi_restful/cbv.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.4.4/fastapi_restful/cbv_base.py` & `fastapi_restful-0.4.5/fastapi_restful/cbv_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.4.4/fastapi_restful/enums.py` & `fastapi_restful-0.4.5/fastapi_restful/enums.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.4.4/fastapi_restful/guid_type.py` & `fastapi_restful-0.4.5/fastapi_restful/guid_type.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.4.4/fastapi_restful/session.py` & `fastapi_restful-0.4.5/fastapi_restful/session.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.4.4/fastapi_restful/tasks.py` & `fastapi_restful-0.4.5/fastapi_restful/tasks.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.4.4/fastapi_restful/timing.py` & `fastapi_restful-0.4.5/fastapi_restful/timing.py`

 * *Files identical despite different names*

### Comparing `fastapi_restful-0.4.4/pyproject.toml` & `fastapi_restful-0.4.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-restful"
-version = "0.4.4"
+version = "0.4.5"
 description = "Quicker FastApi developing tools"
 license = "MIT"
 authors = ["Yuval Levi <yuvall9313@gmail.com>"]
 readme = "README.md"
 homepage = "https://fastapi-restful.netlify.app"
 repository = "https://github.com/yuval9313/fastapi-utils"
 documentation = "https://fastapi-restful.netlify.app"
@@ -37,15 +37,15 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Utilities"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
-fastapi = "^0.89"
+fastapi = ">=0.89,<1.0"
 pydantic = "^1.0,<2.0"
 sqlalchemy =  { version = "^1.4,<2.0", optional = true }
 psutil = "^5"
 
 [tool.poetry.dev-dependencies]
 # Starlette features
 aiofiles = "*"  # Serving static files
```

### Comparing `fastapi_restful-0.4.4/PKG-INFO` & `fastapi_restful-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-restful
-Version: 0.4.4
+Version: 0.4.5
 Summary: Quicker FastApi developing tools
 Home-page: https://fastapi-restful.netlify.app
 License: MIT
 Keywords: fastapi,OOP,RESTful
 Author: Yuval Levi
 Author-email: yuvall9313@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -31,15 +31,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Provides-Extra: all
 Provides-Extra: session
-Requires-Dist: fastapi (>=0.89,<0.90)
+Requires-Dist: fastapi (>=0.89,<1.0)
 Requires-Dist: psutil (>=5,<6)
 Requires-Dist: pydantic (>=1.0,<2.0)
 Requires-Dist: sqlalchemy (>=1.4,<2.0) ; extra == "all" or extra == "session"
 Project-URL: Documentation, https://fastapi-restful.netlify.app
 Project-URL: Repository, https://github.com/yuval9313/fastapi-utils
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-restful Version: 0.4.4 Summary: Quicker
+Metadata-Version: 2.1 Name: fastapi-restful Version: 0.4.5 Summary: Quicker
 FastApi developing tools Home-page: https://fastapi-restful.netlify.app
 License: MIT Keywords: fastapi,OOP,RESTful Author: Yuval Levi Author-email:
 yuvall9313@gmail.com Requires-Python: >=3.7,<4.0 Classifier: Development Status
 :: 4 - Beta Classifier: Environment :: Web Environment Classifier: Framework ::
 AsyncIO Classifier: Framework :: FastAPI Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: License :: OSI Approved
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: Topic :: Internet Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic ::
 Software Development Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities Classifier: Typing :: Typed Provides-Extra: all
-Provides-Extra: session Requires-Dist: fastapi (>=0.89,<0.90) Requires-Dist:
+Provides-Extra: session Requires-Dist: fastapi (>=0.89,<1.0) Requires-Dist:
 psutil (>=5,<6) Requires-Dist: pydantic (>=1.0,<2.0) Requires-Dist: sqlalchemy
 (>=1.4,<2.0) ; extra == "all" or extra == "session" Project-URL: Documentation,
 https://fastapi-restful.netlify.app Project-URL: Repository, https://
 github.com/yuval9313/fastapi-utils Description-Content-Type: text/markdown
                        Quicker FastApi developing tools
   [https://img.shields.io/github/last-commit/yuval9313/fastapi-restful.svg]_
                          [Build_CI] [Netlify_status]
```

