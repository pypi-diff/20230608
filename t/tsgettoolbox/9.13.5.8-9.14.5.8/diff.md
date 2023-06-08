# Comparing `tmp/tsgettoolbox-9.13.5.8.tar.gz` & `tmp/tsgettoolbox-9.14.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tsgettoolbox-9.13.5.8.tar", last modified: Sat Apr 22 00:19:22 2017, max compression
+gzip compressed data, was "dist/tsgettoolbox-9.14.5.8.tar", last modified: Sun Apr 23 16:34:33 2017, max compression
```

## Comparing `tsgettoolbox-9.13.5.8.tar` & `tsgettoolbox-9.14.5.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-04-22 00:19:22.000000 tsgettoolbox-9.13.5.8/
--rw-r--r--   0 tim       (1000) tim       (1000)    10870 2017-02-28 01:04:20.000000 tsgettoolbox-9.13.5.8/README.rst
--rw-r--r--   0 tim       (1000) tim       (1000)    13502 2017-04-22 00:19:22.000000 tsgettoolbox-9.13.5.8/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)       32 2013-09-23 22:32:15.000000 tsgettoolbox-9.13.5.8/AUTHORS.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)       49 2016-09-15 04:42:58.000000 tsgettoolbox-9.13.5.8/pip_requirements.txt
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-04-22 00:19:22.000000 tsgettoolbox-9.13.5.8/tsgettoolbox.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)      887 2017-04-22 00:19:21.000000 tsgettoolbox-9.13.5.8/tsgettoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       49 2017-04-22 00:19:20.000000 tsgettoolbox-9.13.5.8/tsgettoolbox.egg-info/requires.txt
--rw-r--r--   0 tim       (1000) tim       (1000)    13502 2017-04-22 00:19:20.000000 tsgettoolbox-9.13.5.8/tsgettoolbox.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)       47 2016-05-20 13:55:54.000000 tsgettoolbox-9.13.5.8/tsgettoolbox.egg-info/pbr.json
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2013-11-15 04:56:29.000000 tsgettoolbox-9.13.5.8/tsgettoolbox.egg-info/not-zip-safe
--rw-r--r--   0 tim       (1000) tim       (1000)       62 2017-04-22 00:19:20.000000 tsgettoolbox-9.13.5.8/tsgettoolbox.egg-info/top_level.txt
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2017-04-22 00:19:20.000000 tsgettoolbox-9.13.5.8/tsgettoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       65 2017-04-22 00:19:20.000000 tsgettoolbox-9.13.5.8/tsgettoolbox.egg-info/entry_points.txt
--rw-r--r--   0 tim       (1000) tim       (1000)     3097 2013-09-23 22:29:54.000000 tsgettoolbox-9.13.5.8/CONTRIBUTING.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       85 2017-04-22 00:19:22.000000 tsgettoolbox-9.13.5.8/setup.cfg
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-04-22 00:19:22.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2014-04-09 20:10:25.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/__init__.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-04-22 00:19:22.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/services/
--rw-rw-r--   0 tim       (1000) tim       (1000)     5019 2017-02-13 13:56:46.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/services/darksky.py
--rw-rw-r--   0 tim       (1000) tim       (1000)        0 2016-02-13 03:20:45.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/services/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3442 2017-02-13 20:50:51.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/services/unavco.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3901 2017-02-13 14:02:40.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/services/daymet.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3633 2017-02-13 19:38:07.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/services/ndbc.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    11257 2017-04-22 00:08:10.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/services/nwis.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1115 2016-02-25 17:20:14.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/services/ndfd.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-04-22 00:19:22.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/services/ncdc/
--rw-rw-r--   0 tim       (1000) tim       (1000)     6814 2017-02-13 18:05:03.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/services/ncdc/ncdc_cdo.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     9906 2017-02-13 17:41:15.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/services/ncdc/ghcnd_ftp.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    40317 2017-02-13 17:34:55.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/services/modis.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6724 2017-02-13 17:11:37.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/services/ldas.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7473 2017-02-13 13:44:35.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/services/coops.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1369 2017-02-08 21:34:40.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/utils.py
--rw-r--r--   0 tim       (1000) tim       (1000)   494325 2017-04-21 22:35:19.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/tsgettoolbox.py
--rw-r-----   0 tim       (1000) tim       (1000)    23628 2016-04-21 16:06:01.000000 tsgettoolbox-9.13.5.8/tsgettoolbox/appdirs.py
--rw-r--r--   0 tim       (1000) tim       (1000)      134 2013-09-23 22:30:12.000000 tsgettoolbox-9.13.5.8/MANIFEST.in
--rw-r--r--   0 tim       (1000) tim       (1000)     1489 2013-10-25 20:23:16.000000 tsgettoolbox-9.13.5.8/LICENSE.txt
--rw-r--r--   0 tim       (1000) tim       (1000)     2033 2017-02-13 20:55:32.000000 tsgettoolbox-9.13.5.8/setup.py
--rw-r--r--   0 tim       (1000) tim       (1000)        9 2017-04-22 00:17:26.000000 tsgettoolbox-9.13.5.8/VERSION
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-04-23 16:34:33.000000 tsgettoolbox-9.14.5.8/
+-rw-r--r--   0 tim       (1000) tim       (1000)    10870 2017-02-28 01:04:20.000000 tsgettoolbox-9.14.5.8/README.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)    13502 2017-04-23 16:34:33.000000 tsgettoolbox-9.14.5.8/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)       32 2013-09-23 22:32:15.000000 tsgettoolbox-9.14.5.8/AUTHORS.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)       49 2016-09-15 04:42:58.000000 tsgettoolbox-9.14.5.8/pip_requirements.txt
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-04-23 16:34:33.000000 tsgettoolbox-9.14.5.8/tsgettoolbox.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)      887 2017-04-23 16:34:32.000000 tsgettoolbox-9.14.5.8/tsgettoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       49 2017-04-23 16:34:32.000000 tsgettoolbox-9.14.5.8/tsgettoolbox.egg-info/requires.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)    13502 2017-04-23 16:34:32.000000 tsgettoolbox-9.14.5.8/tsgettoolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)       47 2016-05-20 13:55:54.000000 tsgettoolbox-9.14.5.8/tsgettoolbox.egg-info/pbr.json
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2013-11-15 04:56:29.000000 tsgettoolbox-9.14.5.8/tsgettoolbox.egg-info/not-zip-safe
+-rw-r--r--   0 tim       (1000) tim       (1000)       62 2017-04-23 16:34:32.000000 tsgettoolbox-9.14.5.8/tsgettoolbox.egg-info/top_level.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2017-04-23 16:34:32.000000 tsgettoolbox-9.14.5.8/tsgettoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       65 2017-04-23 16:34:32.000000 tsgettoolbox-9.14.5.8/tsgettoolbox.egg-info/entry_points.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)     3097 2013-09-23 22:29:54.000000 tsgettoolbox-9.14.5.8/CONTRIBUTING.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       85 2017-04-23 16:34:33.000000 tsgettoolbox-9.14.5.8/setup.cfg
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-04-23 16:34:33.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2014-04-09 20:10:25.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/__init__.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-04-23 16:34:33.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/services/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5019 2017-02-13 13:56:46.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/services/darksky.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)        0 2016-02-13 03:20:45.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/services/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3442 2017-02-13 20:50:51.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/services/unavco.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3901 2017-02-13 14:02:40.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/services/daymet.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3633 2017-02-13 19:38:07.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/services/ndbc.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    11235 2017-04-23 06:07:55.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/services/nwis.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1115 2016-02-25 17:20:14.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/services/ndfd.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2017-04-23 16:34:33.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/services/ncdc/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6814 2017-02-13 18:05:03.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/services/ncdc/ncdc_cdo.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     9906 2017-02-13 17:41:15.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/services/ncdc/ghcnd_ftp.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    40317 2017-02-13 17:34:55.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/services/modis.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6724 2017-02-13 17:11:37.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/services/ldas.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7473 2017-02-13 13:44:35.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/services/coops.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1369 2017-02-08 21:34:40.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/utils.py
+-rw-r--r--   0 tim       (1000) tim       (1000)   494325 2017-04-23 06:08:26.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/tsgettoolbox.py
+-rw-r-----   0 tim       (1000) tim       (1000)    23628 2016-04-21 16:06:01.000000 tsgettoolbox-9.14.5.8/tsgettoolbox/appdirs.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      134 2013-09-23 22:30:12.000000 tsgettoolbox-9.14.5.8/MANIFEST.in
+-rw-r--r--   0 tim       (1000) tim       (1000)     1489 2013-10-25 20:23:16.000000 tsgettoolbox-9.14.5.8/LICENSE.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)     2033 2017-02-13 20:55:32.000000 tsgettoolbox-9.14.5.8/setup.py
+-rw-r--r--   0 tim       (1000) tim       (1000)        9 2017-04-23 16:32:03.000000 tsgettoolbox-9.14.5.8/VERSION
```

### Comparing `tsgettoolbox-9.13.5.8/README.rst` & `tsgettoolbox-9.14.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/PKG-INFO` & `tsgettoolbox-9.14.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tsgettoolbox
-Version: 9.13.5.8
+Version: 9.14.5.8
 Summary: Will get time series from different sources on the internet.
 Home-page: http://timcera.bitbucket.org/tsgettoolbox/docsrc/index.html
 Author: Tim Cera, P.E.
 Author-email: tim@cerazone.net
 License: UNKNOWN
 Description: .. image:: https://travis-ci.org/timcera/tsgettoolbox.svg?branch=master
             :target: https://travis-ci.org/timcera/tsgettoolbox
