# Comparing `tmp/posemaro-1.1.8-py3-none-any.whl.zip` & `tmp/posemaro-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 248742 bytes, number of entries: 132
+Zip file size: 248744 bytes, number of entries: 132
 -rw-r--r--  2.0 unx       78 b- defN 22-Sep-19 00:57 datumaro/__init__.py
 -rw-r--r--  2.0 unx      179 b- defN 22-Sep-19 00:57 datumaro/__main__.py
--rw-r--r--  2.0 unx       18 b- defN 22-Sep-19 01:03 datumaro/version.py
+-rw-r--r--  2.0 unx       18 b- defN 22-Sep-20 08:36 datumaro/version.py
 -rw-r--r--  2.0 unx       78 b- defN 22-Sep-19 00:57 datumaro/cli/__init__.py
 -rw-r--r--  2.0 unx     4606 b- defN 22-Sep-19 00:57 datumaro/cli/__main__.py
 -rw-r--r--  2.0 unx      259 b- defN 22-Sep-19 00:57 datumaro/cli/commands/__init__.py
 -rw-r--r--  2.0 unx      176 b- defN 22-Sep-19 00:57 datumaro/cli/commands/add.py
 -rw-r--r--  2.0 unx     4322 b- defN 22-Sep-19 00:57 datumaro/cli/commands/convert.py
 -rw-r--r--  2.0 unx      180 b- defN 22-Sep-19 00:57 datumaro/cli/commands/create.py
 -rw-r--r--  2.0 unx      178 b- defN 22-Sep-19 00:57 datumaro/cli/commands/diff.py
@@ -121,14 +121,14 @@
 -rw-r--r--  2.0 unx    13313 b- defN 22-Sep-19 00:57 datumaro/util/image.py
 -rw-r--r--  2.0 unx      965 b- defN 22-Sep-19 00:57 datumaro/util/image_cache.py
 -rw-r--r--  2.0 unx      351 b- defN 22-Sep-19 00:57 datumaro/util/log_utils.py
 -rw-r--r--  2.0 unx     9935 b- defN 22-Sep-19 00:57 datumaro/util/mask_tools.py
 -rw-r--r--  2.0 unx     1975 b- defN 22-Sep-19 00:57 datumaro/util/os_util.py
 -rw-r--r--  2.0 unx     7775 b- defN 22-Sep-19 00:57 datumaro/util/test_utils.py
 -rw-r--r--  2.0 unx     2513 b- defN 22-Sep-19 00:57 datumaro/util/tf_util.py
--rw-r--r--  2.0 unx     1090 b- defN 22-Sep-19 01:04 posemaro-1.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx    11911 b- defN 22-Sep-19 01:04 posemaro-1.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Sep-19 01:04 posemaro-1.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 22-Sep-19 01:04 posemaro-1.1.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 22-Sep-19 01:04 posemaro-1.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    12114 b- defN 22-Sep-19 01:04 posemaro-1.1.8.dist-info/RECORD
-132 files, 891931 bytes uncompressed, 229294 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx     1090 b- defN 22-Sep-20 08:39 posemaro-1.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11926 b- defN 22-Sep-20 08:39 posemaro-1.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Sep-20 08:39 posemaro-1.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 22-Sep-20 08:39 posemaro-1.1.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 22-Sep-20 08:39 posemaro-1.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    12114 b- defN 22-Sep-20 08:39 posemaro-1.1.9.dist-info/RECORD
+132 files, 891947 bytes uncompressed, 229296 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -372,26 +372,26 @@
 
 Filename: datumaro/util/test_utils.py
 Comment: 
 
 Filename: datumaro/util/tf_util.py
 Comment: 
 
-Filename: posemaro-1.1.8.dist-info/LICENSE
+Filename: posemaro-1.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: posemaro-1.1.8.dist-info/METADATA
+Filename: posemaro-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: posemaro-1.1.8.dist-info/WHEEL
+Filename: posemaro-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: posemaro-1.1.8.dist-info/entry_points.txt
+Filename: posemaro-1.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: posemaro-1.1.8.dist-info/top_level.txt
+Filename: posemaro-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: posemaro-1.1.8.dist-info/RECORD
+Filename: posemaro-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datumaro/version.py

```diff
@@ -1 +1 @@
-VERSION = '1.1.8'
+VERSION = '1.1.9'
```

## Comparing `posemaro-1.1.8.dist-info/LICENSE` & `posemaro-1.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `posemaro-1.1.8.dist-info/METADATA` & `posemaro-1.1.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: posemaro
-Version: 1.1.8
+Version: 1.1.9
 Summary: Dataset Management Framework (Posemaro)
 Home-page: https://github.com/certiware/datumaro
 Author: certiware
 Author-email: certiware.study@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: GitPython (>=3.0.8)
+Requires-Dist: Pillow (>=6.1.0)
+Requires-Dist: PyYAML (>=5.3.1)
 Requires-Dist: attrs (>=19.3.0)
 Requires-Dist: defusedxml (>=0.6.0)
-Requires-Dist: GitPython (>=3.0.8)
 Requires-Dist: lxml (>=4.4.1)
 Requires-Dist: matplotlib (>=3.3.1)
 Requires-Dist: numpy (>=1.17.3)
-Requires-Dist: Pillow (>=6.1.0)
-Requires-Dist: PyYAML (>=5.3.1)
+Requires-Dist: opencv-python
 Requires-Dist: scikit-image (>=0.15.0)
 Requires-Dist: tensorboardX (!=2.3,>=1.8)
