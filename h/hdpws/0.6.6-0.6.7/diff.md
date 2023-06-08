# Comparing `tmp/hdpws-0.6.6.tar.gz` & `tmp/hdpws-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdpws-0.6.6.tar", last modified: Tue Jun  6 11:33:05 2023, max compression
+gzip compressed data, was "hdpws-0.6.7.tar", last modified: Wed Jun  7 15:39:08 2023, max compression
```

## Comparing `hdpws-0.6.6.tar` & `hdpws-0.6.7.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwx------   0 btharris (971688066) staff       (20)        0 2023-06-06 11:33:05.362469 hdpws-0.6.6/
--rw-------   0 btharris (971688066) staff       (20)    12589 2023-02-22 18:33:31.000000 hdpws-0.6.6/LICENSE
--rw-------   0 btharris (971688066) staff       (20)     3453 2023-06-06 11:33:05.362145 hdpws-0.6.6/PKG-INFO
--rw-------   0 btharris (971688066) staff       (20)     2467 2023-04-20 10:54:35.000000 hdpws-0.6.6/README.md
-drwx------   0 btharris (971688066) staff       (20)        0 2023-06-06 11:33:05.359229 hdpws-0.6.6/hdpws/
--rwx------   0 btharris (971688066) staff       (20)     2048 2023-06-05 18:50:40.000000 hdpws-0.6.6/hdpws/__init__.py
--rwx------   0 btharris (971688066) staff       (20)    13440 2023-06-05 18:48:54.000000 hdpws-0.6.6/hdpws/__main__.py
--rw-------   0 btharris (971688066) staff       (20)     4901 2023-02-27 14:08:19.000000 hdpws-0.6.6/hdpws/dateinterval.py
--rwx------   0 btharris (971688066) staff       (20)    32132 2023-06-05 18:49:35.000000 hdpws-0.6.6/hdpws/hdpws.py
--rwx------   0 btharris (971688066) staff       (20)     1745 2023-03-21 11:12:21.000000 hdpws-0.6.6/hdpws/resourcetype.py
-drwx------   0 btharris (971688066) staff       (20)        0 2023-06-06 11:33:05.361636 hdpws-0.6.6/hdpws.egg-info/
--rw-------   0 btharris (971688066) staff       (20)     3453 2023-06-06 11:33:05.000000 hdpws-0.6.6/hdpws.egg-info/PKG-INFO
--rw-------   0 btharris (971688066) staff       (20)      265 2023-06-06 11:33:05.000000 hdpws-0.6.6/hdpws.egg-info/SOURCES.txt
--rw-------   0 btharris (971688066) staff       (20)        1 2023-06-06 11:33:05.000000 hdpws-0.6.6/hdpws.egg-info/dependency_links.txt
--rw-------   0 btharris (971688066) staff       (20)       38 2023-06-06 11:33:05.000000 hdpws-0.6.6/hdpws.egg-info/requires.txt
--rw-------   0 btharris (971688066) staff       (20)        6 2023-06-06 11:33:05.000000 hdpws-0.6.6/hdpws.egg-info/top_level.txt
--rw-------   0 btharris (971688066) staff       (20)       38 2023-06-06 11:33:05.362578 hdpws-0.6.6/setup.cfg
--rw-------   0 btharris (971688066) staff       (20)     1742 2023-06-05 18:50:59.000000 hdpws-0.6.6/setup.py
+drwx------   0 btharris (971688066) staff       (20)        0 2023-06-07 15:39:08.131962 hdpws-0.6.7/
+-rw-------   0 btharris (971688066) staff       (20)    12589 2023-02-22 18:33:31.000000 hdpws-0.6.7/LICENSE
+-rw-------   0 btharris (971688066) staff       (20)     3453 2023-06-07 15:39:08.131652 hdpws-0.6.7/PKG-INFO
+-rw-------   0 btharris (971688066) staff       (20)     2467 2023-04-20 10:54:35.000000 hdpws-0.6.7/README.md
+drwx------   0 btharris (971688066) staff       (20)        0 2023-06-07 15:39:08.128902 hdpws-0.6.7/hdpws/
+-rwx------   0 btharris (971688066) staff       (20)     2048 2023-06-07 12:00:23.000000 hdpws-0.6.7/hdpws/__init__.py
+-rwx------   0 btharris (971688066) staff       (20)    13440 2023-06-05 18:48:54.000000 hdpws-0.6.7/hdpws/__main__.py
+-rw-------   0 btharris (971688066) staff       (20)     4901 2023-02-27 14:08:19.000000 hdpws-0.6.7/hdpws/dateinterval.py
+-rwx------   0 btharris (971688066) staff       (20)    32132 2023-06-05 18:49:35.000000 hdpws-0.6.7/hdpws/hdpws.py
+-rwx------   0 btharris (971688066) staff       (20)     1745 2023-03-21 11:12:21.000000 hdpws-0.6.7/hdpws/resourcetype.py
+-rw-------   0 btharris (971688066) staff       (20)    14038 2023-06-07 15:29:38.000000 hdpws-0.6.7/hdpws/spase.py
+drwx------   0 btharris (971688066) staff       (20)        0 2023-06-07 15:39:08.131182 hdpws-0.6.7/hdpws.egg-info/
+-rw-------   0 btharris (971688066) staff       (20)     3453 2023-06-07 15:39:08.000000 hdpws-0.6.7/hdpws.egg-info/PKG-INFO
+-rw-------   0 btharris (971688066) staff       (20)      280 2023-06-07 15:39:08.000000 hdpws-0.6.7/hdpws.egg-info/SOURCES.txt
+-rw-------   0 btharris (971688066) staff       (20)        1 2023-06-07 15:39:08.000000 hdpws-0.6.7/hdpws.egg-info/dependency_links.txt
+-rw-------   0 btharris (971688066) staff       (20)       55 2023-06-07 15:39:08.000000 hdpws-0.6.7/hdpws.egg-info/requires.txt
+-rw-------   0 btharris (971688066) staff       (20)        6 2023-06-07 15:39:08.000000 hdpws-0.6.7/hdpws.egg-info/top_level.txt
+-rw-------   0 btharris (971688066) staff       (20)       38 2023-06-07 15:39:08.132075 hdpws-0.6.7/setup.cfg
+-rw-------   0 btharris (971688066) staff       (20)     1762 2023-06-07 11:59:37.000000 hdpws-0.6.7/setup.py
```

### Comparing `hdpws-0.6.6/LICENSE` & `hdpws-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hdpws-0.6.6/PKG-INFO` & `hdpws-0.6.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdpws
-Version: 0.6.6
+Version: 0.6.7
 Summary: NASA's Heliophysics Data Portal Web Service Client Library
 Home-page: https://heliophysicsdata.gsfc.nasa.gov/WebServices
 Author: Bernie Harris
 Author-email: NASA-SPDF-Support@nasa.onmicrosoft.com
 License: NOSA
 Keywords: heliophysics,spase,space physics,spdf,hdp
 Platform: UNKNOWN
