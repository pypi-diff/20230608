# Comparing `tmp/man_etl-0.0.4.tar.gz` & `tmp/man_etl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "man_etl-0.0.4.tar", last modified: Wed Jun  7 22:35:56 2023, max compression
+gzip compressed data, was "man_etl-0.0.5.tar", last modified: Thu Jun  8 16:03:30 2023, max compression
```

## Comparing `man_etl-0.0.4.tar` & `man_etl-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,33 @@
-drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:35:56.672844 man_etl-0.0.4/
--rw-r--r--   0 johnphillips   (501) staff       (20)       51 2023-06-07 22:35:56.672596 man_etl-0.0.4/PKG-INFO
--rw-r--r--   0 johnphillips   (501) staff       (20)       22 2023-06-05 19:31:25.000000 man_etl-0.0.4/README.md
-drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:35:56.666998 man_etl-0.0.4/WM9L8_IMA/
--rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 17:47:11.000000 man_etl-0.0.4/WM9L8_IMA/__init__.py
-drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:35:56.668567 man_etl-0.0.4/WM9L8_IMA/etl_pipelines/
--rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 21:52:42.000000 man_etl-0.0.4/WM9L8_IMA/etl_pipelines/__init__.py
--rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 17:47:11.000000 man_etl-0.0.4/WM9L8_IMA/etl_pipelines/arctic_transform.py
--rw-r--r--   0 johnphillips   (501) staff       (20)     1499 2023-06-07 22:09:59.000000 man_etl-0.0.4/WM9L8_IMA/etl_pipelines/csv_to_arctic.py
--rw-r--r--   0 johnphillips   (501) staff       (20)      146 2023-06-07 17:47:11.000000 man_etl-0.0.4/WM9L8_IMA/generate_db.py
-drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:35:56.670339 man_etl-0.0.4/WM9L8_IMA/python/
--rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 17:47:11.000000 man_etl-0.0.4/WM9L8_IMA/python/__init__.py
--rw-r--r--   0 johnphillips   (501) staff       (20)      611 2023-06-07 17:47:11.000000 man_etl-0.0.4/WM9L8_IMA/python/app.py
--rw-r--r--   0 johnphillips   (501) staff       (20)       59 2023-06-07 17:47:11.000000 man_etl-0.0.4/WM9L8_IMA/python/main.py
--rw-r--r--   0 johnphillips   (501) staff       (20)       77 2023-06-07 17:47:11.000000 man_etl-0.0.4/WM9L8_IMA/python/utils.py
-drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:35:56.672156 man_etl-0.0.4/man_etl.egg-info/
--rw-r--r--   0 johnphillips   (501) staff       (20)       51 2023-06-07 22:35:56.000000 man_etl-0.0.4/man_etl.egg-info/PKG-INFO
--rw-r--r--   0 johnphillips   (501) staff       (20)      478 2023-06-07 22:35:56.000000 man_etl-0.0.4/man_etl.egg-info/SOURCES.txt
--rw-r--r--   0 johnphillips   (501) staff       (20)        1 2023-06-07 22:35:56.000000 man_etl-0.0.4/man_etl.egg-info/dependency_links.txt
--rw-r--r--   0 johnphillips   (501) staff       (20)       86 2023-06-07 22:35:56.000000 man_etl-0.0.4/man_etl.egg-info/entry_points.txt
--rw-r--r--   0 johnphillips   (501) staff       (20)       29 2023-06-07 22:35:56.000000 man_etl-0.0.4/man_etl.egg-info/requires.txt
--rw-r--r--   0 johnphillips   (501) staff       (20)       10 2023-06-07 22:35:56.000000 man_etl-0.0.4/man_etl.egg-info/top_level.txt
--rw-r--r--   0 johnphillips   (501) staff       (20)       38 2023-06-07 22:35:56.673209 man_etl-0.0.4/setup.cfg
--rw-r--r--   0 johnphillips   (501) staff       (20)      379 2023-06-07 22:35:47.000000 man_etl-0.0.4/setup.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:20:16.170463 man_etl-0.0.5/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       51 2023-06-08 16:20:16.170463 man_etl-0.0.5/PKG-INFO
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      374 2023-06-08 08:17:19.000000 man_etl-0.0.5/README.md
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:20:14.248754 man_etl-0.0.5/man_etl/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-07 17:32:55.000000 man_etl-0.0.5/man_etl/__init__.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:20:14.997733 man_etl-0.0.5/man_etl/etl_pipelines/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 08:17:19.000000 man_etl-0.0.5/man_etl/etl_pipelines/__init__.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1168 2023-06-08 13:36:53.000000 man_etl-0.0.5/man_etl/etl_pipelines/arctic_transform.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:20:15.647123 man_etl-0.0.5/man_etl/etl_pipelines/core/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 08:40:26.000000 man_etl-0.0.5/man_etl/etl_pipelines/core/__init__.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1363 2023-06-08 10:16:49.000000 man_etl-0.0.5/man_etl/etl_pipelines/core/arctic.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      788 2023-06-08 10:01:21.000000 man_etl-0.0.5/man_etl/etl_pipelines/core/base.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     2159 2023-06-08 13:36:53.000000 man_etl-0.0.5/man_etl/etl_pipelines/core/extractors.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      468 2023-06-08 13:36:53.000000 man_etl-0.0.5/man_etl/etl_pipelines/core/storers.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1171 2023-06-08 13:36:53.000000 man_etl-0.0.5/man_etl/etl_pipelines/core/transformers.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1020 2023-06-08 13:36:53.000000 man_etl-0.0.5/man_etl/etl_pipelines/csv_to_arctic.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      651 2023-06-08 13:36:53.000000 man_etl-0.0.5/man_etl/etl_pipelines/ons_to_arctic.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      147 2023-06-08 08:17:19.000000 man_etl-0.0.5/man_etl/generate_db.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:20:16.097316 man_etl-0.0.5/man_etl/python/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-07 17:32:56.000000 man_etl-0.0.5/man_etl/python/__init__.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      612 2023-06-08 08:17:19.000000 man_etl-0.0.5/man_etl/python/app.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       59 2023-06-07 17:32:57.000000 man_etl-0.0.5/man_etl/python/main.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       94 2023-06-08 09:31:02.000000 man_etl-0.0.5/man_etl/python/pyarrow_client.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       79 2023-06-08 08:17:19.000000 man_etl-0.0.5/man_etl/python/utils.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:20:14.663031 man_etl-0.0.5/man_etl.egg-info/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       51 2023-06-08 16:20:08.000000 man_etl-0.0.5/man_etl.egg-info/PKG-INFO
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      765 2023-06-08 16:20:11.000000 man_etl-0.0.5/man_etl.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        1 2023-06-08 16:20:08.000000 man_etl-0.0.5/man_etl.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       84 2023-06-08 16:20:09.000000 man_etl-0.0.5/man_etl.egg-info/entry_points.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       22 2023-06-08 16:20:09.000000 man_etl-0.0.5/man_etl.egg-info/requires.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        8 2023-06-08 16:20:09.000000 man_etl-0.0.5/man_etl.egg-info/top_level.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       38 2023-06-08 16:20:16.186375 man_etl-0.0.5/setup.cfg
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      369 2023-06-08 16:19:56.000000 man_etl-0.0.5/setup.py
```

### Comparing `man_etl-0.0.4/WM9L8_IMA/python/app.py` & `man_etl-0.0.5/man_etl/python/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 TICKERS = ["AAPL", "GOOG", "TSLA"]
 for i, ticker in enumerate(TICKERS):
     TICKERS[i] = ticker_to_yf(ticker)
 
 for ticker in TICKERS:
     data = ticker.history(period=PERIOD, interval=INTERVAL)
     st.write(f"Volume data for {ticker.info['longName']} for {PERIOD}")
-    st.line_chart(data['Volume'])
+    st.line_chart(data["Volume"])
 
 
 @click.command()
 @click.option("--arg", default="no args", help="Test argument")
 def etl(arg):
-    print(f"The pipeline was run with {arg}")
+    print(f"The pipeline was run with {arg}")
```

