# Comparing `tmp/pymerkle-5.0.1b0.tar.gz` & `tmp/pymerkle-5.0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymerkle-5.0.1b0.tar", last modified: Tue Nov 12 14:15:10 2019, max compression
+gzip compressed data, was "dist/pymerkle-5.0.3b0.tar", last modified: Fri Nov 15 17:12:06 2019, max compression
```

## Comparing `pymerkle-5.0.1b0.tar` & `pymerkle-5.0.3b0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-12 14:15:10.000000 pymerkle-5.0.1b0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-12 14:15:10.000000 pymerkle-5.0.1b0/pymerkle/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-12 14:15:10.000000 pymerkle-5.0.1b0/pymerkle/validations/
--rwxr-xr-x   0 root         (0) root         (0)     9185 2019-11-01 19:35:41.000000 pymerkle-5.0.1b0/pymerkle/validations/mechanisms.py
--rw-r--r--   0 root         (0) root         (0)      112 2019-10-30 18:07:48.000000 pymerkle-5.0.1b0/pymerkle/validations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-12 14:15:10.000000 pymerkle-5.0.1b0/pymerkle/core/
--rwxr-xr-x   0 root         (0) root         (0)    12346 2019-11-01 21:52:00.000000 pymerkle-5.0.1b0/pymerkle/core/prover.py
--rwxr-xr-x   0 root         (0) root         (0)    12228 2019-11-01 19:18:15.000000 pymerkle-5.0.1b0/pymerkle/core/nodes.py
--rwxr-xr-x   0 root         (0) root         (0)    26038 2019-11-01 19:42:30.000000 pymerkle-5.0.1b0/pymerkle/core/tree.py
--rw-r--r--   0 root         (0) root         (0)       91 2019-10-27 15:32:24.000000 pymerkle-5.0.1b0/pymerkle/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6031 2019-10-31 18:42:38.000000 pymerkle-5.0.1b0/pymerkle/core/encryption.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-12 14:15:10.000000 pymerkle-5.0.1b0/pymerkle/pymerkle.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2019-11-12 12:35:43.000000 pymerkle-5.0.1b0/pymerkle/pymerkle.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      539 2019-11-12 14:15:10.000000 pymerkle-5.0.1b0/pymerkle/pymerkle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-11-12 14:15:10.000000 pymerkle-5.0.1b0/pymerkle/pymerkle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2019-11-12 14:15:10.000000 pymerkle-5.0.1b0/pymerkle/pymerkle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     9157 2019-11-12 14:15:10.000000 pymerkle-5.0.1b0/pymerkle/pymerkle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2019-11-12 14:15:10.000000 pymerkle-5.0.1b0/pymerkle/pymerkle.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-12 14:15:10.000000 pymerkle-5.0.1b0/pymerkle/hashing/
--rw-r--r--   0 root         (0) root         (0)      132 2019-10-21 17:45:51.000000 pymerkle-5.0.1b0/pymerkle/hashing/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5246 2019-11-01 07:12:24.000000 pymerkle-5.0.1b0/pymerkle/hashing/machine.py
--rw-r--r--   0 root         (0) root         (0)     3921 2019-11-01 06:49:29.000000 pymerkle-5.0.1b0/pymerkle/hashing/encoding.py
--rwxr-xr-x   0 root         (0) root         (0)     6754 2019-11-12 14:04:20.000000 pymerkle-5.0.1b0/README.md
--rwxr-xr-x   0 root         (0) root         (0)     1928 2019-11-12 14:08:46.000000 pymerkle-5.0.1b0/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2019-11-12 14:15:10.000000 pymerkle-5.0.1b0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9157 2019-11-12 14:15:10.000000 pymerkle-5.0.1b0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/validations/
+-rwxr-xr-x   0 root         (0) root         (0)     9185 2019-11-01 19:35:41.000000 pymerkle-5.0.3b0/pymerkle/validations/mechanisms.py
+-rw-r--r--   0 root         (0) root         (0)      112 2019-10-30 18:07:48.000000 pymerkle-5.0.3b0/pymerkle/validations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/core/
+-rwxr-xr-x   0 root         (0) root         (0)    12346 2019-11-01 21:52:00.000000 pymerkle-5.0.3b0/pymerkle/core/prover.py
+-rwxr-xr-x   0 root         (0) root         (0)    12228 2019-11-01 19:18:15.000000 pymerkle-5.0.3b0/pymerkle/core/nodes.py
+-rwxr-xr-x   0 root         (0) root         (0)    26038 2019-11-01 19:42:30.000000 pymerkle-5.0.3b0/pymerkle/core/tree.py
+-rw-r--r--   0 root         (0) root         (0)       91 2019-10-27 15:32:24.000000 pymerkle-5.0.3b0/pymerkle/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6031 2019-10-31 18:42:38.000000 pymerkle-5.0.3b0/pymerkle/core/encryption.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2019-11-12 12:35:43.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      539 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     9157 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/pymerkle/hashing/
+-rw-r--r--   0 root         (0) root         (0)      132 2019-10-21 17:45:51.000000 pymerkle-5.0.3b0/pymerkle/hashing/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5246 2019-11-01 07:12:24.000000 pymerkle-5.0.3b0/pymerkle/hashing/machine.py
+-rw-r--r--   0 root         (0) root         (0)     3921 2019-11-01 06:49:29.000000 pymerkle-5.0.3b0/pymerkle/hashing/encoding.py
+-rwxr-xr-x   0 root         (0) root         (0)     6754 2019-11-12 14:04:20.000000 pymerkle-5.0.3b0/README.md
+-rwxr-xr-x   0 root         (0) root         (0)     1871 2019-11-15 17:11:39.000000 pymerkle-5.0.3b0/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9157 2019-11-15 17:12:06.000000 pymerkle-5.0.3b0/PKG-INFO
```

### Comparing `pymerkle-5.0.1b0/pymerkle/validations/mechanisms.py` & `pymerkle-5.0.3b0/pymerkle/validations/mechanisms.py`

 * *Files identical despite different names*

### Comparing `pymerkle-5.0.1b0/pymerkle/core/prover.py` & `pymerkle-5.0.3b0/pymerkle/core/prover.py`

 * *Files identical despite different names*

### Comparing `pymerkle-5.0.1b0/pymerkle/core/nodes.py` & `pymerkle-5.0.3b0/pymerkle/core/nodes.py`

 * *Files identical despite different names*

### Comparing `pymerkle-5.0.1b0/pymerkle/core/tree.py` & `pymerkle-5.0.3b0/pymerkle/core/tree.py`

 * *Files identical despite different names*

### Comparing `pymerkle-5.0.1b0/pymerkle/core/encryption.py` & `pymerkle-5.0.3b0/pymerkle/core/encryption.py`

 * *Files identical despite different names*

### Comparing `pymerkle-5.0.1b0/pymerkle/pymerkle.egg-info/SOURCES.txt` & `pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymerkle-5.0.1b0/pymerkle/pymerkle.egg-info/PKG-INFO` & `pymerkle-5.0.3b0/pymerkle/pymerkle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymerkle
-Version: 5.0.1b0
+Version: 5.0.3b0
 Summary: Merkle-tree cryptographic library for generation and validation of Proofs
 Home-page: https://github.com/FoteinosMerg/pymerkle
 Author: FoteinosMerg
 Author-email: foteinosmerg@protonmail.com
 License: UNKNOWN
 Project-URL: github, https://github.com/FoteinosMerg/pymerkle
 Project-URL: source, https://github.com/FoteinosMerg/pymerkle/tree/master/pymerkle
