# Comparing `tmp/reliably_cli-0.6.1.tar.gz` & `tmp/reliably_cli-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliably_cli-0.6.1.tar", last modified: Thu Jun  8 09:47:08 2023, max compression
+gzip compressed data, was "reliably_cli-0.6.2.tar", last modified: Thu Jun  8 09:53:33 2023, max compression
```

## Comparing `reliably_cli-0.6.1.tar` & `reliably_cli-0.6.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-06-08 09:46:50.565153 reliably_cli-0.6.1/LICENSE
--rw-r--r--   0        0        0     1478 2023-06-08 09:46:50.565153 reliably_cli-0.6.1/README.md
--rw-r--r--   0        0        0     3015 2023-06-08 09:47:08.252962 reliably_cli-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      114 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/__init__.py
--rw-r--r--   0        0        0      881 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/__main__.py
--rw-r--r--   0        0        0      166 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/__version__.py
--rw-r--r--   0        0        0     1221 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/agent/__init__.py
--rw-r--r--   0        0        0     1545 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/agent/cli.py
--rw-r--r--   0        0        0     2770 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/agent/plan/__init__.py
--rw-r--r--   0        0        0     1352 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/agent/plan/providers/__init__.py
--rw-r--r--   0        0        0     3493 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/agent/plan/providers/github.py
--rw-r--r--   0        0        0     1215 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/client.py
--rw-r--r--   0        0        0     1087 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/config/__init__.py
--rw-r--r--   0        0        0     3552 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/config/cli.py
--rw-r--r--   0        0        0     2403 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/config/types.py
--rw-r--r--   0        0        0      566 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/format.py
--rw-r--r--   0        0        0      126 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/log.py
--rw-r--r--   0        0        0        0 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/services/__init__.py
--rw-r--r--   0        0        0      211 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/services/cli.py
--rw-r--r--   0        0        0     2388 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/services/org.py
--rw-r--r--   0        0        0    10148 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/services/plan.py
--rw-r--r--   0        0        0     2068 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/reliably_cli/types.py
--rw-r--r--   0        0        0      662 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/tests/conftest.py
--rw-r--r--   0        0        0      581 2023-06-08 09:46:50.569153 reliably_cli-0.6.1/tests/test_cli.py
--rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 reliably_cli-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-08 09:53:10.817398 reliably_cli-0.6.2/LICENSE
+-rw-r--r--   0        0        0     1478 2023-06-08 09:53:10.817398 reliably_cli-0.6.2/README.md
+-rw-r--r--   0        0        0     3015 2023-06-08 09:53:33.981644 reliably_cli-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/__init__.py
+-rw-r--r--   0        0        0      881 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/__main__.py
+-rw-r--r--   0        0        0      166 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/__version__.py
+-rw-r--r--   0        0        0     1221 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/agent/__init__.py
+-rw-r--r--   0        0        0     1545 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/agent/cli.py
+-rw-r--r--   0        0        0     2770 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/agent/plan/__init__.py
+-rw-r--r--   0        0        0     1352 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/agent/plan/providers/__init__.py
+-rw-r--r--   0        0        0     3493 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/agent/plan/providers/github.py
+-rw-r--r--   0        0        0     1215 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/client.py
+-rw-r--r--   0        0        0     1087 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/config/__init__.py
+-rw-r--r--   0        0        0     3552 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/config/cli.py
+-rw-r--r--   0        0        0     2403 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/config/types.py
+-rw-r--r--   0        0        0      566 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/format.py
+-rw-r--r--   0        0        0      126 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/log.py
+-rw-r--r--   0        0        0        0 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/services/__init__.py
+-rw-r--r--   0        0        0      211 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/services/cli.py
+-rw-r--r--   0        0        0     2388 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/services/org.py
+-rw-r--r--   0        0        0    10148 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/services/plan.py
+-rw-r--r--   0        0        0     2068 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/reliably_cli/types.py
+-rw-r--r--   0        0        0      662 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/tests/conftest.py
+-rw-r--r--   0        0        0      581 2023-06-08 09:53:10.821398 reliably_cli-0.6.2/tests/test_cli.py
+-rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 reliably_cli-0.6.2/PKG-INFO
```

### Comparing `reliably_cli-0.6.1/LICENSE` & `reliably_cli-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/README.md` & `reliably_cli-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/pyproject.toml` & `reliably_cli-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "rich>=13.3.1",
     "chaostoolkit-addons>=0.4.0",
     "chaostoolkit>=1.15.0",
     "chaostoolkit-lib>=1.33.1",
     "chaostoolkit-reliably>=0.22.0",
     "orjson>=3.8.10",
 ]
-version = "0.6.1"
+version = "0.6.2"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 Homepage = "https://reliably.com/"
 Repository = "https://github.com/reliablyhq/cli"
```

### Comparing `reliably_cli-0.6.1/reliably_cli/__main__.py` & `reliably_cli-0.6.2/reliably_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/reliably_cli/agent/__init__.py` & `reliably_cli-0.6.2/reliably_cli/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/reliably_cli/agent/cli.py` & `reliably_cli-0.6.2/reliably_cli/agent/cli.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/reliably_cli/agent/plan/__init__.py` & `reliably_cli-0.6.2/reliably_cli/agent/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/reliably_cli/agent/plan/providers/__init__.py` & `reliably_cli-0.6.2/reliably_cli/agent/plan/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/reliably_cli/agent/plan/providers/github.py` & `reliably_cli-0.6.2/reliably_cli/agent/plan/providers/github.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/reliably_cli/client.py` & `reliably_cli-0.6.2/reliably_cli/client.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/reliably_cli/config/__init__.py` & `reliably_cli-0.6.2/reliably_cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/reliably_cli/config/cli.py` & `reliably_cli-0.6.2/reliably_cli/config/cli.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/reliably_cli/config/types.py` & `reliably_cli-0.6.2/reliably_cli/config/types.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/reliably_cli/format.py` & `reliably_cli-0.6.2/reliably_cli/format.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/reliably_cli/services/org.py` & `reliably_cli-0.6.2/reliably_cli/services/org.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/reliably_cli/services/plan.py` & `reliably_cli-0.6.2/reliably_cli/services/plan.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/reliably_cli/types.py` & `reliably_cli-0.6.2/reliably_cli/types.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/tests/conftest.py` & `reliably_cli-0.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/tests/test_cli.py` & `reliably_cli-0.6.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `reliably_cli-0.6.1/PKG-INFO` & `reliably_cli-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reliably-cli
-Version: 0.6.1
+Version: 0.6.2
 Summary: Reliably CLI
 Author-Email: Sylvain Hellegouarch <sylvain@reliably.com>
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reliably-cli Version: 0.6.1 Summary: Reliably CLI
+Metadata-Version: 2.1 Name: reliably-cli Version: 0.6.2 Summary: Reliably CLI
 Author-Email: Sylvain Hellegouarch
 reliably.com> License: Apache-2.0 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Development Status :: 4 - Beta Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities Project-URL: Homepage, https://reliably.com/
```

