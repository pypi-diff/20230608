# Comparing `tmp/pororo_ocr-0.4.5-py3-none-any.whl.zip` & `tmp/pororo_ocr-0.4.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 61713 bytes, number of entries: 36
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-08 09:24 prrocr/__init__.py
--rw-r--r--  2.0 unx       18 b- defN 23-Jun-08 09:25 prrocr/__version__.py
+Zip file size: 61709 bytes, number of entries: 36
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-08 09:48 prrocr/__init__.py
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-08 09:52 prrocr/__version__.py
 -rw-r--r--  2.0 unx     2900 b- defN 23-Jun-08 09:24 prrocr/pororo.py
 -rw-r--r--  2.0 unx     6496 b- defN 23-Jun-08 09:24 prrocr/prrocr.py
 -rw-r--r--  2.0 unx     2222 b- defN 23-May-31 02:46 prrocr/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-31 02:46 prrocr/models/__init__.py
 -rw-r--r--  2.0 unx       37 b- defN 23-May-31 02:46 prrocr/models/brainOCR/__init__.py
 -rw-r--r--  2.0 unx     1022 b- defN 23-May-31 02:46 prrocr/models/brainOCR/_dataset.py
 -rw-r--r--  2.0 unx    20996 b- defN 23-May-31 02:46 prrocr/models/brainOCR/_modules.py
@@ -24,15 +24,15 @@
 -rw-r--r--  2.0 unx     8768 b- defN 23-May-31 02:46 prrocr/models/brainOCR/modules/transformation.py
 -rw-r--r--  2.0 unx      388 b- defN 23-Jun-08 09:24 prrocr/tasks/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-31 02:46 prrocr/tasks/utils/__init__.py
 -rw-r--r--  2.0 unx     5011 b- defN 23-May-31 02:46 prrocr/tasks/utils/base.py
 -rw-r--r--  2.0 unx     3386 b- defN 23-May-31 02:46 prrocr/tasks/utils/config.py
 -rw-r--r--  2.0 unx     8101 b- defN 23-Jun-08 09:24 prrocr/tasks/utils/download_utils.py
 -rw-r--r--  2.0 unx     2804 b- defN 23-May-31 02:46 prrocr/tasks/utils/tokenizer.py
--rw-r--r--  2.0 unx    11360 b- defN 23-Jun-08 09:25 pororo_ocr-0.4.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    26965 b- defN 23-Jun-08 09:25 pororo_ocr-0.4.5.dist-info/LICENSE.3rd_party_library
--rw-r--r--  2.0 unx      966 b- defN 23-Jun-08 09:25 pororo_ocr-0.4.5.dist-info/LICENSE.3rd_party_model
--rw-r--r--  2.0 unx     8749 b- defN 23-Jun-08 09:25 pororo_ocr-0.4.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 09:25 pororo_ocr-0.4.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-08 09:25 pororo_ocr-0.4.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3193 b- defN 23-Jun-08 09:25 pororo_ocr-0.4.5.dist-info/RECORD
-36 files, 197461 bytes uncompressed, 56533 bytes compressed:  71.4%
+-rw-r--r--  2.0 unx    11360 b- defN 23-Jun-08 09:52 pororo_ocr-0.4.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    26965 b- defN 23-Jun-08 09:52 pororo_ocr-0.4.6.dist-info/LICENSE.3rd_party_library
+-rw-r--r--  2.0 unx      966 b- defN 23-Jun-08 09:52 pororo_ocr-0.4.6.dist-info/LICENSE.3rd_party_model
+-rw-r--r--  2.0 unx     8749 b- defN 23-Jun-08 09:52 pororo_ocr-0.4.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 09:52 pororo_ocr-0.4.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-08 09:52 pororo_ocr-0.4.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3193 b- defN 23-Jun-08 09:52 pororo_ocr-0.4.6.dist-info/RECORD
+36 files, 197450 bytes uncompressed, 56529 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -81,29 +81,29 @@
 
 Filename: prrocr/tasks/utils/download_utils.py
 Comment: 
 
 Filename: prrocr/tasks/utils/tokenizer.py
 Comment: 
 
