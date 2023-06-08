# Comparing `tmp/dedscumulus-0.1.1.tar.gz` & `tmp/dedscumulus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dedscumulus-0.1.1.tar", last modified: Mon May 15 11:08:35 2023, max compression
+gzip compressed data, was "dedscumulus-0.1.2.tar", last modified: Thu Jun  8 19:36:38 2023, max compression
```

## Comparing `dedscumulus-0.1.1.tar` & `dedscumulus-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 11:08:35.938595 dedscumulus-0.1.1/
--rw-rw-rw-   0        0        0     1091 2023-04-20 20:25:57.000000 dedscumulus-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      566 2023-05-15 11:08:35.939155 dedscumulus-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-04-21 00:56:16.000000 dedscumulus-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 11:08:35.908651 dedscumulus-0.1.1/dedscumulus/
--rw-rw-rw-   0        0        0      465 2023-04-21 13:58:35.000000 dedscumulus-0.1.1/dedscumulus/RequestHandler.py
--rw-rw-rw-   0        0        0    14284 2023-04-25 13:13:55.000000 dedscumulus-0.1.1/dedscumulus/SharePointHandler.py
--rw-rw-rw-   0        0        0     2250 2023-02-20 20:06:50.000000 dedscumulus-0.1.1/dedscumulus/TableLogHandler.py
--rw-rw-rw-   0        0        0        0 2022-05-17 10:12:58.000000 dedscumulus-0.1.1/dedscumulus/__init__.py
--rw-rw-rw-   0        0        0     8815 2023-02-21 02:51:22.000000 dedscumulus-0.1.1/dedscumulus/brzGlobal.py
--rw-rw-rw-   0        0        0     5689 2023-04-25 11:57:59.000000 dedscumulus-0.1.1/dedscumulus/gbtGlobal.py
--rw-rw-rw-   0        0        0    14664 2023-05-15 11:03:56.000000 dedscumulus-0.1.1/dedscumulus/mstAst.py
--rw-rw-rw-   0        0        0      824 2023-04-21 13:55:52.000000 dedscumulus-0.1.1/dedscumulus/mstLog.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:08:35.936595 dedscumulus-0.1.1/dedscumulus.egg-info/
--rw-rw-rw-   0        0        0      566 2023-05-15 11:08:35.000000 dedscumulus-0.1.1/dedscumulus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-05-15 11:08:35.000000 dedscumulus-0.1.1/dedscumulus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 11:08:35.000000 dedscumulus-0.1.1/dedscumulus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-15 11:08:35.000000 dedscumulus-0.1.1/dedscumulus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      235 2023-04-21 01:29:23.000000 dedscumulus-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      593 2023-05-15 11:08:35.941381 dedscumulus-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      661 2023-05-15 11:04:45.000000 dedscumulus-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:36:38.595858 dedscumulus-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-20 20:25:57.000000 dedscumulus-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      566 2023-06-08 19:36:38.596859 dedscumulus-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-04-21 00:56:16.000000 dedscumulus-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 19:36:38.549133 dedscumulus-0.1.2/dedscumulus/
+-rw-rw-rw-   0        0        0      465 2023-04-21 13:58:35.000000 dedscumulus-0.1.2/dedscumulus/RequestHandler.py
+-rw-rw-rw-   0        0        0    14284 2023-04-25 13:13:55.000000 dedscumulus-0.1.2/dedscumulus/SharePointHandler.py
+-rw-rw-rw-   0        0        0     2250 2023-02-20 20:06:50.000000 dedscumulus-0.1.2/dedscumulus/TableLogHandler.py
+-rw-rw-rw-   0        0        0        0 2022-05-17 10:12:58.000000 dedscumulus-0.1.2/dedscumulus/__init__.py
+-rw-rw-rw-   0        0        0     8815 2023-02-21 02:51:22.000000 dedscumulus-0.1.2/dedscumulus/brzGlobal.py
+-rw-rw-rw-   0        0        0     6485 2023-06-08 19:34:55.000000 dedscumulus-0.1.2/dedscumulus/gbtGlobal.py
+-rw-rw-rw-   0        0        0    14664 2023-05-15 11:03:56.000000 dedscumulus-0.1.2/dedscumulus/mstAst.py
+-rw-rw-rw-   0        0        0      824 2023-04-21 13:55:52.000000 dedscumulus-0.1.2/dedscumulus/mstLog.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:36:38.584086 dedscumulus-0.1.2/dedscumulus.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-06-08 19:36:38.000000 dedscumulus-0.1.2/dedscumulus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-06-08 19:36:38.000000 dedscumulus-0.1.2/dedscumulus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 19:36:38.000000 dedscumulus-0.1.2/dedscumulus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-08 19:36:38.000000 dedscumulus-0.1.2/dedscumulus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-04-21 01:29:23.000000 dedscumulus-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      593 2023-06-08 19:36:38.601193 dedscumulus-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      661 2023-06-08 19:35:53.000000 dedscumulus-0.1.2/setup.py
```

### Comparing `dedscumulus-0.1.1/LICENSE` & `dedscumulus-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.1.1/PKG-INFO` & `dedscumulus-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dedscumulus
-Version: 0.1.1
+Version: 0.1.2
 Summary: Kernel functions for Cumulus
 Home-page: https://github.com/nino-baywa/dedscumulus
 Author: BayWa r.e. Data Services GmbH
 Author-email: no-reply@baywa-re.com
 License: UNKNOWN
 Project-URL: repository, https://github.com/nino-baywa/dedscumulus
 Platform: UNKNOWN
