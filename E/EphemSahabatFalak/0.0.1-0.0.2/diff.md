# Comparing `tmp/EphemSahabatFalak-0.0.1.tar.gz` & `tmp/EphemSahabatFalak-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EphemSahabatFalak-0.0.1.tar", last modified: Thu Jun  8 11:21:36 2023, max compression
+gzip compressed data, was "EphemSahabatFalak-0.0.2.tar", last modified: Thu Jun  8 11:30:48 2023, max compression
```

## Comparing `EphemSahabatFalak-0.0.1.tar` & `EphemSahabatFalak-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-08 11:21:36.442226 EphemSahabatFalak-0.0.1/
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-08 11:21:36.438528 EphemSahabatFalak-0.0.1/EphemSahabatFalak.egg-info/
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    11720 2023-06-08 11:21:36.000000 EphemSahabatFalak-0.0.1/EphemSahabatFalak.egg-info/PKG-INFO
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      371 2023-06-08 11:21:36.000000 EphemSahabatFalak-0.0.1/EphemSahabatFalak.egg-info/SOURCES.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        1 2023-06-08 11:21:36.000000 EphemSahabatFalak-0.0.1/EphemSahabatFalak.egg-info/dependency_links.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       46 2023-06-08 11:21:36.000000 EphemSahabatFalak-0.0.1/EphemSahabatFalak.egg-info/requires.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        9 2023-06-08 11:21:36.000000 EphemSahabatFalak-0.0.1/EphemSahabatFalak.egg-info/top_level.txt
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-08 11:21:36.441311 EphemSahabatFalak-0.0.1/Falak_Py/
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      298 2023-06-08 07:06:06.000000 EphemSahabatFalak-0.0.1/Falak_Py/Contoh_azimut_kiblat.py
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      508 2023-06-08 08:08:12.000000 EphemSahabatFalak-0.0.1/Falak_Py/Contoh_efemeris_hilal.py
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      492 2023-06-08 08:08:12.000000 EphemSahabatFalak-0.0.1/Falak_Py/Contoh_takwim_solat.py
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    39538 2023-06-08 11:10:54.000000 EphemSahabatFalak-0.0.1/Falak_Py/KiraanWaktuSolat.py
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       35 2023-06-08 11:13:34.000000 EphemSahabatFalak-0.0.1/Falak_Py/__init__.py
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    11720 2023-06-08 11:21:36.441860 EphemSahabatFalak-0.0.1/PKG-INFO
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    11077 2023-06-08 10:15:38.000000 EphemSahabatFalak-0.0.1/README.md
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       38 2023-06-08 11:21:36.442326 EphemSahabatFalak-0.0.1/setup.cfg
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1228 2023-06-08 11:20:31.000000 EphemSahabatFalak-0.0.1/setup.py
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-08 11:30:48.892016 EphemSahabatFalak-0.0.2/
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-08 11:30:48.888565 EphemSahabatFalak-0.0.2/EphemSahabatFalak.egg-info/
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    11718 2023-06-08 11:30:48.000000 EphemSahabatFalak-0.0.2/EphemSahabatFalak.egg-info/PKG-INFO
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      371 2023-06-08 11:30:48.000000 EphemSahabatFalak-0.0.2/EphemSahabatFalak.egg-info/SOURCES.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        1 2023-06-08 11:30:48.000000 EphemSahabatFalak-0.0.2/EphemSahabatFalak.egg-info/dependency_links.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       46 2023-06-08 11:30:48.000000 EphemSahabatFalak-0.0.2/EphemSahabatFalak.egg-info/requires.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        9 2023-06-08 11:30:48.000000 EphemSahabatFalak-0.0.2/EphemSahabatFalak.egg-info/top_level.txt
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-08 11:30:48.890801 EphemSahabatFalak-0.0.2/Falak_Py/
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      298 2023-06-08 07:06:06.000000 EphemSahabatFalak-0.0.2/Falak_Py/Contoh_azimut_kiblat.py
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      508 2023-06-08 08:08:12.000000 EphemSahabatFalak-0.0.2/Falak_Py/Contoh_efemeris_hilal.py
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      492 2023-06-08 08:08:12.000000 EphemSahabatFalak-0.0.2/Falak_Py/Contoh_takwim_solat.py
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    39538 2023-06-08 11:10:54.000000 EphemSahabatFalak-0.0.2/Falak_Py/KiraanWaktuSolat.py
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       35 2023-06-08 11:13:34.000000 EphemSahabatFalak-0.0.2/Falak_Py/__init__.py
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    11718 2023-06-08 11:30:48.891216 EphemSahabatFalak-0.0.2/PKG-INFO
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    11075 2023-06-08 11:28:01.000000 EphemSahabatFalak-0.0.2/README.md
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       38 2023-06-08 11:30:48.892096 EphemSahabatFalak-0.0.2/setup.cfg
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1228 2023-06-08 11:30:37.000000 EphemSahabatFalak-0.0.2/setup.py
```

### Comparing `EphemSahabatFalak-0.0.1/EphemSahabatFalak.egg-info/PKG-INFO` & `EphemSahabatFalak-0.0.2/EphemSahabatFalak.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EphemSahabatFalak
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak
 Home-page: UNKNOWN
 Author: cartcosine (izzatzubir)
 Author-email: <cart.cosine.0x@icloud.com>
 License: UNKNOWN
 Keywords: python,falak,solat,hilal,waktu,matahari,bulan
 Platform: UNKNOWN
