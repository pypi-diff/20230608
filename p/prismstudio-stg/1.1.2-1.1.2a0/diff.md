# Comparing `tmp/prismstudio-stg-1.1.2.tar.gz` & `tmp/prismstudio_stg-1.1.2a0-py310-none-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prismstudio-stg-1.1.2.tar", last modified: Wed Jun  7 02:29:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