-Requires-Dist: opencv-python
 Requires-Dist: pycocotools (!=2.0.2,>=2.0.0) ; platform_system != "Windows"
 Requires-Dist: pycocotools-windows ; platform_system == "Windows"
 Provides-Extra: tf
 Requires-Dist: tensorflow ; extra == 'tf'
 Provides-Extra: tf-gpu
 Requires-Dist: tensorflow-gpu ; extra == 'tf-gpu'
 
@@ -304,7 +305,9 @@
 [(Back to top)](#table-of-contents)
 
 Feel free to
 [open an Issue](https://github.com/openvinotoolkit/datumaro/issues/new), if you
 think something needs to be changed. You are welcome to participate in
 development, instructions are available in our
 [contribution guide](CONTRIBUTING.md).
+
+
```

## Comparing `posemaro-1.1.8.dist-info/RECORD` & `posemaro-1.1.9.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 datumaro/__init__.py,sha256=vrsBr3_EjpNCjsrdyx_bu1VD9FIcSJK2j6Ui-SFHdWI,78
 datumaro/__main__.py,sha256=WXL9B9smpNHYMw7xIGcx0aLXpS0Ednl0-FWT9VMDtwY,179
-datumaro/version.py,sha256=hO_RUxTNacyXlic0vuKeq-HjK9z4un-bVCWh5sr9lU0,18
+datumaro/version.py,sha256=kUV2nJGB-9B_CoaYf-p6NoiuZYF0snw2oCdKnW-hdhg,18
 datumaro/cli/__init__.py,sha256=BELD2JsHcy2paVHq5PRdKPEkUu-oQR-PV3Kflewa6H8,78
 datumaro/cli/__main__.py,sha256=wUvXWHQrIc3sALgdPE7ETGhc0_yv7fIJPj0FThu3-1c,4606
 datumaro/cli/commands/__init__.py,sha256=MQX47KiQLE0cfbgjX8hRspcVS8gCvSNQQFYFgS1o0Qs,259
 datumaro/cli/commands/add.py,sha256=OJYVe1A2AxIIVfFDNQR9CBqzYEgR6PxZH59AO7sOxzs,176
 datumaro/cli/commands/convert.py,sha256=0nRA3xHl2nA04RsZ3V5jqpky64JB8-sxpxk_83bpFsY,4322
 datumaro/cli/commands/create.py,sha256=laON9wHI4oYkQDN3KmOOZWtLuebg5t4ynIimNhBYa6E,180
 datumaro/cli/commands/diff.py,sha256=ZIsHPlmGKDSBPVeC02knA83MatwGnnxnTGGchVhuk7I,178
@@ -120,13 +120,13 @@
 datumaro/util/image.py,sha256=7Jiqr5xQWdp7d8KdIbt1x0HyHkM7h28uoorg1vYZ0dA,13313
 datumaro/util/image_cache.py,sha256=LZN8JsW3ccsrQz_nAB4kH7CiR3oQi5aT0XeIR7AZSvU,965
 datumaro/util/log_utils.py,sha256=JobNtG1yar6XPQuDZYhNeJLtaypDhLPNL2WlI9pi4E8,351
 datumaro/util/mask_tools.py,sha256=9HDrjN1xE_r3xr41aGH-pWoLf806LkF0etRxRbJe2qc,9935
 datumaro/util/os_util.py,sha256=k2DlniJsKM4CHwFtD-KGt5hhM4iXl8cAzAhayfCw_7Y,1975
 datumaro/util/test_utils.py,sha256=0Tpe4xr48SOd3fOh-Fsl-9NsWf4zVwUtAqBhXFMoXvw,7775
 datumaro/util/tf_util.py,sha256=BGUwbLY30_zaJwZ5-_FXlnzGtW5Vu_YY5gEd49JQicM,2513
-posemaro-1.1.8.dist-info/LICENSE,sha256=D3c1Ypv9ODBtNTQm6D6xN8TIOVbRHwoizPN4h8ZlfL0,1090
-posemaro-1.1.8.dist-info/METADATA,sha256=ynFUJk_SVyMXTyr7gkRU6Xyg5wW2bCz6uPBRZejACzM,11911
-posemaro-1.1.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-posemaro-1.1.8.dist-info/entry_points.txt,sha256=QtPjorWaKr8L84ZChndeyAnKLfD131fi_mgOqwmUG4c,53
-posemaro-1.1.8.dist-info/top_level.txt,sha256=ynFxR41Xut_ByouULFZYFfekgf5p0eeACHj-ddCTLRA,9
-posemaro-1.1.8.dist-info/RECORD,,
+posemaro-1.1.9.dist-info/LICENSE,sha256=D3c1Ypv9ODBtNTQm6D6xN8TIOVbRHwoizPN4h8ZlfL0,1090
+posemaro-1.1.9.dist-info/METADATA,sha256=gIVbaJof34BbzeqD7waa8SwliZ6JeDwqgVVHsCUYubY,11926
+posemaro-1.1.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+posemaro-1.1.9.dist-info/entry_points.txt,sha256=2bI7-_hB7V6TD9PnQ7ODsNepUJPSBy7_eIQoX3mpNAE,54
+posemaro-1.1.9.dist-info/top_level.txt,sha256=ynFxR41Xut_ByouULFZYFfekgf5p0eeACHj-ddCTLRA,9
+posemaro-1.1.9.dist-info/RECORD,,
```

