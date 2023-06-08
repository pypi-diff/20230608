# Comparing `tmp/pyenv-encrypt-0.0.1.tar.gz` & `tmp/pyenv-encrypt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenv-encrypt-0.0.1.tar", last modified: Thu Jun  8 00:51:34 2023, max compression
+gzip compressed data, was "pyenv-encrypt-0.1.0.tar", last modified: Thu Jun  8 01:54:31 2023, max compression
```

## Comparing `pyenv-encrypt-0.0.1.tar` & `pyenv-encrypt-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 akhlak    (1000) akhlak    (1000)        0 2023-06-08 00:51:34.927713 pyenv-encrypt-0.0.1/
--rw-rw-r--   0 akhlak    (1000) akhlak    (1000)     1061 2023-06-08 00:22:01.000000 pyenv-encrypt-0.0.1/LICENSE
--rw-rw-r--   0 akhlak    (1000) akhlak    (1000)     3267 2023-06-08 00:51:34.927713 pyenv-encrypt-0.0.1/PKG-INFO
--rw-r--r--   0 akhlak    (1000) akhlak    (1000)     2710 2023-06-08 00:38:24.000000 pyenv-encrypt-0.0.1/README.md
-drwxrwxr-x   0 akhlak    (1000) akhlak    (1000)        0 2023-06-08 00:51:34.927713 pyenv-encrypt-0.0.1/pyenv_enc/
--rw-rw-r--   0 akhlak    (1000) akhlak    (1000)        0 2023-06-07 23:28:26.000000 pyenv-encrypt-0.0.1/pyenv_enc/__init__.py
--rw-rw-r--   0 akhlak    (1000) akhlak    (1000)     6563 2023-06-08 00:29:01.000000 pyenv-encrypt-0.0.1/pyenv_enc/enc.py
-drwxrwxr-x   0 akhlak    (1000) akhlak    (1000)        0 2023-06-08 00:51:34.927713 pyenv-encrypt-0.0.1/pyenv_encrypt.egg-info/
--rw-rw-r--   0 akhlak    (1000) akhlak    (1000)     3267 2023-06-08 00:51:34.000000 pyenv-encrypt-0.0.1/pyenv_encrypt.egg-info/PKG-INFO
--rw-rw-r--   0 akhlak    (1000) akhlak    (1000)      295 2023-06-08 00:51:34.000000 pyenv-encrypt-0.0.1/pyenv_encrypt.egg-info/SOURCES.txt
--rw-rw-r--   0 akhlak    (1000) akhlak    (1000)        1 2023-06-08 00:51:34.000000 pyenv-encrypt-0.0.1/pyenv_encrypt.egg-info/dependency_links.txt
--rw-rw-r--   0 akhlak    (1000) akhlak    (1000)       45 2023-06-08 00:51:34.000000 pyenv-encrypt-0.0.1/pyenv_encrypt.egg-info/entry_points.txt
--rw-rw-r--   0 akhlak    (1000) akhlak    (1000)       21 2023-06-08 00:51:34.000000 pyenv-encrypt-0.0.1/pyenv_encrypt.egg-info/requires.txt
--rw-rw-r--   0 akhlak    (1000) akhlak    (1000)       10 2023-06-08 00:51:34.000000 pyenv-encrypt-0.0.1/pyenv_encrypt.egg-info/top_level.txt
--rw-rw-r--   0 akhlak    (1000) akhlak    (1000)      786 2023-06-08 00:22:58.000000 pyenv-encrypt-0.0.1/pyproject.toml
--rw-rw-r--   0 akhlak    (1000) akhlak    (1000)       38 2023-06-08 00:51:34.927713 pyenv-encrypt-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:54:31.488946 pyenv-encrypt-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-08 01:54:17.000000 pyenv-encrypt-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-08 01:54:31.488946 pyenv-encrypt-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-08 01:54:17.000000 pyenv-encrypt-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:54:31.484946 pyenv-encrypt-0.1.0/pyenv_enc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:54:17.000000 pyenv-encrypt-0.1.0/pyenv_enc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-08 01:54:17.000000 pyenv-encrypt-0.1.0/pyenv_enc/enc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:54:31.488946 pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-08 01:54:31.000000 pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-08 01:54:31.000000 pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 01:54:31.000000 pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 01:54:31.000000 pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 01:54:31.000000 pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 01:54:31.000000 pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-08 01:54:17.000000 pyenv-encrypt-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 01:54:31.488946 pyenv-encrypt-0.1.0/setup.cfg
```

### Comparing `pyenv-encrypt-0.0.1/LICENSE` & `pyenv-encrypt-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenv-encrypt-0.0.1/PKG-INFO` & `pyenv-encrypt-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenv-encrypt
-Version: 0.0.1
+Version: 0.1.0
 Summary: GPG based env file encryptor utility.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/pyenv-encrypt
 Project-URL: Bug Tracker, https://github.com/akhlakm/pyenv-encrypt/issues
 Keywords: encryption,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -34,24 +34,25 @@
     - .env
     - yaml
     - json
 - Recursive update of all text fields.
 - Automatic decision of encryption or decryption based on file contents.
 
 ## Installation
