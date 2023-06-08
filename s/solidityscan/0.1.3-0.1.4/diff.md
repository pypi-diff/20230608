# Comparing `tmp/solidityscan-0.1.3.tar.gz` & `tmp/solidityscan-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidityscan-0.1.3.tar", last modified: Tue Jun  6 06:17:29 2023, max compression
+gzip compressed data, was "solidityscan-0.1.4.tar", last modified: Thu Jun  8 10:39:26 2023, max compression
```

## Comparing `solidityscan-0.1.3.tar` & `solidityscan-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-06-06 06:17:29.385325 solidityscan-0.1.3/
--rw-r--r--   0 manosriram   (501) staff       (20)      272 2023-06-06 06:17:29.385193 solidityscan-0.1.3/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)       55 2023-05-15 17:56:15.000000 solidityscan-0.1.3/README.md
--rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-06-06 06:17:29.385359 solidityscan-0.1.3/setup.cfg
--rw-r--r--   0 manosriram   (501) staff       (20)     1290 2023-06-06 06:16:28.000000 solidityscan-0.1.3/setup.py
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-06-06 06:17:29.384295 solidityscan-0.1.3/solidityscan.egg-info/
--rw-r--r--   0 manosriram   (501) staff       (20)      272 2023-06-06 06:17:29.000000 solidityscan-0.1.3/solidityscan.egg-info/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)      415 2023-06-06 06:17:29.000000 solidityscan-0.1.3/solidityscan.egg-info/SOURCES.txt
--rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-06-06 06:17:29.000000 solidityscan-0.1.3/solidityscan.egg-info/dependency_links.txt
--rw-r--r--   0 manosriram   (501) staff       (20)       74 2023-06-06 06:17:29.000000 solidityscan-0.1.3/solidityscan.egg-info/entry_points.txt
--rw-r--r--   0 manosriram   (501) staff       (20)      387 2023-06-06 06:17:29.000000 solidityscan-0.1.3/solidityscan.egg-info/requires.txt
--rw-r--r--   0 manosriram   (501) staff       (20)       19 2023-06-06 06:17:29.000000 solidityscan-0.1.3/solidityscan.egg-info/top_level.txt
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-06-06 06:17:29.385032 solidityscan-0.1.3/solidityscan_agent/
--rw-r--r--   0 manosriram   (501) staff       (20)     3346 2023-06-06 06:16:12.000000 solidityscan-0.1.3/solidityscan_agent/__init__.py
--rw-r--r--   0 manosriram   (501) staff       (20)     1833 2023-06-06 06:16:06.000000 solidityscan-0.1.3/solidityscan_agent/config.py
--rw-r--r--   0 manosriram   (501) staff       (20)      211 2023-06-06 06:05:13.000000 solidityscan-0.1.3/solidityscan_agent/constants.py
--rw-r--r--   0 manosriram   (501) staff       (20)     1356 2023-06-06 06:16:01.000000 solidityscan-0.1.3/solidityscan_agent/exceptions.py
--rw-r--r--   0 manosriram   (501) staff       (20)      916 2023-06-06 06:15:58.000000 solidityscan-0.1.3/solidityscan_agent/lang.py
--rw-r--r--   0 manosriram   (501) staff       (20)     2872 2023-06-06 06:15:55.000000 solidityscan-0.1.3/solidityscan_agent/scan.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-06-08 10:39:26.140337 solidityscan-0.1.4/
+-rw-r--r--   0 manosriram   (501) staff       (20)      272 2023-06-08 10:39:26.140198 solidityscan-0.1.4/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)       55 2023-05-15 17:56:15.000000 solidityscan-0.1.4/README.md
+-rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-06-08 10:39:26.140376 solidityscan-0.1.4/setup.cfg
+-rw-r--r--   0 manosriram   (501) staff       (20)     1290 2023-06-08 10:39:12.000000 solidityscan-0.1.4/setup.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-06-08 10:39:26.139279 solidityscan-0.1.4/solidityscan.egg-info/
+-rw-r--r--   0 manosriram   (501) staff       (20)      272 2023-06-08 10:39:26.000000 solidityscan-0.1.4/solidityscan.egg-info/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)      415 2023-06-08 10:39:26.000000 solidityscan-0.1.4/solidityscan.egg-info/SOURCES.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-06-08 10:39:26.000000 solidityscan-0.1.4/solidityscan.egg-info/dependency_links.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)       74 2023-06-08 10:39:26.000000 solidityscan-0.1.4/solidityscan.egg-info/entry_points.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)      387 2023-06-08 10:39:26.000000 solidityscan-0.1.4/solidityscan.egg-info/requires.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)       19 2023-06-08 10:39:26.000000 solidityscan-0.1.4/solidityscan.egg-info/top_level.txt
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-06-08 10:39:26.140010 solidityscan-0.1.4/solidityscan_agent/
+-rw-r--r--   0 manosriram   (501) staff       (20)     3352 2023-06-08 10:37:57.000000 solidityscan-0.1.4/solidityscan_agent/__init__.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1833 2023-06-08 10:37:59.000000 solidityscan-0.1.4/solidityscan_agent/config.py
+-rw-r--r--   0 manosriram   (501) staff       (20)      211 2023-06-06 06:05:13.000000 solidityscan-0.1.4/solidityscan_agent/constants.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1356 2023-06-08 10:38:02.000000 solidityscan-0.1.4/solidityscan_agent/exceptions.py
+-rw-r--r--   0 manosriram   (501) staff       (20)      916 2023-06-08 10:38:07.000000 solidityscan-0.1.4/solidityscan_agent/lang.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     2872 2023-06-08 10:38:09.000000 solidityscan-0.1.4/solidityscan_agent/scan.py
```

### Comparing `solidityscan-0.1.3/setup.py` & `solidityscan-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 def readme():
     with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
         return f.read()
 
 setup(name="solidityscan",
-      version="0.1.3",
+      version="0.1.4",
       description="Get your smart contracts audited by a smarter tool",
       long_description=readme(),
       long_description_content_type='text/markdown',
       url="https://solidityscan.com",
       entry_points={
         'console_scripts': [
             'solidityscan=solidityscan_agent.__init__:solidityscan',
```

### Comparing `solidityscan-0.1.3/solidityscan_agent/__init__.py` & `solidityscan-0.1.4/solidityscan_agent/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 @config.command()
 def show_config_path():
     """show default config path"""
     Config.get_config_path()
 
 # does a scan
 @solidityscan.command()
-@click.option("--scan-type", "-s", required=True, type=click.Choice(["project", "block"]), prompt=False, help="type of scan to perform")
+@click.option("--scan-type", "-s", required=True, type=click.Choice(["project", "contract"]), prompt=False, help="type of scan to perform")
 @click.option("-project-url", required=False, help="project url to scan")
 @click.option("-project-branch", required=False, help="branch of the project")
 @click.option("-skip-file-paths", required=False, help="file paths to skip scanning", multiple=True)
 @click.option("-rescan", "-r", is_flag=True, required=False, help="flag to denote if the scan is a rescan")
 @click.option("-contract-address", required=False, help="address of the contract")
 @click.option("-contract-chain", required=False, help="chain of the contract")
 @click.option("-contract-platform", required=False, help="platform of the contract")
@@ -64,15 +64,15 @@
     if scan_type == "project":
         if not project_url:
             raise click.UsageError("-project-url flag is required")
         if not project_branch:
             raise click.UsageError("-project-branch flag is required")
 
         s.project_scan(project_url, project_branch, rescan, skip_file_paths, token)
-    elif scan_type == "block":
+    elif scan_type == "contract":
         if not contract_address:
             raise click.UsageError("-contract-address flag is required")
         if not contract_chain:
             raise click.UsageError("-contract-chain flag is required")
         if not contract_platform:
             raise click.UsageError("-contract-platform flag is required")
```

### Comparing `solidityscan-0.1.3/solidityscan_agent/config.py` & `solidityscan-0.1.4/solidityscan_agent/config.py`

 * *Files identical despite different names*

### Comparing `solidityscan-0.1.3/solidityscan_agent/exceptions.py` & `solidityscan-0.1.4/solidityscan_agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `solidityscan-0.1.3/solidityscan_agent/lang.py` & `solidityscan-0.1.4/solidityscan_agent/lang.py`

 * *Files identical despite different names*

### Comparing `solidityscan-0.1.3/solidityscan_agent/scan.py` & `solidityscan-0.1.4/solidityscan_agent/scan.py`

 * *Files identical despite different names*