-Filename: pororo_ocr-0.4.5.dist-info/LICENSE
+Filename: pororo_ocr-0.4.6.dist-info/LICENSE
 Comment: 
 
-Filename: pororo_ocr-0.4.5.dist-info/LICENSE.3rd_party_library
+Filename: pororo_ocr-0.4.6.dist-info/LICENSE.3rd_party_library
 Comment: 
 
-Filename: pororo_ocr-0.4.5.dist-info/LICENSE.3rd_party_model
+Filename: pororo_ocr-0.4.6.dist-info/LICENSE.3rd_party_model
 Comment: 
 
-Filename: pororo_ocr-0.4.5.dist-info/METADATA
+Filename: pororo_ocr-0.4.6.dist-info/METADATA
 Comment: 
 
-Filename: pororo_ocr-0.4.5.dist-info/WHEEL
+Filename: pororo_ocr-0.4.6.dist-info/WHEEL
 Comment: 
 
-Filename: pororo_ocr-0.4.5.dist-info/top_level.txt
+Filename: pororo_ocr-0.4.6.dist-info/top_level.txt
 Comment: 
 
-Filename: pororo_ocr-0.4.5.dist-info/RECORD
+Filename: pororo_ocr-0.4.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## prrocr/__init__.py

```diff
@@ -1,2 +1,2 @@
 from prrocr.__version__ import version as __version__  # noqa
-from prrocr.prrocr import PororoOCR as prrocr  # noqa
+from prrocr.prrocr import PororoOCR # noqa
```

## prrocr/__version__.py

```diff
@@ -1 +1 @@
-version = "0.4.5"
+version = "0.4.6"
```

## Comparing `pororo_ocr-0.4.5.dist-info/LICENSE` & `pororo_ocr-0.4.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pororo_ocr-0.4.5.dist-info/LICENSE.3rd_party_library` & `pororo_ocr-0.4.6.dist-info/LICENSE.3rd_party_library`

 * *Files identical despite different names*

## Comparing `pororo_ocr-0.4.5.dist-info/LICENSE.3rd_party_model` & `pororo_ocr-0.4.6.dist-info/LICENSE.3rd_party_model`

 * *Files identical despite different names*

## Comparing `pororo_ocr-0.4.5.dist-info/METADATA` & `pororo_ocr-0.4.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pororo-ocr
-Version: 0.4.5
+Version: 0.4.6
 Summary: Rebuilding only the OCR part of the pororo package for lightweight and fast operation.
 Home-page: https://github.com/stellarway/pororo-ocr
 Author: Wonhee Go
 Author-email: whgo.nlp@gmail.com
 License: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pororo-ocr Version: 0.4.5 Summary: Rebuilding only
+Metadata-Version: 2.1 Name: pororo-ocr Version: 0.4.6 Summary: Rebuilding only
 the OCR part of the pororo package for lightweight and fast operation. Home-
 page: https://github.com/stellarway/pororo-ocr Author: Wonhee Go Author-email:
 whgo.nlp@gmail.com License: Apache-2.0 Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Development Status :: 3 - Alpha Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
```

## Comparing `pororo_ocr-0.4.5.dist-info/RECORD` & `pororo_ocr-0.4.6.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-prrocr/__init__.py,sha256=3VmgTLun6lObVBEWfRnWToy_0XC4ZlEV3kO4va-zZZM,116
-prrocr/__version__.py,sha256=GzDw9yI90LiIOYlw5gZBih8gPe3URgiM0vAFi2-I3ro,18
+prrocr/__init__.py,sha256=acfP4UbzfDzYmAT4YAehrOv8QlQPuzP3jn8r7e8pZis,105
+prrocr/__version__.py,sha256=DWNNbWBv-hyqVy76bKbnHWaDUbqL0BOtdkPSV_88dx0,18
 prrocr/pororo.py,sha256=sKBnwVS_D4UaphAHZPtcfCtzGyjgCCyUMzhFgO4FUno,2900
 prrocr/prrocr.py,sha256=UkAsyPODb_niXPi_uuPdamYBB_hp7rUS9awmjajx9mI,6496
 prrocr/utils.py,sha256=jsF8Un5cUDUoN1rt4vxnSi8hUPlriW2OAfo9pRrkFGs,2222
 prrocr/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 prrocr/models/brainOCR/__init__.py,sha256=NJjH7zI5cSQU-u4yAIi-J3gC2DIpo-Yvn6EtDD_Zyfo,37
 prrocr/models/brainOCR/_dataset.py,sha256=2_GyQpc1rgbsPI3H06_QHW4x6NgZElVRaNmwKISMaa0,1022
 prrocr/models/brainOCR/_modules.py,sha256=i2ls_LZmS9BVxttpIBKtJuavddfa1AiVqv91Hf2F_1w,20996
