# Comparing `tmp/pyakamai-1.1-py3-none-any.whl.zip` & `tmp/pyakamai-1.11-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 24775 bytes, number of entries: 19
+Zip file size: 25766 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      454 b- defN 23-May-01 03:11 pyakamai/__init__.py
 -rw-r--r--  2.0 unx     3821 b- defN 23-May-01 03:18 pyakamai/akamaicasemanagement.py
 -rw-r--r--  2.0 unx     1473 b- defN 23-May-01 03:29 pyakamai/akamaicpcode.py
 -rw-r--r--  2.0 unx     2332 b- defN 23-Apr-30 11:30 pyakamai/akamaicps.py
 -rw-r--r--  2.0 unx     9439 b- defN 23-Jun-08 00:37 pyakamai/akamaidatastream.py
 -rw-r--r--  2.0 unx     4408 b- defN 23-Apr-30 10:57 pyakamai/akamaiedns.py
 -rw-r--r--  2.0 unx     2843 b- defN 23-Apr-30 15:28 pyakamai/akamaiehn.py
@@ -10,12 +10,12 @@
 -rw-r--r--  2.0 unx     5689 b- defN 23-May-01 03:31 pyakamai/akamaiksd2.py
 -rw-r--r--  2.0 unx     2443 b- defN 23-Apr-30 11:42 pyakamai/akamailds.py
 -rw-r--r--  2.0 unx     3878 b- defN 23-Jun-08 00:38 pyakamai/akamaimsl.py
 -rw-r--r--  2.0 unx    28281 b- defN 23-Jun-08 00:35 pyakamai/akamaiproperty.py
 -rw-r--r--  2.0 unx     3506 b- defN 23-Apr-30 15:04 pyakamai/akamaipurge.py
 -rw-r--r--  2.0 unx     8058 b- defN 23-May-12 02:25 pyakamai/http_calls.py
 -rw-r--r--  2.0 unx     2624 b- defN 23-Jun-08 00:08 pyakamai/pyakamai.py
--rw-r--r--  2.0 unx      492 b- defN 23-Jun-08 00:38 pyakamai-1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 00:38 pyakamai-1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-08 00:38 pyakamai-1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1493 b- defN 23-Jun-08 00:38 pyakamai-1.1.dist-info/RECORD
-19 files, 95528 bytes uncompressed, 22371 bytes compressed:  76.6%
+-rw-r--r--  2.0 unx     2916 b- defN 23-Jun-08 01:03 pyakamai-1.11.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 01:03 pyakamai-1.11.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-08 01:03 pyakamai-1.11.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1498 b- defN 23-Jun-08 01:03 pyakamai-1.11.dist-info/RECORD
+19 files, 97957 bytes uncompressed, 23354 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: pyakamai/http_calls.py
 Comment: 
 
 Filename: pyakamai/pyakamai.py
 Comment: 
 
-Filename: pyakamai-1.1.dist-info/METADATA
+Filename: pyakamai-1.11.dist-info/METADATA
 Comment: 
 
-Filename: pyakamai-1.1.dist-info/WHEEL
+Filename: pyakamai-1.11.dist-info/WHEEL
 Comment: 
 
-Filename: pyakamai-1.1.dist-info/top_level.txt
+Filename: pyakamai-1.11.dist-info/top_level.txt
 Comment: 
 
-Filename: pyakamai-1.1.dist-info/RECORD
+Filename: pyakamai-1.11.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyakamai-1.1.dist-info/RECORD` & `pyakamai-1.11.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 pyakamai/akamaiksd2.py,sha256=CWo_ejWDPoyiTWROrbc_OTmcq7RXZBb8n8xOYVXQ3w8,5689
 pyakamai/akamailds.py,sha256=Rt4Lp4Hmu6T5sx0jCp3iB7YMowKSdIrk6E2NP_JWYXA,2443
 pyakamai/akamaimsl.py,sha256=ykRv_yy-qVWs37Wu2auDddX4IEuSWiO-1g9p59LTYww,3878
 pyakamai/akamaiproperty.py,sha256=mUgCU9GJ-o3A1um8T55_ihS37K9DrIgqLI-RxD-PANo,28281
 pyakamai/akamaipurge.py,sha256=FLwfjbhjn0PZyRRq68SpKFF9f8JPk76DKvCmmVg2NtU,3506
 pyakamai/http_calls.py,sha256=vH5oWXTuMtSq64crAycijH5EFQC-9QAQf--Da-qlS-I,8058
 pyakamai/pyakamai.py,sha256=xqX5Ms9Rcl4qTxkvpI5tm_AUI0qgIEyf0Jda6b-gP9c,2624
-pyakamai-1.1.dist-info/METADATA,sha256=it82c6r3vdR2hfuJtwR0LbjxC3FsqNjLyHJPVtK2_Wk,492
-pyakamai-1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyakamai-1.1.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
-pyakamai-1.1.dist-info/RECORD,,
+pyakamai-1.11.dist-info/METADATA,sha256=hRiwtZqSERN85owjJT0HGhj9mEQrJGtX-pn6TbKiWTM,2916
+pyakamai-1.11.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pyakamai-1.11.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
+pyakamai-1.11.dist-info/RECORD,,
```

