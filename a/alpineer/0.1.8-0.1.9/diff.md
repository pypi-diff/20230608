# Comparing `tmp/alpineer-0.1.8.tar.gz` & `tmp/alpineer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpineer-0.1.8.tar", max compression
+gzip compressed data, was "alpineer-0.1.9.tar", max compression
```

## Comparing `alpineer-0.1.8.tar` & `alpineer-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11845 2023-05-15 23:49:45.083226 alpineer-0.1.8/LICENSE
--rw-r--r--   0        0        0     5220 2023-05-15 23:49:45.083226 alpineer-0.1.8/README.md
--rw-r--r--   0        0        0     2758 2023-05-15 23:50:11.882977 alpineer-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/__init__.py
--rw-r--r--   0        0        0     1398 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/data_utils.py
--rw-r--r--   0        0        0      939 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/image_utils.py
--rw-r--r--   0        0        0     7760 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/io_utils.py
--rw-r--r--   0        0        0    22840 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/load_utils.py
--rw-r--r--   0        0        0     8209 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/misc_utils.py
--rw-r--r--   0        0        0        0 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/py.typed
--rw-r--r--   0        0        0      223 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/settings.py
--rw-r--r--   0        0        0    20206 2023-05-15 23:49:45.087226 alpineer-0.1.8/src/alpineer/test_utils.py
--rw-r--r--   0        0        0     5109 2023-05-15 23:49:45.087226 alpineer-0.1.8/src/alpineer/tiff_utils.py
--rw-r--r--   0        0        0     6298 1970-01-01 00:00:00.000000 alpineer-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11845 2023-06-08 20:52:51.457512 alpineer-0.1.9/LICENSE
+-rw-r--r--   0        0        0     5214 2023-06-08 20:52:51.457512 alpineer-0.1.9/README.md
+-rw-r--r--   0        0        0     2758 2023-06-08 20:53:14.261643 alpineer-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 20:52:51.457512 alpineer-0.1.9/src/alpineer/__init__.py
+-rw-r--r--   0        0        0     1398 2023-06-08 20:52:51.457512 alpineer-0.1.9/src/alpineer/data_utils.py
+-rw-r--r--   0        0        0      939 2023-06-08 20:52:51.457512 alpineer-0.1.9/src/alpineer/image_utils.py
+-rw-r--r--   0        0        0     7760 2023-06-08 20:52:51.457512 alpineer-0.1.9/src/alpineer/io_utils.py
+-rw-r--r--   0        0        0    22835 2023-06-08 20:52:51.457512 alpineer-0.1.9/src/alpineer/load_utils.py
+-rw-r--r--   0        0        0     8209 2023-06-08 20:52:51.457512 alpineer-0.1.9/src/alpineer/misc_utils.py
+-rw-r--r--   0        0        0        0 2023-06-08 20:52:51.457512 alpineer-0.1.9/src/alpineer/py.typed
+-rw-r--r--   0        0        0      223 2023-06-08 20:52:51.457512 alpineer-0.1.9/src/alpineer/settings.py
+-rw-r--r--   0        0        0    20206 2023-06-08 20:52:51.457512 alpineer-0.1.9/src/alpineer/test_utils.py
+-rw-r--r--   0        0        0     5109 2023-06-08 20:52:51.457512 alpineer-0.1.9/src/alpineer/tiff_utils.py
+-rw-r--r--   0        0        0     6282 1970-01-01 00:00:00.000000 alpineer-0.1.9/PKG-INFO
```

### Comparing `alpineer-0.1.8/LICENSE` & `alpineer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.8/README.md` & `alpineer-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Alpineer
 
 <div align="center">
 
 | | |
 | ---        |    ---  |
