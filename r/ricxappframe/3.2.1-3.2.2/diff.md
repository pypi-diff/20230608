# Comparing `tmp/ricxappframe-3.2.1.tar.gz` & `tmp/ricxappframe-3.2.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ricxappframe-3.2.1.tar", last modified: Mon Dec 12 12:04:35 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