```

### Comparing `pymerkle-5.0.1b0/pymerkle/hashing/machine.py` & `pymerkle-5.0.3b0/pymerkle/hashing/machine.py`

 * *Files identical despite different names*

### Comparing `pymerkle-5.0.1b0/pymerkle/hashing/encoding.py` & `pymerkle-5.0.3b0/pymerkle/hashing/encoding.py`

 * *Files identical despite different names*

### Comparing `pymerkle-5.0.1b0/README.md` & `pymerkle-5.0.3b0/README.md`

 * *Files identical despite different names*

### Comparing `pymerkle-5.0.1b0/setup.py` & `pymerkle-5.0.3b0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     long_description = __file.read()
 
 def main():
     setup(
        name=pymerkle.__name__,
        version=pymerkle.__version__,
        description=pymerkle.__doc__.strip(),
-       long_description=open('README.md').read(),
+       long_description=long_description,
        long_description_content_type='text/markdown',
-       packages=find_packages("pymerkle", exclude=("benchmarks", "docs", "dev", "tests",)),
+       packages=find_packages("pymerkle"),
        package_dir={'': 'pymerkle'},
        url=URL,
        project_urls={
             "github": URL,
             "source": "%s/%s" % (URL, "tree/master/%s" % pymerkle.__name__),
             "docs": "https://%s.readthedocs.io/en/latest/" % pymerkle.__name__,
        },
```

### Comparing `pymerkle-5.0.1b0/PKG-INFO` & `pymerkle-5.0.3b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymerkle
-Version: 5.0.1b0
+Version: 5.0.3b0
 Summary: Merkle-tree cryptographic library for generation and validation of Proofs
 Home-page: https://github.com/FoteinosMerg/pymerkle
 Author: FoteinosMerg
 Author-email: foteinosmerg@protonmail.com
 License: UNKNOWN
 Project-URL: github, https://github.com/FoteinosMerg/pymerkle
 Project-URL: source, https://github.com/FoteinosMerg/pymerkle/tree/master/pymerkle
```

