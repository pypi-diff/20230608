# Comparing `tmp/predictapi-0.0.4.tar.gz` & `tmp/predictapi-0.0.5.win-amd64.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predictapi-0.0.4.tar", last modified: Thu Jun  8 10:00:50 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