-To use, clone this repo and install with `pip`.
+You can install `pyenv-encrypt` directly from [PyPI](https://pypi.org/project/pyenv-encrypt) using `pip`.
+
 ```sh
-git clone git+https://github.com/akhlakm/pyenv-encrypt.git
-cd pyenv-encrypt
-pip install -e .
+pip install pyenv-encrypt
 ```
 
-Alternatively, use the following for packaging (for example, in your `requirements.txt` file).
+Alternatively, clone this repo and install with `pip`.
 ```sh
-pip install git+https://github.com/akhlakm/pyenv-encrypt.git
+git clone https://github.com/akhlakm/pyenv-encrypt.git
+cd pyenv-encrypt
+pip install -e .
 ```
 
 ### Dependencies
 The `gpg` utility must be installed in your system. GPG comes built-in with most versions of Linux OS. For Mac, use homebrew: `brew install gpg`.
 
 See the official [installation instructions](https://gnupg.org/download/) for more info. Run the following command to check if GPG is installed.
 
@@ -78,14 +79,16 @@
 
 `pyenc` will toggle between encryption and decryption. To force encryption or decryption specify `-e` or `-d` respectively.
 
 ```sh
 pyenc -e .env vault.yaml data.json
 ```
 
+To make sure you do not commit unencrypted files, you can setup a githook for your repository.
+See an [example pre-commit](pre-commit) file here.
 
 ## Use As A Python Module
 
 ```python
 import os
 from pyenv_enc import enc
```

### Comparing `pyenv-encrypt-0.0.1/README.md` & `pyenv-encrypt-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -19,24 +19,25 @@
     - .env
     - yaml
     - json
 - Recursive update of all text fields.
 - Automatic decision of encryption or decryption based on file contents.
 
 ## Installation
-To use, clone this repo and install with `pip`.
+You can install `pyenv-encrypt` directly from [PyPI](https://pypi.org/project/pyenv-encrypt) using `pip`.
+
 ```sh
-git clone git+https://github.com/akhlakm/pyenv-encrypt.git
-cd pyenv-encrypt
-pip install -e .
+pip install pyenv-encrypt
 ```
 
-Alternatively, use the following for packaging (for example, in your `requirements.txt` file).
+Alternatively, clone this repo and install with `pip`.
 ```sh
-pip install git+https://github.com/akhlakm/pyenv-encrypt.git
+git clone https://github.com/akhlakm/pyenv-encrypt.git
+cd pyenv-encrypt
+pip install -e .
 ```
 
 ### Dependencies
 The `gpg` utility must be installed in your system. GPG comes built-in with most versions of Linux OS. For Mac, use homebrew: `brew install gpg`.
 
 See the official [installation instructions](https://gnupg.org/download/) for more info. Run the following command to check if GPG is installed.
 
@@ -63,14 +64,16 @@
 
 `pyenc` will toggle between encryption and decryption. To force encryption or decryption specify `-e` or `-d` respectively.
 
 ```sh
 pyenc -e .env vault.yaml data.json
 ```
 
+To make sure you do not commit unencrypted files, you can setup a githook for your repository.
+See an [example pre-commit](pre-commit) file here.
 
 ## Use As A Python Module
 
 ```python
 import os
 from pyenv_enc import enc
```

### Comparing `pyenv-encrypt-0.0.1/pyenv_enc/enc.py` & `pyenv-encrypt-0.1.0/pyenv_enc/enc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -191,20 +191,20 @@
 
         # Read the file
         content = read_file(filepath)
 
         if args.decrypt:
             data = decrypt_data(content)
             save_file(filepath, data)
-            print("Encrypt:", filepath)
+            print("Decrypt:", filepath)
 
         if args.encrypt:
             data = encrypt_data(args.user, content)
             save_file(filepath, data)
-            print("Decrypt:", filepath)
+            print("Encrypt:", filepath)
 
         if args.decrypt == False and args.encrypt == False:
             pattern = re.compile(rf"{_MARKUP}")
             match = pattern.search(str(content))
             if match is None:
                 data = encrypt_data(args.user, content)
                 save_file(filepath, data)
```

### Comparing `pyenv-encrypt-0.0.1/pyenv_encrypt.egg-info/PKG-INFO` & `pyenv-encrypt-0.1.0/pyenv_encrypt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenv-encrypt
-Version: 0.0.1
+Version: 0.1.0
 Summary: GPG based env file encryptor utility.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/pyenv-encrypt
 Project-URL: Bug Tracker, https://github.com/akhlakm/pyenv-encrypt/issues
 Keywords: encryption,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -34,24 +34,25 @@
     - .env
     - yaml
     - json
 - Recursive update of all text fields.
 - Automatic decision of encryption or decryption based on file contents.
 
 ## Installation
-To use, clone this repo and install with `pip`.
+You can install `pyenv-encrypt` directly from [PyPI](https://pypi.org/project/pyenv-encrypt) using `pip`.
+
 ```sh
-git clone git+https://github.com/akhlakm/pyenv-encrypt.git
-cd pyenv-encrypt
-pip install -e .
+pip install pyenv-encrypt
 ```
 
-Alternatively, use the following for packaging (for example, in your `requirements.txt` file).
+Alternatively, clone this repo and install with `pip`.
 ```sh
-pip install git+https://github.com/akhlakm/pyenv-encrypt.git
+git clone https://github.com/akhlakm/pyenv-encrypt.git
+cd pyenv-encrypt
+pip install -e .
 ```
 
 ### Dependencies
 The `gpg` utility must be installed in your system. GPG comes built-in with most versions of Linux OS. For Mac, use homebrew: `brew install gpg`.
 
 See the official [installation instructions](https://gnupg.org/download/) for more info. Run the following command to check if GPG is installed.
 
@@ -78,14 +79,16 @@
 
 `pyenc` will toggle between encryption and decryption. To force encryption or decryption specify `-e` or `-d` respectively.
 
 ```sh
 pyenc -e .env vault.yaml data.json
 ```
 
+To make sure you do not commit unencrypted files, you can setup a githook for your repository.
+See an [example pre-commit](pre-commit) file here.
 
 ## Use As A Python Module
 
 ```python
 import os
 from pyenv_enc import enc
```

### Comparing `pyenv-encrypt-0.0.1/pyproject.toml` & `pyenv-encrypt-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyenv-encrypt"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
     { name="Akhlak Mahmood", email="akhlakm@gatech.edu" },
 ]
 description = "GPG based env file encryptor utility."
 readme = "README.md"
 requires-python = ">=3.0"
```

