# Comparing `tmp/rising_plugin-0.333.3.tar.gz` & `tmp/rising_plugin-0.333.4.tar.gz`

## Comparing `rising_plugin-0.333.3.tar` & `rising_plugin-0.333.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/.github/workflows/lint.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/.idea/.gitignore
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/.idea/Rising_Plugin.iml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/.idea/misc.xml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/.idea/vcs.xml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/.idea/watcherTasks.xml
--rw-r--r--   0        0        0     7479 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/.idea/workspace.xml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/.idea/inspectionProfiles/profiles_settings.xml
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/src/rising_plugin/__init__.py
--rwxr-xr-x   0        0        0      796 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/src/rising_plugin/csv_embed.py
--rwxr-xr-x   0        0        0     1756 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/src/rising_plugin/image_embedding.py
--rwxr-xr-x   0        0        0     1916 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/src/rising_plugin/pinecone_engine.py
--rwxr-xr-x   0        0        0     3664 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/src/rising_plugin/risingplugin.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/src/rising_plugin/common/__init__.py
--rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/src/rising_plugin/common/utils.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/src/rising_plugin/guardrails-config/__init__.py
--rwxr-xr-x   0        0        0      881 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/src/rising_plugin/guardrails-config/config.yml
--rwxr-xr-x   0        0        0      552 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/src/rising_plugin/guardrails-config/general.co
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/src/rising_plugin/guardrails-config/off-security.co
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/src/rising_plugin/guardrails-config/actions/__init__.py
--rwxr-xr-x   0        0        0     3056 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/src/rising_plugin/guardrails-config/actions/actions.py
--rwxr-xr-x   0        0        0     2415 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/src/rising_plugin/guardrails-config/actions/phone.csv
--rwxr-xr-x   0        0        0   486145 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/src/rising_plugin/guardrails-config/actions/phone.json
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/tests/__init__.py
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/LICENSE
--rwxr-xr-x   0        0        0      482 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/README.md
--rwxr-xr-x   0        0        0     1047 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/pyproject.toml
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 rising_plugin-0.333.3/PKG-INFO
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/.idea/.gitignore
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/.idea/Rising_Plugin.iml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/.idea/misc.xml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/.idea/watcherTasks.xml
+-rw-r--r--   0        0        0     7479 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/.idea/workspace.xml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/.idea/inspectionProfiles/profiles_settings.xml
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/src/rising_plugin/__init__.py
+-rwxr-xr-x   0        0        0      796 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/src/rising_plugin/csv_embed.py
+-rwxr-xr-x   0        0        0     1756 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/src/rising_plugin/image_embedding.py
+-rwxr-xr-x   0        0        0     1916 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/src/rising_plugin/pinecone_engine.py
+-rwxr-xr-x   0        0        0     3664 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/src/rising_plugin/risingplugin.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/src/rising_plugin/common/__init__.py
+-rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/src/rising_plugin/common/utils.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/src/rising_plugin/guardrails-config/__init__.py
+-rwxr-xr-x   0        0        0      881 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/src/rising_plugin/guardrails-config/config.yml
+-rwxr-xr-x   0        0        0      552 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/src/rising_plugin/guardrails-config/general.co
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/src/rising_plugin/guardrails-config/off-security.co
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/src/rising_plugin/guardrails-config/actions/__init__.py
+-rwxr-xr-x   0        0        0     3056 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/src/rising_plugin/guardrails-config/actions/actions.py
+-rwxr-xr-x   0        0        0     2415 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/src/rising_plugin/guardrails-config/actions/phone.csv
+-rwxr-xr-x   0        0        0   486145 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/src/rising_plugin/guardrails-config/actions/phone.json
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/tests/__init__.py
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/LICENSE
+-rwxr-xr-x   0        0        0      482 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/README.md
+-rwxr-xr-x   0        0        0     1047 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/pyproject.toml
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 rising_plugin-0.333.4/PKG-INFO
```

### Comparing `rising_plugin-0.333.3/.idea/watcherTasks.xml` & `rising_plugin-0.333.4/.idea/watcherTasks.xml`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.333.3/.idea/workspace.xml` & `rising_plugin-0.333.4/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.333.3/.idea/inspectionProfiles/Project_Default.xml` & `rising_plugin-0.333.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.333.3/src/rising_plugin/csv_embed.py` & `rising_plugin-0.333.4/src/rising_plugin/csv_embed.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.333.3/src/rising_plugin/image_embedding.py` & `rising_plugin-0.333.4/src/rising_plugin/image_embedding.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.333.3/src/rising_plugin/pinecone_engine.py` & `rising_plugin-0.333.4/src/rising_plugin/pinecone_engine.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.333.3/src/rising_plugin/risingplugin.py` & `rising_plugin-0.333.4/src/rising_plugin/risingplugin.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.333.3/src/rising_plugin/common/utils.py` & `rising_plugin-0.333.4/src/rising_plugin/common/utils.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.333.3/src/rising_plugin/guardrails-config/config.yml` & `rising_plugin-0.333.4/src/rising_plugin/guardrails-config/config.yml`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.333.3/src/rising_plugin/guardrails-config/general.co` & `rising_plugin-0.333.4/src/rising_plugin/guardrails-config/general.co`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.333.3/src/rising_plugin/guardrails-config/actions/actions.py` & `rising_plugin-0.333.4/src/rising_plugin/guardrails-config/actions/actions.py`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.333.3/src/rising_plugin/guardrails-config/actions/phone.csv` & `rising_plugin-0.333.4/src/rising_plugin/guardrails-config/actions/phone.csv`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.333.3/src/rising_plugin/guardrails-config/actions/phone.json` & `rising_plugin-0.333.4/src/rising_plugin/guardrails-config/actions/phone.json`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.333.3/LICENSE` & `rising_plugin-0.333.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rising_plugin-0.333.3/pyproject.toml` & `rising_plugin-0.333.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rising_plugin"
-version = "0.333.3"
+version = "0.333.4"
 authors = [
   { name="Thomas Richardson", email="thomasr37oss@gmail.com" },
 ]
 description = "It is a plugin for Rising GPT"
 readme = "README.md"
 dependencies = [
     "langchain==0.0.167",
     "pinecone-client==2.2.1",
     "openai==0.27.4",
     "pydantic==1.10.6",
     "aiohttp==3.8.4",
     "requests==2.28.2",
     "typer==0.7.0",
     "PyYAML~=6.0",
-    "setuptools==59.6.0",
+    "setuptools==65.5.1",
     "annoy==1.17.1",
     "sentence-transformers==2.2.2",
     "fastapi==0.95.0",
     "starlette==0.26.1",
     "uvicorn==0.21.1",
     "httpx==0.23.3",
     "simpleeval==0.9.13",
```

### Comparing `rising_plugin-0.333.3/PKG-INFO` & `rising_plugin-0.333.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rising_plugin
-Version: 0.333.3
+Version: 0.333.4
 Summary: It is a plugin for Rising GPT
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Thomas Richardson <thomasr37oss@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 Requires-Dist: nemoguardrails==0.2.0
 Requires-Dist: openai==0.27.4
 Requires-Dist: pinecone-client==2.2.1
 Requires-Dist: pydantic==1.10.6
 Requires-Dist: pyyaml~=6.0
 Requires-Dist: requests==2.28.2
 Requires-Dist: sentence-transformers==2.2.2
-Requires-Dist: setuptools==59.6.0
+Requires-Dist: setuptools==65.5.1
 Requires-Dist: simpleeval==0.9.13
 Requires-Dist: starlette==0.26.1
 Requires-Dist: typer==0.7.0
 Requires-Dist: typing-extensions==4.5.0
 Requires-Dist: uvicorn==0.21.1
 Description-Content-Type: text/markdown
```