```

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox.egg-info/SOURCES.txt` & `tsgettoolbox-9.14.5.8/tsgettoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox.egg-info/PKG-INFO` & `tsgettoolbox-9.14.5.8/tsgettoolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tsgettoolbox
-Version: 9.13.5.8
+Version: 9.14.5.8
 Summary: Will get time series from different sources on the internet.
 Home-page: http://timcera.bitbucket.org/tsgettoolbox/docsrc/index.html
 Author: Tim Cera, P.E.
 Author-email: tim@cerazone.net
 License: UNKNOWN
 Description: .. image:: https://travis-ci.org/timcera/tsgettoolbox.svg?branch=master
             :target: https://travis-ci.org/timcera/tsgettoolbox
```

### Comparing `tsgettoolbox-9.13.5.8/CONTRIBUTING.rst` & `tsgettoolbox-9.14.5.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox/services/darksky.py` & `tsgettoolbox-9.14.5.8/tsgettoolbox/services/darksky.py`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox/services/unavco.py` & `tsgettoolbox-9.14.5.8/tsgettoolbox/services/unavco.py`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox/services/daymet.py` & `tsgettoolbox-9.14.5.8/tsgettoolbox/services/daymet.py`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox/services/ndbc.py` & `tsgettoolbox-9.14.5.8/tsgettoolbox/services/ndbc.py`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox/services/nwis.py` & `tsgettoolbox-9.14.5.8/tsgettoolbox/services/nwis.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,14 @@
 @convert.register(pd.DataFrame, USGS_MEASUREMENTS_PEAK_RDB)
 def usgs_measurements_peak_rdb_to_df(data, **kwargs):
     ndf = _read_rdb(data)
     if 'measurements' in data.url:
         dname = 'measurement_dt'
     elif 'peak' in data.url:
         dname = 'peak_dt'
