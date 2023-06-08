# Comparing `tmp/pyttb-1.6.1.tar.gz` & `tmp/pyttb-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyttb-1.6.1.tar", last modified: Thu Apr 27 15:01:50 2023, max compression
+gzip compressed data, was "pyttb-1.6.2.tar", last modified: Thu Jun  8 20:40:51 2023, max compression
```

## Comparing `pyttb-1.6.1.tar` & `pyttb-1.6.2.tar`

### file list

```diff
@@ -1,47 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:01:50.288733 pyttb-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-27 15:01:19.000000 pyttb-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-27 15:01:50.288733 pyttb-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-27 15:01:19.000000 pyttb-1.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:01:50.284733 pyttb-1.6.1/pyttb/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/cp_als.py
--rw-r--r--   0 runner    (1001) docker     (123)    58614 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/cp_apr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/export_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/hosvd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/import_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/khatrirao.py
--rw-r--r--   0 runner    (1001) docker     (123)    80311 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/ktensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21785 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/pyttb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/sptenmat.py
--rw-r--r--   0 runner    (1001) docker     (123)    93748 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/sptensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/sptensor3.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/sumtensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/symktensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/symtensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14833 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/tenmat.py
--rw-r--r--   0 runner    (1001) docker     (123)    60229 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/ttensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-27 15:01:19.000000 pyttb-1.6.1/pyttb/tucker_als.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:01:50.284733 pyttb-1.6.1/pyttb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-27 15:01:50.000000 pyttb-1.6.1/pyttb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-27 15:01:50.000000 pyttb-1.6.1/pyttb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:01:50.000000 pyttb-1.6.1/pyttb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-27 15:01:50.000000 pyttb-1.6.1/pyttb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 15:01:50.000000 pyttb-1.6.1/pyttb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:01:50.288733 pyttb-1.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:01:50.288733 pyttb-1.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_cp_als.py
--rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_cp_apr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_hosvd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_import_export_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_khatrirao.py
--rw-r--r--   0 runner    (1001) docker     (123)    42650 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_ktensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    16756 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_pyttb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68449 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_sptensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_tenmat.py
--rw-r--r--   0 runner    (1001) docker     (123)    57951 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_ttensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-27 15:01:19.000000 pyttb-1.6.1/tests/test_tucker_als.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:40:51.594371 pyttb-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-08 20:40:29.000000 pyttb-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-08 20:40:51.594371 pyttb-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-08 20:40:29.000000 pyttb-1.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:40:51.590371 pyttb-1.6.2/pyttb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/cp_als.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58992 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/cp_apr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/export_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/hosvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/import_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/khatrirao.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81352 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/ktensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21786 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/pyttb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/sptenmat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93809 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/sptensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/sptensor3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/sumtensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/symktensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/symtensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/tenmat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62163 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18296 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/ttensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-08 20:40:29.000000 pyttb-1.6.2/pyttb/tucker_als.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:40:51.590371 pyttb-1.6.2/pyttb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-08 20:40:51.000000 pyttb-1.6.2/pyttb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-08 20:40:51.000000 pyttb-1.6.2/pyttb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:40:51.000000 pyttb-1.6.2/pyttb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 20:40:51.000000 pyttb-1.6.2/pyttb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 20:40:51.000000 pyttb-1.6.2/pyttb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:40:51.594371 pyttb-1.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:40:51.594371 pyttb-1.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_cp_als.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_cp_apr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_hosvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_import_export_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_khatrirao.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44033 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_ktensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16756 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_pyttb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_sptenmat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69373 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_sptensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_sptensor3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_sumtensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_symktensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_symtensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_tenmat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59738 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_ttensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-08 20:40:29.000000 pyttb-1.6.2/tests/test_tucker_als.py
```

### Comparing `pyttb-1.6.1/LICENSE` & `pyttb-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.1/PKG-INFO` & `pyttb-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttb
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python Tensor Toolbox
 Author-email: "Daniel M. Dunlavy" <dmdunla@sandia.gov>
 License: BSD 2-Clause License
 Project-URL: homepage, https://github.com/sandialabs/pyttb
 Project-URL: coverage, https://coveralls.io/github/sandialabs/pyttb
 Project-URL: documentation, https://pyttb.readthedocs.io
 Classifier: License :: OSI Approved :: BSD License