```

### Comparing `hdpws-0.6.6/README.md` & `hdpws-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `hdpws-0.6.6/hdpws/__init__.py` & `hdpws-0.6.7/hdpws/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 Copyright &copy; 2023 United States Government as represented by the
 National Aeronautics and Space Administration. No copyright is claimed in
 the United States under Title 17, U.S.Code. All Other Rights Reserved.
 
 """
 
 
-__version__ = "0.6.6"
+__version__ = "0.6.7"
 
 
 #
 # Limit on the number of times an HTTP request which returns a
 # 429 or 503 status with a Retry-After header will be retried.
 #
 #RETRY_LIMIT = 100
```

### Comparing `hdpws-0.6.6/hdpws/__main__.py` & `hdpws-0.6.7/hdpws/__main__.py`

 * *Files identical despite different names*

### Comparing `hdpws-0.6.6/hdpws/dateinterval.py` & `hdpws-0.6.7/hdpws/dateinterval.py`

 * *Files identical despite different names*

### Comparing `hdpws-0.6.6/hdpws/hdpws.py` & `hdpws-0.6.7/hdpws/hdpws.py`

 * *Files identical despite different names*

### Comparing `hdpws-0.6.6/hdpws/resourcetype.py` & `hdpws-0.6.7/hdpws/resourcetype.py`

 * *Files identical despite different names*

### Comparing `hdpws-0.6.6/hdpws.egg-info/PKG-INFO` & `hdpws-0.6.7/hdpws.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdpws
-Version: 0.6.6
+Version: 0.6.7
 Summary: NASA's Heliophysics Data Portal Web Service Client Library
 Home-page: https://heliophysicsdata.gsfc.nasa.gov/WebServices
 Author: Bernie Harris
 Author-email: NASA-SPDF-Support@nasa.onmicrosoft.com
 License: NOSA
 Keywords: heliophysics,spase,space physics,spdf,hdp
 Platform: UNKNOWN
```

### Comparing `hdpws-0.6.6/setup.py` & `hdpws-0.6.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="hdpws",
-    version="0.6.6",
+    version="0.6.7",
     description="NASA's Heliophysics Data Portal Web Service Client Library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://heliophysicsdata.gsfc.nasa.gov/WebServices",
     author="Bernie Harris",
     author_email="NASA-SPDF-Support@nasa.onmicrosoft.com",
     license="NOSA",
     packages=["hdpws"],
 #    packages=find_packages(exclude=["tests"]),
 #    packages=find_packages(),
     include_package_data=True,
-    install_requires=["python-dateutil>=2.8.0", "requests>=2.20"],
+    install_requires=["python-dateutil>=2.8.0", "requests>=2.20", "urllib3>=1.26.14"],
 #    extras_require={
 #        'plot': ["matplotlib>=3.3.2"],
 #    },
     keywords=["heliophysics", "spase", "space physics", "spdf", "hdp"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
```

