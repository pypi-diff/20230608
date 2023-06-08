# Comparing `tmp/comet_llm-0.0.4.tar.gz` & `tmp/comet_llm-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comet_llm-0.0.4.tar", last modified: Mon Jun  5 17:33:47 2023, max compression
+gzip compressed data, was "comet_llm-1.0.0.tar", last modified: Thu Jun  8 15:09:33 2023, max compression
```

## Comparing `comet_llm-0.0.4.tar` & `comet_llm-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:33:47.685722 comet_llm-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-05 17:33:47.685722 comet_llm-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-05 17:33:30.000000 comet_llm-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:33:47.685722 comet_llm-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-05 17:33:30.000000 comet_llm-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:33:47.681722 comet_llm-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:33:47.681722 comet_llm-0.0.4/src/comet_llm/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/datetimes.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:33:47.685722 comet_llm-0.0.4/src/comet_llm/experiment_api/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/experiment_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/experiment_api/comet_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/experiment_api/experiment_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/experiment_api/request_exception_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/experiment_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-05 17:33:30.000000 comet_llm-0.0.4/src/comet_llm/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:33:47.685722 comet_llm-0.0.4/src/comet_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-05 17:33:47.000000 comet_llm-0.0.4/src/comet_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-05 17:33:47.000000 comet_llm-0.0.4/src/comet_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:33:47.000000 comet_llm-0.0.4/src/comet_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:33:47.000000 comet_llm-0.0.4/src/comet_llm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-05 17:33:47.000000 comet_llm-0.0.4/src/comet_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 17:33:47.000000 comet_llm-0.0.4/src/comet_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:09:33.932143 comet_llm-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-08 15:09:16.000000 comet_llm-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-08 15:09:33.932143 comet_llm-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-08 15:09:16.000000 comet_llm-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:09:33.932143 comet_llm-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-08 15:09:16.000000 comet_llm-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:09:33.928142 comet_llm-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:09:33.928142 comet_llm-1.0.0/src/comet_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/datetimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:09:33.932143 comet_llm-1.0.0/src/comet_llm/experiment_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/experiment_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/experiment_api/comet_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/experiment_api/experiment_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/experiment_api/request_exception_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/experiment_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-08 15:09:16.000000 comet_llm-1.0.0/src/comet_llm/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:09:33.928142 comet_llm-1.0.0/src/comet_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-08 15:09:33.000000 comet_llm-1.0.0/src/comet_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-08 15:09:33.000000 comet_llm-1.0.0/src/comet_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:09:33.000000 comet_llm-1.0.0/src/comet_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:09:33.000000 comet_llm-1.0.0/src/comet_llm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 15:09:33.000000 comet_llm-1.0.0/src/comet_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 15:09:33.000000 comet_llm-1.0.0/src/comet_llm.egg-info/top_level.txt
```

### Comparing `comet_llm-0.0.4/setup.py` & `comet_llm-1.0.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -19,42 +19,44 @@
 
 requirements = [
     "comet_ml",
     "dataclasses; python_version<'3.7.0'",
     "flatten-dict",
     "types-requests",
 ]
-
-
+project_urls = {"Source code": "https://github.com/comet-ml/comet-llm"}
 this_directory = Path(__file__).parent
+long_description = (this_directory / ".github" / "PACKAGE_README.md").read_text()
 
 
 setup(
     author="Comet ML Inc.",
-    author_email="mail@comet.ml",
+    author_email="mail@comet.com",
     python_requires=">=3.6",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
     ],
     description="Comet logger for LLM",
     install_requires=requirements,
-    long_description="Comet SDK for logging LLM chains",
+    long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="comet_llm",
     name="comet_llm",
     packages=find_packages("src"),
     package_dir={"": "src"},
-    url="https://www.comet.ml",
-    version="0.0.4",
+    url="https://www.comet.com",
+    project_urls=project_urls,
+    version="1.0.0",
     zip_safe=False,
-    license="Proprietary",
+    license="MIT",
 )
```

### Comparing `comet_llm-0.0.4/src/comet_llm/__init__.py` & `comet_llm-1.0.0/src/comet_llm/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.4/src/comet_llm/api.py` & `comet_llm-1.0.0/src/comet_llm/api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.4/src/comet_llm/config.py` & `comet_llm-1.0.0/src/comet_llm/config.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.4/src/comet_llm/convert.py` & `comet_llm-1.0.0/src/comet_llm/convert.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.4/src/comet_llm/datetimes.py` & `comet_llm-1.0.0/src/comet_llm/datetimes.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.4/src/comet_llm/exceptions.py` & `comet_llm-1.0.0/src/comet_llm/exceptions.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.4/src/comet_llm/experiment_api/__init__.py` & `comet_llm-1.0.0/src/comet_llm/experiment_api/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.4/src/comet_llm/experiment_api/comet_api_client.py` & `comet_llm-1.0.0/src/comet_llm/experiment_api/comet_api_client.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.4/src/comet_llm/experiment_api/experiment_api.py` & `comet_llm-1.0.0/src/comet_llm/experiment_api/experiment_api.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.4/src/comet_llm/experiment_api/request_exception_wrapper.py` & `comet_llm-1.0.0/src/comet_llm/experiment_api/request_exception_wrapper.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.4/src/comet_llm/experiment_info.py` & `comet_llm-1.0.0/src/comet_llm/experiment_info.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.4/src/comet_llm/preprocess.py` & `comet_llm-1.0.0/src/comet_llm/preprocess.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.4/src/comet_llm/types.py` & `comet_llm-1.0.0/src/comet_llm/types.py`

 * *Files identical despite different names*

### Comparing `comet_llm-0.0.4/src/comet_llm.egg-info/SOURCES.txt` & `comet_llm-1.0.0/src/comet_llm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 src/comet_llm/__init__.py
 src/comet_llm/api.py
 src/comet_llm/config.py
 src/comet_llm/convert.py
 src/comet_llm/datetimes.py
```