@@ -23,14 +23,14 @@
 prrocr/models/brainOCR/modules/transformation.py,sha256=XT3JJH4Xedmkd6jx2daWn00ofNxSTKqk5CDa7xV5Z-s,8768
 prrocr/tasks/__init__.py,sha256=36HpriUdBsUSqv2U7m9AekbGLmnIupqbKEuTdUilB8I,388
 prrocr/tasks/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 prrocr/tasks/utils/base.py,sha256=Kb3tF01RBGfpIbebzyc2LAoesBNW6o2Tr0Wc3U0LA38,5011
 prrocr/tasks/utils/config.py,sha256=VL4jz_Oz6XWsNXZ10OcrM-niBvcnI1CyWKQWCQynlI4,3386
 prrocr/tasks/utils/download_utils.py,sha256=vSFUpIwgvf5_-urStMwIkMzzA3btaDaIKE_dIkoMUpA,8101
 prrocr/tasks/utils/tokenizer.py,sha256=XR-_VH3A2YEJ_IoXoWLSE8C5Cebl8u3yfHwQOWLq4U8,2804
-pororo_ocr-0.4.5.dist-info/LICENSE,sha256=MUQMax-oXcGRIfQm7KUyMvagMVACVmtSCThi_KM5uJM,11360
-pororo_ocr-0.4.5.dist-info/LICENSE.3rd_party_library,sha256=vzTLs7Ez8WDngBP5YaPgj-43EUU_3oZ0-QnscuiUj-A,26965
-pororo_ocr-0.4.5.dist-info/LICENSE.3rd_party_model,sha256=xs2P3XJWWcOV3uShs6-b1otvxxqX4d17yIQQEuEa5_4,966
-pororo_ocr-0.4.5.dist-info/METADATA,sha256=qejU-D2Q8s_UrELZrySznaj5VojqZiTiUDRvfaLj6JI,8749
-pororo_ocr-0.4.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pororo_ocr-0.4.5.dist-info/top_level.txt,sha256=fzB2InJjGHzJwA9-GTgkNWslDAsnZv9DLYj2YvotPbA,7
-pororo_ocr-0.4.5.dist-info/RECORD,,
+pororo_ocr-0.4.6.dist-info/LICENSE,sha256=MUQMax-oXcGRIfQm7KUyMvagMVACVmtSCThi_KM5uJM,11360
+pororo_ocr-0.4.6.dist-info/LICENSE.3rd_party_library,sha256=vzTLs7Ez8WDngBP5YaPgj-43EUU_3oZ0-QnscuiUj-A,26965
+pororo_ocr-0.4.6.dist-info/LICENSE.3rd_party_model,sha256=xs2P3XJWWcOV3uShs6-b1otvxxqX4d17yIQQEuEa5_4,966
+pororo_ocr-0.4.6.dist-info/METADATA,sha256=aBcHBl16kdVpiPZO0S-uvq2s5dieFBpVzt8q03zP2B8,8749
+pororo_ocr-0.4.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pororo_ocr-0.4.6.dist-info/top_level.txt,sha256=fzB2InJjGHzJwA9-GTgkNWslDAsnZv9DLYj2YvotPbA,7
+pororo_ocr-0.4.6.dist-info/RECORD,,
```

