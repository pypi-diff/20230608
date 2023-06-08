# Comparing `tmp/evilHunter-0.1.3a0.tar.gz` & `tmp/evilHunter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.1.3a0.tar", last modified: Thu Jun  8 20:17:24 2023, max compression
+gzip compressed data, was "evilHunter-0.1.4.tar", last modified: Thu Jun  8 20:21:16 2023, max compression
```

## Comparing `evilHunter-0.1.3a0.tar` & `evilHunter-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-08 20:17:24.298020 evilHunter-0.1.3a0/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1236 2023-06-08 20:17:24.298020 evilHunter-0.1.3a0/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1002 2023-06-08 20:13:21.000000 evilHunter-0.1.3a0/README.md
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-08 20:17:24.298020 evilHunter-0.1.3a0/evilHunter.egg-info/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1236 2023-06-08 20:17:24.000000 evilHunter-0.1.3a0/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      201 2023-06-08 20:17:24.000000 evilHunter-0.1.3a0/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-08 20:17:24.000000 evilHunter-0.1.3a0/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        9 2023-06-08 20:17:24.000000 evilHunter-0.1.3a0/evilHunter.egg-info/requires.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-08 20:17:24.000000 evilHunter-0.1.3a0/evilHunter.egg-info/top_level.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)    15454 2023-06-08 20:09:43.000000 evilHunter-0.1.3a0/evilHunter.py
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-08 20:17:24.298020 evilHunter-0.1.3a0/setup.cfg
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      520 2023-06-08 20:14:06.000000 evilHunter-0.1.3a0/setup.py
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-08 20:21:16.570668 evilHunter-0.1.4/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1131 2023-06-08 20:21:16.570668 evilHunter-0.1.4/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      899 2023-06-08 20:20:36.000000 evilHunter-0.1.4/README.md
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-08 20:21:16.570668 evilHunter-0.1.4/evilHunter.egg-info/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1131 2023-06-08 20:21:16.000000 evilHunter-0.1.4/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      201 2023-06-08 20:21:16.000000 evilHunter-0.1.4/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-08 20:21:16.000000 evilHunter-0.1.4/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        9 2023-06-08 20:21:16.000000 evilHunter-0.1.4/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-08 20:21:16.000000 evilHunter-0.1.4/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)    15454 2023-06-08 20:09:43.000000 evilHunter-0.1.4/evilHunter.py
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-08 20:21:16.570668 evilHunter-0.1.4/setup.cfg
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      519 2023-06-08 20:21:13.000000 evilHunter-0.1.4/setup.py
```

### Comparing `evilHunter-0.1.3a0/PKG-INFO` & `evilHunter-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.3a0
+Version: 0.1.4
 Summary: Cracking WiFi(Hanshake)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
 
 
 
 Argumentos:
     
-        ** Esta herramineta se puede ejecutar sin argumentos y usa'top400.txt' como diccionario **     
-
-
-    # OPTIONAL:
+    OBLIGATORIO
         
         [♦] evilHunter -w /path/to/wordlists
         
             (-w / -wordlist)
               (-h / --help)
               
 # INSTALACIÓN:
@@ -48,10 +45,11 @@
         -  aircrack-ng
         -  aireplay-ng
         -  airodump-ng
                
 # DICCIONARIO:
 
     Diccionario default "top400.txt"
+
     RockYou install -> (https://github.com/an0mal1a/evilHunter/releases/tag/RockYou)
     
-    Para especificar el diccionario con -w /path/to/dict
+    Para especificar el diccionario con "-w /path/to/dict"
```

### Comparing `evilHunter-0.1.3a0/README.md` & `evilHunter-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # evilHunter
 
 
 
 Argumentos:
     
-        ** Esta herramineta se puede ejecutar sin argumentos y usa'top400.txt' como diccionario **     
-
-
-    # OPTIONAL:
+    OBLIGATORIO
         
         [♦] evilHunter -w /path/to/wordlists
         
             (-w / -wordlist)
               (-h / --help)
               
 # INSTALACIÓN:
@@ -39,10 +36,11 @@
         -  aircrack-ng
         -  aireplay-ng
         -  airodump-ng
                
 # DICCIONARIO:
 
     Diccionario default "top400.txt"
+
     RockYou install -> (https://github.com/an0mal1a/evilHunter/releases/tag/RockYou)
     
-    Para especificar el diccionario con -w /path/to/dict
+    Para especificar el diccionario con "-w /path/to/dict"
```

### Comparing `evilHunter-0.1.3a0/evilHunter.egg-info/PKG-INFO` & `evilHunter-0.1.4/evilHunter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.3a0
+Version: 0.1.4
 Summary: Cracking WiFi(Hanshake)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
 
 
 
 Argumentos:
     
-        ** Esta herramineta se puede ejecutar sin argumentos y usa'top400.txt' como diccionario **     
-
-
-    # OPTIONAL:
+    OBLIGATORIO
         
         [♦] evilHunter -w /path/to/wordlists
         
             (-w / -wordlist)
               (-h / --help)
               
 # INSTALACIÓN:
@@ -48,10 +45,11 @@
         -  aircrack-ng
         -  aireplay-ng
         -  airodump-ng
                
 # DICCIONARIO:
 
     Diccionario default "top400.txt"
+
     RockYou install -> (https://github.com/an0mal1a/evilHunter/releases/tag/RockYou)
     
-    Para especificar el diccionario con -w /path/to/dict
+    Para especificar el diccionario con "-w /path/to/dict"
```

### Comparing `evilHunter-0.1.3a0/evilHunter.py` & `evilHunter-0.1.4/evilHunter.py`

 * *Files identical despite different names*

### Comparing `evilHunter-0.1.3a0/setup.py` & `evilHunter-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="evilHunter",
-    version="0.1.3a",
+    version="0.1.4",
     description="Cracking WiFi(Hanshake)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="an0mal1a",
     url="https://github.com/an0mal1a/evilHunter",
     author_email="pablodiez024@proton.me",
     packages=["words"],
```

