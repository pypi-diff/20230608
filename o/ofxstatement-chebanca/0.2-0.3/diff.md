# Comparing `tmp/ofxstatement-chebanca-0.2.tar.gz` & `tmp/ofxstatement-chebanca-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofxstatement-chebanca-0.2.tar", last modified: Mon Mar  6 01:13:27 2023, max compression
+gzip compressed data, was "ofxstatement-chebanca-0.3.tar", last modified: Thu Jun  8 11:00:24 2023, max compression
```

## Comparing `ofxstatement-chebanca-0.2.tar` & `ofxstatement-chebanca-0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-03-06 01:13:27.683115 ofxstatement-chebanca-0.2/
--rw-rw-r--   0 marco     (1000) marco     (1000)       18 2023-03-05 20:26:32.000000 ofxstatement-chebanca-0.2/MANIFEST.in
--rw-rw-r--   0 marco     (1000) marco     (1000)     1769 2023-03-06 01:13:27.683115 ofxstatement-chebanca-0.2/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     1040 2023-03-06 01:09:58.000000 ofxstatement-chebanca-0.2/README.md
--rw-rw-r--   0 marco     (1000) marco     (1000)       72 2023-03-06 01:13:27.683115 ofxstatement-chebanca-0.2/setup.cfg
--rwxrwxr-x   0 marco     (1000) marco     (1000)     1442 2023-03-06 01:12:47.000000 ofxstatement-chebanca-0.2/setup.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-03-06 01:13:27.679115 ofxstatement-chebanca-0.2/src/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-03-06 01:13:27.679115 ofxstatement-chebanca-0.2/src/ofxstatement/
--rw-rw-r--   0 marco     (1000) marco     (1000)       56 2023-03-05 20:03:22.000000 ofxstatement-chebanca-0.2/src/ofxstatement/__init__.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-03-06 01:13:27.679115 ofxstatement-chebanca-0.2/src/ofxstatement/plugins/
--rw-rw-r--   0 marco     (1000) marco     (1000)       56 2023-03-05 20:03:22.000000 ofxstatement-chebanca-0.2/src/ofxstatement/plugins/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     9096 2023-03-06 01:08:41.000000 ofxstatement-chebanca-0.2/src/ofxstatement/plugins/chebanca.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     7248 2023-03-06 01:10:38.000000 ofxstatement-chebanca-0.2/src/ofxstatement/plugins/chebanca_pdf.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-03-06 01:13:27.683115 ofxstatement-chebanca-0.2/src/ofxstatement_chebanca.egg-info/
--rw-rw-r--   0 marco     (1000) marco     (1000)     1769 2023-03-06 01:13:27.000000 ofxstatement-chebanca-0.2/src/ofxstatement_chebanca.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      582 2023-03-06 01:13:27.000000 ofxstatement-chebanca-0.2/src/ofxstatement_chebanca.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2023-03-06 01:13:27.000000 ofxstatement-chebanca-0.2/src/ofxstatement_chebanca.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)      139 2023-03-06 01:13:27.000000 ofxstatement-chebanca-0.2/src/ofxstatement_chebanca.egg-info/entry_points.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       34 2023-03-06 01:13:27.000000 ofxstatement-chebanca-0.2/src/ofxstatement_chebanca.egg-info/namespace_packages.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       13 2023-03-06 01:13:27.000000 ofxstatement-chebanca-0.2/src/ofxstatement_chebanca.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       13 2023-03-06 01:13:27.000000 ofxstatement-chebanca-0.2/src/ofxstatement_chebanca.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2023-03-05 20:30:59.000000 ofxstatement-chebanca-0.2/src/ofxstatement_chebanca.egg-info/zip-safe
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-06-08 11:00:24.309242 ofxstatement-chebanca-0.3/
+-rw-rw-r--   0 marco     (1000) marco     (1000)       18 2023-03-05 20:26:32.000000 ofxstatement-chebanca-0.3/MANIFEST.in
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2070 2023-06-08 11:00:24.309242 ofxstatement-chebanca-0.3/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1040 2023-03-06 01:09:58.000000 ofxstatement-chebanca-0.3/README.md
+-rw-rw-r--   0 marco     (1000) marco     (1000)       72 2023-06-08 11:00:24.309242 ofxstatement-chebanca-0.3/setup.cfg
+-rwxrwxr-x   0 marco     (1000) marco     (1000)     1467 2023-06-08 10:58:53.000000 ofxstatement-chebanca-0.3/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-06-08 11:00:24.305242 ofxstatement-chebanca-0.3/src/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-06-08 11:00:24.309242 ofxstatement-chebanca-0.3/src/ofxstatement/
+-rw-rw-r--   0 marco     (1000) marco     (1000)       56 2023-03-05 20:03:22.000000 ofxstatement-chebanca-0.3/src/ofxstatement/__init__.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-06-08 11:00:24.309242 ofxstatement-chebanca-0.3/src/ofxstatement/plugins/
+-rw-rw-r--   0 marco     (1000) marco     (1000)       56 2023-03-05 20:03:22.000000 ofxstatement-chebanca-0.3/src/ofxstatement/plugins/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     9096 2023-03-06 01:08:41.000000 ofxstatement-chebanca-0.3/src/ofxstatement/plugins/chebanca.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     7248 2023-03-06 01:10:38.000000 ofxstatement-chebanca-0.3/src/ofxstatement/plugins/chebanca_pdf.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2023-06-08 11:00:24.309242 ofxstatement-chebanca-0.3/src/ofxstatement_chebanca.egg-info/
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2070 2023-06-08 11:00:24.000000 ofxstatement-chebanca-0.3/src/ofxstatement_chebanca.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      582 2023-06-08 11:00:24.000000 ofxstatement-chebanca-0.3/src/ofxstatement_chebanca.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2023-06-08 11:00:24.000000 ofxstatement-chebanca-0.3/src/ofxstatement_chebanca.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)      139 2023-06-08 11:00:24.000000 ofxstatement-chebanca-0.3/src/ofxstatement_chebanca.egg-info/entry_points.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       34 2023-06-08 11:00:24.000000 ofxstatement-chebanca-0.3/src/ofxstatement_chebanca.egg-info/namespace_packages.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       22 2023-06-08 11:00:24.000000 ofxstatement-chebanca-0.3/src/ofxstatement_chebanca.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       13 2023-06-08 11:00:24.000000 ofxstatement-chebanca-0.3/src/ofxstatement_chebanca.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2023-03-05 20:30:59.000000 ofxstatement-chebanca-0.3/src/ofxstatement_chebanca.egg-info/zip-safe
```

### Comparing `ofxstatement-chebanca-0.2/PKG-INFO` & `ofxstatement-chebanca-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 Metadata-Version: 2.1
 Name: ofxstatement-chebanca