@@ -39,11 +39,11 @@
 * `cp_als`, `cp_apr`: Canonical Polyadic (CP) decompositions
 * `tucker_als`: Tucker decompostions
 
 # Getting Started
 Check out the [Documentation](https://pyttb.readthedocs.io) to get started.
 
 # Contributing
-Check out our [contributing guide](CONTRIBUTOR_GUIDE.md).
+Check out our [contributing guide](CONTRIBUTING.md).
 
 ---
 [![Regression tests](https://github.com/sandialabs/pyttb/actions/workflows/regression-tests.yml/badge.svg)](https://github.com/sandialabs/pyttb/actions/workflows/regression-tests.yml) [![Coverage Status](https://coveralls.io/repos/github/sandialabs/pyttb/badge.svg?branch=main)](https://coveralls.io/github/sandialabs/pyttb?branch=main)
```

### Comparing `pyttb-1.6.1/README.md` & `pyttb-1.6.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -47,31 +47,30 @@
 000002e0: 2074 6865 205b 446f 6375 6d65 6e74 6174   the [Documentat
 000002f0: 696f 6e5d 2868 7474 7073 3a2f 2f70 7974  ion](https://pyt
 00000300: 7462 2e72 6561 6474 6865 646f 6373 2e69  tb.readthedocs.i
 00000310: 6f29 2074 6f20 6765 7420 7374 6172 7465  o) to get starte
 00000320: 642e 0a0a 2320 436f 6e74 7269 6275 7469  d...# Contributi
 00000330: 6e67 0a43 6865 636b 206f 7574 206f 7572  ng.Check out our
 00000340: 205b 636f 6e74 7269 6275 7469 6e67 2067   [contributing g
-00000350: 7569 6465 5d28 434f 4e54 5249 4255 544f  uide](CONTRIBUTO
-00000360: 525f 4755 4944 452e 6d64 292e 0a0a 2d2d  R_GUIDE.md)...--
-00000370: 2d0a 5b21 5b52 6567 7265 7373 696f 6e20  -.[![Regression 
-00000380: 7465 7374 735d 2868 7474 7073 3a2f 2f67  tests](https://g
-00000390: 6974 6875 622e 636f 6d2f 7361 6e64 6961  ithub.com/sandia
-000003a0: 6c61 6273 2f70 7974 7462 2f61 6374 696f  labs/pyttb/actio
-000003b0: 6e73 2f77 6f72 6b66 6c6f 7773 2f72 6567  ns/workflows/reg
-000003c0: 7265 7373 696f 6e2d 7465 7374 732e 796d  ression-tests.ym
-000003d0: 6c2f 6261 6467 652e 7376 6729 5d28 6874  l/badge.svg)](ht
-000003e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000003f0: 2f73 616e 6469 616c 6162 732f 7079 7474  /sandialabs/pytt
-00000400: 622f 6163 7469 6f6e 732f 776f 726b 666c  b/actions/workfl
-00000410: 6f77 732f 7265 6772 6573 7369 6f6e 2d74  ows/regression-t
-00000420: 6573 7473 2e79 6d6c 2920 5b21 5b43 6f76  ests.yml) [![Cov
-00000430: 6572 6167 6520 5374 6174 7573 5d28 6874  erage Status](ht
-00000440: 7470 733a 2f2f 636f 7665 7261 6c6c 732e  tps://coveralls.
-00000450: 696f 2f72 6570 6f73 2f67 6974 6875 622f  io/repos/github/
-00000460: 7361 6e64 6961 6c61 6273 2f70 7974 7462  sandialabs/pyttb
-00000470: 2f62 6164 6765 2e73 7667 3f62 7261 6e63  /badge.svg?branc
-00000480: 683d 6d61 696e 295d 2868 7474 7073 3a2f  h=main)](https:/
-00000490: 2f63 6f76 6572 616c 6c73 2e69 6f2f 6769  /coveralls.io/gi
-000004a0: 7468 7562 2f73 616e 6469 616c 6162 732f  thub/sandialabs/
-000004b0: 7079 7474 623f 6272 616e 6368 3d6d 6169  pyttb?branch=mai
-000004c0: 6e29 0a                                  n).
+00000350: 7569 6465 5d28 434f 4e54 5249 4255 5449  uide](CONTRIBUTI
+00000360: 4e47 2e6d 6429 2e0a 0a2d 2d2d 0a5b 215b  NG.md)...---.[![
+00000370: 5265 6772 6573 7369 6f6e 2074 6573 7473  Regression tests
+00000380: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000390: 2e63 6f6d 2f73 616e 6469 616c 6162 732f  .com/sandialabs/
+000003a0: 7079 7474 622f 6163 7469 6f6e 732f 776f  pyttb/actions/wo
+000003b0: 726b 666c 6f77 732f 7265 6772 6573 7369  rkflows/regressi
+000003c0: 6f6e 2d74 6573 7473 2e79 6d6c 2f62 6164  on-tests.yml/bad
+000003d0: 6765 2e73 7667 295d 2868 7474 7073 3a2f  ge.svg)](https:/
+000003e0: 2f67 6974 6875 622e 636f 6d2f 7361 6e64  /github.com/sand
+000003f0: 6961 6c61 6273 2f70 7974 7462 2f61 6374  ialabs/pyttb/act
+00000400: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f72  ions/workflows/r
+00000410: 6567 7265 7373 696f 6e2d 7465 7374 732e  egression-tests.
+00000420: 796d 6c29 205b 215b 436f 7665 7261 6765  yml) [![Coverage
+00000430: 2053 7461 7475 735d 2868 7474 7073 3a2f   Status](https:/
+00000440: 2f63 6f76 6572 616c 6c73 2e69 6f2f 7265  /coveralls.io/re
+00000450: 706f 732f 6769 7468 7562 2f73 616e 6469  pos/github/sandi
+00000460: 616c 6162 732f 7079 7474 622f 6261 6467  alabs/pyttb/badg
+00000470: 652e 7376 673f 6272 616e 6368 3d6d 6169  e.svg?branch=mai
+00000480: 6e29 5d28 6874 7470 733a 2f2f 636f 7665  n)](https://cove
+00000490: 7261 6c6c 732e 696f 2f67 6974 6875 622f  ralls.io/github/
+000004a0: 7361 6e64 6961 6c61 6273 2f70 7974 7462  sandialabs/pyttb
+000004b0: 3f62 7261 6e63 683d 6d61 696e 290a       ?branch=main).
```

### Comparing `pyttb-1.6.1/pyproject.toml` & `pyttb-1.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.1/pyttb/__init__.py` & `pyttb-1.6.2/pyttb/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright 2022 National Technology & Engineering Solutions of Sandia,
 # LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 # U.S. Government retains certain rights in this software.
 
-__version__ = "1.6.1"
+__version__ = "1.6.2"
 
 import warnings
 
 from pyttb.cp_als import cp_als
 from pyttb.cp_apr import *
 from pyttb.export_data import export_data
 from pyttb.hosvd import hosvd
```

### Comparing `pyttb-1.6.1/pyttb/cp_als.py` & `pyttb-1.6.2/pyttb/cp_als.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,42 +5,42 @@
 import numpy as np
 
 import pyttb as ttb
 from pyttb.pyttb_utils import *
 
 
 def cp_als(
-    tensor,
+    input_tensor,
     rank,
     stoptol=1e-4,
     maxiters=1000,
     dimorder=None,
     init="random",
     printitn=1,
     fixsigns=True,
 ):
     """
     Compute CP decomposition with alternating least squares
 
     Parameters
     ----------
-    tensor: :class:`pyttb.tensor` or :class:`pyttb.sptensor` or :class:`pyttb.ktensor`
+    input_tensor: :class:`pyttb.tensor` or :class:`pyttb.sptensor` or :class:`pyttb.ktensor`
     rank: int
         Rank of the decomposition
     stoptol: float
         Tolerance used for termination - when the change in the fitness function in successive iterations drops
         below this value, the iterations terminate (default: 1e-4)
     dimorder: list
         Order to loop through dimensions (default: [range(tensor.ndims)])
     maxiters: int
         Maximum number of iterations (default: 1000)
     init: str or :class:`pyttb.ktensor`
         Initial guess (default: "random")
 
-             * "random": initialize using a :class:`pyttb.ktensor` with values chosen from a Normal distribution with mean 1 and standard deviation 0
+             * "random": initialize using a :class:`pyttb.ktensor` with values chosen from a Normal distribution with mean 0 and standard deviation 1
              * "nvecs": initialize factor matrices of a :class:`pyttb.ktensor` using the eigenvectors of the outer product of the matricized input tensor
              * :class:`pyttb.ktensor`: initialize using a specific :class:`pyttb.ktensor` as input - must be the same shape as the input tensor and have the same rank as the input rank
 
     printitn: int
         Number of iterations to perform before printing iteration status - 0 for no status printing (default: 1)
     fixsigns: bool
         Align the signs of the columns of the factorization to align with the input tensor data (default: True)
@@ -110,16 +110,16 @@
     CP_ALS:
      Iter 0: f = ... f-delta = ...
      Iter 1: f = ... f-delta = ...
      Final f = ...
     """
 
     # Extract number of dimensions and norm of tensor
-    N = tensor.ndims
-    normX = tensor.norm()
+    N = input_tensor.ndims
+    normX = input_tensor.norm()
 
     # Set up dimorder if not specified
     if not dimorder:
         dimorder = list(range(N))
     else:
         if not isinstance(dimorder, list):
             assert False, "Dimorder must be a list"
@@ -135,35 +135,37 @@
     if isinstance(init, ttb.ktensor):
         # User provided an initial ktensor; validate it
         assert init.ndims == N, "Initial guess does not have {} modes".format(N)
         assert (
             init.ncomponents == rank
         ), "Initial guess does not have {} components".format(rank)
         for n in dimorder:
-            if init.factor_matrices[n].shape != (tensor.shape[n], rank):
+            if init.factor_matrices[n].shape != (input_tensor.shape[n], rank):
                 assert False, "Mode {} of the initial guess is the wrong size".format(n)
     elif isinstance(init, str) and init.lower() == "random":
         factor_matrices = []
         for n in range(N):
-            factor_matrices.append(np.random.uniform(0, 1, (tensor.shape[n], rank)))
+            factor_matrices.append(
+                np.random.uniform(0, 1, (input_tensor.shape[n], rank))
+            )
         init = ttb.ktensor.from_factor_matrices(factor_matrices)
     elif isinstance(init, str) and init.lower() == "nvecs":
         factor_matrices = []
         for n in range(N):
-            factor_matrices.append(tensor.nvecs(n, rank))
+            factor_matrices.append(input_tensor.nvecs(n, rank))
         init = ttb.ktensor.from_factor_matrices(factor_matrices)
     else:
         assert False, "The selected initialization method is not supported"
 
     # Set up for iterates and fit
     U = init.copy().factor_matrices
     fit = 0
 
     # Store the last MTTKRP result to accelerate fitness computation
-    U_mttkrp = np.zeros((tensor.shape[dimorder[-1]], rank))
+    U_mttkrp = np.zeros((input_tensor.shape[dimorder[-1]], rank))
 
     if printitn > 0:
         print("CP_ALS:")
 
     # Main Loop: Iterate until convergence
 
     UtU = np.zeros((rank, rank, N))
@@ -172,15 +174,15 @@
 
     for iter in range(maxiters):
         fitold = fit
 
         # Iterate over all N modes of the tensor
         for n in dimorder:
             # Calculate Unew = X_(n) * khatrirao(all U except n, 'r').
-            Unew = tensor.mttkrp(U, n)
+            Unew = input_tensor.mttkrp(U, n)
 
             # Save the last MTTKRP result for fitness check.
             if n == dimorder[-1]:
                 U_mttkrp = Unew
 
             # Compute the matrix of coefficients for linear system
             Y = np.prod(UtU, axis=2, where=[i != n for i in range(N)])
@@ -241,19 +243,19 @@
     M.arrange()
     # Fix the signs if requested
     if fixsigns:
         M = M.fixsigns()
 
     if printitn > 0:
         if normX == 0:
-            normresidual = M.norm() ** 2 - 2 * tensor.innerprod(M)
+            normresidual = M.norm() ** 2 - 2 * input_tensor.innerprod(M)
             fit = normresidual
         else:
             normresidual = np.sqrt(
-                np.abs(normX**2 + M.norm() ** 2 - 2 * tensor.innerprod(M))
+                np.abs(normX**2 + M.norm() ** 2 - 2 * input_tensor.innerprod(M))
             )
             fit = 1 - (normresidual / normX)  # fraction explained by model
         print(f" Final f = {fit:e}")
 
     output = {}
     output["params"] = (stoptol, maxiters, printitn, dimorder)
     output["iters"] = iter
```

### Comparing `pyttb-1.6.1/pyttb/cp_apr.py` & `pyttb-1.6.2/pyttb/cp_apr.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import pyttb as ttb
 
 from .pyttb_utils import *
 
 
 def cp_apr(
-    tensor,
+    input_tensor,
     rank,
     algorithm="mu",
     stoptol=1e-4,
     stoptime=1e6,
     maxiters=1000,
     init="random",
     maxinneriters=10,
@@ -34,15 +34,15 @@
     lbfgsMem=3,
 ):
     """
     Compute non-negative CP with alternating Poisson regression.
 
     Parameters
     ----------
-    tensor: :class:`pyttb.tensor` or :class:`pyttb.sptensor`
+    input_tensor: :class:`pyttb.tensor` or :class:`pyttb.sptensor`
     rank: int
         Rank of the decomposition
     algorithm: str
         in {'mu', 'pdnr, 'pqnr'}
     stoptol: float
         Tolerance on overall KKT violation
     stoptime: float
@@ -81,49 +81,51 @@
     Minit: :class:`pyttb.ktensor`
         Initial Guess
     output: dict
         Additional output #TODO document this more appropriately
 
     """
     # Extract the number of modes in tensor X
-    N = tensor.ndims
+    N = input_tensor.ndims
 
     assert rank > 0, "Number of components requested must be positive"
 
     # Check that the data is non-negative.
-    tmp = tensor < 0.0
+    tmp = input_tensor < 0.0
     assert (
         tmp.nnz == 0
     ), "Data tensor must be nonnegative for Poisson-based factorization"
 
     # Set up an initial guess for the factor matrices.
     if isinstance(init, ttb.ktensor):
         # User provided an initial ktensor; validate it
         assert init.ndims == N, "Initial guess does not have the right number of modes"
         assert (
             init.ncomponents == rank
         ), "Initial guess does not have the right number of componenets"
         for n in range(N):
-            if init.shape[n] != tensor.shape[n]:
+            if init.shape[n] != input_tensor.shape[n]:
                 assert False, "Mode {} of the initial guess is the wrong size".format(n)
             if np.min(init.factor_matrices[n]) < 0.0:
                 assert False, "Initial guess has negative element in mode {}".format(n)
         if np.min(init.weights) < 0:
             assert False, "Initial guess has a negative ktensor weight"
 
     elif init.lower() == "random":
         factor_matrices = []
         for n in range(N):
-            factor_matrices.append(np.random.uniform(0, 1, (tensor.shape[n], rank)))
+            factor_matrices.append(
+                np.random.uniform(0, 1, (input_tensor.shape[n], rank))
+            )
         init = ttb.ktensor.from_factor_matrices(factor_matrices)
 
     # Call solver based on the couce of algorithm parameter, passing all the other input parameters
     if algorithm.lower() == "mu":
         M, output = tt_cp_apr_mu(
-            tensor,
+            input_tensor,
             rank,
             init,
             stoptol,
             stoptime,
             maxiters,
             maxinneriters,
             epsDivZero,
@@ -131,15 +133,15 @@
             printinneritn,
             kappa,
             kappatol,
         )
         output["algorithm"] = "mu"
     elif algorithm.lower() == "pdnr":
         M, output = tt_cp_apr_pdnr(
-            tensor,
+            input_tensor,
             rank,
             init,
             stoptol,
             stoptime,
             maxiters,
             maxinneriters,
             epsDivZero,
@@ -149,15 +151,15 @@
             mu0,
             precompinds,
             inexact,
         )
         output["algorithm"] = "pdnr"
     elif algorithm.lower() == "pqnr":
         M, output = tt_cp_apr_pqnr(
-            tensor,
+            input_tensor,
             rank,
             init,
             stoptol,
             stoptime,
             maxiters,
             maxinneriters,
             epsDivZero,
@@ -171,15 +173,15 @@
     else:
         assert False, "{} is not a supported cp_als algorithm".format(algorithm)
 
     return M, init, output
 
 
 def tt_cp_apr_mu(
-    tensor,
+    input_tensor,
     rank,
     init,
     stoptol,
     stoptime,
     maxiters,
     maxinneriters,
     epsDivZero,
@@ -189,15 +191,15 @@
     kappatol,
 ):
     """
     Compute nonnegative CP with alternating Poisson regression.
 
     Parameters
     ----------
-    tensor: :class:`pyttb.tensor` or :class:`pyttb.sptensor`
+    input_tensor: :class:`pyttb.tensor` or :class:`pyttb.sptensor`
     rank: int
         Rank of the decomposition
     init: :class:`pyttb.ktensor`
         Initial guess
     stoptol: float
         Tolerance on overall KKT violation
     stoptime: float
@@ -223,15 +225,15 @@
     Notes
     -----
     REFERENCE: E. C. Chi and T. G. Kolda. On Tensors, Sparsity, and
     Nonnegative Factorizations, arXiv:1112.2414 [math.NA], December 2011,
     URL: http://arxiv.org/abs/1112.2414. Submitted for publication.
 
     """
-    N = tensor.ndims
+    N = input_tensor.ndims
 
     # TODO I vote no duplicate error checking, copy error checking from cp_apr for initial guess here if disagree
 
     # Initialize output arrays
     # fnEvals = np.zeros((maxiters,))
     kktViolations = -np.ones((maxiters,))
     # TODO we initialize nInnerIters of size max outer iters?
@@ -247,15 +249,15 @@
     Phi = []  # np.zeros((N,))#cell(N,1)
     for n in range(N):
         # TODO prepopulation Phi instead of appen should be faster
         Phi.append(np.zeros(M[n].shape))
     kktModeViolations = np.zeros((N,))
 
     if printitn > 0:
-        print("\nCP_APR:\n")
+        print("CP_APR:")
 
     # Start the wall clock timer.
     start = time.time()
 
     # PDN-R and PQN-R benefit from precomputing sparse indices of X for each mode subproblem.
     # However, MU execution time barely changes, so the precomputer option is not offered.
 
@@ -272,23 +274,23 @@
                     M.factor_matrices[n][V > 0] += kappa
 
             # Shift the weight from lambda to mode n
             M.redistribute(mode=n)
 
             # Calculate product of all matrices but the n-th
             # Sparse case only calculates entries corresponding to nonzeros in X
-            Pi = calculatePi(tensor, M, rank, n, N)
+            Pi = calculatePi(input_tensor, M, rank, n, N)
 
             # Do the multiplicative updates
             for i in range(maxinneriters):
                 # Count the inner iterations
                 nInnerIters[iter] += 1
 
                 # Calculate matrix for multiplicative update
-                Phi[n] = calculatePhi(tensor, M, rank, n, Pi, epsDivZero)
+                Phi[n] = calculatePhi(input_tensor, M, rank, n, Pi, epsDivZero)
 
                 # Check for convergence
                 kktModeViolations[n] = np.max(
                     np.abs(vectorizeForMu(np.minimum(M.factor_matrices[n], 1 - Phi[n])))
                 )
                 if kktModeViolations[n] < stoptol:
                     break
@@ -298,15 +300,15 @@
                 # Do the multiplicative update
                 # TODO cannot update M[n] in this way
                 M.factor_matrices[n] *= Phi[n]
 
                 # Print status
                 if printinneritn != 0 and divmod(i, printinneritn)[1] == 0:
                     print(
-                        "\t\tMode = {}, Inner Iter = {}, KKT violation = {}\n".format(
+                        "\t\tMode = {}, Inner Iter = {}, KKT violation = {}".format(
                             n, i, kktModeViolations[n]
                         )
                     )
 
             # Shift weight from mode n back to lambda
             M.normalize(normtype=1, mode=n)
 
@@ -319,40 +321,40 @@
             )
 
         nTimes[iter] = time.time() - start
 
         # Check for convergence
         if isConverged:
             if printitn > 0:
-                print("Exiting because all subproblems reached KKT tol.\n")
+                print("Exiting because all subproblems reached KKT tol.")
             break
         if nTimes[iter] > stoptime:
             if printitn > 0:
-                print("Exiting because time limit exceeded.\n")
+                print("Exiting because time limit exceeded.")
             break
 
     t_stop = time.time() - start
 
     # Clean up final result
     M.normalize(sort=True, normtype=1)
 
-    obj = tt_loglikelihood(tensor, M)
+    obj = tt_loglikelihood(input_tensor, M)
 
     if printitn > 0:
-        normTensor = tensor.norm()
+        normTensor = input_tensor.norm()
         normresidual = np.sqrt(
-            normTensor**2 + M.norm() ** 2 - 2 * tensor.innerprod(M)
+            normTensor**2 + M.norm() ** 2 - 2 * input_tensor.innerprod(M)
         )
         fit = 1 - (normresidual / normTensor)  # fraction explained by model
-        print("===========================================\n")
-        print(" Final log-likelihood = {} \n".format(obj))
-        print(" Final least squares fit = {} \n".format(fit))
-        print(" Final KKT violation = {}\n".format(kktViolations[iter]))
-        print(" Total inner iterations = {}\n".format(sum(nInnerIters)))
-        print(" Total execution time = {} secs\n".format(t_stop))
+        print("===========================================")
+        print(" Final log-likelihood = {}".format(obj))
+        print(" Final least squares fit = {}".format(fit))
+        print(" Final KKT violation = {}".format(kktViolations[iter]))
+        print(" Total inner iterations = {}".format(sum(nInnerIters)))
+        print(" Total execution time = {} secs".format(t_stop))
 
     output = {}
     output["params"] = (
         stoptol,
         stoptime,
         maxiters,
         maxinneriters,
@@ -370,15 +372,15 @@
     output["totalTime"] = t_stop
     output["obj"] = obj
 
     return M, output
 
 
 def tt_cp_apr_pdnr(
-    tensor,
+    input_tensor,
     rank,
     init,
     stoptol,
     stoptime,
     maxiters,
     maxinneriters,
     epsDivZero,
@@ -395,15 +397,15 @@
     CP model of a tensor X using an alternating Poisson regression.
     The algorithm solves "row subproblems" in each alternating subproblem,
     using a Hessian of size R^2.
 
     Parameters
     ----------
     # TODO it looks like this method of define union helps the typ hinting better than or
-    tensor: Union[:class:`pyttb.tensor`,:class:`pyttb.sptensor`]
+    input_tensor: Union[:class:`pyttb.tensor`,:class:`pyttb.sptensor`]
     rank: int
         Rank of the decomposition
     init: str or :class:`pyttb.ktensor`
         Initial guess
     stoptol: float
         Tolerance on overall KKT violation
     stoptime: float
@@ -436,15 +438,15 @@
     REFERENCE: Samantha Hansen, Todd Plantenga, Tamara G. Kolda.
     Newton-Based Optimization for Nonnegative Tensor Factorizations,
     arXiv:1304.4964 [math.NA], April 2013,
     URL: http://arxiv.org/abs/1304.4964. Submitted for publication.
 
     """
     # Extract the number of modes in tensor X
-    N = tensor.ndims
+    N = input_tensor.ndims
 
     # If the initial guess has any rows of all zero elements, then modify so the row subproblem is not taking log(0).
     # Values will be restored to zero later if the unfolded X for the row has no zeros.
     for n in range(N):
         rowsum = np.sum(init[n], axis=1)
         tmpIdx = np.where(rowsum == 0)[0]
         if tmpIdx.size != 0:
@@ -452,29 +454,29 @@
 
     # Start with the initial guess, normalized using the vector L1 norm
     # TODO replace with copy
     M = ttb.ktensor.from_tensor_type(init)
     M.normalize(normtype=1)
 
     # Sparse tensor flag affects how Pi and Phi are computed.
-    if isinstance(tensor, ttb.sptensor):
+    if isinstance(input_tensor, ttb.sptensor):
         isSparse = True
     else:
         isSparse = False
 
     # Initialize output arrays
     fnEvals = np.zeros((maxiters, 1))
     fnVals = np.zeros((maxiters, 1))
     kktViolations = -np.ones((maxiters, 1))
     nInnerIters = np.zeros((maxiters, 1))
     nzeros = np.zeros((maxiters, 1))
     times = np.zeros((maxiters, 1))
 
     if printitn > 0:
-        print("\nCP_PDNR (alternating Poisson regression using damped Newton)\n")
+        print("CP_PDNR (alternating Poisson regression using damped Newton)")
 
     dispLineWarn = printinneritn > 0
 
     # Start the wall clock timer.
     start = time.time()
 
     if isSparse and precompinds:
@@ -483,19 +485,19 @@
         if printitn > 0:
             print("\tPrecomuting sparse index sets...")
         sparseIx = []
         for n in range(N):
             num_rows = M[n].shape[0]
             row_indices = []
             for jj in range(num_rows):
-                row_indices.append(np.where(tensor.subs[:, n] == jj)[0])
+                row_indices.append(np.where(input_tensor.subs[:, n] == jj)[0])
             sparseIx.append(row_indices)
 
         if printitn > 0:
-            print("done\n")
+            print("done")
 
     e_vec = np.ones((1, rank))
 
     rowsubprobStopTol = stoptol
 
     # Main loop: iterate until convergence or a max threshold is reached
     for iter in range(maxiters):
@@ -507,43 +509,43 @@
         for n in range(N):
             # Shift the weight from lambda to mode n.
             M.redistribute(mode=n)
 
             # calculate khatri-rao product of all matrices but the n-th
             if isSparse == False:
                 # Data is not a sparse tensor.
-                Pi = ttb.tt_calcpi_prowsubprob(tensor, M, rank, n, N, isSparse)
-                X_mat = ttb.tt_to_dense_matrix(tensor, n)
+                Pi = ttb.tt_calcpi_prowsubprob(input_tensor, M, rank, n, N, isSparse)
+                X_mat = ttb.tt_to_dense_matrix(input_tensor, n)
 
             num_rows = M[n].shape[0]
             isRowNOTconverged = np.zeros((num_rows,))
 
             # Loop over the row subproblems in mode n.
             for jj in range(num_rows):
                 # Initialize the damped Hessian parameter for the row subproblem.
                 mu = mu0
 
                 # Get data values for row jj of matricized mode n,
                 if isSparse:
                     # Data is a sparse tensor
                     if not precompinds:
-                        sparse_indices = np.where(tensor.subs[:, n] == jj)[0]
+                        sparse_indices = np.where(input_tensor.subs[:, n] == jj)[0]
                     else:
                         sparse_indices = sparseIx[n][jj]
 
                     if sparse_indices.size == 0:
                         # The row jj of matricized tensor X in mode n is empty
                         M.factor_matrices[n][jj, :] = 0
                         continue
 
-                    x_row = tensor.vals[sparse_indices]
+                    x_row = input_tensor.vals[sparse_indices]
 
                     # Calculate just the columns of Pi needed for this row.
                     Pi = ttb.tt_calcpi_prowsubprob(
-                        tensor, M, rank, n, N, isSparse, sparse_indices
+                        input_tensor, M, rank, n, N, isSparse, sparse_indices
                     )
 
                 else:
                     x_row = X_mat[jj, :]
 
                 # Get current values of the row subproblem variables.
                 m_row = M[n][jj, :]
@@ -572,21 +574,24 @@
                     )
 
                     # Report largest row subproblem initial violation
                     if i == 0 and kkt_violation > kktModeViolations[n]:
                         kktModeViolations[n] = kkt_violation
 
                     if printinneritn > 0 and np.mod(i, printinneritn) == 0:
-                        print("\tMode = {}, Row = {}, InnerIt = {}".format(n, jj, i))
+                        print(
+                            "\tMode = {}, Row = {}, InnerIt = {}".format(n, jj, i),
+                            end="",
+                        )
 
                         if i == 0:
-                            print(", RowKKT = {}\n".format(kkt_violation))
+                            print(", RowKKT = {}".format(kkt_violation))
                         else:
                             print(
-                                ", RowKKT = {}, RowObj = {}\n".format(
+                                ", RowKKT = {}, RowObj = {}".format(
                                     kkt_violation, -f_new
                                 )
                             )
 
                     # Check for row subproblem convergence.
                     if kkt_violation < stoptol:
                         break
@@ -659,17 +664,17 @@
         kktViolations[iter] = np.max(kktModeViolations)
 
         if inexact:
             rowsubprobStopTol = np.maximum(stoptol, kktViolations[iter]) / 100.0
 
             # Print outer iteration status.
             if printitn > 0 and np.mod(iter, printitn) == 0:
-                fnVals[iter] = -tt_loglikelihood(tensor, M)
+                fnVals[iter] = -tt_loglikelihood(input_tensor, M)
                 print(
-                    "{}. Ttl Inner Its: {}, KKT viol = {}, obj = {}, nz: {}\n".format(
+                    "{}. Ttl Inner Its: {}, KKT viol = {}, obj = {}, nz: {}".format(
                         iter,
                         nInnerIters[iter],
                         kktViolations[iter],
                         fnVals[iter],
                         num_zero,
                     )
                 )
@@ -678,36 +683,36 @@
 
         # Check for convergence
         if isConverged and inexact == False:
             break
         if isConverged and inexact and rowsubprobStopTol <= stoptol:
             break
         if times[iter] > stoptime:
-            print("EXiting because time limit exceeded\n")
+            print("EXiting because time limit exceeded")
             break
 
     t_stop = time.time() - start
 
     # Clean up final result
     M.normalize(sort=True, normtype=1)
 
-    obj = tt_loglikelihood(tensor, M)
+    obj = tt_loglikelihood(input_tensor, M)
 
     if printitn > 0:
-        normTensor = tensor.norm()
+        normTensor = input_tensor.norm()
         normresidual = np.sqrt(
-            normTensor**2 + M.norm() ** 2 - 2 * tensor.innerprod(M)
+            normTensor**2 + M.norm() ** 2 - 2 * input_tensor.innerprod(M)
         )
         fit = 1 - (normresidual / normTensor)  # fraction explained by model
-        print("===========================================\n")
-        print(" Final log-likelihood = {} \n".format(obj))
-        print(" Final least squares fit = {} \n".format(fit))
-        print(" Final KKT violation = {}\n".format(kktViolations[iter]))
-        print(" Total inner iterations = {}\n".format(sum(nInnerIters)))
-        print(" Total execution time = {} secs\n".format(t_stop))
+        print("===========================================")
+        print(" Final log-likelihood = {}".format(obj))
+        print(" Final least squares fit = {}".format(fit))
+        print(" Final KKT violation = {}".format(kktViolations[iter]))
+        print(" Total inner iterations = {}".format(sum(nInnerIters)))
+        print(" Total execution time = {} secs".format(t_stop))
 
     output = {}
     output["params"] = (
         stoptol,
         stoptime,
         maxiters,
         maxinneriters,
@@ -728,15 +733,15 @@
     output["times"] = times[: iter + 1]
     output["totalTime"] = t_stop
 
     return M, output
 
 
 def tt_cp_apr_pqnr(
-    tensor,
+    input_tensor,
     rank,
     init,
     stoptol,
     stoptime,
     maxiters,
     maxinneriters,
     epsDivZero,
@@ -765,15 +770,15 @@
     precompinds: bool
         PDNR & PQNR ALGORITHM PARAMETER: Precompute sparse tensor indices
     inexact: bool
         PDNR ALGORITHM PARAMETER: Compute inexact Newton steps
 
     Parameters
     ----------
-    tensor: Union[:class:`pyttb.tensor`,:class:`pyttb.sptensor`]
+    input_tensor: Union[:class:`pyttb.tensor`,:class:`pyttb.sptensor`]
     rank: int
         Rank of the decomposition
     init: str or :class:`pyttb.ktensor`
         Initial guess
     stoptol: float
         Tolerance on overall KKT violation
     stoptime: float
@@ -804,15 +809,15 @@
     Newton-Based Optimization for Nonnegative Tensor Factorizations,
     arXiv:1304.4964 [math.NA], April 2013,
     URL: http://arxiv.org/abs/1304.4964. Submitted for publication.
 
     """
     # TODO first ~100 lines are identical to PDNR, consider abstracting just the algorithm portion
     # Extract the number of modes in data tensor
-    N = tensor.ndims
+    N = input_tensor.ndims
 
     # If the initial guess has any rows of all zero elements, then modify so the row subproblem is not taking log(0).
     # Values will be restored to zero later if the unfolded X for the row has no zeros.
     for n in range(N):
         rowsum = np.sum(init[n], axis=1)
         tmpIdx = np.where(rowsum == 0)[0]
         if tmpIdx.size != 0:
@@ -820,29 +825,29 @@
 
     # Start with the initial guess, normalized using the vector L1 norm
     # TODO replace with copy
     M = ttb.ktensor.from_tensor_type(init)
     M.normalize(normtype=1)
 
     # Sparse tensor flag affects how Pi and Phi are computed.
-    if isinstance(tensor, ttb.sptensor):
+    if isinstance(input_tensor, ttb.sptensor):
         isSparse = True
     else:
         isSparse = False
 
     # Initialize output arrays
     fnEvals = np.zeros((maxiters, 1))
     fnVals = np.zeros((maxiters, 1))
     kktViolations = -np.ones((maxiters, 1))
     nInnerIters = np.zeros((maxiters, 1))
     nzeros = np.zeros((maxiters, 1))
     times = np.zeros((maxiters, 1))
 
     if printitn > 0:
-        print("\nCP_PQNR (alternating Poisson regression using quasi-Newton)\n")
+        print("CP_PQNR (alternating Poisson regression using quasi-Newton)")
 
     dispLineWarn = printinneritn > 0
 
     # Start the wall clock timer.
     start = time.time()
 
     if isSparse and precompinds:
@@ -851,19 +856,19 @@
         if printitn > 0:
             print("\tPrecomuting sparse index sets...")
         sparseIx = []
         for n in range(N):
             num_rows = M[n].shape[0]
             row_indices = []
             for jj in range(num_rows):
-                row_indices.append(np.where(tensor.subs[:, n] == jj)[0])
+                row_indices.append(np.where(input_tensor.subs[:, n] == jj)[0])
             sparseIx.append(row_indices)
 
         if printitn > 0:
-            print("done\n")
+            print("done")
 
     # Main loop: iterate until convergence or a max threshold is reached
     for iter in range(maxiters):
         isConverged = True
         kktModeViolations = np.zeros((N,))
         countInnerIters = np.zeros((N,))
 
@@ -871,40 +876,40 @@
         for n in range(N):
             # Shift the weight from lambda to mode n.
             M.redistribute(mode=n)
 
             # calculate khatri-rao product of all matrices but the n-th
             if isSparse == False:
                 # Data is not a sparse tensor.
-                Pi = ttb.tt_calcpi_prowsubprob(tensor, M, rank, n, N, isSparse)
-                X_mat = ttb.tt_to_dense_matrix(tensor, n)
+                Pi = ttb.tt_calcpi_prowsubprob(input_tensor, M, rank, n, N, isSparse)
+                X_mat = ttb.tt_to_dense_matrix(input_tensor, n)
 
             num_rows = M[n].shape[0]
             isRowNOTconverged = np.zeros((num_rows,))
 
             # Loop over the row subproblems in mode n.
             for jj in range(num_rows):
                 # Get data values for row jj of matricized mode n,
                 if isSparse:
                     # Data is a sparse tensor
                     if not precompinds:
-                        sparse_indices = np.where(tensor.subs[:, n] == jj)[0]
+                        sparse_indices = np.where(input_tensor.subs[:, n] == jj)[0]
                     else:
                         sparse_indices = sparseIx[n][jj]
 
                     if sparse_indices.size == 0:
                         # The row jj of matricized tensor X in mode n is empty
                         M.factor_matrices[n][jj, :] = 0
                         continue
 
-                    x_row = tensor.vals[sparse_indices]
+                    x_row = input_tensor.vals[sparse_indices]
 
                     # Calculate just the columns of Pi needed for this row.
                     Pi = ttb.tt_calcpi_prowsubprob(
-                        tensor, M, rank, n, N, isSparse, sparse_indices
+                        input_tensor, M, rank, n, N, isSparse, sparse_indices
                     )
 
                 else:
                     x_row = X_mat[jj, :]
 
                 # Get current values of the row subproblem variables.
                 m_row = M[n][jj, :]
@@ -952,28 +957,30 @@
                     # Compute the row subproblem kkt_violation.
 
                     # Note experiments in the original paper used:
                     # kkt_violation = np.norm(np.abs(np.minimum(m_row, gradM.transpose())))
 
                     # We now use \| KKT \|_{inf}:
                     kkt_violation = np.max(np.abs(np.minimum(m_row, gradM)))
-                    # print("Intermediate Printing m_row: {}\n and gradM{}".format(m_row, gradM))
 
                     # Report largest row subproblem initial violation
                     if i == 0 and kkt_violation > kktModeViolations[n]:
                         kktModeViolations[n] = kkt_violation
 
                     if printinneritn > 0 and np.mod(i, printinneritn) == 0:
-                        print("\tMode = {}, Row = {}, InnerIt = {}".format(n, jj, i))
+                        print(
+                            "\tMode = {}, Row = {}, InnerIt = {}".format(n, jj, i),
+                            end="",
+                        )
 
                         if i == 0:
-                            print(", RowKKT = {}\n".format(kkt_violation))
+                            print(", RowKKT = {}".format(kkt_violation))
                         else:
                             print(
-                                ", RowKKT = {}, RowObj = {}\n".format(
+                                ", RowKKT = {}, RowObj = {}".format(
                                     kkt_violation, -f_new
                                 )
                             )
 
                     # Check for row subproblem convergence.
                     if kkt_violation < stoptol:
                         break
@@ -1067,49 +1074,49 @@
             num_zero += np.count_nonzero(M[n] == 0)  # [0].size
 
         nzeros[iter] = num_zero
         kktViolations[iter] = np.max(kktModeViolations)
 
         # Print outer iteration status.
         if printitn > 0 and np.mod(iter, printitn) == 0:
-            fnVals[iter] = -tt_loglikelihood(tensor, M)
+            fnVals[iter] = -tt_loglikelihood(input_tensor, M)
             print(
-                "{}. Ttl Inner Its: {}, KKT viol = {}, obj = {}, nz: {}\n".format(
+                "{}. Ttl Inner Its: {}, KKT viol = {}, obj = {}, nz: {}".format(
                     iter, nInnerIters[iter], kktViolations[iter], fnVals[iter], num_zero
                 )
             )
 
         times[iter] = time.time() - start
 
         # Check for convergence
         if isConverged:
             break
         if times[iter] > stoptime:
-            print("Exiting because time limit exceeded\n")
+            print("Exiting because time limit exceeded")
             break
 
     t_stop = time.time() - start
 
     # Clean up final result
     M.normalize(sort=True, normtype=1)
 
-    obj = tt_loglikelihood(tensor, M)
+    obj = tt_loglikelihood(input_tensor, M)
 
     if printitn > 0:
-        normTensor = tensor.norm()
+        normTensor = input_tensor.norm()
         normresidual = np.sqrt(
-            normTensor**2 + M.norm() ** 2 - 2 * tensor.innerprod(M)
+            normTensor**2 + M.norm() ** 2 - 2 * input_tensor.innerprod(M)
         )
         fit = 1 - (normresidual / normTensor)  # fraction explained by model
-        print("===========================================\n")
-        print(" Final log-likelihood = {} \n".format(obj))
-        print(" Final least squares fit = {} \n".format(fit))
-        print(" Final KKT violation = {}\n".format(kktViolations[iter]))
-        print(" Total inner iterations = {}\n".format(sum(nInnerIters)))
-        print(" Total execution time = {} secs\n".format(t_stop))
+        print("===========================================")
+        print(" Final log-likelihood = {}".format(obj))
+        print(" Final least squares fit = {}".format(fit))
+        print(" Final KKT violation = {}".format(kktViolations[iter]))
+        print(" Total inner iterations = {}".format(sum(nInnerIters)))
+        print(" Total execution time = {} secs".format(t_stop))
 
     output = {}
     output["params"] = (
         stoptol,
         stoptime,
         maxiters,
         maxinneriters,
@@ -1165,16 +1172,18 @@
         num_row_nnz = len(sparse_indices)
 
         Pi = np.ones((num_row_nnz, rank))
         for i in np.setdiff1d(np.arange(ndims), factorIndex).astype(int):
             Pi *= Model[i][Data.subs[sparse_indices, i], :]
     else:
         Pi = ttb.khatrirao(
-            Model.factor_matrices[:factorIndex]
-            + Model.factor_matrices[factorIndex + 1 : ndims + 1],
+            *(
+                Model.factor_matrices[:factorIndex]
+                + Model.factor_matrices[factorIndex + 1 : ndims + 1]
+            ),
             reverse=True,
         )
 
     return Pi
 
 
 def calc_partials(isSparse, Pi, epsilon, data_row, model_row):
@@ -1654,16 +1663,18 @@
     """
     if isinstance(Data, ttb.sptensor):
         Pi = np.ones((Data.nnz, rank))
         for i in np.setdiff1d(np.arange(ndims), factorIndex).astype(int):
             Pi *= Model[i][Data.subs[:, i], :]
     else:
         Pi = ttb.khatrirao(
-            Model.factor_matrices[:factorIndex]
-            + Model.factor_matrices[factorIndex + 1 :],
+            *(
+                Model.factor_matrices[:factorIndex]
+                + Model.factor_matrices[factorIndex + 1 :]
+            ),
             reverse=True,
         )
 
     return Pi
 
 
 def calculatePhi(Data, Model, rank, factorIndex, Pi, epsilon):
```

### Comparing `pyttb-1.6.1/pyttb/export_data.py` & `pyttb-1.6.2/pyttb/export_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 from .pyttb_utils import *
 
 
 def export_data(data, filename, fmt_data=None, fmt_weights=None):
     """
     Export tensor-related data to a file.
     """
+    if not isinstance(data, (ttb.tensor, ttb.sptensor, ttb.ktensor, np.ndarray)):
+        assert False, f"Invalid data type for export: {type(data)}"
+
     # open file
     fp = open(filename, "w")
 
     if isinstance(data, ttb.tensor):
         print("tensor", file=fp)
         export_size(fp, data.shape)
         export_array(fp, data.data, fmt_data)
@@ -50,17 +53,14 @@
         """
 
     elif isinstance(data, np.ndarray):
         print("matrix", file=fp)
         export_size(fp, data.shape)
         export_array(fp, data, fmt_data)
 
-    else:
-        assert False, "Invalid data type for export"
-
 
 def export_size(fp, shape):
     # Export the size of something to a file
     print(f"{len(shape)}", file=fp)  # # of dimensions on one line
     shape_str = " ".join([str(d) for d in shape])
     print(f"{shape_str}", file=fp)  # size of each dimensions on the next line
```

### Comparing `pyttb-1.6.1/pyttb/hosvd.py` & `pyttb-1.6.2/pyttb/hosvd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 """Higher Order SVD Implementation"""
+# Copyright 2022 National Technology & Engineering Solutions of Sandia,
+# LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
+# U.S. Government retains certain rights in this software.
+
 import warnings
 from typing import List, Optional
 
 import numpy as np
 import scipy
 
 import pyttb as ttb
 
 
 def hosvd(
-    tensor,
+    input_tensor,
     tol: float,
     verbosity: float = 1,
     dimorder: Optional[List[int]] = None,
     sequential: bool = True,
     ranks: Optional[List[int]] = None,
 ):
     """Compute sequentially-truncated higher-order SVD (Tucker).
 
     Computes a Tucker decomposition with relative error
     specified by tol, i.e., it computes a ttensor T such that
     ||X-T||/||X|| <= tol.
 
     Parameters
     ----------
-    tensor: Tensor to factor
+    input_tensor: Tensor to factor
     tol: Relative error to stop at
     verbosity: Print level
     dimorder: Order to loop through dimensions
     sequential: Use sequentially-truncated version
     ranks: Specify ranks to consider rather than computing
 
     Example
@@ -38,15 +42,15 @@
     >>> disable_printing = -1
     >>> tensorInstance = ttb.tensor().from_data(data)
     >>> result = hosvd(tensorInstance, tol, verbosity=disable_printing)
     >>> ((result.full() - tensorInstance).norm() / tensorInstance.norm()) < tol
     True
     """
     # In tucker als this is N
-    d = tensor.ndims
+    d = input_tensor.ndims
 
     if ranks is not None:
         if len(ranks) != d:
             raise ValueError(
                 f"Ranks must be a list of length tensor ndims. Ndims: {d} but got "
                 f"ranks: {ranks}."
             )
@@ -64,28 +68,28 @@
                 "Dimorder must be a list or permutation of range(tensor.ndims)"
             )
 
     # TODO should unify printing throughout. Probably easier to use python logging levels
     if verbosity > 0:
         print("Computing HOSVD...\n")
 
-    normxsqr = (tensor**2).collapse()
+    normxsqr = (input_tensor**2).collapse()
     eigsumthresh = ((tol**2) * normxsqr) / d
 
     if verbosity > 2:
         print(
             f"||X||^2 = {normxsqr: g}\n"
             f"tol = {tol: g}\n"
             f"eigenvalue sum threshold = tol^2 ||X||^2 / d = {eigsumthresh: g}"
         )
 
     # Main Loop
     factor_matrices = [np.empty(1)] * d
     # Copy input tensor, shrinks every step for sequential
-    Y = ttb.tensor.from_tensor_type(tensor)
+    Y = ttb.tensor.from_tensor_type(input_tensor)
 
     for k in dimorder:
         # Compute Gram matrix
         Yk = ttb.tenmat.from_tensor_type(Y, np.array([k])).double()
         Z = np.dot(Yk, Yk.transpose())
 
         # Compute eigenvalue decomposition
@@ -119,15 +123,15 @@
         G = Y
     else:
         G = Y.ttm(factor_matrices, transpose=True)
 
     result = ttb.ttensor.from_data(G, factor_matrices)
 
     if verbosity > 0:
-        diffnormsqr = ((tensor - result.full()) ** 2).collapse()
+        diffnormsqr = ((input_tensor - result.full()) ** 2).collapse()
         relnorm = np.sqrt(diffnormsqr / normxsqr)
         print(f" Size of core: {G.shape}")
         if relnorm <= tol:
             print(f"||X-T||/||X|| = {relnorm: g} <=" f"{tol: f} (tol)")
         else:
             print(
                 "Tolerance not satisfied!! "
```

### Comparing `pyttb-1.6.1/pyttb/import_data.py` & `pyttb-1.6.2/pyttb/import_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,49 +20,51 @@
     fp = open(filename, "r")
 
     # tensor type should be on the first line
     # valid: tensor, sptensor, matrix, ktensor
     data_type = import_type(fp)
 
     if data_type not in ["tensor", "sptensor", "matrix", "ktensor"]:
+        fp.close()
         assert False, f"Invalid data type found: {data_type}"
 
     if data_type == "tensor":
         shape = import_shape(fp)
         data = import_array(fp, np.prod(shape))
+        fp.close()
         return ttb.tensor().from_data(data, shape)
 
     elif data_type == "sptensor":
         shape = import_shape(fp)
         nz = import_nnz(fp)
         subs, vals = import_sparse_array(fp, len(shape), nz)
+        fp.close()
         return ttb.sptensor().from_data(subs, vals, shape)
 
     elif data_type == "matrix":
         shape = import_shape(fp)
         mat = import_array(fp, np.prod(shape))
         mat = np.reshape(mat, np.array(shape))
+        fp.close()
         return mat
 
     elif data_type == "ktensor":
         shape = import_shape(fp)
         r = import_rank(fp)
         weights = import_array(fp, r)
         factor_matrices = []
         for n in range(len(shape)):
             fac_type = fp.readline().strip()
             fac_shape = import_shape(fp)
             fac = import_array(fp, np.prod(fac_shape))
             fac = np.reshape(fac, np.array(fac_shape))
             factor_matrices.append(fac)
+        fp.close()
         return ttb.ktensor().from_data(weights, factor_matrices)
 
-    # Close file
-    fp.close()
-
 
 def import_type(fp):
     # Import IO data type
     return fp.readline().strip().split(" ")[0]
 
 
 def import_shape(fp):
```

### Comparing `pyttb-1.6.1/pyttb/ktensor.py` & `pyttb-1.6.2/pyttb/ktensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+"""Classes and functions for working with Kruskal tensors."""
 # Copyright 2022 National Technology & Engineering Solutions of Sandia,
 # LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 # U.S. Government retains certain rights in this software.
 
-"""Classes and functions for working with Kruskal tensors."""
 from __future__ import annotations
 
 import logging
 import warnings
 
 import numpy as np
 import scipy.sparse as sparse
@@ -491,33 +491,35 @@
             )
             factor_matrices.append(factor_matrix)
 
         return cls().from_data(weights, factor_matrices)
 
     def arrange(self, weight_factor=None, permutation=None):
         """
-        Arrange the rank-1 components of a :class:`pyttb.ktensor`. The
-        columns are permuted in place, so you must make a copy before calling
-        this method if you want to store the original :class:`pyttb.ktensor`.
-        One of the parameters, either `weight_factor` or `permutation`
-        must be passed, and passing both parameters leads to an error.
+        Arrange the rank-1 components of a :class:`pyttb.ktensor` in place.
+        If `permutation` is passed, the columns of `self.factor_matrices` are
+        arranged using the provided permutation, so you must make a copy
+        before calling this method if you want to store the original
+        :class:`pyttb.ktensor`. If `weight_factor` is passed, then the values
+        in `self.weights` are absorbed into
+        `self.factor_matrices[weight_factor]`. If no parameters are passed,
+        then the columns of `self.factor_matrices` are normalized and then
+        permuted such that the resulting `self.weights` are sorted by
+        magnitude, greatest to least. Passing both parameters leads to an
+        error.
 
         Parameters
         ----------
         weight_factor: int, optional
-            The index of the factor that the weights will be absorbed into
-        permutation: :class:`tuple`, :class:`list`, :class:`numpy.ndarray`, optional
+            The index of the factor matrix that the weights will be absorbed into.
+        permutation: :class:`tuple`, :class:`list`, or :class:`numpy.ndarray`, optional
             The new order of the components of the :class:`pyttb.ktensor`
             into which to permute. The permutation must be of length equal to
-            the number of components of the :class:`pyttb.ktensor`, N, and
-            must be a permutation of 1 to N.
-
-        Returns
-        -------
-        :class:`pyttb.ktensor`
+            the number of components of the :class:`pyttb.ktensor`, `self.ncomponents`
+            and must be a permutation of [0,...,`self.ncomponents`-1].
 
         Examples
         --------
         Create the initial :class:`pyttb.ktensor`:
 
         >>> weights = np.array([1., 2.])
         >>> fm0 = np.array([[1., 2.], [3., 4.]])
@@ -542,54 +544,78 @@
         weights=[2. 1.]
         factor_matrices[0] =
         [[2. 1.]
          [4. 3.]]
         factor_matrices[1] =
         [[6. 5.]
          [8. 7.]]
-        """
 
+        Normalize and permute columns such that `weights` are sorted in
+        decreasing order:
+
+        >>> K.arrange()
+        >>> print(K) # doctest: +ELLIPSIS
+        ktensor of shape 2 x 2
+        weights=[89.4427... 27.2029...]
+        factor_matrices[0] =
+        [[0.4472... 0.3162...]
+         [0.8944... 0.9486...]]
+        factor_matrices[1] =
+        [[0.6... 0.5812...]
+         [0.8... 0.8137...]]
+
+        Absorb the weights into the second factor:
+
+        >>> K.arrange(weight_factor=1)
+        >>> print(K) # doctest: +ELLIPSIS
+        ktensor of shape 2 x 2
+        weights=[1. 1.]
+        factor_matrices[0] =
+        [[0.4472... 0.3162...]
+         [0.8944... 0.9486...]]
+        factor_matrices[1] =
+        [[53.6656... 15.8113...]
+         [71.5541... 22.1359...]]
+        """
         if permutation is not None and weight_factor is not None:
             assert (
                 False
             ), "Weighting and permuting the ktensor at the same time is not allowed."
 
+        # arrange columns of factor matrices using the permutation provided
         if permutation is not None and isinstance(
             permutation, (tuple, list, np.ndarray)
         ):
             if len(permutation) == self.ncomponents:
                 self.weights = self.weights[permutation]
                 for i in range(self.ndims):
                     self.factor_matrices[i] = self.factor_matrices[i][:, permutation]
                 return
             else:
                 assert (
                     False
                 ), "Number of elements in permutation does not match number of components in ktensor."
 
-        # TODO there is a relationship here between normalize and arrange that repeats tasks. Can this be made to be more efficient?
-        # ensure that factor matrices are normalized
+        # TODO there is a relationship here between normalize and arrange that repeats tasks.
+        # Can this be made to be more efficient? ensure that factor matrices are normalized
         self.normalize()
 
         # sort
         p = np.argsort(self.weights)[::-1]
         self.weights = self.weights[p]
         for i in range(self.ndims):
             self.factor_matrices[i] = self.factor_matrices[i][:, p]
 
-        # TODO is this necessary? Matlab only absorbs into the last factor, not factor N as is documented
-        # absorb weight into one factor if requested
+        # absorb the weights into one factor, optional
         if weight_factor is not None:
-            pass
-        # if exist('foo','var')
-        #     r = length(X.lambda);
-        #     X.u{end} = full(X.u{end} * spdiags(X.lambda,0,r,r));
-        #     X.lambda = ones(size(X.lambda));
-        # end
-        return self
+            r = len(self.weights)
+            self.factor_matrices[weight_factor] *= self.weights
+            self.weights = np.ones_like(self.weights)
+
+        return
 
     def copy(self):
         """
         Make a deep copy of a :class:`pyttb.ktensor`.
 
         Returns
         -------
@@ -960,15 +986,15 @@
         >>> print(K.full()) # doctest: +NORMALIZE_WHITESPACE
         tensor of shape 2 x 2
         data[:, :] =
         [[29. 39.]
          [63. 85.]]
         <BLANKLINE>
         """
-        data = self.weights @ ttb.khatrirao(self.factor_matrices, reverse=True).T
+        data = self.weights @ ttb.khatrirao(*self.factor_matrices, reverse=True).T
         return ttb.tensor.from_data(data, self.shape)
 
     def innerprod(self, other):
         """
         Efficient inner product with a :class:`pyttb.ktensor`.
 
         Efficiently computes the inner product between two tensors, `self`
@@ -1256,39 +1282,39 @@
         for f in self.factor_matrices:
             coefMatrix = coefMatrix * (f.T @ f)
         return np.sqrt(np.abs(np.sum(coefMatrix)))
 
     def normalize(self, weight_factor=None, sort=False, normtype=2, mode=None):
         """
         Normalize the columns of the factor matrices of a
-        :class:`pyttb.ktensor`.
+        :class:`pyttb.ktensor` in place.
 
         Parameters
         ----------
         weight_factor: {"all", int}, optional
             Absorb the weights into one or more factors. If "all", absorb
             weight equally across all factors. If `int`, absorb weight into a
             single dimension (value must be in range(self.ndims)).
         sort: bool, optional
             Sort the columns in descending order of the weights.
         normtype: {non-negative int, -1, -2, np.inf, -np.inf}, optional
             Order of the norm (see :func:`numpy.linalg.norm` for possible
             values).
-        mode: {int, None}, optional
+        mode: int, optional
             Index of factor matrix to normalize. A value of `None` means
             normalize all factor matrices.
 
         Returns
         -------
         :class:`pyttb.ktensor`
 
         Examples
         --------
         >>> K = ttb.ktensor.from_function(np.ones, (2, 3, 4), 2)
-        >>> print(K.normalize())  # doctest: +ELLIPSIS
+        >>> print(K.normalize()) # doctest: +ELLIPSIS
         ktensor of shape 2 x 3 x 4
         weights=[4.898... 4.898...]
         factor_matrices[0] =
         [[0.7071... 0.7071...]
          [0.7071... 0.7071...]]
         factor_matrices[1] =
         [[0.5773... 0.5773...]
@@ -1306,15 +1332,15 @@
                 for r in range(self.ncomponents):
                     tmp = np.linalg.norm(self.factor_matrices[mode][:, r], ord=normtype)
                     if tmp > 0:
                         self.factor_matrices[mode][:, r] = (
                             1.0 / tmp * self.factor_matrices[mode][:, r]
                         )
                     self.weights[r] = self.weights[r] * tmp
-                return
+                return self
             else:
                 assert (
                     False
                 ), "Parameter single_factor is invalid; index must be an int in range of number of dimensions"
 
         # ensure that all factor_matrices are normalized
         for mode in range(self.ndims):
@@ -1345,15 +1371,15 @@
             ] @ np.diag(self.weights)
             self.weights = np.ones((self.weights.shape))
 
         if sort:
             if self.ncomponents > 1:
                 # indices of srting in descending order
                 p = np.argsort(self.weights)[::-1]
-                self = self.arrange(permutation=p)
+                self.arrange(permutation=p)
 
         return self
 
     def nvecs(self, n, r, flipsign=True):
         """
         Compute the leading mode-n vectors for a :class:`pyttb.ktensor`.
```

### Comparing `pyttb-1.6.1/pyttb/pyttb_utils.py` & `pyttb-1.6.2/pyttb/pyttb_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+"""PYTTB shared utilities across tensor types"""
 # Copyright 2022 National Technology & Engineering Solutions of Sandia,
 # LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 # U.S. Government retains certain rights in this software.
-"""PYTTB shared utilities across tensor types"""
+
 from inspect import signature
 from typing import Optional, Tuple, overload
 
 import numpy as np
 
 import pyttb as ttb
```

### Comparing `pyttb-1.6.1/pyttb/sptensor.py` & `pyttb-1.6.2/pyttb/sptensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+"""Sparse Tensor Implementation"""
 # Copyright 2022 National Technology & Engineering Solutions of Sandia,
 # LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 # U.S. Government retains certain rights in this software.
-"""Sparse Tensor Implementation"""
+
 from __future__ import annotations
 
 import logging
 import warnings
-from collections.abc import Sequence
+from collections.abc import Iterable, Sequence
 from typing import Any, Callable, List, Optional, Tuple, Union, cast, overload
 
 import numpy as np
 import scipy.sparse.linalg
 from numpy_groupies import aggregate as accumarray
 from scipy import sparse
 
@@ -117,14 +118,17 @@
 
     @classmethod
     def from_data(
         cls, subs: np.ndarray, vals: np.ndarray, shape: Tuple[int, ...]
     ) -> sptensor:
         """
         Construct an sptensor from fully defined SUB, VAL and SIZE matrices.
+        This does no validation to optimize for speed when components are known.
+        For default initializer with error checking see
+        :func:`~pyttb.sptensor.sptensor.from_aggregator`.
 
         Parameters
         ----------
         subs: location of non-zero entries
         vals: values for non-zero entries
         shape: shape of sparse tensor
 
@@ -344,15 +348,15 @@
         for n in range(0, self.ndims):
             o.append(np.ones((self.shape[n], 1)))
 
         # Generate each column of the subscripts in turn
         for n in range(0, self.ndims):
             i = o.copy()
             i[n] = np.expand_dims(np.arange(0, self.shape[n]), axis=1)
-            s[:, n] = np.squeeze(ttb.khatrirao(i))
+            s[:, n] = np.squeeze(ttb.khatrirao(*i))
 
         return s.astype(int)
 
     def collapse(
         self,
         dims: Optional[np.ndarray] = None,
         fun: Callable[[np.ndarray], Union[float, np.ndarray]] = np.sum,
@@ -616,15 +620,15 @@
                 valsSelf = self.extract(subsOther)
             return valsOther.transpose().dot(valsSelf)
 
         if isinstance(other, ttb.tensor):
             if self.shape != other.shape:
                 assert False, "Sptensor and tensor must be same shape for innerproduct"
             [subsSelf, valsSelf] = self.find()
-            valsOther = other[subsSelf, "extract"]
+            valsOther = other[subsSelf.transpose(), "extract"]
             return valsOther.transpose().dot(valsSelf)
 
         if isinstance(other, (ttb.ktensor, ttb.ttensor)):  # pragma: no cover
             # Reverse arguments to call ktensor/ttensor implementation
             return other.innerprod(self)
 
         assert False, f"Inner product between sptensor and {type(other)} not supported"
@@ -667,29 +671,26 @@
             return C
         # Case 2: Argument is a tensor of some sort
         if isinstance(B, sptensor):
             # Check that the shapes match
             if not self.shape == B.shape:
                 assert False, "Must be tensors of the same shape"
 
-            def is_length_2(x):
-                return len(x) == 2
-
             C = sptensor.from_aggregator(
                 np.vstack((self.subs, B.subs)),
                 np.vstack((self.vals, B.vals)),
                 self.shape,
-                is_length_2,
+                lambda x: len(x) == 2,
             )
 
             return C
 
         if isinstance(B, ttb.tensor):
             BB = sptensor.from_data(
-                self.subs, B[self.subs, "extract"][:, None], self.shape
+                self.subs, B[self.subs.transpose(), "extract"][:, None], self.shape
             )
             C = self.logical_and(BB)
             return C
 
         # Otherwise
         assert False, "The arguments must be two sptensors or an sptensor and a scalar."
 
@@ -731,23 +732,19 @@
             return self.full().logical_or(B)
 
         # Case 2: Argument is an sptensor
         if self.shape != B.shape:
             assert False, "Logical Or requires tensors of the same size"
 
         if isinstance(B, ttb.sptensor):
-
-            def is_length_ge_1(x):
-                return len(x) >= 1
-
             return sptensor.from_aggregator(
                 np.vstack((self.subs, B.subs)),
                 np.ones((self.subs.shape[0] + B.subs.shape[0], 1)),
                 self.shape,
-                is_length_ge_1,
+                lambda x: len(x) >= 1,
             )
 
         assert False, "Sptensor Logical Or argument must be scalar or sptensor"
 
     @overload
     def logical_xor(self, other: Union[float, ttb.tensor]) -> ttb.tensor:
         ...  # pragma: no cover see coveragepy/issues/970
@@ -776,20 +773,17 @@
 
         # Case 2: Argument is an sptensor
         if isinstance(other, ttb.sptensor):
             # Check shape consistency
             if self.shape != other.shape:
                 assert False, "Logical XOR requires tensors of the same size"
 
-            def length1(x):
-                return len(x) == 1
-
             subs = np.vstack((self.subs, other.subs))
             return ttb.sptensor.from_aggregator(
-                subs, np.ones((len(subs), 1)), self.shape, length1
+                subs, np.ones((len(subs), 1)), self.shape, lambda x: len(x) == 1
             )
 
         assert False, "The argument must be an sptensor, tensor or scalar"
 
     def mask(self, W: sptensor) -> np.ndarray:
         """
         Extract values as specified by a mask tensor
@@ -1049,15 +1043,15 @@
 
         if isinstance(factor, ttb.tensor):
             shapeArray = np.array(self.shape)
             if not np.array_equal(factor.shape, shapeArray[dims]):
                 assert False, "Size mismatch in scale"
             return ttb.sptensor.from_data(
                 self.subs,
-                self.vals * factor[self.subs[:, dims], "extract"][:, None],
+                self.vals * factor[self.subs[:, dims].transpose(), "extract"][:, None],
                 self.shape,
             )
         if isinstance(factor, ttb.sptensor):
             shapeArray = np.array(self.shape)
             if not np.array_equal(factor.shape, shapeArray[dims]):
                 assert False, "Size mismatch in scale"
             return ttb.sptensor.from_data(
@@ -1364,17 +1358,17 @@
         # TODO understand how/ why this is used, logic doesn't translate immediately
         # Case 2: EXTRACT
 
         # *** CASE 2a: Subscript indexing ***
         if (
             isinstance(item, np.ndarray)
             and len(item.shape) == 2
-            and item.shape[1] == self.ndims
+            and item.shape[0] == self.ndims
         ):
-            srchsubs = np.array(item)
+            srchsubs = np.array(item.transpose())
 
         # *** CASE 2b: Linear indexing ***
         else:
             # Error checking
             if isinstance(item, list):
                 idx = np.array(item)
             elif isinstance(item, np.ndarray):
@@ -1389,15 +1383,14 @@
             srchsubs = tt_ind2sub(self.shape, idx)
 
         a = self.extract(srchsubs)
         a = tt_subsubsref(a, item)
 
         return a
 
-    # pylint:disable=too-many-statements, too-many-branches, too-many-locals
     def __setitem__(self, key, value):
         """
         Subscripted assignment for sparse tensor.
 
         We can assign elements to a sptensor in three ways.
 
         Case 1: X(R1,R2,...,RN) = Y, in which case we replace the
@@ -1439,302 +1432,318 @@
         # TODO IndexError for value outside of indices
         # TODO Key error if item not in container
         # If empty sptensor and assignment is empty list or empty nparray
         if self.vals.size == 0 and (
             (isinstance(value, np.ndarray) and value.size == 0)
             or (isinstance(value, list) and value == [])
         ):
-            return
+            return None
 
         # Determine if we are doing a substenor or list of subscripts
         objectType = tt_assignment_type(self, key, value)
 
         # Case 1: Replace a sub-tensor
-        if objectType == "subtensor":  # pylint:disable=too-many-nested-blocks
-            # Case I(a): RHS is another sparse tensor
-            if isinstance(value, ttb.sptensor):
-                # First, Resize the tensor and check the size match with the tensor
-                # that's being inserted.
-                m = 0
-                newsz = []
-                for n, key_n in enumerate(key):
-                    if isinstance(key_n, slice):
-                        if self.ndims <= n:
-                            if key_n.stop is None:
-                                newsz.append(value.shape[m])
-                            else:
-                                newsz.append(key_n.stop)
-                        else:
-                            if key_n.stop is None:
-                                newsz.append(max([self.shape[n], value.shape[m]]))
-                            else:
-                                newsz.append(max([self.shape[n], key_n.stop]))
-                        m = m + 1
-                    elif isinstance(key_n, (float, int)):
-                        if self.ndims <= n:
-                            newsz.append(key_n + 1)
-                        else:
-                            newsz.append(max([self.shape[n], key_n + 1]))
-                    else:
-                        if len(key_n) != value.shape[m]:
-                            assert False, "RHS does not match range size"
-                        if self.ndims <= n:
-                            newsz.append(max(key_n) + 1)
-                        else:
-                            newsz.append(max([self.shape[n], max(key_n) + 1]))
-                self.shape = tuple(newsz)
-
-                # Expand subs array if there are new modes, i.e., if the order
-                # has increased.
-                if self.subs.size > 0 and (len(self.shape) > self.subs.shape[1]):
-                    self.subs = np.append(
+        if objectType == "subtensor":
+            return self._set_subtensor(key, value)
+        # Case 2: Subscripts
+        if objectType == "subscripts":
+            return self._set_subscripts(key, value)
+        raise ValueError("Unknown assignment type")  # pragma: no cover
+
+    def _set_subscripts(self, key, value):
+        # Case II: Replacing values at specific indices
+        newsubs = key
+        if len(newsubs.shape) == 1:
+            newsubs = np.expand_dims(newsubs, axis=0)
+        tt_subscheck(newsubs, nargout=False)
+
+        # Error check on subscripts
+        if newsubs.shape[0] < self.ndims:
+            assert False, "Invalid subscripts"
+
+        # Check for expanding the order
+        if newsubs.shape[0] > self.ndims:
+            newshape = list(self.shape)
+            # TODO no need for loop, just add correct size
+            for _ in range(self.ndims, newsubs.shape[0]):
+                newshape.append(1)
+            if self.subs.size > 0:
+                self.subs = np.concatenate(
+                    (
                         self.subs,
-                        np.zeros(
-                            shape=(
-                                self.subs.shape[0],
-                                len(self.shape) - self.subs.shape[1],
-                            )
+                        np.ones(
+                            (self.shape[0], newsubs.shape[0] - self.ndims),
+                            dtype=int,
                         ),
-                        axis=1,
-                    )
-                # Delete what currently occupies the specified range
-                rmloc = self.subdims(key)
-                kploc = np.setdiff1d(range(0, self.nnz), rmloc)
-                # TODO: evaluate solution for assigning value to empty sptensor
-                if len(self.subs.shape) > 1:
-                    newsubs = self.subs[kploc.astype(int), :]
-                else:
-                    newsubs = self.subs[kploc.astype(int)]
-                newvals = self.vals[kploc.astype(int)]
+                    ),
+                    axis=1,
+                )
+            self.shape = tuple(newshape)
 
-                # Renumber the subscripts
-                addsubs = ttb.tt_irenumber(value, self.shape, key)
-                if newsubs.size > 0 and addsubs.size > 0:
-                    self.subs = np.vstack((newsubs, addsubs))
-                    self.vals = np.vstack((newvals, value.vals))
-                elif newsubs.size > 0:
-                    self.subs = newsubs
-                    self.vals = newvals
-                elif addsubs.size > 0:
-                    self.subs = addsubs
-                    self.vals = value.vals
-                else:
-                    self.subs = np.array([], ndmin=2, dtype=int)
-                    self.vals = np.array([], ndmin=2)
+        # Copy rhs to newvals
+        newvals = value
+
+        if isinstance(newvals, (float, int)):
+            newvals = np.expand_dims([newvals], axis=1)
 
-                return
-            # Case I(b): Value is zero or scalar
+        # Error check the rhs is a column vector. We don't bother to handle any
+        # other type with sparse tensors
+        tt_valscheck(newvals, nargout=False)
+
+        # Determine number of nonzeros being inserted.
+        # (This is determined by number of subscripts)
+        newnnz = newsubs.shape[1]
+
+        # Error check on size of newvals
+        if newvals.size == 1:
+            # Special case where newvals is a single element to be assigned
+            # to multiple LHS. Fix to correct size
+            newvals = newvals * np.ones((newnnz, 1))
+
+        elif newvals.shape[0] != newnnz:
+            # Sizes don't match
+            assert False, "Number of subscripts and number of values do not match!"
+
+        # Remove duplicates and print warning if any duplicates were removed
+        newsubs, idx = np.unique(newsubs.transpose(), axis=0, return_index=True)
+        if newsubs.shape[0] != newnnz:
+            warnings.warn("Duplicate assignments discarded")
+
+        newvals = newvals[idx]
+
+        # Find which subscripts already exist and their locations
+        tf = ttb.tt_ismember_rows(newsubs, self.subs)
+        loc = np.where(tf >= 0)[0].astype(int)
+
+        # Split into three groups for processing:
+        #
+        # Group A: Elements that already exist and need to be changed
+        # Group B: Elements that already exist and need to be removed
+        # Group C: Elements that do not exist and need to be added
+        #
+        # Note that we are ignoring any new zero elements, because
+        # those obviously do not need to be added. Also, it's
+        # important to process Group A before Group B because the
+        # processing of Group B may change the locations of the
+        # remaining elements.
+
+        # TF+1 for logical consideration because 0 is valid index
+        # and -1 is our null flag
+        idxa = np.logical_and(tf + 1, newvals)[0]
+        idxb = np.logical_and(tf + 1, np.logical_not(newvals))[0]
+        idxc = np.logical_and(np.logical_not(tf + 1), newvals)[0]
+
+        # Process Group A: Changing values
+        if np.sum(idxa) > 0:
+            self.vals[tf[idxa]] = newvals[idxa]
+        # Proces Group B: Removing Values
+        if np.sum(idxb) > 0:
+            removesubs = loc[idxb]
+            keepsubs = np.setdiff1d(range(0, self.nnz), removesubs)
+            self.subs = self.subs[keepsubs, :]
+            self.vals = self.vals[keepsubs]
+        # Process Group C: Adding new, nonzero values
+        if np.sum(idxc) > 0:
+            if self.subs.size > 0:
+                self.subs = np.vstack((self.subs, newsubs[idxc, :]))
+                self.vals = np.vstack((self.vals, newvals[idxc]))
+            else:
+                self.subs = newsubs[idxc, :]
+                self.vals = newvals[idxc]
 
-            # First, resize the tensor, determine new size of existing modes
+        # Resize the tensor
+        newshape = []
+        for n, dim in enumerate(self.shape):
+            smax = max(newsubs[:, n] + 1)
+            newshape.append(max(dim, smax))
+        self.shape = tuple(newshape)
+
+    # pylint:disable=too-many-statements
+    def _set_subtensor(self, key, value):
+        # Case I(a): RHS is another sparse tensor
+        if isinstance(value, ttb.sptensor):
+            # First, Resize the tensor and check the size match with the tensor
+            # that's being inserted.
+            m = 0
             newsz = []
-            for n in range(0, self.ndims):
-                if isinstance(key[n], slice):
-                    if key[n].stop is None:
-                        newsz.append(self.shape[n])
+            for n, key_n in enumerate(key):
+                if isinstance(key_n, slice):
+                    if self.ndims <= n:
+                        if key_n.stop is None:
+                            newsz.append(value.shape[m])
+                        else:
+                            newsz.append(key_n.stop)
                     else:
-                        newsz.append(max([self.shape[n], key[n].stop]))
-                else:
-                    newsz.append(max([self.shape[n], key[n] + 1]))
-
-            # Determine size of new modes, if any
-            for n in range(self.ndims, len(key)):
-                if isinstance(key[n], slice):
-                    if key[n].stop is None:
-                        assert False, (
-                            "Must have well defined slice when expanding sptensor "
-                            "shape with setitem"
-                        )
+                        if key_n.stop is None:
+                            newsz.append(max([self.shape[n], value.shape[m]]))
+                        else:
+                            newsz.append(max([self.shape[n], key_n.stop]))
+                    m = m + 1
+                elif isinstance(key_n, (float, int)):
+                    if self.ndims <= n:
+                        newsz.append(key_n + 1)
                     else:
-                        newsz.append(key[n].stop)
-                elif isinstance(key[n], np.ndarray):
-                    newsz.append(max(key[n]) + 1)
+                        newsz.append(max([self.shape[n], key_n + 1]))
                 else:
-                    newsz.append(key[n] + 1)
+                    if len(key_n) != value.shape[m]:
+                        assert False, "RHS does not match range size"
+                    if self.ndims <= n:
+                        newsz.append(max(key_n) + 1)
+                    else:
+                        newsz.append(max([self.shape[n], max(key_n) + 1]))
             self.shape = tuple(newsz)
 
-            # Expand subs array if there are new modes, i.e. if the order has increased
-            if self.subs.size > 0 and len(self.shape) > self.subs.shape[1]:
+            # Expand subs array if there are new modes, i.e., if the order
+            # has increased.
+            if self.subs.size > 0 and (len(self.shape) > self.subs.shape[1]):
                 self.subs = np.append(
                     self.subs,
                     np.zeros(
-                        shape=(self.subs.shape[0], len(self.shape) - self.subs.shape[1])
+                        shape=(
+                            self.subs.shape[0],
+                            len(self.shape) - self.subs.shape[1],
+                        )
                     ),
                     axis=1,
                 )
+            # Delete what currently occupies the specified range
+            rmloc = self.subdims(key)
+            kploc = np.setdiff1d(range(0, self.nnz), rmloc)
+            # TODO: evaluate solution for assigning value to empty sptensor
+            if len(self.subs.shape) > 1:
+                newsubs = self.subs[kploc.astype(int), :]
+            else:
+                newsubs = self.subs[kploc.astype(int)]
+            newvals = self.vals[kploc.astype(int)]
 
-            # Case I(b)i: Zero right-hand side
-            if isinstance(value, (int, float)) and value == 0:
-                # Delete what currently occupies the specified range
-                rmloc = self.subdims(key)
-                kploc = np.setdiff1d(range(0, self.nnz), rmloc).astype(int)
-                self.subs = self.subs[kploc, :]
-                self.vals = self.vals[kploc]
-                return
-
-            # Case I(b)ii: Scalar Right Hand Side
-            if isinstance(value, (int, float)):
-                # Determine number of dimensions (may be larger than current number)
-                N = len(key)
-                keyCopy = np.array(key)
-                # Figure out how many indices are in each dimension
-                nssubs = np.zeros((N, 1))
-                for n in range(0, N):
-                    if isinstance(key[n], slice):
-                        # Generate slice explicitly to determine its length
-                        keyCopy[n] = np.arange(0, self.shape[n])[key[n]]
-                        indicesInN = len(keyCopy[n])
-                    else:
-                        indicesInN = 1
-                    nssubs[n] = indicesInN
-
-                # Preallocate (discover any memory issues here!)
-                addsubs = np.zeros((np.prod(nssubs).astype(int), N))
-
-                # Generate appropriately sized ones vectors
-                o = []
-                for n in range(N):
-                    o.append(np.ones((int(nssubs[n]), 1)))
-
-                # Generate each column of the subscripts in turn
-                for n in range(N):
-                    i = o.copy()
-                    if not np.isscalar(keyCopy[n]):
-                        i[n] = np.array(keyCopy[n])[:, None]
-                    else:
-                        i[n] = np.array(keyCopy[n], ndmin=2)
-                    addsubs[:, n] = ttb.khatrirao(i).transpose()[:]
-
-                if self.subs.size > 0:
-                    # Replace existing values
-                    loc = ttb.tt_intersect_rows(self.subs, addsubs)
-                    self.vals[loc] = value
-                    # pare down list of subscripts to add
-                    addsubs = addsubs[ttb.tt_setdiff_rows(addsubs, self.subs)]
-
-                # If there are things to insert then insert them
-                if addsubs.size > 0:
-                    if self.subs.size > 0:
-                        self.subs = np.vstack((self.subs, addsubs.astype(int)))
-                        self.vals = np.vstack(
-                            (self.vals, value * np.ones((addsubs.shape[0], 1)))
-                        )
-                    else:
-                        self.subs = addsubs.astype(int)
-                        self.vals = value * np.ones(addsubs.shape[0])
-                return
+            # Renumber the subscripts
+            addsubs = ttb.tt_irenumber(value, self.shape, key)
+            if newsubs.size > 0 and addsubs.size > 0:
+                self.subs = np.vstack((newsubs, addsubs))
+                self.vals = np.vstack((newvals, value.vals))
+            elif newsubs.size > 0:
+                self.subs = newsubs
+                self.vals = newvals
+            elif addsubs.size > 0:
+                self.subs = addsubs
+                self.vals = value.vals
+            else:
+                self.subs = np.array([], ndmin=2, dtype=int)
+                self.vals = np.array([], ndmin=2)
 
-            assert False, "Invalid assignment value"
+            return
+        # Case I(b): Value is zero or scalar
 
-        # Case 2: Subscripts
-        elif objectType == "subscripts":
-            # Case II: Replacing values at specific indices
+        # First, resize the tensor, determine new size of existing modes
+        newsz = []
+        for n in range(0, self.ndims):
+            if isinstance(key[n], slice):
+                if key[n].stop is None:
+                    newsz.append(self.shape[n])
+                else:
+                    newsz.append(max([self.shape[n], key[n].stop]))
+            elif isinstance(key[n], Iterable):
+                newsz.append(max([self.shape[n], max(key[n]) + 1]))
+            else:
+                newsz.append(max([self.shape[n], key[n] + 1]))
 
-            newsubs = key
-            if len(newsubs.shape) == 1:
-                newsubs = np.expand_dims(newsubs, axis=0)
-            tt_subscheck(newsubs, nargout=False)
-
-            # Error check on subscripts
-            if newsubs.shape[1] < self.ndims:
-                assert False, "Invalid subscripts"
-
-            # Check for expanding the order
-            if newsubs.shape[1] > self.ndims:
-                newshape = list(self.shape)
-                for i in range(self.ndims, newsubs.shape[1]):
-                    newshape.append(1)
-                if self.subs.size > 0:
-                    self.subs = np.concatenate(
-                        (
-                            self.subs,
-                            np.ones(
-                                (self.shape[0], newsubs.shape[1] - self.ndims),
-                                dtype=int,
-                            ),
-                        ),
-                        axis=1,
+        # Determine size of new modes, if any
+        for n in range(self.ndims, len(key)):
+            if isinstance(key[n], slice):
+                if key[n].stop is None:
+                    assert False, (
+                        "Must have well defined slice when expanding sptensor "
+                        "shape with setitem"
                     )
-                self.shape = tuple(newshape)
+                else:
+                    newsz.append(key[n].stop)
+            elif isinstance(key[n], (np.ndarray, Iterable)):
+                newsz.append(max(key[n]) + 1)
+            else:
+                newsz.append(key[n] + 1)
+        self.shape = tuple(newsz)
 
-            # Copy rhs to newvals
-            newvals = value
+        # Expand subs array if there are new modes, i.e. if the order has increased
+        if self.subs.size > 0 and len(self.shape) > self.subs.shape[1]:
+            self.subs = np.append(
+                self.subs,
+                np.zeros(
+                    shape=(self.subs.shape[0], len(self.shape) - self.subs.shape[1]),
+                    dtype=int,
+                ),
+                axis=1,
+            )
 
-            if isinstance(newvals, (float, int)):
-                newvals = np.expand_dims([newvals], axis=1)
+        # Case I(b)i: Zero right-hand side
+        if isinstance(value, (int, float)) and value == 0:
+            # Delete what currently occupies the specified range
+            rmloc = self.subdims(key)
+            kploc = np.setdiff1d(range(0, self.nnz), rmloc).astype(int)
+            self.subs = self.subs[kploc, :]
+            self.vals = self.vals[kploc]
+            return
 
-            # Error check the rhs is a column vector. We don't bother to handle any
-            # other type with sparse tensors
-            tt_valscheck(newvals, nargout=False)
-
-            # Determine number of nonzeros being inserted.
-            # (This is determined by number of subscripts)
-            newnnz = newsubs.shape[0]
-
-            # Error check on size of newvals
-            if newvals.size == 1:
-                # Special case where newvals is a single element to be assigned
-                # to multiple LHS. Fix to correct size
-                newvals = newvals * np.ones((newnnz, 1))
-
-            elif newvals.shape[0] != newnnz:
-                # Sizes don't match
-                assert False, "Number of subscripts and number of values do not match!"
-
-            # Remove duplicates and print warning if any duplicates were removed
-            newsubs, idx = np.unique(newsubs, axis=0, return_index=True)
-            if newsubs.shape[0] != newnnz:
-                warnings.warn("Duplicate assignments discarded")
-
-            newvals = newvals[idx]
-
-            # Find which subscripts already exist and their locations
-            tf = ttb.tt_ismember_rows(newsubs, self.subs)
-            loc = np.where(tf >= 0)[0].astype(int)
-
-            # Split into three groups for processing:
-            #
-            # Group A: Elements that already exist and need to be changed
-            # Group B: Elements that already exist and need to be removed
-            # Group C: Elements that do not exist and need to be added
-            #
-            # Note that we are ignoring any new zero elements, because
-            # those obviously do not need to be added. Also, it's
-            # important to process Group A before Group B because the
-            # processing of Group B may change the locations of the
-            # remaining elements.
-
-            # TF+1 for logical consideration because 0 is valid index
-            # and -1 is our null flag
-            idxa = np.logical_and(tf + 1, newvals)[0]
-            idxb = np.logical_and(tf + 1, np.logical_not(newvals))[0]
-            idxc = np.logical_and(np.logical_not(tf + 1), newvals)[0]
-
-            # Process Group A: Changing values
-            if np.sum(idxa) > 0:
-                self.vals[tf[idxa]] = newvals[idxa]
-            # Proces Group B: Removing Values
-            if np.sum(idxb) > 0:
-                removesubs = loc[idxb]
-                keepsubs = np.setdiff1d(range(0, self.nnz), removesubs)
-                self.subs = self.subs[keepsubs, :]
-                self.vals = self.vals[keepsubs]
-            # Process Group C: Adding new, nonzero values
-            if np.sum(idxc) > 0:
-                self.subs = np.vstack((self.subs, newsubs[idxc, :]))
-                self.vals = np.vstack((self.vals, newvals[idxc]))
+        # Case I(b)ii: Scalar Right Hand Side
+        if isinstance(value, (int, float)):
+            # Determine number of dimensions (may be larger than current number)
+            N = len(key)
+            keyCopy = [None] * N
+            # Figure out how many indices are in each dimension
+            nssubs = np.zeros((N, 1))
+            for n in range(0, N):
+                if isinstance(key[n], slice):
+                    # Generate slice explicitly to determine its length
+                    keyCopy[n] = np.arange(0, self.shape[n])[key[n]]
+                    indicesInN = len(keyCopy[n])
+                elif isinstance(key[n], Iterable):
+                    keyCopy[n] = key[n]
+                    indicesInN = len(key[n])
+                else:
+                    keyCopy[n] = key[n]
+                    indicesInN = 1
+                nssubs[n] = indicesInN
+
+            # Preallocate (discover any memory issues here!)
+            addsubs = np.zeros((np.prod(nssubs).astype(int), N))
+
+            # Generate appropriately sized ones vectors
+            o = []
+            for n in range(N):
+                o.append(np.ones((int(nssubs[n]), 1)))
+
+            # Generate each column of the subscripts in turn
+            for n in range(N):
+                i = o.copy()
+                if not np.isscalar(keyCopy[n]):
+                    i[n] = np.array(keyCopy[n])[:, None]
+                else:
+                    i[n] = np.array(keyCopy[n], ndmin=2)
+                addsubs[:, n] = ttb.khatrirao(*i).transpose()[:]
 
-            # Resize the tensor
-            newshape = []
-            for n, dim in enumerate(self.shape):
-                smax = max(newsubs[:, n] + 1)
-                newshape.append(max(dim, smax))
-            self.shape = tuple(newshape)
+            if self.subs.size > 0:
+                # Replace existing values
+                loc = ttb.tt_intersect_rows(self.subs, addsubs)
+                self.vals[loc] = value
+                # pare down list of subscripts to add
+                addsubs = addsubs[ttb.tt_setdiff_rows(addsubs, self.subs)]
 
+            # If there are things to insert then insert them
+            if addsubs.size > 0:
+                if self.subs.size > 0:
+                    self.subs = np.vstack((self.subs, addsubs.astype(int)))
+                    self.vals = np.vstack(
+                        (self.vals, value * np.ones((addsubs.shape[0], 1)))
+                    )
+                else:
+                    self.subs = addsubs.astype(int)
+                    self.vals = value * np.ones((addsubs.shape[0], 1))
             return
 
+        assert False, "Invalid assignment value"
+
     def __eq__(self, other):
         """
         Equal comparator for sptensors
 
         Parameters
         ----------
         other: compare equality of sptensor to other
@@ -1794,15 +1803,15 @@
             # Find where their zeros interact
             otherzerosubs, _ = (other == 0).find()
             zzerosubs = otherzerosubs[
                 (self.extract(otherzerosubs) == 0).transpose()[0], :
             ]
 
             # Find where their nonzeros intersect
-            othervals = other[self.subs, "extract"]
+            othervals = other[self.subs.transpose(), "extract"]
             znzsubs = self.subs[(othervals[:, None] == self.vals).transpose()[0], :]
 
             return sptensor.from_data(
                 np.vstack((zzerosubs, znzsubs)),
                 True * np.ones((zzerosubs.shape[0] + znzsubs.shape[0])).astype(bool),
                 self.shape,
             )
@@ -1875,15 +1884,15 @@
             if unionSubs.shape[0] != np.prod(self.shape):
                 subs1Idx = ttb.tt_setdiff_rows(self.allsubs(), unionSubs)
                 subs1 = self.allsubs()[subs1Idx]
             else:
                 subs1 = np.empty((0, self.subs.shape[1]))
             # find entries where x is nonzero but not equal to y
             subs2 = self.subs[
-                self.vals.transpose()[0] != other[self.subs, "extract"], :
+                self.vals.transpose()[0] != other[self.subs.transpose(), "extract"], :
             ]
             if subs2.size == 0:
                 subs2 = np.empty((0, self.subs.shape[1]))
             # put it all together
             return ttb.sptensor.from_data(
                 np.vstack((subs1, subs2)),
                 True * np.ones((subs1.shape[0] + subs2.shape[0], 1)).astype(bool),
@@ -1990,15 +1999,15 @@
             return ttb.sptensor.from_data(
                 self.subs[idxSelf],
                 self.vals[idxSelf] * other.vals[idxOther],
                 self.shape,
             )
         if isinstance(other, ttb.tensor):
             csubs = self.subs
-            cvals = self.vals * other[csubs, "extract"][:, None]
+            cvals = self.vals * other[csubs.transpose(), "extract"][:, None]
             return ttb.sptensor.from_data(csubs, cvals, self.shape)
         if isinstance(other, ttb.ktensor):
             csubs = self.subs
             cvals = np.zeros(self.vals.shape)
             R = other.weights.size
             N = self.ndims
             for r in range(R):
@@ -2112,15 +2121,15 @@
         if isinstance(other, ttb.tensor):
             # self zero
             subs1, _ = (other >= 0).find()
             subs1 = subs1[ttb.tt_setdiff_rows(subs1, self.subs), :]
 
             # self nonzero
             subs2 = self.subs[
-                self.vals.transpose()[0] <= other[self.subs, "extract"], :
+                self.vals.transpose()[0] <= other[self.subs.transpose(), "extract"], :
             ]
 
             # assemble
             subs = np.vstack((subs1, subs2))
             return ttb.sptensor.from_data(
                 subs, True * np.ones((len(subs), 1)), self.shape
             )
@@ -2200,15 +2209,17 @@
         # Case 2b: One dense tensor
         if isinstance(other, ttb.tensor):
             # self zero
             subs1, _ = (other > 0).find()
             subs1 = subs1[ttb.tt_setdiff_rows(subs1, self.subs), :]
 
             # self nonzero
-            subs2 = self.subs[self.vals.transpose()[0] < other[self.subs, "extract"], :]
+            subs2 = self.subs[
+                self.vals.transpose()[0] < other[self.subs.transpose(), "extract"], :
+            ]
 
             # assemble
             subs = np.vstack((subs1, subs2))
             return ttb.sptensor.from_data(
                 subs, True * np.ones((len(subs), 1)), self.shape
             )
 
@@ -2255,15 +2266,18 @@
         if isinstance(other, ttb.tensor):
             # self zero
             subs1, _ = (other <= 0).find()
             subs1 = subs1[ttb.tt_setdiff_rows(subs1, self.subs), :]
 
             # self nonzero
             subs2 = self.subs[
-                (self.vals >= other[self.subs, "extract"][:, None]).transpose()[0], :
+                (
+                    self.vals >= other[self.subs.transpose(), "extract"][:, None]
+                ).transpose()[0],
+                :,
             ]
 
             # assemble
             return ttb.sptensor.from_data(
                 np.vstack((subs1, subs2)),
                 True * np.ones((len(subs1) + len(subs2), 1)),
                 self.shape,
@@ -2313,15 +2327,18 @@
             # self zero and other < 0
             subs1, _ = (other < 0).find()
             if subs1.size > 0:
                 subs1 = subs1[ttb.tt_setdiff_rows(subs1, self.subs), :]
 
             # self and other nonzero
             subs2 = self.subs[
-                (self.vals > other[self.subs, "extract"][:, None]).transpose()[0], :
+                (
+                    self.vals > other[self.subs.transpose(), "extract"][:, None]
+                ).transpose()[0],
+                :,
             ]
 
             # assemble
             return ttb.sptensor.from_data(
                 np.vstack((subs1, subs2)),
                 True * np.ones((len(subs1) + len(subs2), 1)),
                 self.shape,
@@ -2416,15 +2433,15 @@
                 newsubs = np.vstack((newsubs, SelfZeroSubs[moresubs, :]))
                 newvals = np.vstack((newvals, morevals))
 
             return ttb.sptensor.from_data(newsubs, newvals, self.shape)
 
         if isinstance(other, ttb.tensor):
             csubs = self.subs
-            cvals = self.vals / other[csubs, "extract"][:, None]
+            cvals = self.vals / other[csubs.transpose(), "extract"][:, None]
             return ttb.sptensor.from_data(csubs, cvals, self.shape)
         if isinstance(other, ttb.ktensor):
             # TODO consider removing epsilon and generating nans consistent with above
             epsilon = np.finfo(float).eps
             subs = self.subs
             vals = np.zeros(self.vals.shape)
             R = (other.weights).size
```

### Comparing `pyttb-1.6.1/pyttb/tenmat.py` & `pyttb-1.6.2/pyttb/tenmat.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 
 import pyttb as ttb
 
 from .pyttb_utils import *
 
 
-class tenmat(object):
+class tenmat:
     """
     TENMAT Store tensor as a matrix.
 
     """
 
     def __init__(self):
         """
```

### Comparing `pyttb-1.6.1/pyttb/tensor.py` & `pyttb-1.6.2/pyttb/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+"""Dense Tensor Implementation"""
 # Copyright 2022 National Technology & Engineering Solutions of Sandia,
 # LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 # U.S. Government retains certain rights in this software.
-"""Dense Tensor Implementation"""
+
 from __future__ import annotations
 
 import logging
+from collections.abc import Iterable
 from itertools import permutations
 from math import factorial
 from typing import Any, Callable, List, Optional, Tuple, Union
 
 import numpy as np
 import scipy.sparse.linalg
 from numpy_groupies import aggregate as accumarray
@@ -697,24 +699,26 @@
                 assert False, f"Entry {i} of list of arrays is wrong size"
 
         szl = int(np.prod(self.shape[0:n]))
         szr = int(np.prod(self.shape[n + 1 :]))
         szn = self.shape[n]
 
         if n == 0:
-            Ur = ttb.khatrirao(U[1 : self.ndims], reverse=True)
+            Ur = ttb.khatrirao(*U[1 : self.ndims], reverse=True)
             Y = np.reshape(self.data, (szn, szr), order="F")
             return Y @ Ur
         if n == self.ndims - 1:  # pylint: disable=no-else-return
-            Ul = ttb.khatrirao(U[0 : self.ndims - 1], reverse=True)
+            Ul = ttb.khatrirao(*U[0 : self.ndims - 1], reverse=True)
             Y = np.reshape(self.data, (szl, szn), order="F")
             return Y.T @ Ul
         else:
-            Ul = ttb.khatrirao(U[n + 1 :], reverse=True)
-            Ur = np.reshape(ttb.khatrirao(U[0:n], reverse=True), (szl, 1, R), order="F")
+            Ul = ttb.khatrirao(*U[n + 1 :], reverse=True)
+            Ur = np.reshape(
+                ttb.khatrirao(*U[0:n], reverse=True), (szl, 1, R), order="F"
+            )
             Y = np.reshape(self.data, (-1, szr), order="F")
             Y = Y @ Ul
             Y = np.reshape(Y, (szl, szn, R), order="F")
             V = np.zeros((szn, R))
             for r in range(R):
                 V[:, [r]] = Y[:, :, r].T @ Ur[:, :, r]
             return V
@@ -1243,17 +1247,15 @@
             if dnew > 2:
                 return ttb.tensor.from_data(
                     np.reshape(y, newshape=sz * np.ones(dnew, dtype=int), order="F")
                 )
             return y
         assert False, "Invalid value for version; should be None, 1, or 2"
 
-    def __setitem__(
-        self, key, value
-    ):  # pylint: disable=too-many-branches, too-many-statements
+    def __setitem__(self, key, value):
         """
         SUBSASGN Subscripted assignment for a tensor.
 
         We can assign elements to a tensor in three ways.
 
         Case 1: X(R1,R2,...,RN) = Y, in which case we replace the
         rectangular subtensor (or single element) specified by the ranges
@@ -1274,132 +1276,157 @@
         X([1;13]) = [5;7] <-- does the same thing
         X(1,1,2:3) = 1 <-- grows tensor
         X(1,1,4) = 1 %<- grows the size of the tensor
         """
         # Figure out if we are doing a subtensor, a list of subscripts or a list of
         # linear indices
         access_type = "error"
-        if self.ndims <= 1:
-            if isinstance(key, np.ndarray):
-                access_type = "subscripts"
-            else:
+        # TODO pull out this big decision tree into a function
+        if isinstance(key, (float, int, np.generic, slice)):
+            access_type = "linear indices"
+        elif self.ndims <= 1:
+            if isinstance(key, tuple):
                 access_type = "subtensor"
+            elif isinstance(key, np.ndarray):
+                access_type = "subscripts"
         else:
             if isinstance(key, np.ndarray):
                 if len(key.shape) > 1 and key.shape[1] >= self.ndims:
                     access_type = "subscripts"
                 elif len(key.shape) == 1 or key.shape[1] == 1:
                     access_type = "linear indices"
             elif isinstance(key, tuple):
                 validSubtensor = [
-                    isinstance(keyElement, (int, slice)) for keyElement in key
+                    isinstance(keyElement, (int, slice, Iterable)) for keyElement in key
                 ]
                 if np.all(validSubtensor):
                     access_type = "subtensor"
+            elif isinstance(key, Iterable):
+                key = np.array(key)
+                if len(key.shape) == 1 or key.shape[1] == 1:
+                    access_type = "linear indices"
 
         # Case 1: Rectangular Subtensor
         if access_type == "subtensor":
-            # Extract array of subscripts
-            subs = key
-
-            # Will the size change? If so we first need to resize x
-            n = self.ndims
-            sliceCheck = []
-            for element in subs:
-                if isinstance(element, slice):
-                    if element.stop is None:
-                        sliceCheck.append(1)
-                    else:
-                        sliceCheck.append(element.stop)
-                else:
-                    sliceCheck.append(element)
-            bsiz = np.array(sliceCheck)
-            if n == 0:
-                newsiz = (bsiz[n:] + 1).astype(int)
-            else:
-                newsiz = np.concatenate(
-                    (np.max((self.shape, bsiz[0:n] + 1), axis=0), bsiz[n:] + 1)
-                ).astype(int)
-            if (newsiz != self.shape).any():
-                # We need to enlarge x.data.
-                newData = np.zeros(shape=tuple(newsiz))
-                idx = [slice(None, currentShape) for currentShape in self.shape]
-                if self.data.size > 0:
-                    newData[tuple(idx)] = self.data
-                self.data = newData
-
-                self.shape = tuple(newsiz)
-            if isinstance(value, ttb.tensor):
-                self.data[key] = value.data
-            else:
-                self.data[key] = value
-
-            return
+            return self._set_subtensor(key, value)
 
         # Case 2a: Subscript indexing
         if access_type == "subscripts":
-            # Extract array of subscripts
-            subs = key
-
-            # Will the size change? If so we first need to resize x
-            n = self.ndims
-            if (
-                len(subs.shape) == 1
-                and len(self.shape) == 1
-                and self.shape[0] < subs.shape[0]
-            ):
-                bsiz = subs
-            elif len(subs.shape) == 1:
-                bsiz = np.array([np.max(subs, axis=0)])
-                key = key.tolist()
-            else:
-                bsiz = np.array(np.max(subs, axis=0))
-            if n == 0:
-                newsiz = (bsiz[n:] + 1).astype(int)
-            else:
-                newsiz = np.concatenate(
-                    (np.max((self.shape, bsiz[0:n] + 1), axis=0), bsiz[n:] + 1)
-                ).astype(int)
-
-            if (newsiz != self.shape).any():
-                # We need to enlarge x.data.
-                newData = np.zeros(shape=tuple(newsiz))
-                idx = [slice(None, currentShape) for currentShape in self.shape]
-                if self.data.size > 0:
-                    newData[idx] = self.data
-                self.data = newData
-
-                self.shape = tuple(newsiz)
-
-            # Finally we can copy in new data
-            if isinstance(key, list):
-                self.data[key] = value
-            elif key.shape[0] == 1:  # and len(key.shape) == 1:
-                self.data[tuple(key[0, :])] = value
-            else:
-                self.data[tuple(key)] = value
-            return
+            return self._set_subscripts(key, value)
 
         # Case 2b: Linear Indexing
         if access_type == "linear indices":
-            idx = key
-            if (idx > np.prod(self.shape)).any():
-                assert (
-                    False
-                ), "TTB:BadIndex In assignment X[I] = Y, a tensor X cannot be resized"
-            idx = tt_ind2sub(self.shape, idx)
-            if idx.shape[0] == 1:
-                self.data[tuple(idx[0, :])] = value
-            else:
-                actualIdx = tuple(idx.transpose())
-                self.data[actualIdx] = value
-            return
+            return self._set_linear(key, value)
 
         assert False, "Invalid use of tensor setitem"
 
+    def _set_linear(self, key, value):
+        idx = key
+        if not isinstance(idx, slice) and (idx > np.prod(self.shape)).any():
+            assert (
+                False
+            ), "TTB:BadIndex In assignment X[I] = Y, a tensor X cannot be resized"
+        if isinstance(key, (int, float, np.generic)):
+            idx = np.array([key])
+        elif isinstance(key, slice):
+            idx = np.array(range(np.prod(self.shape))[key])
+        idx = tt_ind2sub(self.shape, idx)
+        if idx.shape[0] == 1:
+            self.data[tuple(idx[0, :])] = value
+        else:
+            actualIdx = tuple(idx.transpose())
+            self.data[actualIdx] = value
+
+    def _set_subtensor(self, key, value):
+        # Extract array of subscripts
+        subs = key
+        # Will the size change? If so we first need to resize x
+        n = self.ndims
+        sliceCheck = []
+        for element in subs:
+            if isinstance(element, slice):
+                if element.stop is None:
+                    sliceCheck.append(1)
+                else:
+                    sliceCheck.append(element.stop)
+            elif isinstance(element, Iterable):
+                if any(
+                    not isinstance(entry, (float, int, np.generic)) for entry in element
+                ):
+                    raise ValueError(
+                        f"Entries for setitem must be numeric but recieved, {element}"
+                    )
+                sliceCheck.append(max(element))
+            else:
+                sliceCheck.append(element)
+        bsiz = np.array(sliceCheck)
+        if n == 0:
+            newsiz = (bsiz[n:] + 1).astype(int)
+        else:
+            newsiz = np.concatenate(
+                (np.max((self.shape, bsiz[0:n] + 1), axis=0), bsiz[n:] + 1)
+            ).astype(int)
+        if not np.array_equal(newsiz, self.shape):
+            # We need to enlarge x.data.
+            newData = np.zeros(shape=tuple(newsiz))
+            if self.data.size > 0:
+                idx = [slice(None, currentShape) for currentShape in self.shape]
+                idx.extend([0] * (len(newsiz) - self.ndims))
+                newData[tuple(idx)] = self.data
+            self.data = newData
+
+            self.shape = tuple(newsiz)
+        if isinstance(value, ttb.tensor):
+            self.data[key] = value.data
+        else:
+            self.data[key] = value
+
+    def _set_subscripts(self, key, value):
+        # Extract array of subscripts
+        subs = key
+
+        # Will the size change? If so we first need to resize x
+        n = self.ndims
+        if (
+            len(subs.shape) == 1
+            and len(self.shape) == 1
+            and self.shape[0] < subs.shape[0]
+        ):
+            bsiz = subs
+        elif len(subs.shape) == 1:
+            bsiz = np.array([np.max(subs, axis=0)])
+            key = key.tolist()
+        else:
+            bsiz = np.array(np.max(subs, axis=0))
+        if n == 0:
+            newsiz = (bsiz[n:] + 1).astype(int)
+        else:
+            newsiz = np.concatenate(
+                (np.max((self.shape, bsiz[0:n] + 1), axis=0), bsiz[n:] + 1)
+            ).astype(int)
+
+        if not np.array_equal(newsiz, self.shape):
+            # We need to enlarge x.data.
+            newData = np.zeros(shape=tuple(newsiz))
+            if self.data.size > 0:
+                idx = [slice(None, currentShape) for currentShape in self.shape]
+                idx.extend([0] * (len(newsiz) - self.ndims))
+                newData[tuple(idx)] = self.data
+            self.data = newData
+
+            self.shape = tuple(newsiz)
+
+        # Finally we can copy in new data
+        if isinstance(key, list):
+            self.data[key] = value
+        elif key.shape[0] == 1:  # and len(key.shape) == 1:
+            self.data[tuple(key[0, :])] = value
+        else:
+            self.data[tuple(key)] = value
+
     def __getitem__(self, item):
         """
         SUBSREF Subscripted reference for tensors.
 
         We can extract elements or subtensors from a tensor in the
         following ways.
 
@@ -1435,14 +1462,25 @@
         Parameters
         ----------
 
         Returns
         -------
         :class:`pyttb.tensor` or :class:`numpy.ndarray`
         """
+        # Case 0: Single Index Linear
+        if isinstance(item, (int, float, np.generic, slice)):
+            if isinstance(item, (int, float, np.generic)):
+                idx = np.array(item)
+            elif isinstance(item, slice):
+                idx = np.array(range(np.prod(self.shape))[item])
+            a = np.squeeze(
+                self.data[tuple(ttb.tt_ind2sub(self.shape, idx).transpose())]
+            )
+            # Todo if row make column?
+            return ttb.tt_subsubsref(a, idx)
         # Case 1: Rectangular Subtensor
         if (
             isinstance(item, tuple)
             and len(item) == self.ndims
             and item[len(item) - 1] != "extract"
         ):
             # Copy the subscripts
@@ -1476,25 +1514,36 @@
             if newsiz.size == 0:
                 a = newdata
             else:
                 a = ttb.tensor.from_data(newdata)
             return a
 
         # *** CASE 2a: Subscript indexing ***
-        if len(item) > 1 and isinstance(item[-1], str) and item[-1] == "extract":
+        if isinstance(item, np.ndarray) and len(item) > 1:
             # Extract array of subscripts
+            subs = np.array(item)
+            a = np.squeeze(self.data[tuple(subs)])
+            # TODO if is row make column?
+            return ttb.tt_subsubsref(a, subs)
+        if (
+            len(item) > 1
+            and isinstance(item[0], np.ndarray)
+            and isinstance(item[-1], str)
+            and item[-1] == "extract"
+        ):
+            # TODO dry this up
             subs = np.array(item[0])
-            a = np.squeeze(self.data[tuple(subs.transpose())])
+            a = np.squeeze(self.data[tuple(subs)])
             # TODO if is row make column?
             return ttb.tt_subsubsref(a, subs)
 
         # Case 2b: Linear Indexing
-        if len(item) >= 2 and not isinstance(item[-1], str):
+        if isinstance(item, tuple) and len(item) >= 2 and not isinstance(item[-1], str):
             assert False, "Linear indexing requires single input array"
-        idx = item[0]
+        idx = np.array(item)
         a = np.squeeze(self.data[tuple(ttb.tt_ind2sub(self.shape, idx).transpose())])
         # Todo if row make column?
         return ttb.tt_subsubsref(a, idx)
 
     def __eq__(self, other):
         """
         Equal for tensors
```

### Comparing `pyttb-1.6.1/pyttb/ttensor.py` & `pyttb-1.6.2/pyttb/ttensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pyttb import ktensor
 from pyttb import pyttb_utils as ttb_utils
 from pyttb import sptenmat, sptensor, tenmat, tensor
 
 ALT_CORE_ERROR = "TTensor doesn't support non-tensor cores yet"
 
 
-class ttensor(object):
+class ttensor:
     """
     TTENSOR Class for Tucker tensors (decomposed).
 
     """
 
     def __init__(self):
         """
```

### Comparing `pyttb-1.6.1/pyttb/tucker_als.py` & `pyttb-1.6.2/pyttb/tucker_als.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,33 @@
+# Copyright 2022 National Technology & Engineering Solutions of Sandia,
+# LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
+# U.S. Government retains certain rights in this software.
+
 from numbers import Real
 
 import numpy as np
 
 from pyttb.ttensor import ttensor
 
 
 def tucker_als(
-    tensor, rank, stoptol=1e-4, maxiters=1000, dimorder=None, init="random", printitn=1
+    input_tensor,
+    rank,
+    stoptol=1e-4,
+    maxiters=1000,
+    dimorder=None,
+    init="random",
+    printitn=1,
 ):
     """
     Compute Tucker decomposition with alternating least squares
 
     Parameters
     ----------
-    tensor: :class:`pyttb.tensor`
+    input_tensor: :class:`pyttb.tensor`
     rank: int, list[int]
         Rank of the decomposition(s)
     stoptol: float
         Tolerance used for termination - when the change in the fitness function in successive iterations drops
         below this value, the iterations terminate (default: 1e-4)
     dimorder: list
         Order to loop through dimensions (default: [range(tensor.ndims)])
@@ -44,16 +54,16 @@
 
             * `params` : tuple of (stoptol, maxiters, printitn, dimorder)
             * `iters`: number of iterations performed
             * `normresidual`: norm of the difference between the input tensor and ktensor factorization
             * `fit`: value of the fitness function (fraction of tensor data explained by the model)
 
     """
-    N = tensor.ndims
-    normX = tensor.norm()
+    N = input_tensor.ndims
+    normX = input_tensor.norm()
 
     # TODO: These argument checks look common with CP-ALS factor out
     if not isinstance(stoptol, Real):
         raise ValueError(
             f"stoptol must be a real valued scalar but received: {stoptol}"
         )
     if not isinstance(maxiters, Real) or maxiters < 0:
@@ -82,34 +92,34 @@
     if isinstance(init, list):
         Uinit = init
         if len(init) != N:
             raise ValueError(
                 f"Init needs to be of length tensor.ndim (which was {N}) but only got length {len(init)}."
             )
         for n in dimorder[1::]:
-            correct_shape = (tensor.shape[n], rank[n])
+            correct_shape = (input_tensor.shape[n], rank[n])
             if Uinit[n].shape != correct_shape:
                 raise ValueError(
                     f"Init factor {n} had incorrect shape. Expected {correct_shape} but got {Uinit[n].shape}"
                 )
     elif isinstance(init, str) and init.lower() == "random":
         Uinit = [None] * N
         # Observe that we don't need to calculate an initial guess for the
         # first index in dimorder because that will be solved for in the first
         # inner iteration.
         for n in range(1, N):
-            Uinit[n] = np.random.uniform(0, 1, (tensor.shape[n], rank[n]))
+            Uinit[n] = np.random.uniform(0, 1, (input_tensor.shape[n], rank[n]))
     elif isinstance(init, str) and init.lower() in ("nvecs", "eigs"):
         # Compute an orthonormal basis for the dominant
         # Rn-dimensional left singular subspace of
         # X_(n) (0 <= n < N).
         Uinit = [None] * N
         for n in dimorder[1::]:
             print(f" Computing {rank[n]} leading e-vector for factor {n}.\n")
-            Uinit[n] = tensor.nvecs(n, rank[n])
+            Uinit[n] = input_tensor.nvecs(n, rank[n])
     else:
         raise ValueError(
             f"The selected initialization method is not supported. Provided: {init}"
         )
 
     # Set up for iterations - initializing U and the fit.
     U = Uinit.copy()
@@ -120,15 +130,15 @@
 
     # Main loop: Iterate until convergence
     for iter in range(maxiters):
         fitold = fit
 
         # Iterate over all N modes of the tensor
         for n in dimorder:
-            Utilde = tensor.ttm(U, exclude_dims=n, transpose=True)
+            Utilde = input_tensor.ttm(U, exclude_dims=n, transpose=True)
             # Maximize norm(Utilde x_n W') wrt W and
             # maintain orthonormality of W
             U[n] = Utilde.nvecs(n, rank[n])
 
         # Assemble the current approximation
         core = Utilde.ttm(U, n, transpose=True)
```

### Comparing `pyttb-1.6.1/pyttb.egg-info/PKG-INFO` & `pyttb-1.6.2/pyttb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttb
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python Tensor Toolbox
 Author-email: "Daniel M. Dunlavy" <dmdunla@sandia.gov>
 License: BSD 2-Clause License
 Project-URL: homepage, https://github.com/sandialabs/pyttb
 Project-URL: coverage, https://coveralls.io/github/sandialabs/pyttb
 Project-URL: documentation, https://pyttb.readthedocs.io
 Classifier: License :: OSI Approved :: BSD License
@@ -39,11 +39,11 @@
 * `cp_als`, `cp_apr`: Canonical Polyadic (CP) decompositions
 * `tucker_als`: Tucker decompostions
 
 # Getting Started
 Check out the [Documentation](https://pyttb.readthedocs.io) to get started.
 
 # Contributing
-Check out our [contributing guide](CONTRIBUTOR_GUIDE.md).
+Check out our [contributing guide](CONTRIBUTING.md).
 
 ---
 [![Regression tests](https://github.com/sandialabs/pyttb/actions/workflows/regression-tests.yml/badge.svg)](https://github.com/sandialabs/pyttb/actions/workflows/regression-tests.yml) [![Coverage Status](https://coveralls.io/repos/github/sandialabs/pyttb/badge.svg?branch=main)](https://coveralls.io/github/sandialabs/pyttb?branch=main)
```

### Comparing `pyttb-1.6.1/pyttb.egg-info/SOURCES.txt` & `pyttb-1.6.2/pyttb.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -30,12 +30,17 @@
 tests/test_hosvd.py
 tests/test_import_export_data.py
 tests/test_khatrirao.py
 tests/test_ktensor.py
 tests/test_package.py
 tests/test_packaging.py
 tests/test_pyttb_utils.py
+tests/test_sptenmat.py
 tests/test_sptensor.py
+tests/test_sptensor3.py
+tests/test_sumtensor.py
+tests/test_symktensor.py
+tests/test_symtensor.py
 tests/test_tenmat.py
 tests/test_tensor.py
 tests/test_ttensor.py
 tests/test_tucker_als.py
```

### Comparing `pyttb-1.6.1/tests/test_cp_als.py` & `pyttb-1.6.2/tests/test_cp_als.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.1/tests/test_cp_apr.py` & `pyttb-1.6.2/tests/test_cp_apr.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     weights = np.array([1.0, 2.0])
     fm0 = np.array([[0.0, 0.0], [3.0, 4.0]])
     fm1 = np.array([[0.0, 6.0], [7.0, 8.0]])
     factor_matrices = [fm0, fm1]
     ktensorInstance = ttb.ktensor.from_data(weights, factor_matrices)
     tensorInstance = ktensorInstance.full()
     np.random.seed(123)
-    M, _, _ = ttb.cp_apr(tensorInstance, 2)
+    M, _, _ = ttb.cp_apr(tensorInstance, 2, printinneritn=1)
     # Consume the cp_apr diagnostic printing
     capsys.readouterr()
     assert np.isclose(M.full().data, ktensorInstance.full().data).all()
     # Assert given an inital guess of the final answer yields immediate convergence
     M, _, output = ttb.cp_apr(tensorInstance, 2, init=ktensorInstance)
     capsys.readouterr()
     assert output["nTotalIters"] == 2
@@ -171,15 +171,17 @@
     weights = np.array([1.0, 2.0])
     fm0 = np.array([[0.0, 0.0], [3.0, 4.0]])
     fm1 = np.array([[0.0, 6.0], [7.0, 8.0]])
     factor_matrices = [fm0, fm1]
     ktensorInstance = ttb.ktensor.from_data(weights, factor_matrices)
     tensorInstance = ktensorInstance.full()
     np.random.seed(123)
-    M, _, _ = ttb.cp_apr(tensorInstance, 2, algorithm="pdnr")
+    M, _, _ = ttb.cp_apr(
+        tensorInstance, 2, algorithm="pdnr", printinneritn=1, inexact=False
+    )
     capsys.readouterr()
     assert np.isclose(M.full().data, ktensorInstance.full().data, rtol=1e-04).all()
 
     # Try solve with sptensor
     sptensorInstance = ttb.sptensor.from_tensor_type(tensorInstance)
     np.random.seed(123)
     M, _, _ = ttb.cp_apr(sptensorInstance, 2, algorithm="pdnr")
@@ -217,15 +219,15 @@
     weights = np.array([1.0, 2.0])
     fm0 = np.array([[1.0, 1.0], [3.0, 4.0]])
     fm1 = np.array([[1.0, 6.0], [7.0, 8.0]])
     factor_matrices = [fm0, fm1]
     ktensorInstance = ttb.ktensor.from_data(weights, factor_matrices)
     tensorInstance = ktensorInstance.full()
     np.random.seed(123)
-    M, _, _ = ttb.cp_apr(tensorInstance, 2, algorithm="pqnr")
+    M, _, _ = ttb.cp_apr(tensorInstance, 2, algorithm="pqnr", printinneritn=1)
     capsys.readouterr()
     assert np.isclose(M.full().data, ktensorInstance.full().data, rtol=1e-01).all()
 
     # Try solve with sptensor
     sptensorInstance = ttb.sptensor.from_tensor_type(tensorInstance)
     np.random.seed(123)
     M, _, _ = ttb.cp_apr(sptensorInstance, 2, algorithm="pqnr")
```

### Comparing `pyttb-1.6.1/tests/test_hosvd.py` & `pyttb-1.6.2/tests/test_hosvd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright 2022 National Technology & Engineering Solutions of Sandia,
+# LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
+# U.S. Government retains certain rights in this software.
+
 import numpy as np
 import pytest
 
 import pyttb as ttb
 
 
 @pytest.fixture()
```

### Comparing `pyttb-1.6.1/tests/test_khatrirao.py` & `pyttb-1.6.2/tests/test_khatrirao.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,39 +20,40 @@
             [16, 50, 108],
             [4, 20, 54],
             [16, 50, 108],
             [16, 50, 108],
             [64, 125, 216],
         ]
     )
-    assert (ttb.khatrirao([A, A, A]) == answer).all()
-    assert (ttb.khatrirao([A, A, A], reverse=True) == answer).all()
+    assert (ttb.khatrirao(*[A, A, A]) == answer).all()
+    assert (ttb.khatrirao(*[A, A, A], reverse=True) == answer).all()
     assert (ttb.khatrirao(A, A, A) == answer).all()
 
     # Test case where inputs are column vectors
     a_1 = np.array([[1], [1], [1], [1]])
     a_2 = np.array([[0], [1], [2], [3]])
     a_3 = np.array([[0, 0], [1, 0], [2, 0], [3, 0]])
     result = np.vstack(
         (
             a_2[0, 0] * np.ones((16, 1)),
             a_2[1, 0] * np.ones((16, 1)),
             a_2[2, 0] * np.ones((16, 1)),
             a_2[3, 0] * np.ones((16, 1)),
         )
     )
-    assert (ttb.khatrirao([a_2, a_1, a_1]) == result).all()
+    assert (ttb.khatrirao(*[a_2, a_1, a_1]) == result).all()
     assert (ttb.khatrirao(a_2, a_1, a_1) == result).all()
 
     with pytest.raises(AssertionError) as excinfo:
-        ttb.khatrirao([a_2, a_1, a_1], a_2)
-    assert "Khatri Rao Acts on multiple Array arguments or a list of Arrays" in str(
-        excinfo
-    )
-
-    with pytest.raises(AssertionError) as excinfo:
         ttb.khatrirao(a_2, a_1, np.ones((2, 2, 2)))
     assert "Each argument must be a matrix" in str(excinfo)
 
     with pytest.raises(AssertionError) as excinfo:
         ttb.khatrirao(a_2, a_1, a_3)
     assert "All matrices must have the same number of columns." in str(excinfo)
+
+    # Check old interface error
+    with pytest.raises(ValueError):
+        ttb.khatrirao([a_1, a_1, a_1])
+
+    with pytest.raises(ValueError):
+        ttb.khatrirao(a_1, a_1, reverse="cat")
```

### Comparing `pyttb-1.6.1/tests/test_ktensor.py` & `pyttb-1.6.2/tests/test_ktensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,14 +370,32 @@
         ]
     )
     factor_matrix11 = np.array([[0.5812381937190965, -0.6], [0.813733471206735, -0.8]])
     assert np.linalg.norm(K.weights - weights1) < 1e-8
     assert np.linalg.norm(K.factor_matrices[0] - factor_matrix10) < 1e-8
     assert np.linalg.norm(K.factor_matrices[1] - factor_matrix11) < 1e-8
 
+    # test invalid call with non-ktensor argument
+    with pytest.raises(AssertionError) as excinfo:
+        K = K.fixsigns([1, 2, 3])
+    assert "other must be a ktensor" in str(excinfo)
+
+    # test odd number of vectors to flip
+    K = ttb.ktensor.from_data(
+        np.array([3, 2, 1]), np.ones((3, 3)), np.ones((4, 3)), np.ones((5, 3))
+    )
+    K2 = K.copy()
+    # one column to flip
+    K2.factor_matrices[0][:, 0] = -1
+    # 3 columns to flip
+    K2.factor_matrices[0][:, 0] = -1
+    K2.factor_matrices[1][:, 1] = -1
+    K2.factor_matrices[2][:, 2] = -1
+    K = K.fixsigns(K2)
+
 
 @pytest.mark.indevelopment
 def test_ktensor_full(sample_ktensor_2way, sample_ktensor_3way):
     (data, K2) = sample_ktensor_2way
     assert K2.full().isequal(
         ttb.tensor.from_data(np.array([[29.0, 39.0], [63.0, 85.0]]), (2, 2))
     )
@@ -810,14 +828,24 @@
     # compare just factor matrices (i.e., do not use weights)
     score, Aperm, flag, best_perm = A.score(B, weight_penalty=False)
     assert score == 1.0
     assert np.allclose(Aperm.weights, np.array([15.49193338, 7.74596669, 23.23790008]))
     assert flag == 1
     assert (best_perm == np.array([0, 1, 2])).all()
 
+    # zero lambda values lead to equal components
+    A0 = ttb.ktensor.from_data(
+        np.array([2, 0]), np.ones((3, 2)), np.ones((4, 2)), np.ones((5, 2))
+    )
+    B0 = ttb.ktensor.from_data(
+        np.array([2, 0]), np.ones((3, 2)), np.ones((4, 2)), np.ones((5, 2))
+    )
+    score, Aperm, flag, best_perm = A0.score(B0)
+    assert score == 1.0
+
     # compute score using exhaustive search
     with pytest.raises(AssertionError) as excinfo:
         score, Aperm, flag, best_perm = A.score(B, greedy=False)
     assert "Not yet implemented. Only greedy method is implemented currently." in str(
         excinfo
     )
 
@@ -831,14 +859,23 @@
         # A is 3x4x5; B is 3x4x4
         B = ttb.ktensor.from_data(
             np.array([2, 4]), np.ones((3, 2)), np.ones((4, 2)), np.ones((4, 2))
         )
         score, Aperm, flag, best_perm = A.score(B)
     assert "Size mismatch" in str(excinfo)
 
+    # invalid: number of compnents of first ktensor must be greater than or
+    # equal to number of components of second ktensor
+    with pytest.raises(AssertionError) as excinfo:
+        B = ttb.ktensor.from_data(
+            np.array([2, 4]), np.ones((3, 2)), np.ones((4, 2)), np.ones((5, 2))
+        )
+        score, Aperm, flag, best_perm = B.score(A)
+    assert "Tensor A must have at least as many components as tensor B" in str(excinfo)
+
 
 pytest.mark.indevelopment
 
 
 def test_ktensor_shape(sample_ktensor_2way, sample_ktensor_3way):
     (data, K0) = sample_ktensor_2way
     assert K0.shape == (2, 2)
```

### Comparing `pyttb-1.6.1/tests/test_pyttb_utils.py` & `pyttb-1.6.2/tests/test_pyttb_utils.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.1/tests/test_sptensor.py` & `pyttb-1.6.2/tests/test_sptensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,17 +289,17 @@
     )
     assert sptensorInstance[:, :, :].isequal(
         sptensorInstance[[0, 1, 2, 3], [0, 1, 2, 3], [0, 1, 2, 3]]
     )
 
     # TODO need to understand what this intends to do
     ## Case 2 subscript indexing
-    assert sptensorInstance[np.array([[1, 2, 1]])] == np.array([[0]])
+    assert sptensorInstance[np.array([[1], [2], [1]])] == np.array([[0]])
     assert (
-        sptensorInstance[np.array([[1, 2, 1], [1, 3, 1]])] == np.array([[0], [0]])
+        sptensorInstance[np.array([[1, 1], [2, 3], [1, 1]])] == np.array([[0], [0]])
     ).all()
 
     ## Case 2 Linear Indexing
     ind = ttb.tt_sub2ind(data["shape"], np.array([[1, 1, 1], [1, 1, 3], [2, 2, 2]]))
     assert (sptensorInstance[ind] == np.array([[0.5], [1.5], [2.5]])).all()
     list_ind = list(ind)
     assert (sptensorInstance[list_ind] == np.array([[0.5], [1.5], [2.5]])).all()
@@ -437,14 +437,20 @@
     old_value = data["vals"][1, 0]
     sptensorInstance[1, 1, 3] = 0
     subSelection = [0, 2, 3]
     assert (sptensorInstance.subs == data["subs"][subSelection]).all()
     assert (sptensorInstance.vals == data["vals"][subSelection]).all()
     assert sptensorInstance.shape == data["shape"]
 
+    # Case I(b)i: Set with non-zero, no subs exist
+    empty_tensor = ttb.sptensor()
+    empty_tensor[0, 0] = 1
+    # Validate entry worked correctly
+    empty_tensor.__repr__()
+
     # Case I(b)i: Set with zero, sub doesn't exist
     sptensorInstance[1, 1, 3] = old_value
     reorder = [0, 2, 3, 1]
     assert (sptensorInstance.subs == data["subs"][reorder]).all()
     assert (sptensorInstance.vals == data["vals"][reorder]).all()
     assert sptensorInstance.shape == data["shape"]
     # Reset tensor data
@@ -523,14 +529,26 @@
     sptensorInstance[1, 1, 2] = 7
     assert (
         sptensorInstance.subs == np.vstack((data["subs"], np.array([[1, 1, 2]])))
     ).all()
     assert (sptensorInstance.vals == np.vstack((data["vals"], np.array([[7]])))).all()
     assert sptensorInstance.shape == data["shape"]
 
+    # Case I(b)ii: Set with scalar, iterable index, empty sptensor
+    someTensor = ttb.sptensor()
+    someTensor[[0, 1], 0] = 1
+    assert someTensor[0, 0] == 1
+    assert someTensor[1, 0] == 1
+    assert np.all(someTensor[[0, 1], 0].vals == 1)
+    # Case I(b)ii: Set with scalar, iterable index, non-empty sptensor
+    someTensor[[0, 1], 1] = 2
+    assert someTensor[0, 1] == 2
+    assert someTensor[1, 1] == 2
+    assert np.all(someTensor[[0, 1], 1].vals == 2)
+
     # Case I: Assign with non-scalar or sptensor
     sptensorInstanceLarger = ttb.sptensor.from_tensor_type(sptensorInstance)
     with pytest.raises(AssertionError) as excinfo:
         sptensorInstanceLarger[1, 1, 1] = "String"
     assert "Invalid assignment value" in str(excinfo)
 
 
@@ -541,82 +559,89 @@
     # Case II: Too few modes in setitem key
     with pytest.raises(AssertionError) as excinfo:
         sptensorInstance[np.array([1, 1]).astype(int)] = 999.0
     assert "Invalid subscripts" in str(excinfo)
 
     # Case II: Too few keys in setitem for number of assignement values
     with pytest.raises(AssertionError) as excinfo:
-        sptensorInstance[np.array([1, 1, 1]).astype(int)] = np.array([[999.0], [888.0]])
+        sptensorInstance[np.array([[1], [1], [1]]).astype(int)] = np.array(
+            [[999.0], [888.0]]
+        )
     assert "Number of subscripts and number of values do not match!" in str(excinfo)
 
     # Case II: Warning For duplicates
     with pytest.warns(Warning) as record:
-        sptensorInstance[np.array([[1, 1, 1], [1, 1, 1]]).astype(int)] = np.array(
+        sptensorInstance[np.array([[1, 1], [1, 1], [1, 1]]).astype(int)] = np.array(
             [[999.0], [999.0]]
         )
     assert "Duplicate assignments discarded" in str(record[0].message)
 
+    # Case II: Single entry, no subs exist
+    empty_tensor = ttb.sptensor()
+    empty_tensor[np.array([[0, 1], [2, 2]])] = 4
+    assert np.all(empty_tensor[np.array([[0, 1], [2, 2]])] == 4)
+
     # Case II: Single entry, for single sub that exists
-    sptensorInstance[np.array([1, 1, 1]).astype(int)] = 999.0
-    assert (sptensorInstance[np.array([[1, 1, 1]])] == np.array([[999]])).all()
+    sptensorInstance[np.array([[1], [1], [1]]).astype(int)] = 999.0
+    assert (sptensorInstance[np.array([[1], [1], [1]])] == np.array([[999]])).all()
     assert (sptensorInstance.subs == data["subs"]).all()
 
     # Case II: Single entry, for multiple subs that exist
     (data, sptensorInstance) = sample_sptensor
-    sptensorInstance[np.array([[1, 1, 1], [1, 1, 3]]).astype(int)] = 999.0
+    sptensorInstance[np.array([[1, 1], [1, 1], [1, 3]]).astype(int)] = 999.0
     assert (
-        sptensorInstance[np.array([[1, 1, 1], [1, 1, 3]])] == np.array([[999], [999]])
+        sptensorInstance[np.array([[1, 1], [1, 1], [1, 3]])] == np.array([[999], [999]])
     ).all()
     assert (sptensorInstance.subs == data["subs"]).all()
 
     # Case II: Multiple entries, for multiple subs that exist
     (data, sptensorInstance) = sample_sptensor
-    sptensorInstance[np.array([[1, 1, 1], [1, 1, 3]]).astype(int)] = np.array(
+    sptensorInstance[np.array([[1, 1], [1, 1], [1, 3]]).astype(int)] = np.array(
         [[888], [999]]
     )
     assert (
-        sptensorInstance[np.array([[1, 1, 3], [1, 1, 1]])] == np.array([[999], [888]])
+        sptensorInstance[np.array([[1, 1], [1, 1], [3, 1]])] == np.array([[999], [888]])
     ).all()
     assert (sptensorInstance.subs == data["subs"]).all()
 
     # Case II: Single entry, for single sub that doesn't exist
     (data, sptensorInstance) = sample_sptensor
     copy = ttb.sptensor.from_tensor_type(sptensorInstance)
-    copy[np.array([[1, 1, 2]]).astype(int)] = 999.0
-    assert (copy[np.array([[1, 1, 2]])] == np.array([999])).all()
+    copy[np.array([[1], [1], [2]]).astype(int)] = 999.0
+    assert (copy[np.array([[1], [1], [2]])] == np.array([999])).all()
     assert (copy.subs == np.concatenate((data["subs"], np.array([[1, 1, 2]])))).all()
 
     # Case II: Single entry, for single sub that doesn't exist, expand dimensions
     (data, sptensorInstance) = sample_sptensor
     copy = ttb.sptensor.from_tensor_type(sptensorInstance)
-    copy[np.array([[1, 1, 2, 1]]).astype(int)] = 999.0
-    assert (copy[np.array([[1, 1, 2, 1]])] == np.array([999])).all()
+    copy[np.array([[1], [1], [2], [1]]).astype(int)] = 999.0
+    assert (copy[np.array([[1], [1], [2], [1]])] == np.array([999])).all()
     # assert (copy.subs == np.concatenate((data['subs'], np.array([[1, 1, 2]])))).all()
 
     # Case II: Single entry, for multiple subs one that exists and the other doesn't
     (data, sptensorInstance) = sample_sptensor
     copy = ttb.sptensor.from_tensor_type(sptensorInstance)
-    copy[np.array([[1, 1, 1], [2, 1, 3]]).astype(int)] = 999.0
-    assert (copy[np.array([[2, 1, 3]])] == np.array([999])).all()
+    copy[np.array([[1, 2], [1, 1], [1, 3]]).astype(int)] = 999.0
+    assert (copy[np.array([[2], [1], [3]])] == np.array([999])).all()
     assert (copy.subs == np.concatenate((data["subs"], np.array([[2, 1, 3]])))).all()
 
     # Case II: Multiple entries, for multiple subs that don't exist
     (data, sptensorInstance) = sample_sptensor
     copy = ttb.sptensor.from_tensor_type(sptensorInstance)
-    copy[np.array([[1, 1, 2], [2, 1, 3]]).astype(int)] = np.array([[888], [999]])
-    assert (copy[np.array([[1, 1, 2], [2, 1, 3]])] == np.array([[888], [999]])).all()
+    copy[np.array([[1, 2], [1, 1], [2, 3]]).astype(int)] = np.array([[888], [999]])
+    assert (copy[np.array([[1, 2], [1, 1], [2, 3]])] == np.array([[888], [999]])).all()
     assert (
         copy.subs == np.concatenate((data["subs"], np.array([[1, 1, 2], [2, 1, 3]])))
     ).all()
 
     # Case II: Multiple entries, for multiple subs that exist and need to be removed
     (data, sptensorInstance) = sample_sptensor
     copy = ttb.sptensor.from_tensor_type(sptensorInstance)
-    copy[np.array([[1, 1, 1], [1, 1, 3]]).astype(int)] = np.array([[0], [0]])
-    assert (copy[np.array([[1, 1, 2], [2, 1, 3]])] == np.array([[0], [0]])).all()
+    copy[np.array([[1, 1], [1, 1], [1, 3]]).astype(int)] = np.array([[0], [0]])
+    assert (copy[np.array([[1, 2], [1, 1], [1, 3]])] == np.array([[0], [0]])).all()
     assert (copy.subs == np.array([[2, 2, 2], [3, 3, 3]])).all()
 
 
 @pytest.mark.indevelopment
 def test_sptensor_norm(sample_sptensor):
     (data, sptensorInstance) = sample_sptensor
     assert sptensorInstance.norm() == np.linalg.norm(data["vals"])
```

### Comparing `pyttb-1.6.1/tests/test_tenmat.py` & `pyttb-1.6.2/tests/test_tenmat.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.1/tests/test_tensor.py` & `pyttb-1.6.2/tests/test_tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,28 @@
     dataGrowth[0:2, 0:3] = dataCopy
     assert (tensorInstance.data == dataGrowth).all()
 
     # Subtensor assign with tensor
     tensorInstance[:, :] = tensorInstance
     assert (tensorInstance.data == dataGrowth).all()
 
+    # Subtensor add element to empty tensor
+    empty_tensor = ttb.tensor()
+    empty_tensor[0, 0] = 1
+
+    # Subtensor add dimension
+    empty_tensor[0, 0, 0] = 2
+
+    # Subtensor with lists
+    some_tensor = ttb.tenones((3, 3))
+    some_tensor[[0, 1], [0, 1]] = 11
+    assert some_tensor[0, 0] == 11
+    assert some_tensor[1, 1] == 11
+    assert np.all(some_tensor[[0, 1], [0, 1]].data == 11)
+
     # Subscripts with constant
     tensorInstance[np.array([[1, 1]])] = 13.0
     dataGrowth[1, 1] = 13.0
     assert (tensorInstance.data == dataGrowth).all()
 
     # Subscripts with array
     tensorVector = ttb.tensor.from_data(np.array([0, 0, 0, 0]))
@@ -255,24 +269,48 @@
     assert (tensorVector.data == np.array([3, 4, 5, 0])).all()
 
     # Subscripts with constant
     tensorInstance[np.array([[1, 1], [1, 2]])] = 13.0
     dataGrowth[([1, 1], [1, 2])] = 13.0
     assert (tensorInstance.data == dataGrowth).all()
 
+    # Subscripts add element to empty tensor
+    empty_tensor = ttb.tensor()
+    first_arbitrary_index = np.array([[0, 1], [2, 2]])
+    second_arbitrary_index = np.array([[1, 2], [3, 3]])
+    value = 4
+    empty_tensor[first_arbitrary_index] = value
+    # Subscripts grow existing tensor
+    empty_tensor[second_arbitrary_index] = value
+
     # Linear Index with constant
     tensorInstance[np.array([0])] = 13.0
     dataGrowth[np.unravel_index([0], dataGrowth.shape, "F")] = 13.0
     assert (tensorInstance.data == dataGrowth).all()
 
+    tensorInstance[0] = 14.0
+    dataGrowth[np.unravel_index([0], dataGrowth.shape, "F")] = 14.0
+    assert (tensorInstance.data == dataGrowth).all()
+
+    tensorInstance[0:1] = 14.0
+    dataGrowth[np.unravel_index([0], dataGrowth.shape, "F")] = 14.0
+    assert (tensorInstance.data == dataGrowth).all()
+
     # Linear Index with constant
     tensorInstance[np.array([0, 3, 4])] = 13.0
     dataGrowth[np.unravel_index([0, 3, 4], dataGrowth.shape, "F")] = 13
     assert (tensorInstance.data == dataGrowth).all()
 
+    # Linear index with multiple indicies
+    some_tensor = ttb.tenones((3, 3))
+    some_tensor[[0, 1]] = 2
+    assert some_tensor[0] == 2
+    assert some_tensor[1] == 2
+    assert np.array_equal(some_tensor[[0, 1]], [2, 2])
+
     # Test Empty Tensor Set Item, subtensor
     emptyTensor = ttb.tensor.from_data(np.array([]))
     emptyTensor[0, 0, 0] = 0
     assert (emptyTensor.data == np.array([[[0]]])).all()
     assert emptyTensor.shape == (1, 1, 1)
 
     # Test Empty Tensor Set Item, subscripts
@@ -285,16 +323,24 @@
     with pytest.raises(AssertionError) as excinfo:
         tensorInstance[np.array([0, 3, 99])] = 13.0
     assert "TTB:BadIndex In assignment X[I] = Y, a tensor X cannot be resized" in str(
         excinfo
     )
 
     # Attempting to set some other way
-    with pytest.raises(AssertionError) as excinfo:
+    with pytest.raises(ValueError) as excinfo:
         tensorInstance[0, "a", 5] = 13.0
+    assert "must be numeric" in str(excinfo)
+
+    with pytest.raises(AssertionError) as excinfo:
+
+        class BadKey:
+            pass
+
+        tensorInstance[BadKey] = 13.0
     assert "Invalid use of tensor setitem" in str(excinfo)
 
 
 @pytest.mark.indevelopment
 def test_tensor__getitem__(sample_tensor_2way):
     (params, tensorInstance) = sample_tensor_2way
     # Case 1 single element
@@ -315,19 +361,26 @@
     assert (tensorInstance[0, :].data == tensorInstance.data[0, :]).all()
     assert (tensorInstance[:, 0].data == tensorInstance.data[:, 0]).all()
 
     # Case 2a:
     assert tensorInstance[np.array([0, 0]), "extract"] == params["data"][0, 0]
     assert (
         tensorInstance[np.array([[0, 0], [1, 1]]), "extract"]
-        == params["data"][([0, 1], [0, 1])]
+        == params["data"][([0, 0], [1, 1])]
+    ).all()
+    # Case 2a: Extract doesn't seem to be needed
+    assert tensorInstance[np.array([0, 0])] == params["data"][0, 0]
+    assert (
+        tensorInstance[np.array([[0, 0], [1, 1]])] == params["data"][([0, 0], [1, 1])]
     ).all()
 
     # Case 2b: Linear Indexing
     assert tensorInstance[np.array([0])] == params["data"][0, 0]
+    assert tensorInstance[0] == params["data"][0, 0]
+    assert np.array_equal(tensorInstance[0:1], params["data"][0, 0])
     with pytest.raises(AssertionError) as excinfo:
         tensorInstance[np.array([0]), np.array([0]), np.array([0])]
     assert "Linear indexing requires single input array" in str(excinfo)
 
 
 @pytest.mark.indevelopment
 def test_tensor_logical_and(sample_tensor_2way):
```

### Comparing `pyttb-1.6.1/tests/test_ttensor.py` & `pyttb-1.6.2/tests/test_ttensor.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.6.1/tests/test_tucker_als.py` & `pyttb-1.6.2/tests/test_tucker_als.py`

 * *Files identical despite different names*

