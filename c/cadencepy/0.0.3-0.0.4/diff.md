# Comparing `tmp/cadencepy-0.0.3.tar.gz` & `tmp/cadencepy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cadencepy-0.0.3.tar", last modified: Thu Jun  8 16:12:49 2023, max compression
+gzip compressed data, was "dist/cadencepy-0.0.4.tar", last modified: Thu Jun  8 16:17:08 2023, max compression
```

## Comparing `cadencepy-0.0.3.tar` & `cadencepy-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 16:12:49.000000 cadencepy-0.0.3/
-drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 16:12:49.000000 cadencepy-0.0.3/cadencepy.egg-info/
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      495 2023-06-08 16:12:49.000000 cadencepy-0.0.3/cadencepy.egg-info/PKG-INFO
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      246 2023-06-08 16:12:49.000000 cadencepy-0.0.3/cadencepy.egg-info/SOURCES.txt
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        1 2023-06-08 16:12:49.000000 cadencepy-0.0.3/cadencepy.egg-info/dependency_links.txt
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       15 2023-06-08 16:12:49.000000 cadencepy-0.0.3/cadencepy.egg-info/requires.txt
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       10 2023-06-08 16:12:49.000000 cadencepy-0.0.3/cadencepy.egg-info/top_level.txt
-drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 16:12:49.000000 cadencepy-0.0.3/pycadence/
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 14:36:21.000000 cadencepy-0.0.3/pycadence/__init__.py
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)     1572 2023-06-08 16:11:21.000000 cadencepy-0.0.3/pycadence/pycadence.py
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      814 2023-06-08 14:32:37.000000 cadencepy-0.0.3/pycadence/utils.py
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 14:43:55.000000 cadencepy-0.0.3/README.md
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      734 2023-06-08 16:12:35.000000 cadencepy-0.0.3/setup.py
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      495 2023-06-08 16:12:49.000000 cadencepy-0.0.3/PKG-INFO
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       38 2023-06-08 16:12:49.000000 cadencepy-0.0.3/setup.cfg
+drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 16:17:08.000000 cadencepy-0.0.4/
+drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 16:17:08.000000 cadencepy-0.0.4/cadencepy.egg-info/
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      495 2023-06-08 16:17:08.000000 cadencepy-0.0.4/cadencepy.egg-info/PKG-INFO
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      246 2023-06-08 16:17:08.000000 cadencepy-0.0.4/cadencepy.egg-info/SOURCES.txt
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        1 2023-06-08 16:17:08.000000 cadencepy-0.0.4/cadencepy.egg-info/dependency_links.txt
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       15 2023-06-08 16:17:08.000000 cadencepy-0.0.4/cadencepy.egg-info/requires.txt
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       10 2023-06-08 16:17:08.000000 cadencepy-0.0.4/cadencepy.egg-info/top_level.txt
+drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 16:17:08.000000 cadencepy-0.0.4/pycadence/
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 14:36:21.000000 cadencepy-0.0.4/pycadence/__init__.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)     1610 2023-06-08 16:15:56.000000 cadencepy-0.0.4/pycadence/pycadence.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      814 2023-06-08 14:32:37.000000 cadencepy-0.0.4/pycadence/utils.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 14:43:55.000000 cadencepy-0.0.4/README.md
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      734 2023-06-08 16:17:06.000000 cadencepy-0.0.4/setup.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      495 2023-06-08 16:17:08.000000 cadencepy-0.0.4/PKG-INFO
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       38 2023-06-08 16:17:08.000000 cadencepy-0.0.4/setup.cfg
```

### Comparing `cadencepy-0.0.3/pycadence/pycadence.py` & `cadencepy-0.0.4/pycadence/pycadence.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,20 +25,20 @@
             except Exception as e:
                 # print("Error in reading output file")
                 # print(e)
                 pass
         data = np.array(data)
     return data
 
-def simulate(x,default, init_file_path, output_file_path="simulation.ocn", output_log_path="output.txt"):
+def simulate(x,default, init_file_path, output_file_path="simulation.ocn", output_log_path="output.txt", read_output=read_output):
     sim_status_log_path = "sim_status.txt"
     generate_ocn_script(x,default, init_file_path, output_file_path, output_log_path)
     if os.path.exists(sim_status_log_path):
         os.remove(sim_status_log_path)
-    subprocess.call(["./ocean_simulation.sh", output_file_path])
+    subprocess.call(["sh",dir_path+"/ocean_simulation.sh", output_file_path])
     # read output file
     # if time in dead loop exceeds 10minutes system will kill the simulation
     start_time = time.time()
     while not os.path.exists(sim_status_log_path):
         if time.time() - start_time > 120:
             print("Simulation time out!")
             break
```

### Comparing `cadencepy-0.0.3/pycadence/utils.py` & `cadencepy-0.0.4/pycadence/utils.py`

 * *Files identical despite different names*

### Comparing `cadencepy-0.0.3/setup.py` & `cadencepy-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readall(path):
     with open(path) as fp:
         return fp.read()
 
 setup(
     name="cadencepy",
-    version="0.0.3",
+    version="0.0.4",
     author="joetho786",
     author_email="thomas.2@iitj.ac.in",
     description="A python SDK for running simulation and reading data from Ocean Cadence",
     long_description=readall("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/user/reponame",
     packages=find_packages(),
```