-    print(ndf[dname])
     ndf['Datetime'] = pd.to_datetime(ndf[dname], errors='coerce')
     ndf.set_index(['Datetime'],
                   inplace=True)
     ndf.drop([dname,
               'agency_cd',
               'site_no'],
              axis=1,
```

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox/services/ndfd.py` & `tsgettoolbox-9.14.5.8/tsgettoolbox/services/ndfd.py`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox/services/ncdc/ncdc_cdo.py` & `tsgettoolbox-9.14.5.8/tsgettoolbox/services/ncdc/ncdc_cdo.py`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox/services/ncdc/ghcnd_ftp.py` & `tsgettoolbox-9.14.5.8/tsgettoolbox/services/ncdc/ghcnd_ftp.py`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox/services/modis.py` & `tsgettoolbox-9.14.5.8/tsgettoolbox/services/modis.py`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox/services/ldas.py` & `tsgettoolbox-9.14.5.8/tsgettoolbox/services/ldas.py`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox/services/coops.py` & `tsgettoolbox-9.14.5.8/tsgettoolbox/services/coops.py`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox/utils.py` & `tsgettoolbox-9.14.5.8/tsgettoolbox/utils.py`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox/tsgettoolbox.py` & `tsgettoolbox-9.14.5.8/tsgettoolbox/tsgettoolbox.py`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/tsgettoolbox/appdirs.py` & `tsgettoolbox-9.14.5.8/tsgettoolbox/appdirs.py`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/LICENSE.txt` & `tsgettoolbox-9.14.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tsgettoolbox-9.13.5.8/setup.py` & `tsgettoolbox-9.14.5.8/setup.py`

 * *Files identical despite different names*

