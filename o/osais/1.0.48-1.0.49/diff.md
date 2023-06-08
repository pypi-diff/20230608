# Comparing `tmp/osais-1.0.48.tar.gz` & `tmp/osais-1.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-dvy__r4l\osais-1.0.48.tar", last modified: Wed Jun  7 07:09:52 2023, max compression
+gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-p48s059_\osais-1.0.49.tar", last modified: Thu Jun  8 18:11:50 2023, max compression
```

## Comparing `osais-1.0.48.tar` & `osais-1.0.49.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 07:09:52.242742 osais-1.0.48/
--rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.48/LICENSE
--rw-rw-rw-   0        0        0     1172 2023-06-07 07:09:52.242742 osais-1.0.48/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.48/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 07:09:52.236742 osais-1.0.48/osais/
--rw-rw-rw-   0        0        0     1041 2023-06-07 07:09:17.000000 osais-1.0.48/osais/__init__.py
--rw-rw-rw-   0        0        0    57528 2023-06-07 07:09:02.000000 osais-1.0.48/osais/osais.py
-drwxrwxrwx   0        0        0        0 2023-06-07 07:09:52.241742 osais-1.0.48/osais.egg-info/
--rw-rw-rw-   0        0        0     1172 2023-06-07 07:09:52.000000 osais-1.0.48/osais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-06-07 07:09:52.000000 osais-1.0.48/osais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 07:09:52.000000 osais-1.0.48/osais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-06-07 07:09:52.000000 osais-1.0.48/osais.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-07 07:09:52.000000 osais-1.0.48/osais.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.48/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-07 07:09:52.242742 osais-1.0.48/setup.cfg
--rw-rw-rw-   0        0        0     1208 2023-06-07 07:09:23.000000 osais-1.0.48/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 18:11:50.170300 osais-1.0.49/
+-rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.49/LICENSE
+-rw-rw-rw-   0        0        0     1172 2023-06-08 18:11:50.169295 osais-1.0.49/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.49/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 18:11:50.163561 osais-1.0.49/osais/
+-rw-rw-rw-   0        0        0     1041 2023-06-08 18:11:33.000000 osais-1.0.49/osais/__init__.py
+-rw-rw-rw-   0        0        0    57685 2023-06-08 18:09:41.000000 osais-1.0.49/osais/osais.py
+drwxrwxrwx   0        0        0        0 2023-06-08 18:11:50.167289 osais-1.0.49/osais.egg-info/
+-rw-rw-rw-   0        0        0     1172 2023-06-08 18:11:50.000000 osais-1.0.49/osais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-06-08 18:11:50.000000 osais-1.0.49/osais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 18:11:50.000000 osais-1.0.49/osais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-06-08 18:11:50.000000 osais-1.0.49/osais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-08 18:11:50.000000 osais-1.0.49/osais.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.49/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 18:11:50.170300 osais-1.0.49/setup.cfg
+-rw-rw-rw-   0        0        0     1208 2023-06-08 18:11:39.000000 osais-1.0.49/setup.py
```

### Comparing `osais-1.0.48/LICENSE` & `osais-1.0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `osais-1.0.48/PKG-INFO` & `osais-1.0.49/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.48
+Version: 1.0.49
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.48/osais/__init__.py` & `osais-1.0.49/osais/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 A package for OSAIS virtual AI.
 """
-__version__="1.0.48"
+__version__="1.0.49"
 __author__ = "incubiq"
 __email__ = "eric@incubiq.com"
 
 from .osais import osais_isDebug
 from .osais import osais_isDocker
 from .osais import osais_isLocal
 from .osais import osais_isVirtualAI
```

### Comparing `osais-1.0.48/osais/osais.py` & `osais-1.0.49/osais/osais.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__="1.0.48"
+__version__="1.0.49"
 
 ## ========================================================================
 ## 
 ##                      Utilities starts here 
 ## 
 ## ========================================================================
 
@@ -919,21 +919,27 @@
             "Content-Type": 'application/json', 
             'Accept': 'text/plain',
         }
         response = requests.get(f"{gOriginOSAIS}api/v1/public/user/{gUsername}/gateways", headers=headers)
         objRes=response.json()["data"]
         if objRes is None:
             raise ValueError("could not access OSAIS on "+gOriginOSAIS)
+        
+        if len(objRes)==0:
+            raise ValueError("No Gateway for this AI")
 
         ## take the first gateway and notify
         ## todo later ... maybe we update ALL gateways with this AI? (the AI is a slave of all this user's gatyeways?)
-        gOriginGateway=objRes[0]["domain"]
+        try:
+            gOriginGateway=objRes[0]["location"]
+        except:
+            raise ValueError("Gateway is not started")
 
     except Exception as err:
-        consoleLog({"msg":"could not notify OSAIS on "+gOriginOSAIS})
+        consoleLog({"msg":err.args[0]})
         raise err
 
     try:
         _connectWithGateway()
     except Exception as err:
         consoleLog({"msg":"Could not reset connection to Gateway"})
         raise err
```

### Comparing `osais-1.0.48/osais.egg-info/PKG-INFO` & `osais-1.0.49/osais.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.48
+Version: 1.0.49
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.48/setup.py` & `osais-1.0.49/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='osais',
-    version='1.0.48',
+    version='1.0.49',
     author='incubiq',
     author_email='eric@incubiq.com',
     description='The osais Python lib for connecting AIs to OSAIS cloud',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/incubiq/osais',
     keywords = "osais, opensourceais",
```

