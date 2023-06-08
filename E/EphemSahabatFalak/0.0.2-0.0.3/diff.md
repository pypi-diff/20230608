# Comparing `tmp/EphemSahabatFalak-0.0.2.tar.gz` & `tmp/EphemSahabatFalak-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EphemSahabatFalak-0.0.2.tar", last modified: Thu Jun  8 11:30:48 2023, max compression
+gzip compressed data, was "EphemSahabatFalak-0.0.3.tar", last modified: Thu Jun  8 11:42:24 2023, max compression
```

## Comparing `EphemSahabatFalak-0.0.2.tar` & `EphemSahabatFalak-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-08 11:30:48.892016 EphemSahabatFalak-0.0.2/
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-08 11:30:48.888565 EphemSahabatFalak-0.0.2/EphemSahabatFalak.egg-info/
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    11718 2023-06-08 11:30:48.000000 EphemSahabatFalak-0.0.2/EphemSahabatFalak.egg-info/PKG-INFO
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      371 2023-06-08 11:30:48.000000 EphemSahabatFalak-0.0.2/EphemSahabatFalak.egg-info/SOURCES.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        1 2023-06-08 11:30:48.000000 EphemSahabatFalak-0.0.2/EphemSahabatFalak.egg-info/dependency_links.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       46 2023-06-08 11:30:48.000000 EphemSahabatFalak-0.0.2/EphemSahabatFalak.egg-info/requires.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        9 2023-06-08 11:30:48.000000 EphemSahabatFalak-0.0.2/EphemSahabatFalak.egg-info/top_level.txt
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-08 11:30:48.890801 EphemSahabatFalak-0.0.2/Falak_Py/
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      298 2023-06-08 07:06:06.000000 EphemSahabatFalak-0.0.2/Falak_Py/Contoh_azimut_kiblat.py
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      508 2023-06-08 08:08:12.000000 EphemSahabatFalak-0.0.2/Falak_Py/Contoh_efemeris_hilal.py
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      492 2023-06-08 08:08:12.000000 EphemSahabatFalak-0.0.2/Falak_Py/Contoh_takwim_solat.py
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    39538 2023-06-08 11:10:54.000000 EphemSahabatFalak-0.0.2/Falak_Py/KiraanWaktuSolat.py
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       35 2023-06-08 11:13:34.000000 EphemSahabatFalak-0.0.2/Falak_Py/__init__.py
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    11718 2023-06-08 11:30:48.891216 EphemSahabatFalak-0.0.2/PKG-INFO
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    11075 2023-06-08 11:28:01.000000 EphemSahabatFalak-0.0.2/README.md
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       38 2023-06-08 11:30:48.892096 EphemSahabatFalak-0.0.2/setup.cfg
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1228 2023-06-08 11:30:37.000000 EphemSahabatFalak-0.0.2/setup.py
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-08 11:42:24.845796 EphemSahabatFalak-0.0.3/
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-08 11:42:24.844177 EphemSahabatFalak-0.0.3/EphemSahabatFalak.egg-info/
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    11718 2023-06-08 11:42:24.000000 EphemSahabatFalak-0.0.3/EphemSahabatFalak.egg-info/PKG-INFO
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      371 2023-06-08 11:42:24.000000 EphemSahabatFalak-0.0.3/EphemSahabatFalak.egg-info/SOURCES.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        1 2023-06-08 11:42:24.000000 EphemSahabatFalak-0.0.3/EphemSahabatFalak.egg-info/dependency_links.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       46 2023-06-08 11:42:24.000000 EphemSahabatFalak-0.0.3/EphemSahabatFalak.egg-info/requires.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        9 2023-06-08 11:42:24.000000 EphemSahabatFalak-0.0.3/EphemSahabatFalak.egg-info/top_level.txt
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-08 11:42:24.845180 EphemSahabatFalak-0.0.3/Falak_Py/
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      298 2023-06-08 07:06:06.000000 EphemSahabatFalak-0.0.3/Falak_Py/Contoh_azimut_kiblat.py
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      508 2023-06-08 08:08:12.000000 EphemSahabatFalak-0.0.3/Falak_Py/Contoh_efemeris_hilal.py
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      492 2023-06-08 08:08:12.000000 EphemSahabatFalak-0.0.3/Falak_Py/Contoh_takwim_solat.py
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    39538 2023-06-08 11:10:54.000000 EphemSahabatFalak-0.0.3/Falak_Py/KiraanWaktuSolat.py
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       44 2023-06-08 11:40:58.000000 EphemSahabatFalak-0.0.3/Falak_Py/__init__.py
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    11718 2023-06-08 11:42:24.845479 EphemSahabatFalak-0.0.3/PKG-INFO
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    11075 2023-06-08 11:28:01.000000 EphemSahabatFalak-0.0.3/README.md
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       38 2023-06-08 11:42:24.845875 EphemSahabatFalak-0.0.3/setup.cfg
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1228 2023-06-08 11:42:16.000000 EphemSahabatFalak-0.0.3/setup.py
```

### Comparing `EphemSahabatFalak-0.0.2/EphemSahabatFalak.egg-info/PKG-INFO` & `EphemSahabatFalak-0.0.3/EphemSahabatFalak.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EphemSahabatFalak
-Version: 0.0.2
+Version: 0.0.3
 Summary: Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak
 Home-page: UNKNOWN
 Author: cartcosine (izzatzubir)
 Author-email: <cart.cosine.0x@icloud.com>
 License: UNKNOWN
 Keywords: python,falak,solat,hilal,waktu,matahari,bulan
 Platform: UNKNOWN
```

### Comparing `EphemSahabatFalak-0.0.2/Falak_Py/KiraanWaktuSolat.py` & `EphemSahabatFalak-0.0.3/Falak_Py/KiraanWaktuSolat.py`

 * *Files identical despite different names*

### Comparing `EphemSahabatFalak-0.0.2/PKG-INFO` & `EphemSahabatFalak-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EphemSahabatFalak
-Version: 0.0.2
+Version: 0.0.3
 Summary: Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak
 Home-page: UNKNOWN
 Author: cartcosine (izzatzubir)
 Author-email: <cart.cosine.0x@icloud.com>
 License: UNKNOWN
 Keywords: python,falak,solat,hilal,waktu,matahari,bulan
 Platform: UNKNOWN
```

### Comparing `EphemSahabatFalak-0.0.2/README.md` & `EphemSahabatFalak-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `EphemSahabatFalak-0.0.2/setup.py` & `EphemSahabatFalak-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak'
 LONG_DESCRIPTION = 'Sebuah pakej python yang menggunakan ephemeris dari JPL Horizon bagi menghasilkan hitungan falak'
 
 # Setting up
 setup(
     name="EphemSahabatFalak",
     version=VERSION,
```

