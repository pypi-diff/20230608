# Comparing `tmp/bact-archiver-0.0.0.tar.gz` & `tmp/bact_archiver-0.1.0-cp310-cp310-manylinux_2_31_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bact-archiver-0.0.0.tar", last modified: Fri Nov 27 15:34:42 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

