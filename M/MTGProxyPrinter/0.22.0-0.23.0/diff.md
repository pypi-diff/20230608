# Comparing `tmp/MTGProxyPrinter-0.22.0.tar.gz` & `tmp/MTGProxyPrinter-0.23.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MTGProxyPrinter-0.22.0.tar", last modified: Tue Apr 18 18:23:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

