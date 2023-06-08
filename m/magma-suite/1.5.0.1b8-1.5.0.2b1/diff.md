# Comparing `tmp/magma_suite-1.5.0.1b8.tar.gz` & `tmp/magma_suite-1.5.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magma_suite-1.5.0.1b8.tar", max compression
+gzip compressed data, was "magma_suite-1.5.0.2b1.tar", max compression
```

## Comparing `magma_suite-1.5.0.1b8.tar` & `magma_suite-1.5.0.2b1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1083 2023-04-17 13:06:49.055030 magma_suite-1.5.0.1b8/LICENSE.txt
--rw-r--r--   0        0        0       96 2023-04-17 13:06:49.055168 magma_suite-1.5.0.1b8/README.md
--rw-r--r--   0        0        0        1 2023-04-17 13:06:49.056496 magma_suite-1.5.0.1b8/magma/__init__.py
--rw-r--r--   0        0        0     3444 2023-04-17 13:06:49.056599 magma_suite-1.5.0.1b8/magma/checkstatus.py
--rw-r--r--   0        0        0    12922 2023-04-17 13:06:49.056747 magma_suite-1.5.0.1b8/magma/inputgenerator.py
--rw-r--r--   0        0        0    15898 2023-04-17 13:06:49.056890 magma_suite-1.5.0.1b8/magma/metawfl.py
--rw-r--r--   0        0        0     8908 2023-04-17 13:06:49.057016 magma_suite-1.5.0.1b8/magma/metawflrun.py
--rw-r--r--   0        0        0     4087 2023-04-17 13:06:49.057111 magma_suite-1.5.0.1b8/magma/runupdate.py
--rw-r--r--   0        0        0        0 2023-04-17 13:06:49.057170 magma_suite-1.5.0.1b8/magma_ff/__init__.py
--rw-r--r--   0        0        0     2391 2023-06-02 15:40:57.870914 magma_suite-1.5.0.1b8/magma_ff/checkstatus.py
--rw-r--r--   0        0        0        0 2023-05-17 18:56:40.284445 magma_suite-1.5.0.1b8/magma_ff/commands/__init__.py
--rw-r--r--   0        0        0     1229 2023-05-17 18:56:40.284626 magma_suite-1.5.0.1b8/magma_ff/commands/create_meta_workflow_run.py
--rw-r--r--   0        0        0    53452 2023-05-17 18:56:40.285676 magma_suite-1.5.0.1b8/magma_ff/create_metawfr.py
--rw-r--r--   0        0        0     6670 2023-04-17 13:06:49.057654 magma_suite-1.5.0.1b8/magma_ff/import_metawfr.py
--rw-r--r--   0        0        0     5097 2023-04-17 13:06:49.057752 magma_suite-1.5.0.1b8/magma_ff/inputgenerator.py
--rw-r--r--   0        0        0      778 2023-04-17 13:06:49.057830 magma_suite-1.5.0.1b8/magma_ff/metawfl.py
--rw-r--r--   0        0        0     3162 2023-04-17 13:06:49.057893 magma_suite-1.5.0.1b8/magma_ff/metawflrun.py
--rw-r--r--   0        0        0     5032 2023-04-17 13:06:49.058001 magma_suite-1.5.0.1b8/magma_ff/parser.py
--rw-r--r--   0        0        0     6915 2023-04-17 13:06:49.058109 magma_suite-1.5.0.1b8/magma_ff/reset_metawfr.py
--rw-r--r--   0        0        0     2465 2023-04-17 13:06:49.058190 magma_suite-1.5.0.1b8/magma_ff/run_metawfr.py
--rw-r--r--   0        0        0       30 2023-04-17 13:06:49.058247 magma_suite-1.5.0.1b8/magma_ff/runupdate.py
--rw-r--r--   0        0        0     5650 2023-04-17 13:06:49.058329 magma_suite-1.5.0.1b8/magma_ff/status_metawfr.py
--rw-r--r--   0        0        0     1398 2023-04-17 13:06:49.058411 magma_suite-1.5.0.1b8/magma_ff/update_cost_metawfr.py
--rw-r--r--   0        0        0     3843 2023-06-02 15:40:57.871181 magma_suite-1.5.0.1b8/magma_ff/utils.py
--rw-r--r--   0        0        0     4066 2023-06-02 15:40:57.871562 magma_suite-1.5.0.1b8/magma_ff/wfrutils.py
--rw-r--r--   0        0        0     1037 2023-06-02 16:22:59.429419 magma_suite-1.5.0.1b8/pyproject.toml
--rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 magma_suite-1.5.0.1b8/setup.py
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 magma_suite-1.5.0.1b8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-17 13:06:49.055030 magma_suite-1.5.0.2b1/LICENSE.txt
+-rw-r--r--   0        0        0       96 2023-04-17 13:06:49.055168 magma_suite-1.5.0.2b1/README.md
+-rw-r--r--   0        0        0        1 2023-04-17 13:06:49.056496 magma_suite-1.5.0.2b1/magma/__init__.py
+-rw-r--r--   0        0        0     3444 2023-04-17 13:06:49.056599 magma_suite-1.5.0.2b1/magma/checkstatus.py
+-rw-r--r--   0        0        0    12922 2023-04-17 13:06:49.056747 magma_suite-1.5.0.2b1/magma/inputgenerator.py
+-rw-r--r--   0        0        0    15898 2023-04-17 13:06:49.056890 magma_suite-1.5.0.2b1/magma/metawfl.py
+-rw-r--r--   0        0        0     8908 2023-04-17 13:06:49.057016 magma_suite-1.5.0.2b1/magma/metawflrun.py
+-rw-r--r--   0        0        0     4087 2023-04-17 13:06:49.057111 magma_suite-1.5.0.2b1/magma/runupdate.py
+-rw-r--r--   0        0        0        0 2023-04-17 13:06:49.057170 magma_suite-1.5.0.2b1/magma_ff/__init__.py
+-rw-r--r--   0        0        0     2391 2023-06-02 15:40:57.870914 magma_suite-1.5.0.2b1/magma_ff/checkstatus.py
+-rw-r--r--   0        0        0        0 2023-06-08 12:40:47.290014 magma_suite-1.5.0.2b1/magma_ff/commands/__init__.py
+-rw-r--r--   0        0        0     1229 2023-06-08 12:40:47.290237 magma_suite-1.5.0.2b1/magma_ff/commands/create_meta_workflow_run.py
+-rw-r--r--   0        0        0    53452 2023-06-08 12:40:47.290830 magma_suite-1.5.0.2b1/magma_ff/create_metawfr.py
+-rw-r--r--   0        0        0     6670 2023-04-17 13:06:49.057654 magma_suite-1.5.0.2b1/magma_ff/import_metawfr.py
+-rw-r--r--   0        0        0     5097 2023-04-17 13:06:49.057752 magma_suite-1.5.0.2b1/magma_ff/inputgenerator.py
+-rw-r--r--   0        0        0      778 2023-04-17 13:06:49.057830 magma_suite-1.5.0.2b1/magma_ff/metawfl.py
+-rw-r--r--   0        0        0     3162 2023-04-17 13:06:49.057893 magma_suite-1.5.0.2b1/magma_ff/metawflrun.py
+-rw-r--r--   0        0        0     5032 2023-04-17 13:06:49.058001 magma_suite-1.5.0.2b1/magma_ff/parser.py
+-rw-r--r--   0        0        0     6915 2023-04-17 13:06:49.058109 magma_suite-1.5.0.2b1/magma_ff/reset_metawfr.py
+-rw-r--r--   0        0        0     2465 2023-04-17 13:06:49.058190 magma_suite-1.5.0.2b1/magma_ff/run_metawfr.py
+-rw-r--r--   0        0        0       30 2023-04-17 13:06:49.058247 magma_suite-1.5.0.2b1/magma_ff/runupdate.py
+-rw-r--r--   0        0        0     5650 2023-04-17 13:06:49.058329 magma_suite-1.5.0.2b1/magma_ff/status_metawfr.py
+-rw-r--r--   0        0        0     1398 2023-04-17 13:06:49.058411 magma_suite-1.5.0.2b1/magma_ff/update_cost_metawfr.py
+-rw-r--r--   0        0        0     3843 2023-06-08 12:40:47.291139 magma_suite-1.5.0.2b1/magma_ff/utils.py
+-rw-r--r--   0        0        0     4066 2023-06-02 15:40:57.871562 magma_suite-1.5.0.2b1/magma_ff/wfrutils.py
+-rw-r--r--   0        0        0     1037 2023-06-08 12:47:15.613036 magma_suite-1.5.0.2b1/pyproject.toml
+-rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 magma_suite-1.5.0.2b1/setup.py
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 magma_suite-1.5.0.2b1/PKG-INFO
```

### Comparing `magma_suite-1.5.0.1b8/LICENSE.txt` & `magma_suite-1.5.0.2b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma/checkstatus.py` & `magma_suite-1.5.0.2b1/magma/checkstatus.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma/inputgenerator.py` & `magma_suite-1.5.0.2b1/magma/inputgenerator.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma/metawfl.py` & `magma_suite-1.5.0.2b1/magma/metawfl.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma/metawflrun.py` & `magma_suite-1.5.0.2b1/magma/metawflrun.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma/runupdate.py` & `magma_suite-1.5.0.2b1/magma/runupdate.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma_ff/checkstatus.py` & `magma_suite-1.5.0.2b1/magma_ff/checkstatus.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma_ff/commands/create_meta_workflow_run.py` & `magma_suite-1.5.0.2b1/magma_ff/commands/create_meta_workflow_run.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma_ff/create_metawfr.py` & `magma_suite-1.5.0.2b1/magma_ff/create_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma_ff/import_metawfr.py` & `magma_suite-1.5.0.2b1/magma_ff/import_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma_ff/inputgenerator.py` & `magma_suite-1.5.0.2b1/magma_ff/inputgenerator.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma_ff/metawfl.py` & `magma_suite-1.5.0.2b1/magma_ff/metawfl.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma_ff/metawflrun.py` & `magma_suite-1.5.0.2b1/magma_ff/metawflrun.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma_ff/parser.py` & `magma_suite-1.5.0.2b1/magma_ff/parser.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma_ff/reset_metawfr.py` & `magma_suite-1.5.0.2b1/magma_ff/reset_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma_ff/run_metawfr.py` & `magma_suite-1.5.0.2b1/magma_ff/run_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma_ff/status_metawfr.py` & `magma_suite-1.5.0.2b1/magma_ff/status_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma_ff/update_cost_metawfr.py` & `magma_suite-1.5.0.2b1/magma_ff/update_cost_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma_ff/utils.py` & `magma_suite-1.5.0.2b1/magma_ff/utils.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/magma_ff/wfrutils.py` & `magma_suite-1.5.0.2b1/magma_ff/wfrutils.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b8/pyproject.toml` & `magma_suite-1.5.0.2b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magma-suite"
-version = "1.5.0.1b8"  # to become 1.5.0
+version = "1.5.0.2b1"  # to become 1.5.0
 description = "Collection of tools to manage meta-workflows automation."
 authors = ["Michele Berselli <berselli.michele@gmail.com>", "Doug Rioux", "Soo Lee", "CGAP team"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbmi-bgm/magma"
 homepage = "https://github.com/dbmi-bgm/magma"
 classifiers = [
@@ -17,15 +17,15 @@
     { include="magma" },
     { include="magma_ff" }
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.9"
-dcicutils = "^7.5.0"
+dcicutils = "^7.5.1"
 tibanna-ff = "^1.3.3"
 
 
 [tool.poetry.dev-dependencies]
 mock = "*"
 pytest = "*"
```

### Comparing `magma_suite-1.5.0.1b8/setup.py` & `magma_suite-1.5.0.2b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 packages = \
 ['magma', 'magma_ff', 'magma_ff.commands']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['dcicutils>=7.5.0,<8.0.0', 'tibanna-ff>=1.3.3,<2.0.0']
+['dcicutils>=7.5.1,<8.0.0', 'tibanna-ff>=1.3.3,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['create-meta-workflow-run = '
                      'magma_ff.commands.create_meta_workflow_run:main',
                      'publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'magma-suite',
-    'version': '1.5.0.1b8',
+    'version': '1.5.0.2b1',
     'description': 'Collection of tools to manage meta-workflows automation.',
     'long_description': '# magma\n\n[*Documentation*](https://magma-suite.readthedocs.io/en/latest/ "magma documentation")\n',
     'author': 'Michele Berselli',
     'author_email': 'berselli.michele@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dbmi-bgm/magma',
```