-Version: 0.2
+Version: 0.3
 Summary: CheBanca! plugin for ofxstatement
 Home-page: https://github.com/3v1n0/ofxstatement-chebanca
 Author: Marco Trevisan
 Author-email: mail@3v1n0.net
 License: GPLv3
-Keywords: ofx,banking,statement,chebanca,che-banca
+Description: # CheBanca! Plugin for [ofxstatement](https://github.com/kedder/ofxstatement/)
+        
+        Parses CheBanca! xslx statement files to be used with GNU Cash or HomeBank.
+        
+        ## Installation
+        
+        You can install the plugin as usual from pip or directly from the downloaded git
+        
+        ### `pip`
+        
+            pip3 install --user ofxstatement-chebanca
+        
+        ### `setup.py`
+        
+            python3 setup.py install --user
+        
+        ## Usage
+        Download your transactions file from the official bank's site and then run
+        
+            ofxstatement convert -t chebanca CheBanca.xlsx CheBanca.ofx
+        
+        
+        ### Loading Historical data
+        
+        This only supports the statements for the last year, however it's also possible
+        to convert the old per-quarter statements that are available from the archive as
+        PDF files.
+        
+        A plugin is provided that uses `poppler-util`'s `pdftotext` to easily generate
+        machine parse-able data.
+        
+        This is an experimental plugin, that may not alwyas work but it can be used via:
+        
+            ofxstatement -d convert -t chebanca-pdf ./dir-containing-all-pdfs
+            ofxstatement -d convert -t chebanca-pdf CheBanca-20-Q2.pdf
+        
+Keywords: ofx,banking,statement,chebanca,che-banca,che banca
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Utilities
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
-
-# CheBanca! Plugin for [ofxstatement](https://github.com/kedder/ofxstatement/)
-
-Parses CheBanca! xslx statement files to be used with GNU Cash or HomeBank.
-
-## Installation
-
-You can install the plugin as usual from pip or directly from the downloaded git
-
-### `pip`
-
-    pip3 install --user ofxstatement-chebanca
-
-### `setup.py`
-
-    python3 setup.py install --user
-
-## Usage
-Download your transactions file from the official bank's site and then run
-
-    ofxstatement convert -t chebanca CheBanca.xlsx CheBanca.ofx
-
-
-### Loading Historical data
-
-This only supports the statements for the last year, however it's also possible
-to convert the old per-quarter statements that are available from the archive as
-PDF files.
-
-A plugin is provided that uses `poppler-util`'s `pdftotext` to easily generate
-machine parse-able data.
-
-This is an experimental plugin, that may not alwyas work but it can be used via:
-
-    ofxstatement -d convert -t chebanca-pdf ./dir-containing-all-pdfs
-    ofxstatement -d convert -t chebanca-pdf CheBanca-20-Q2.pdf
-
-
```

### Comparing `ofxstatement-chebanca-0.2/README.md` & `ofxstatement-chebanca-0.3/README.md`

 * *Files identical despite different names*

### Comparing `ofxstatement-chebanca-0.2/setup.py` & `ofxstatement-chebanca-0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #!/usr/bin/python3
 """Setup
 """
 from setuptools import find_packages
 from distutils.core import setup
 