-| CI / CD | [![CI](https://github.com/angelolab/alpineer/actions/workflows/ci.yml/badge.svg)](https://github.com/angelolab/alpineer/actions/workflows/ci.yml) [![Coverage Status](https://coveralls.io/repos/github/angelolab/alpineer/badge.svg?branch=main)](https://coveralls.io/github/angelolab/mibi-bin-tools?branch=main) |
+| CI / CD | [![CI](https://github.com/angelolab/alpineer/actions/workflows/ci.yml/badge.svg)](https://github.com/angelolab/alpineer/actions/workflows/ci.yml) [![Coverage Status](https://coveralls.io/repos/github/angelolab/alpineer/badge.svg?branch=main)](https://coveralls.io/github/angelolab/alpineer?branch=main) |
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/alpineer.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/alpineer/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/alpineer.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold)](https://pypi.org/project/alpineer/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/alpineer.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/alpineer/) |
 |Meta | [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![PyPI - License](https://img.shields.io/pypi/l/alpineer?color=9400d3)](LICENSE) |
 </div>
 
 Toolbox for Multiplexed Imaging. Contains scripts and little tools which are used throughout [ark-analysis](https://github.com/angelolab/ark-analysis), [mibi-bin-tools](https://github.com/angelolab/mibi-bin-tools), and [toffy](https://github.com/angelolab/toffy)
 
 - [alpineer](#alpineer)
```

### Comparing `alpineer-0.1.8/pyproject.toml` & `alpineer-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alpineer"
-version = "0.1.8"
+version = "0.1.9"
 description = "Toolbox for Multiplexed Imaging. Contains scripts and little tools which are used throughout ark-analysis, mibi-bin-tools, and toffy."
 authors = [
     "Noah Frey Greenwald <nfgreen@stanford.edu>",
     "Adam Kagel <ackagel@stanford.edu>",
     "Alex Kong <alkong@stanford.edu>",
     "Cami Laura Sowers <csowers@stanford.edu>",
     "Sricharan Reddy Varra <srivarra@stanford.edu>",
```

### Comparing `alpineer-0.1.8/src/alpineer/data_utils.py` & `alpineer-0.1.9/src/alpineer/data_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.8/src/alpineer/image_utils.py` & `alpineer-0.1.9/src/alpineer/image_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.8/src/alpineer/io_utils.py` & `alpineer-0.1.9/src/alpineer/io_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.8/src/alpineer/load_utils.py` & `alpineer-0.1.9/src/alpineer/load_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -448,15 +448,15 @@
         tiled_names = list(fovs.keys())
     else:
         fov_list = fovs
         tiled_names = []
 
     # missing fov directories, read in a test image to get data type
     if single_dir:
-        test_path = os.path.join(data_dir, expected_fovs[0] + "_" + channel + "." + file_ext)
+        test_path = os.path.join(data_dir, fov_list[0] + "_" + channel + "." + file_ext)
     else:
         test_path = os.path.join(
             os.path.join(data_dir, fov_list[0], img_sub_folder, channel + "." + file_ext)
         )
     test_img = io.imread(test_path)
     img_data = np.zeros(
         (len(expected_fovs), test_img.shape[0], test_img.shape[1], 1), dtype=test_img.dtype
```

### Comparing `alpineer-0.1.8/src/alpineer/misc_utils.py` & `alpineer-0.1.9/src/alpineer/misc_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.8/src/alpineer/test_utils.py` & `alpineer-0.1.9/src/alpineer/test_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.8/src/alpineer/tiff_utils.py` & `alpineer-0.1.9/src/alpineer/tiff_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.8/PKG-INFO` & `alpineer-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: alpineer
-Version: 0.1.8
+Version: 0.1.9
 Summary: Toolbox for Multiplexed Imaging. Contains scripts and little tools which are used throughout ark-analysis, mibi-bin-tools, and toffy.
 Home-page: https://github.com/angelolab/tmi
 License: Modified Apache 2.0
 Author: Noah Frey Greenwald
 Author-email: nfgreen@stanford.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: charset-normalizer (>=2.1.1,<3.0.0)
 Requires-Dist: matplotlib (>=3,<4)
 Requires-Dist: natsort (>=8,<9)
-Requires-Dist: numpy (>=1.0.0,<2.0.0)
+Requires-Dist: numpy (==1.*)
 Requires-Dist: pillow (>=9,<10)
-Requires-Dist: scikit-image (<1.0.0)
+Requires-Dist: scikit-image (==0.*)
 Requires-Dist: tifffile
 Requires-Dist: xarray
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Documentation, https://tmi.readthedocs.io
 Project-URL: Repository, https://github.com/angelolab/tmi
 Description-Content-Type: text/markdown
 
 # Alpineer
 
 <div align="center">
 
 | | |
 | ---        |    ---  |
-| CI / CD | [![CI](https://github.com/angelolab/alpineer/actions/workflows/ci.yml/badge.svg)](https://github.com/angelolab/alpineer/actions/workflows/ci.yml) [![Coverage Status](https://coveralls.io/repos/github/angelolab/alpineer/badge.svg?branch=main)](https://coveralls.io/github/angelolab/mibi-bin-tools?branch=main) |
+| CI / CD | [![CI](https://github.com/angelolab/alpineer/actions/workflows/ci.yml/badge.svg)](https://github.com/angelolab/alpineer/actions/workflows/ci.yml) [![Coverage Status](https://coveralls.io/repos/github/angelolab/alpineer/badge.svg?branch=main)](https://coveralls.io/github/angelolab/alpineer?branch=main) |
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/alpineer.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/alpineer/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/alpineer.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold)](https://pypi.org/project/alpineer/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/alpineer.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/alpineer/) |
 |Meta | [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![PyPI - License](https://img.shields.io/pypi/l/alpineer?color=9400d3)](LICENSE) |
 </div>
 
 Toolbox for Multiplexed Imaging. Contains scripts and little tools which are used throughout [ark-analysis](https://github.com/angelolab/ark-analysis), [mibi-bin-tools](https://github.com/angelolab/mibi-bin-tools), and [toffy](https://github.com/angelolab/toffy)
 
 - [alpineer](#alpineer)
```