```

### Comparing `dedscumulus-0.1.1/dedscumulus/SharePointHandler.py` & `dedscumulus-0.1.2/dedscumulus/SharePointHandler.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.1.1/dedscumulus/TableLogHandler.py` & `dedscumulus-0.1.2/dedscumulus/TableLogHandler.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.1.1/dedscumulus/brzGlobal.py` & `dedscumulus-0.1.2/dedscumulus/brzGlobal.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.1.1/dedscumulus/gbtGlobal.py` & `dedscumulus-0.1.2/dedscumulus/gbtGlobal.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,19 +71,28 @@
                     LOGGER.warning(f"WARNING: get_devices from Breeze not received, error: "+str(ge))
                 return None
             
 def getTasks(greenbyte_client,QUERY_PARAMS,LOGGER):
     tries=0
     while tries<3:
         try:
-            return greenbyte_client.plan.list_tasks(QUERY_PARAMS['timestampStart'],QUERY_PARAMS['timestampFinish'],
-                        #device_ids=self.turbines,
-                        site_ids=QUERY_PARAMS['sites'],
-                        category_ids=QUERY_PARAMS['categoryIds'],
-                        state=None,fields=None,page_size=QUERY_PARAMS['pageSize'],page=QUERY_PARAMS['page'],use_utc=False)
+            if QUERY_PARAMS['turbines'] is not None:
+                return greenbyte_client.plan.list_tasks(QUERY_PARAMS['timestampStart'],QUERY_PARAMS['timestampFinish'],
+                            device_ids=QUERY_PARAMS['turbines'],
+                            category_ids=QUERY_PARAMS['categoryIds'],
+                            state=None,fields=None,page_size=QUERY_PARAMS['pageSize'],page=QUERY_PARAMS['page'],use_utc=False)
+            elif QUERY_PARAMS['sites'] is not None:
+                return greenbyte_client.plan.list_tasks(QUERY_PARAMS['timestampStart'],QUERY_PARAMS['timestampFinish'],
+                            site_ids=QUERY_PARAMS['sites'],
+                            category_ids=QUERY_PARAMS['categoryIds'],
+                            state=None,fields=None,page_size=QUERY_PARAMS['pageSize'],page=QUERY_PARAMS['page'],use_utc=False)
+            else:
+                return greenbyte_client.plan.list_tasks(QUERY_PARAMS['timestampStart'],QUERY_PARAMS['timestampFinish'],
+                            category_ids=QUERY_PARAMS['categoryIds'],
+                            state=None,fields=None,page_size=QUERY_PARAMS['pageSize'],page=QUERY_PARAMS['page'],use_utc=False)
         except Exception as ge:
             tries+=1
             LOGGER.debug(f"WARNING: list_tasks from Breeze not received, try {tries}, error: "+str(ge))
             if tries==3:
                 if  "Read timed out" in str(ge):
                     LOGGER.warning(f"WARNING: list_tasks from Breeze timed out. Full error: "+str(ge))
                 else:
```

### Comparing `dedscumulus-0.1.1/dedscumulus/mstAst.py` & `dedscumulus-0.1.2/dedscumulus/mstAst.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.1.1/dedscumulus/mstLog.py` & `dedscumulus-0.1.2/dedscumulus/mstLog.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.1.1/dedscumulus.egg-info/PKG-INFO` & `dedscumulus-0.1.2/dedscumulus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dedscumulus
-Version: 0.1.1
+Version: 0.1.2
 Summary: Kernel functions for Cumulus
 Home-page: https://github.com/nino-baywa/dedscumulus
 Author: BayWa r.e. Data Services GmbH
 Author-email: no-reply@baywa-re.com
 License: UNKNOWN
 Project-URL: repository, https://github.com/nino-baywa/dedscumulus
 Platform: UNKNOWN
```

### Comparing `dedscumulus-0.1.1/setup.cfg` & `dedscumulus-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6564 7363 756d 756c 7573 0d0a   = dedscumulus..
-00000020: 7665 7273 696f 6e20 3d20 302e 312e 310d  version = 0.1.1.
+00000020: 7665 7273 696f 6e20 3d20 302e 312e 320d  version = 0.1.2.
 00000030: 0a61 7574 686f 7220 3d20 4261 7957 6120  .author = BayWa 
 00000040: 722e 652e 2044 6174 6120 5365 7276 6963  r.e. Data Servic
 00000050: 6573 2047 6d62 480d 0a61 7574 686f 725f  es GmbH..author_
 00000060: 656d 6169 6c20 3d20 6e6f 2d72 6570 6c79  email = no-reply
 00000070: 4062 6179 7761 2d72 652e 636f 6d0d 0a64  @baywa-re.com..d
 00000080: 6573 6372 6970 7469 6f6e 203d 204b 6572  escription = Ker
 00000090: 6e65 6c20 6675 6e63 7469 6f6e 7320 666f  nel functions fo
```

### Comparing `dedscumulus-0.1.1/setup.py` & `dedscumulus-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
      name='dedscumulus',  
-     version='0.1.1',
+     version='0.1.2',
      author="BayWa r.e. Data Services GmbH",
      author_email="no-reply@baywa-re.com",
      description="Kernel functions for Cumulus",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/nino-baywa/dedscumulus",
      classifiers=[
```