@@ -15,15 +15,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
 # Falak_py
 
-<p>KiraanWaktuSolat.py ialah sebuah file python yang mengandungi sebuah python Class iaitu Takwim() yang mempunyai pelbagai method. </p>
+<p>EphemSahabatFalak ialah sebuah file python yang mengandungi sebuah python Class iaitu Takwim() yang mempunyai pelbagai method. </p>
 <p> Program ini menggunakan data ephemeris dari JPL Horizon (NASA) iaitu de440s. Pengguna boleh untuk mengubah kepada ephemeris lain </p>
 <p> Program ini menggunapakai pakej Skyfield </p>
 <p> Program ini dihasilkan oleh Izzat Zubir, dengan sokongan dari keluarga, beserta maklum balas dari Dr. Abdul Halim Abdul Aziz, Panel Pakar Falak JAKIM </p>
 
 
 <h1> Parameter </h1>
 <p> Terdapat 13 parameter yang boleh diubah:</p>
```

### Comparing `EphemSahabatFalak-0.0.1/Falak_Py/KiraanWaktuSolat.py` & `EphemSahabatFalak-0.0.2/Falak_Py/KiraanWaktuSolat.py`

 * *Files identical despite different names*

### Comparing `EphemSahabatFalak-0.0.1/PKG-INFO` & `EphemSahabatFalak-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EphemSahabatFalak
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak
 Home-page: UNKNOWN
 Author: cartcosine (izzatzubir)
 Author-email: <cart.cosine.0x@icloud.com>
 License: UNKNOWN
 Keywords: python,falak,solat,hilal,waktu,matahari,bulan
 Platform: UNKNOWN
@@ -15,15 +15,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
 # Falak_py
 
-<p>KiraanWaktuSolat.py ialah sebuah file python yang mengandungi sebuah python Class iaitu Takwim() yang mempunyai pelbagai method. </p>
+<p>EphemSahabatFalak ialah sebuah file python yang mengandungi sebuah python Class iaitu Takwim() yang mempunyai pelbagai method. </p>
 <p> Program ini menggunakan data ephemeris dari JPL Horizon (NASA) iaitu de440s. Pengguna boleh untuk mengubah kepada ephemeris lain </p>
 <p> Program ini menggunapakai pakej Skyfield </p>
 <p> Program ini dihasilkan oleh Izzat Zubir, dengan sokongan dari keluarga, beserta maklum balas dari Dr. Abdul Halim Abdul Aziz, Panel Pakar Falak JAKIM </p>
 
 
 <h1> Parameter </h1>
 <p> Terdapat 13 parameter yang boleh diubah:</p>
```

### Comparing `EphemSahabatFalak-0.0.1/README.md` & `EphemSahabatFalak-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Falak_py
 
-<p>KiraanWaktuSolat.py ialah sebuah file python yang mengandungi sebuah python Class iaitu Takwim() yang mempunyai pelbagai method. </p>
+<p>EphemSahabatFalak ialah sebuah file python yang mengandungi sebuah python Class iaitu Takwim() yang mempunyai pelbagai method. </p>
 <p> Program ini menggunakan data ephemeris dari JPL Horizon (NASA) iaitu de440s. Pengguna boleh untuk mengubah kepada ephemeris lain </p>
 <p> Program ini menggunapakai pakej Skyfield </p>
 <p> Program ini dihasilkan oleh Izzat Zubir, dengan sokongan dari keluarga, beserta maklum balas dari Dr. Abdul Halim Abdul Aziz, Panel Pakar Falak JAKIM </p>
 
 
 <h1> Parameter </h1>
 <p> Terdapat 13 parameter yang boleh diubah:</p>
```

### Comparing `EphemSahabatFalak-0.0.1/setup.py` & `EphemSahabatFalak-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak'
 LONG_DESCRIPTION = 'Sebuah pakej python yang menggunakan ephemeris dari JPL Horizon bagi menghasilkan hitungan falak'
 
 # Setting up
 setup(
     name="EphemSahabatFalak",
     version=VERSION,
```

