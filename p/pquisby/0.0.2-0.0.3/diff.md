# Comparing `tmp/pquisby-0.0.2.tar.gz` & `tmp/pquisby-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pquisby-0.0.2.tar", last modified: Thu May 25 01:25:11 2023, max compression
+gzip compressed data, was "pquisby-0.0.3.tar", last modified: Thu Jun  8 04:22:01 2023, max compression
```

## Comparing `pquisby-0.0.2.tar` & `pquisby-0.0.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.166885 pquisby-0.0.2/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)    35149 2023-05-24 16:14:46.000000 pquisby-0.0.2/LICENSE
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)       39 2023-05-24 16:16:23.000000 pquisby-0.0.2/MANIFEST.in
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      798 2023-05-25 01:25:11.165885 pquisby-0.0.2/PKG-INFO
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      474 2023-05-24 16:16:23.000000 pquisby-0.0.2/README.md
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     3903 2023-05-24 16:16:23.000000 pquisby-0.0.2/requirements.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)       38 2023-05-25 01:25:11.166885 pquisby-0.0.2/setup.cfg
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      950 2023-05-25 01:24:19.000000 pquisby-0.0.2/setup.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.159885 pquisby-0.0.2/src/
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.161885 pquisby-0.0.2/src/pquisby/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-24 16:14:46.000000 pquisby-0.0.2/src/pquisby/__init__.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.163885 pquisby-0.0.2/src/pquisby/command/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 00:29:29.000000 pquisby-0.0.2/src/pquisby/command/__init__.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      488 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/command/compare_benchmark.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      300 2023-05-25 00:29:57.000000 pquisby-0.0.2/src/pquisby/command/main.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     2513 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/command/process_benchmark.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.163885 pquisby-0.0.2/src/pquisby/lib/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/__init__.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.164885 pquisby-0.0.2/src/pquisby/lib/benchmarks/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/benchmarks/__init__.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.164885 pquisby-0.0.2/src/pquisby/lib/benchmarks/uperf/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/benchmarks/uperf/__init__.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1214 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/benchmarks/uperf/comparison.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     5175 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/benchmarks/uperf/graph.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     5344 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/benchmarks/uperf/uperf.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1639 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/compare_result.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.164885 pquisby-0.0.2/src/pquisby/lib/credentials/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/credentials/__init__.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1119 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/credentials/creds.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     3699 2023-05-24 16:18:25.000000 pquisby-0.0.2/src/pquisby/lib/get_data.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.165885 pquisby-0.0.2/src/pquisby/lib/pricing/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/pricing/__init__.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     4728 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/pricing/cloud_pricing.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     5927 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/process_result.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.165885 pquisby-0.0.2/src/pquisby/lib/sheet/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/sheet/__init__.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     5692 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/sheet/sheet_util.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      783 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/sheet/sheetapi.py
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     2202 2023-05-24 16:16:23.000000 pquisby-0.0.2/src/pquisby/lib/util.py
-drwxr-xr-x   0 vvijayra  (1000) vvijayra  (1000)        0 2023-05-25 01:25:11.162885 pquisby-0.0.2/src/pquisby.egg-info/
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)      798 2023-05-25 01:25:11.000000 pquisby-0.0.2/src/pquisby.egg-info/PKG-INFO
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1054 2023-05-25 01:25:11.000000 pquisby-0.0.2/src/pquisby.egg-info/SOURCES.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        1 2023-05-25 01:25:11.000000 pquisby-0.0.2/src/pquisby.egg-info/dependency_links.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)       54 2023-05-25 01:25:11.000000 pquisby-0.0.2/src/pquisby.egg-info/entry_points.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)     1990 2023-05-25 01:25:11.000000 pquisby-0.0.2/src/pquisby.egg-info/requires.txt
--rw-r--r--   0 vvijayra  (1000) vvijayra  (1000)        8 2023-05-25 01:25:11.000000 pquisby-0.0.2/src/pquisby.egg-info/top_level.txt
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.928778 pquisby-0.0.3/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)    35149 2023-06-08 04:19:09.000000 pquisby-0.0.3/LICENSE
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)       39 2023-06-08 04:19:30.000000 pquisby-0.0.3/MANIFEST.in
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1265 2023-06-08 04:22:01.928778 pquisby-0.0.3/PKG-INFO
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      940 2023-06-08 04:19:30.000000 pquisby-0.0.3/README.md
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3903 2023-06-08 04:19:30.000000 pquisby-0.0.3/requirements.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)       38 2023-06-08 04:22:01.928778 pquisby-0.0.3/setup.cfg
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      950 2023-06-08 04:22:01.000000 pquisby-0.0.3/setup.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.924778 pquisby-0.0.3/src/
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.925778 pquisby-0.0.3/src/pquisby/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/__init__.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.926778 pquisby-0.0.3/src/pquisby/command/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/command/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      488 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/command/compare_benchmark.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      300 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/command/main.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3382 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/command/process_benchmark.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.927778 pquisby-0.0.3/src/pquisby/lib/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/__init__.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.927778 pquisby-0.0.3/src/pquisby/lib/benchmarks/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/benchmarks/__init__.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.927778 pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1214 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/comparison.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5175 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/graph.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5364 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/uperf.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1655 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/compare_sheets.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.928778 pquisby-0.0.3/src/pquisby/lib/credentials/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/credentials/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1119 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/credentials/creds.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1680 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/post_processing.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.928778 pquisby-0.0.3/src/pquisby/lib/pricing/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/pricing/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     4728 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/pricing/cloud_pricing.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     6775 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/process_result.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.928778 pquisby-0.0.3/src/pquisby/lib/sheet/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/sheet/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5692 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/sheet/sheet_util.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      945 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/sheet/sheetapi.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     2370 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/util.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.926778 pquisby-0.0.3/src/pquisby.egg-info/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1265 2023-06-08 04:22:01.000000 pquisby-0.0.3/src/pquisby.egg-info/PKG-INFO
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1061 2023-06-08 04:22:01.000000 pquisby-0.0.3/src/pquisby.egg-info/SOURCES.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        1 2023-06-08 04:22:01.000000 pquisby-0.0.3/src/pquisby.egg-info/dependency_links.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)       54 2023-06-08 04:22:01.000000 pquisby-0.0.3/src/pquisby.egg-info/entry_points.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1990 2023-06-08 04:22:01.000000 pquisby-0.0.3/src/pquisby.egg-info/requires.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        8 2023-06-08 04:22:01.000000 pquisby-0.0.3/src/pquisby.egg-info/top_level.txt
```

### Comparing `pquisby-0.0.2/LICENSE` & `pquisby-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.2/requirements.txt` & `pquisby-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.2/setup.py` & `pquisby-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 README = (HERE / "README.md").read_text()
 
 # The text of the README file
 REQUIRE = (HERE / "requirements.txt").read_text()
 
 setup(
     name="pquisby",
-    version="0.0.2",
+    version="0.0.3",
     description="Quisby is a data processing and visualization tool for benchmark testing.",
     url = 'https://github.com/sousinha1997/Quisby',
     author = 'Soumya Sinha',
     author_email = 'sinhasoumya97@gmail.com',
     license = 'GPL v3.0',
     packages=find_packages("src"),
     package_dir={"":"src"},
```

### Comparing `pquisby-0.0.2/src/pquisby/command/process_benchmark.py` & `pquisby-0.0.3/src/pquisby/command/process_benchmark.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,88 @@
 import logging
 import os
-
+import shutil
 import click
 from pquisby.lib.process_result import data_handler, extract_data
 from pquisby.lib.util import write_config
 
 
 @click.command()
-@click.option('-l', '--results', help="Results (results_path")
-@click.option('-t', '--test-name', help= "Benchmark test name")
-@click.option('-v', '--os-type', help="Distro")
+@click.option('-l', '--results', help="Results")
+@click.option('-t', '--test-name', help="Test name")
+@click.option('-o', '--os-type', help="Distro")
 @click.option('-v', '--os-version', help="Distro version")
-@click.option('-s', '--system-name', help="Controller Name")
+@click.option('-d', '--dataset-name', help="Dataset Name")
 @click.option('-n', '--spreadsheet-name', help="Any specific spreadsheet name")
 @click.option('-i', '--spreadsheet-id', help="Any specific spreadsheet")
-@click.option('-v', '--cloud', help="cloud/local")
-@click.option('-p', '--platform',help= "platform for processing")
-@click.option('-c', '--config-path',help= "config-path")
-def process_run(results, test_name, os_type, os_version, system_name, spreadsheet_name, spreadsheet_id, cloud, platform, config):
+@click.option('-e', '--environment', help="cloud/localhost")
+@click.option('-p', '--platform', help="platform for processing")
+@click.option('-c', '--config-path', help="config-path")
+@click.option('-it', '--input_type', help="data type for processioning , file/csv/stream ")
+def process_run(results, test_name, os_type, os_version, dataset_name, spreadsheet_name, spreadsheet_id, environment, platform,
+                config, input_type):
     if config:
         config_location = config
     else:
         logging.INFO("No config path found,switching to default location")
-        home_dir = os.getenv("HOME")
-        config_location = home_dir + "/.config/pquisby/config.ini"
+        conf_dir = os.getenv("HOME") + "/.config/pquisby/"
+        config_location = conf_dir + "config.ini"
         if os.path.exists(config_location):
             pass
         else:
-            logging.error("Unable to find config at default location, exiting...")
+            logging.error("Unable to find config at default location, creating...")
+            # Copy the file to the destination directory
+            shutil.copy("pquisby/lib/sample_files/config.ini", conf_dir)
             return
     if results:
         write_config(config_location, "test", "results", results)
     if test_name:
         write_config(config_location, "test", "test_name", test_name)
+    else:
+        return "Test name not provided"
     if os_type:
         write_config(config_location, "test", "os_type", os_type)
+    else:
+        return "OS type not provided"
     if os_version:
         write_config(config_location, "test", "os_version", os_version)
-    if system_name:
-        write_config(config_location, "test", "system_name", system_name)
+    else:
+        return "OS version not provided"
+    if environment:
+        write_config(config_location, "test", "environment", system_name)
+    else:
+        print("Environment not provided. Taking default values..")
+        environment = "baremetal"
+        write_config(config_location, "test", "environment", environment)
+    if dataset_name:
+        write_config(config_location, "test", "dataset_name", dataset_name)
+    else:
+        dataset_name = "test_" +test_name+"_"+environment+"_"+os_type+"_"+os_version
+        write_config(config_location, "test", "dataset_name", dataset_name)
+    if input_type:
+        write_config(config_location, "test", "input_type", input_type)
+    else:
+        input_type = "file"
+        write_config(config_location, "test", "input_type", input_type)
     if spreadsheet_name:
         write_config(config_location, "spreadsheet", "spreadsheet_name", spreadsheet_name)
     if spreadsheet_id:
         write_config(config_location, "spreadsheet", "spreadsheet_id", spreadsheet_id)
-    if cloud:
-        write_config(config_location, "cloud", "cloud_type", cloud)
-    else:
-        write_config(config_location, "cloud", "cloud_type", "baremetal")
+
     if platform == "pbench":
-        ret_val, json_data =extract_data(test_name, system_name, results)
-        if json_data:
-            return json_data
-        else:
-            logging.info("Unable to process data")
-            return None
+        input_type = "stream"
+        json_res = extract_data(test_name, dataset_name, environment, input_type, results)
+        if json_res["jsonData"]:
+            return json_res["jsonData"]
 
     elif platform == "google-doc":
         spreadsheet_id = data_handler(config_location)
 
 
 
 
 
 
-        
+
```

### Comparing `pquisby-0.0.2/src/pquisby/lib/benchmarks/uperf/comparison.py` & `pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/comparison.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.2/src/pquisby/lib/benchmarks/uperf/graph.py` & `pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/graph.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.2/src/pquisby/lib/benchmarks/uperf/uperf.py` & `pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/uperf.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             summary_results.append(
                 [instance_count_data[0], *run_data[instance_count_data[0]]]
             )
 
     return summary_results
 
 
-def extract_uperf_data(system_name,csv_data):
+def extract_uperf_data(dataset_name, system_name,csv_data):
     """"""
     results = []
     data_position = {}
     results_json = {"data": []}
     tests_supported = ["tcp_stream", "tcp_rr", "tcp_bidirec", "tcp_maerts"]
 
     for index, row in enumerate(csv_data[0]):
@@ -95,15 +95,15 @@
                     else:
                         data_dict[key] = [
                             [instance_count, item[data_position[key]]]
                         ]
         test_json = {"vm_name": "", "test_name": "", "metrics_unit": "", "instances": []}
         for key, test_results in data_dict.items():
             if test_results:
-                test_json["vm_name"] = system_name
+                test_json["dataset_name"] = dataset_name
                 test_json["test_name"] = "".join(test_name)
                 test_json["metrics_unit"] = key
                 results.append([""])
                 results.append([system_name])
                 results.append(["".join(test_name)])
                 results.append(["Instance Count", key])
                 for instance_count, items in groupby(test_results, key=lambda x: x[0].split("-")[0]):
```

### Comparing `pquisby-0.0.2/src/pquisby/lib/compare_result.py` & `pquisby-0.0.3/src/pquisby/lib/compare_sheets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import json
 import logging
 import time
-
 from pquisby.lib.sheet.sheet_util import get_sheet, create_spreadsheet
 from pquisby.lib.benchmarks.uperf.comparison import compare_uperf_results
 
-def compare_results(spreadsheet_list,test_name):
+
+def compare_sheets(spreadsheet_list,test_name):
 
     sheet_list = []
     spreadsheet_name = []
     spreadsheets = spreadsheet_list
-    # check if list is passed else conver to list
+    # check if list is passed else convert to list
     if not isinstance(spreadsheets,list):
         spreadsheets = spreadsheets.split(",")
 
     for spreadsheet in spreadsheets:
         sheet_names = []
         sheets = get_sheet(spreadsheet, test_name=test_name)
         spreadsheet_name.append(get_sheet(spreadsheet, test_name=[])["properties"]["title"].strip())
@@ -36,7 +37,11 @@
 
     for index, test_name in enumerate(comparison_list):
         compare_uperf_results(spreadsheets, comp_spreadsheetId, test_name)
         if index + 1 != len(comparison_list):
             logging.info("# Sleeping 10 sec to workaround the Google Sheet per minute API limit")
             time.sleep(10)
     return spreadsheet_name,comp_spreadsheetId
+
+
+
+
```

### Comparing `pquisby-0.0.2/src/pquisby/lib/credentials/creds.py` & `pquisby-0.0.3/src/pquisby/lib/credentials/creds.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.2/src/pquisby/lib/pricing/cloud_pricing.py` & `pquisby-0.0.3/src/pquisby/lib/pricing/cloud_pricing.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.2/src/pquisby/lib/process_result.py` & `pquisby-0.0.3/src/pquisby/lib/process_result.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import fileinput
 import json
 import logging
 import os.path
-import requests
-import csv
-from pquisby.lib.benchmarks.uperf.uperf import extract_uperf_data
 from pquisby.lib.util import read_config
-
 from pquisby.lib.sheet.sheet_util import (create_sheet, append_to_sheet, create_spreadsheet, delete_sheet_content)
 from pquisby.lib.benchmarks.uperf.uperf import create_summary_uperf_data
 from pquisby.lib.benchmarks.uperf.graph import graph_uperf_data
 from pquisby.lib.benchmarks.uperf.comparison import compare_uperf_results
+from pquisby.lib.post_processing import extract_data
 
 
 def process_results(results, test_name, cloud, os_type, os_version, spreadsheet_name, spreadsheet_id):
     # Create spreadsheet if it doesn't exist, otherwise delete old records
     if not spreadsheet_name:
         spreadsheet_name = test_name + "-" + cloud + "-" + os_type + "-" + os_version
     if not spreadsheet_id:
@@ -45,52 +42,56 @@
         logging.error("Error graphing " + str(test_name) + " data")
         return
     return spreadsheet_name, spreadsheet_id
 
 
 def register_details_json(spreadsheet_name, spreadsheet_id):
     home_dir = os.getenv("HOME")
-    filename = home_dir+ "/charts.json"
+    filename = home_dir + "/pquisby/charts.json"
     if not os.path.exists(filename):
         data = {"chartlist": {spreadsheet_name: spreadsheet_id}}
         with open(filename, "w") as f:
             json.dump(data, f)
     else:
         with open(filename, "r") as f:
             data = json.load(f)
         data["chartlist"][spreadsheet_name] = spreadsheet_id
         with open(filename, "w") as f:
             json.dump(data, f)
 
+
 def check_if_chart_exists(test_name):
     home_dir = os.getenv("HOME")
     filename = os.path.join(home_dir, "/pquisby/charts.json")
     if not os.path.exists(filename):
         return ""
     else:
         with open(filename, "r") as f:
             data = json.load(f)
         try:
             id = data["chartlist"][test_name]
         except KeyError:
             return ""
         return id
 
+
 def data_handler(config_location):
     global test_name
     global source
     global count
     results = []
     print(config_location)
-    cloud = read_config(config_location, 'cloud', 'cloud')
+    environment = read_config(config_location, 'test', 'environment')
     os_type = read_config(config_location, 'test', 'os_type')
     os_version = read_config(config_location, 'test', 'os_version')
     spreadsheet_name = read_config(config_location, 'spreadsheet', 'spreadsheet_name')
     spreadsheet_id = read_config(config_location, 'spreadsheet', 'spreadsheet_id')
     results_path = read_config(config_location, 'test', 'results')
+    input_type = read_config(config_location, 'test', 'input_type')
+    dataset_name = read_config(config_location, 'test', 'dataset_name')
     test_path = results_path.strip(results_path.split("/")[-1])
 
     if not spreadsheet_id:
         spreadsheet_id = ""
 
     for line in fileinput.FileInput(results_path, inplace=1):
         if line.rstrip():
@@ -98,54 +99,42 @@
 
     with open(results_path) as file:
         test_result_path = file.readlines()
 
         for data in test_result_path:
             if "test " in data:
                 if results:
-                    spreadsheet_name, spreadsheet_id = process_results(results, test_name, cloud, os_type, os_version, spreadsheet_name,
-                                                     spreadsheet_id)
+                    spreadsheet_name, spreadsheet_id = process_results(results, test_name, cloud, os_type, os_version,
+                                                                       spreadsheet_name,
+                                                                       spreadsheet_id)
                 results = []
                 test_name = data.replace("test ", "").replace("results_", "").replace(".csv", "").strip()
                 source = data.split()[-1].split("_")[0].strip()
             else:
                 try:
                     if test_name == "fio_run":
                         data = data.strip("\n").strip("'").strip()
                         path, system_name = (data.split(",")[0] + "," + data.split(",")[1]), data.split(",")[-1]
                         path = path.replace(os.path.basename(path), "")
                     else:
                         data = data.strip("\n").strip("'")
                         path, system_name = data.split(",")
-                    path = test_path + "/" + path.strip()
-                    try:
-                        csv_data = requests.get(path)
-                        csv_reader = list(csv.reader(csv_data.text.split("\n")))
-                    except Exception:
-                        with open(path) as csv_file:
-                            csv_data = list(csv.reader(csv_file))
-
-                    ret_val, json_data = extract_data(test_name, system_name, csv_data)
-                    if ret_val:
-                        results += ret_val
+                    csv_path = test_path + "/" + path.strip()
+                    json_res = extract_data(test_name,dataset_name, system_name, input_type, csv_path)
+                    if json_res["csvData"]:
+                        results += json_res["csvData"]
                 except ValueError as exc:
                     logging.error(str(exc))
                     continue
         try:
-            spreadsheet_name, spreadsheet_id = process_results(results, test_name, cloud, os_type, os_version, spreadsheet_name,
-                                             spreadsheet_id)
+            spreadsheet_name, spreadsheet_id = process_results(results, test_name, cloud, os_type, os_version,spreadsheet_name,spreadsheet_id)
         except Exception as exc:
-            logging.error(str(exc))
-            pass
+            exception_type = type(exc)
+            return {"status": "failed", "Exception": str(exc), "Exception_type": exception_type}
         print(f"https://docs.google.com/spreadsheets/d/{spreadsheet_id}")
         register_details_json(spreadsheet_name, spreadsheet_id)
         return spreadsheet_id
 
 
-def extract_data(test_name, system_name, csv_data):
-    ret_val = []
-    json_data = {}
-    if test_name == "uperf":
-        ret_val, json_data = extract_uperf_data(system_name, csv_data)
-    else:
-        pass
-    return ret_val, json_data
+
+# if __name__ == '__main__':
+#    extract_data("uperf","localhost",[['iteration_number', 'iteration_name', 'Gb_sec:client_hostname:127.0.0.1-server_hostname:192.168.122.142-server_port:20010', 'Gb_sec:client_hostname:all-server_hostname:all-server_port:all', 'trans_sec:client_hostname:127.0.0.1-server_hostname:192.168.122.142-server_port:20010', 'trans_sec:client_hostname:all-server_hostname:all-server_port:all', 'usec:client_hostname:127.0.0.1-server_hostname:192.168.122.142-server_port:20010', 'usec:client_hostname:all-server_hostname:all-server_port:all'], ['1', 'tcp_stream-65535B-1i', ' 0.0010', ' 0.0010', '', '', '', '', ''], ['2', 'tcp_maerts-65535B-1i', ' 1.1396', ' 1.1396', '', '', '', '', ''], ['3', 'tcp_bidirec-65535B-1i', ' 0.8890', ' 0.8890', '', '', '', '', ''], ['4', 'tcp_rr-65535B-1i', '', '', ' 1.8146', ' 1.8146', ' 592316.6667', ' 592316.6667', ''], ['5', 'udp_stream-65535B-1i', '', '', '', '', '', '', ''], ['6', 'udp_maerts-65535B-1i', '', '', '', '', '', '', ''], ['7', 'udp_bidirec-65535B-1i', '', '', '', '', '', '', ''], ['8', 'udp_rr-65535B-1i', '', '', '', '', '', '', ''], []])
```

### Comparing `pquisby-0.0.2/src/pquisby/lib/sheet/sheet_util.py` & `pquisby-0.0.3/src/pquisby/lib/sheet/sheet_util.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.2/src/pquisby/lib/sheet/sheetapi.py` & `pquisby-0.0.3/src/pquisby/lib/sheet/sheetapi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 from googleapiclient.discovery import build
 from google.oauth2 import service_account
 
 import os
 
 config_dir = os.path.join(os.path.expanduser('~'), '.config/pquisby/')
-SCOPES=['https://www.googleapis.com/auth/spreadsheets', 'https://www.googleapis.com/auth/spreadsheets.readonly','https://www.googleapis.com/auth/drive']
+SCOPES = ['https://www.googleapis.com/auth/spreadsheets', 'https://www.googleapis.com/auth/spreadsheets.readonly',
+          'https://www.googleapis.com/auth/drive']
 SERVICE_ACCOUNT_FILE = os.path.join(config_dir, 'credentials.json')
 DISCOVERY_SERVICE_URL = 'https://sheets.googleapis.com/$discovery/rest?version=v4'
-creds = service_account.Credentials.from_service_account_file(SERVICE_ACCOUNT_FILE, scopes=SCOPES)
-service = build("sheets", "v4", credentials=creds,discoveryServiceUrl=DISCOVERY_SERVICE_URL)
-drive_service = build("drive", "v3", credentials = creds)
-sheet = service.spreadsheets()
-file = drive_service.files()
+creds = None
+sheet = None
+file = None
+
+def get_cred_file(SERVICE_ACCOUNT_FILE):
+    global creds
+    global sheet
+    global file
+    creds = service_account.Credentials.from_service_account_file(SERVICE_ACCOUNT_FILE, scopes=SCOPES)
+    service = build("sheets", "v4", credentials=creds, discoveryServiceUrl=DISCOVERY_SERVICE_URL)
+    drive_service = build("drive", "v3", credentials=creds)
+    sheet = service.spreadsheets()
+    file = drive_service.files()
```

### Comparing `pquisby-0.0.2/src/pquisby/lib/util.py` & `pquisby-0.0.3/src/pquisby/lib/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 import re
 from configparser import ConfigParser
+
 invalid_compare_list = ["pig"]
 
+
 def process_instance(instance_name, *args):
     pattern = r"(?P<family>\D+)(?P<size>\d+)"
     regex_match = re.match(pattern, instance_name, flags=re.IGNORECASE)
     if "size" in args:
         return regex_match.group(2)
     else:
         return regex_match.group(1)
 
 
+def stream_to_csv(data):
+    split_rows = data.split("\n")
+    csv_data = []
+    for row in split_rows:
+        csv_data.append(row.split(","))
+    return csv_data
+
+
 def mk_int(string):
     if string:
         string = string.strip()
         return int(string) if string else 1
     else:
         return 1
 
+
 def create_parser():
     configur = ConfigParser()
     return configur
 
 def read_config(config_path,section,key):
     configur=create_parser()
     with open(config_path) as configfile:
@@ -61,15 +72,15 @@
 
     for lindex, item1 in enumerate(value[0][1:]):
         for rindex, item2 in enumerate(ele[0][1:]):
             if item1.split("-", 1)[0] == item2.split("-", 1)[0]:
                 indexer.append([lindex, rindex])
             elif test_name in invalid_compare_list:
                 indexer.append([lindex, rindex])
- 
+
     for list1, list2 in zip(value, ele):
         holder_list = []
         holder_list.append(list1[0])
 
         for index in indexer:
             holder_list.append(list1[index[0] + 1])
             holder_list.append(list2[index[1] + 1])
```

### Comparing `pquisby-0.0.2/src/pquisby.egg-info/SOURCES.txt` & `pquisby-0.0.3/src/pquisby.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 src/pquisby.egg-info/requires.txt
 src/pquisby.egg-info/top_level.txt
 src/pquisby/command/__init__.py
 src/pquisby/command/compare_benchmark.py
 src/pquisby/command/main.py
 src/pquisby/command/process_benchmark.py
 src/pquisby/lib/__init__.py
-src/pquisby/lib/compare_result.py
-src/pquisby/lib/get_data.py
+src/pquisby/lib/compare_sheets.py
+src/pquisby/lib/post_processing.py
 src/pquisby/lib/process_result.py
 src/pquisby/lib/util.py
 src/pquisby/lib/benchmarks/__init__.py
 src/pquisby/lib/benchmarks/uperf/__init__.py
 src/pquisby/lib/benchmarks/uperf/comparison.py
 src/pquisby/lib/benchmarks/uperf/graph.py
 src/pquisby/lib/benchmarks/uperf/uperf.py
```

### Comparing `pquisby-0.0.2/src/pquisby.egg-info/requires.txt` & `pquisby-0.0.3/src/pquisby.egg-info/requires.txt`

 * *Files identical despite different names*