-version = "0.2"
+version = "0.3"
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="ofxstatement-chebanca",
     version=version,
     author="Marco Trevisan",
     author_email="mail@3v1n0.net",
     url="https://github.com/3v1n0/ofxstatement-chebanca",
     description=("CheBanca! plugin for ofxstatement"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="GPLv3",
-    keywords=["ofx", "banking", "statement", "chebanca", "che-banca"],
+    keywords=["ofx", "banking", "statement", "chebanca", "che-banca", "che banca"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
         "Natural Language :: English",
         "Topic :: Office/Business :: Financial :: Accounting",
         "Topic :: Utilities",
         "Environment :: Console",
@@ -35,11 +35,11 @@
     namespace_packages=["ofxstatement", "ofxstatement.plugins"],
     entry_points={
         "ofxstatement": [
             "chebanca = ofxstatement.plugins.chebanca:CheBancaPlugin",
             "chebanca-pdf = ofxstatement.plugins.chebanca_pdf:CheBancaPdfPlugin",
         ],
     },
-    install_requires=["ofxstatement"],
+    install_requires=["ofxstatement", "openpyxl"],
     include_package_data=True,
     zip_safe=True,
 )
```

### Comparing `ofxstatement-chebanca-0.2/src/ofxstatement/plugins/chebanca.py` & `ofxstatement-chebanca-0.3/src/ofxstatement/plugins/chebanca.py`

 * *Files identical despite different names*

### Comparing `ofxstatement-chebanca-0.2/src/ofxstatement/plugins/chebanca_pdf.py` & `ofxstatement-chebanca-0.3/src/ofxstatement/plugins/chebanca_pdf.py`

 * *Files identical despite different names*

### Comparing `ofxstatement-chebanca-0.2/src/ofxstatement_chebanca.egg-info/PKG-INFO` & `ofxstatement-chebanca-0.3/src/ofxstatement_chebanca.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 Metadata-Version: 2.1
 Name: ofxstatement-chebanca
-Version: 0.2
+Version: 0.3
 Summary: CheBanca! plugin for ofxstatement
 Home-page: https://github.com/3v1n0/ofxstatement-chebanca
 Author: Marco Trevisan
 Author-email: mail@3v1n0.net
 License: GPLv3
-Keywords: ofx,banking,statement,chebanca,che-banca
+Description: # CheBanca! Plugin for [ofxstatement](https://github.com/kedder/ofxstatement/)
+        
+        Parses CheBanca! xslx statement files to be used with GNU Cash or HomeBank.
+        
+        ## Installation
+        
+        You can install the plugin as usual from pip or directly from the downloaded git
+        
+        ### `pip`
+        
+            pip3 install --user ofxstatement-chebanca
+        
+        ### `setup.py`
+        
+            python3 setup.py install --user
+        
+        ## Usage
+        Download your transactions file from the official bank's site and then run
+        
+            ofxstatement convert -t chebanca CheBanca.xlsx CheBanca.ofx
+        
+        
+        ### Loading Historical data
+        
+        This only supports the statements for the last year, however it's also possible
+        to convert the old per-quarter statements that are available from the archive as
+        PDF files.
+        
+        A plugin is provided that uses `poppler-util`'s `pdftotext` to easily generate
+        machine parse-able data.
+        
+        This is an experimental plugin, that may not alwyas work but it can be used via:
+        
+            ofxstatement -d convert -t chebanca-pdf ./dir-containing-all-pdfs
+            ofxstatement -d convert -t chebanca-pdf CheBanca-20-Q2.pdf
+        
+Keywords: ofx,banking,statement,chebanca,che-banca,che banca
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Utilities
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
-
-# CheBanca! Plugin for [ofxstatement](https://github.com/kedder/ofxstatement/)
-
-Parses CheBanca! xslx statement files to be used with GNU Cash or HomeBank.
-
-## Installation
-
-You can install the plugin as usual from pip or directly from the downloaded git
-
-### `pip`
-
-    pip3 install --user ofxstatement-chebanca
-
-### `setup.py`
-
-    python3 setup.py install --user
-
-## Usage
-Download your transactions file from the official bank's site and then run
-
-    ofxstatement convert -t chebanca CheBanca.xlsx CheBanca.ofx
-
-
-### Loading Historical data
-
-This only supports the statements for the last year, however it's also possible
-to convert the old per-quarter statements that are available from the archive as
-PDF files.
-
-A plugin is provided that uses `poppler-util`'s `pdftotext` to easily generate
-machine parse-able data.
-
-This is an experimental plugin, that may not alwyas work but it can be used via:
-
-    ofxstatement -d convert -t chebanca-pdf ./dir-containing-all-pdfs
-    ofxstatement -d convert -t chebanca-pdf CheBanca-20-Q2.pdf
-
-
```

### Comparing `ofxstatement-chebanca-0.2/src/ofxstatement_chebanca.egg-info/SOURCES.txt` & `ofxstatement-chebanca-0.3/src/ofxstatement_chebanca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

