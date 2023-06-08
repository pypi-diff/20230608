# Comparing `tmp/pdfly-0.1.1.tar.gz` & `tmp/pdfly-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfly-0.1.1.tar", last modified: Tue Mar 28 11:51:25 2023, max compression
+gzip compressed data, was "pdfly-0.1.2.tar", last modified: Thu Jun  8 14:12:38 2023, max compression
```

## Comparing `pdfly-0.1.1.tar` & `pdfly-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 moose     (1000) moose     (1000)        0 2023-03-28 11:51:25.370317 pdfly-0.1.1/
--rw-rw-r--   0 moose     (1000) moose     (1000)     1514 2023-03-18 14:12:20.000000 pdfly-0.1.1/LICENSE
--rw-rw-r--   0 moose     (1000) moose     (1000)     4938 2023-03-28 11:51:25.370317 pdfly-0.1.1/PKG-INFO
--rw-rw-r--   0 moose     (1000) moose     (1000)     3938 2023-03-19 13:01:13.000000 pdfly-0.1.1/README.md
-drwxrwxr-x   0 moose     (1000) moose     (1000)        0 2023-03-28 11:51:25.370317 pdfly-0.1.1/pdfly/
--rw-rw-r--   0 moose     (1000) moose     (1000)      164 2023-03-19 13:01:13.000000 pdfly-0.1.1/pdfly/__init__.py
--rw-rw-r--   0 moose     (1000) moose     (1000)      114 2023-03-18 14:12:20.000000 pdfly-0.1.1/pdfly/__main__.py
--rw-rw-r--   0 moose     (1000) moose     (1000)       87 2023-03-19 13:01:13.000000 pdfly-0.1.1/pdfly/_utils.py
--rw-rw-r--   0 moose     (1000) moose     (1000)       22 2023-03-28 11:51:21.000000 pdfly-0.1.1/pdfly/_version.py
--rw-rw-r--   0 moose     (1000) moose     (1000)     2765 2023-03-19 13:01:13.000000 pdfly-0.1.1/pdfly/cat.py
--rw-rw-r--   0 moose     (1000) moose     (1000)     2891 2023-03-19 13:01:13.000000 pdfly-0.1.1/pdfly/cli.py
--rw-rw-r--   0 moose     (1000) moose     (1000)      594 2023-03-19 13:01:13.000000 pdfly-0.1.1/pdfly/compress.py
--rw-rw-r--   0 moose     (1000) moose     (1000)     2161 2023-03-18 15:24:48.000000 pdfly-0.1.1/pdfly/extract_images.py
--rw-rw-r--   0 moose     (1000) moose     (1000)     5591 2023-03-28 11:50:59.000000 pdfly-0.1.1/pdfly/metadata.py
--rw-rw-r--   0 moose     (1000) moose     (1000)     2384 2023-03-19 13:01:13.000000 pdfly-0.1.1/pdfly/pagemeta.py
--rw-rw-r--   0 moose     (1000) moose     (1000)      724 2023-03-19 13:01:13.000000 pdfly-0.1.1/pdfly/up2.py
-drwxrwxr-x   0 moose     (1000) moose     (1000)        0 2023-03-28 11:51:25.370317 pdfly-0.1.1/pdfly.egg-info/
--rw-rw-r--   0 moose     (1000) moose     (1000)     4938 2023-03-28 11:51:25.000000 pdfly-0.1.1/pdfly.egg-info/PKG-INFO
--rw-rw-r--   0 moose     (1000) moose     (1000)      414 2023-03-28 11:51:25.000000 pdfly-0.1.1/pdfly.egg-info/SOURCES.txt
--rw-rw-r--   0 moose     (1000) moose     (1000)        1 2023-03-28 11:51:25.000000 pdfly-0.1.1/pdfly.egg-info/dependency_links.txt
--rw-rw-r--   0 moose     (1000) moose     (1000)       49 2023-03-28 11:51:25.000000 pdfly-0.1.1/pdfly.egg-info/entry_points.txt
--rw-rw-r--   0 moose     (1000) moose     (1000)       39 2023-03-28 11:51:25.000000 pdfly-0.1.1/pdfly.egg-info/requires.txt
--rw-rw-r--   0 moose     (1000) moose     (1000)        6 2023-03-28 11:51:25.000000 pdfly-0.1.1/pdfly.egg-info/top_level.txt
--rw-rw-r--   0 moose     (1000) moose     (1000)     3627 2023-03-19 13:01:13.000000 pdfly-0.1.1/pyproject.toml
--rw-rw-r--   0 moose     (1000) moose     (1000)     1783 2023-03-28 11:51:25.370317 pdfly-0.1.1/setup.cfg
--rw-rw-r--   0 moose     (1000) moose     (1000)      463 2023-03-19 13:01:13.000000 pdfly-0.1.1/setup.py
+drwxrwxr-x   0 moose     (1000) moose     (1000)        0 2023-06-08 14:12:38.962738 pdfly-0.1.2/
+-rw-rw-r--   0 moose     (1000) moose     (1000)     1514 2023-03-18 14:12:20.000000 pdfly-0.1.2/LICENSE
+-rw-rw-r--   0 moose     (1000) moose     (1000)     4938 2023-06-08 14:12:38.962738 pdfly-0.1.2/PKG-INFO
+-rw-rw-r--   0 moose     (1000) moose     (1000)     3938 2023-03-19 13:01:13.000000 pdfly-0.1.2/README.md
+drwxrwxr-x   0 moose     (1000) moose     (1000)        0 2023-06-08 14:12:38.962738 pdfly-0.1.2/pdfly/
+-rw-rw-r--   0 moose     (1000) moose     (1000)      164 2023-03-19 13:01:13.000000 pdfly-0.1.2/pdfly/__init__.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)      114 2023-03-18 14:12:20.000000 pdfly-0.1.2/pdfly/__main__.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)       87 2023-03-19 13:01:13.000000 pdfly-0.1.2/pdfly/_utils.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)       22 2023-06-08 14:12:35.000000 pdfly-0.1.2/pdfly/_version.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)     2765 2023-03-19 13:01:13.000000 pdfly-0.1.2/pdfly/cat.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)     2891 2023-03-19 13:01:13.000000 pdfly-0.1.2/pdfly/cli.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)      594 2023-03-19 13:01:13.000000 pdfly-0.1.2/pdfly/compress.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)      846 2023-06-08 14:12:26.000000 pdfly-0.1.2/pdfly/extract_images.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)     6269 2023-06-08 14:12:26.000000 pdfly-0.1.2/pdfly/metadata.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)     2384 2023-03-19 13:01:13.000000 pdfly-0.1.2/pdfly/pagemeta.py
+-rw-rw-r--   0 moose     (1000) moose     (1000)      724 2023-03-19 13:01:13.000000 pdfly-0.1.2/pdfly/up2.py
+drwxrwxr-x   0 moose     (1000) moose     (1000)        0 2023-06-08 14:12:38.962738 pdfly-0.1.2/pdfly.egg-info/
+-rw-rw-r--   0 moose     (1000) moose     (1000)     4938 2023-06-08 14:12:38.000000 pdfly-0.1.2/pdfly.egg-info/PKG-INFO
+-rw-rw-r--   0 moose     (1000) moose     (1000)      414 2023-06-08 14:12:38.000000 pdfly-0.1.2/pdfly.egg-info/SOURCES.txt
+-rw-rw-r--   0 moose     (1000) moose     (1000)        1 2023-06-08 14:12:38.000000 pdfly-0.1.2/pdfly.egg-info/dependency_links.txt
+-rw-rw-r--   0 moose     (1000) moose     (1000)       49 2023-06-08 14:12:38.000000 pdfly-0.1.2/pdfly.egg-info/entry_points.txt
+-rw-rw-r--   0 moose     (1000) moose     (1000)       40 2023-06-08 14:12:38.000000 pdfly-0.1.2/pdfly.egg-info/requires.txt
+-rw-rw-r--   0 moose     (1000) moose     (1000)        6 2023-06-08 14:12:38.000000 pdfly-0.1.2/pdfly.egg-info/top_level.txt
+-rw-rw-r--   0 moose     (1000) moose     (1000)     3627 2023-03-19 13:01:13.000000 pdfly-0.1.2/pyproject.toml
+-rw-rw-r--   0 moose     (1000) moose     (1000)     1784 2023-06-08 14:12:38.962738 pdfly-0.1.2/setup.cfg
+-rw-rw-r--   0 moose     (1000) moose     (1000)      463 2023-03-19 13:01:13.000000 pdfly-0.1.2/setup.py
```

### Comparing `pdfly-0.1.1/LICENSE` & `pdfly-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.1/PKG-INFO` & `pdfly-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfly
-Version: 0.1.1
+Version: 0.1.2
 Summary: A pure-python CLI application to manipulate PDF files
 Home-page: https://github.com/py-pdf/pdfly
 Author: Martin Thoma
 Author-email: info@martin-thoma.de
 Maintainer: Martin Thoma
 Maintainer-email: info@martin-thoma.de
 License: BSD-3-Clause
```

### Comparing `pdfly-0.1.1/README.md` & `pdfly-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.1/pdfly/cat.py` & `pdfly-0.1.2/pdfly/cat.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.1/pdfly/cli.py` & `pdfly-0.1.2/pdfly/cli.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.1/pdfly/compress.py` & `pdfly-0.1.2/pdfly/compress.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.1/pdfly/metadata.py` & `pdfly-0.1.2/pdfly/metadata.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Show metadata of a PDF file"""
 
 import stat
 from datetime import datetime
 from pathlib import Path
-from typing import Optional, Set
+from typing import List, Optional, Set
 
 from pydantic import BaseModel
 from pypdf import PdfReader
 
 from ._utils import OutputOptions
 
 
@@ -22,14 +22,17 @@
     title: Optional[str] = None
     producer: Optional[str] = None
     author: Optional[str] = None
     pages: Optional[int] = None
     page_mode: Optional[str] = None
     page_layout: Optional[str] = None
     attachments: str = "unknown"
+    id1: Optional[bytes] = None
+    id2: Optional[bytes] = None
+    images: List[int] = []
 
     # OS Information
     file_permissions: str
     file_size: int  # in bytes
     creation_time: datetime
     modification_time: datetime
     access_time: datetime
@@ -37,18 +40,18 @@
 
 def main(pdf: Path, output: OutputOptions) -> None:
     reader = PdfReader(str(pdf))
     if reader.is_encrypted:
         pdf_stat = pdf.stat()
         meta = MetaInfo(
             encryption=EncryptionData(
-                v_value=reader._encryption.algV,
-                revision=reader._encryption.algR,
+                v_value=reader._encryption.V,
+                revision=reader._encryption.R,
             )
-            if reader.is_encrypted
+            if reader.is_encrypted and reader._encryption
             else None,
             pdf_file_version=reader.stream.read(8).decode("utf-8"),
             # OS Info
             file_permissions=f"{stat.filemode(pdf_stat.st_mode)}",
             file_size=pdf_stat.st_size,
             creation_time=datetime.fromtimestamp(pdf_stat.st_ctime),
             modification_time=datetime.fromtimestamp(pdf_stat.st_mtime),
@@ -56,32 +59,40 @@
         )
     else:
         info = reader.metadata
 
         reader.stream.seek(0)
         pdf_file_version = reader.stream.read(8).decode("utf-8")
         pdf_stat = pdf.stat()
+        pdf_id = reader.trailer.get("/ID")
         meta = MetaInfo(
             pages=len(reader.pages),
             encryption=EncryptionData(
-                v_value=reader._encryption.algV,
-                revision=reader._encryption.algR,
+                v_value=reader._encryption.V,  # type: ignore
+                revision=reader._encryption.R,  # type: ignore
             )
-            if reader.is_encrypted
+            if reader.is_encrypted and reader._encryption
             else None,
             page_mode=reader.page_mode,
             pdf_file_version=pdf_file_version,
             page_layout=reader.page_layout,
             attachments=str(list(reader.attachments.keys())),
+            id1=pdf_id[0] if pdf_id is not None else None,
+            id2=pdf_id[1] if pdf_id is not None and len(pdf_id) >= 2 else None,
             # OS Info
             file_permissions=f"{stat.filemode(pdf_stat.st_mode)}",
             file_size=pdf_stat.st_size,
             creation_time=datetime.fromtimestamp(pdf_stat.st_ctime),
             modification_time=datetime.fromtimestamp(pdf_stat.st_mtime),
             access_time=datetime.fromtimestamp(pdf_stat.st_atime),
+            images=[
+                len(image.data)
+                for page in reader.pages
+                for image in page.images
+            ],
         )
         if info is not None:
             meta.title = info.title
             meta.producer = info.producer
             meta.author = info.author
 
     if output == OutputOptions.json:
@@ -100,28 +111,32 @@
         table.add_row("Producer", meta.producer)
         table.add_row("Author", meta.author)
         table.add_row("Pages", f"{meta.pages:,}" if meta.pages else "unknown")
         table.add_row("Encrypted", f"{meta.encryption}")
         table.add_row("PDF File Version", meta.pdf_file_version)
         table.add_row("Page Layout", meta.page_layout)
         table.add_row("Page Mode", meta.page_mode)
+        table.add_row("PDF ID", f"ID1={meta.id1!r} ID2={meta.id2!r}")
         embedded_fonts: Set[str] = set()
         unemedded_fonts: Set[str] = set()
         if not reader.is_encrypted:
             for page in reader.pages:
                 emb, unemb = page._get_fonts()
                 embedded_fonts = embedded_fonts.union(set(emb))
                 unemedded_fonts = unemedded_fonts.union(set(unemb))
             table.add_row(
                 "Fonts (unembedded)", ", ".join(sorted(unemedded_fonts))
             )
             table.add_row(
                 "Fonts (embedded)", ", ".join(sorted(embedded_fonts))
             )
         table.add_row("Attachments", meta.attachments)
+        table.add_row(
+            "Images", f"{len(meta.images)} images ({sum(meta.images):,} bytes)"
+        )
 
         enc_table = Table(title="Encryption information")
         enc_table.add_column(
             "Attribute", justify="right", style="cyan", no_wrap=True
         )
         enc_table.add_column("Value", style="white")
         if meta.encryption:
```

### Comparing `pdfly-0.1.1/pdfly/pagemeta.py` & `pdfly-0.1.2/pdfly/pagemeta.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.1/pdfly/up2.py` & `pdfly-0.1.2/pdfly/up2.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.1/pdfly.egg-info/PKG-INFO` & `pdfly-0.1.2/pdfly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfly
-Version: 0.1.1
+Version: 0.1.2
 Summary: A pure-python CLI application to manipulate PDF files
 Home-page: https://github.com/py-pdf/pdfly
 Author: Martin Thoma
 Author-email: info@martin-thoma.de
 Maintainer: Martin Thoma
 Maintainer-email: info@martin-thoma.de
 License: BSD-3-Clause
```

### Comparing `pdfly-0.1.1/pyproject.toml` & `pdfly-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdfly-0.1.1/setup.cfg` & `pdfly-0.1.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 python_requires = >=3.6.1
 install_requires = 
-	pypdf>3.0.0
+	pypdf>=3.8.2
 	typer
 	pillow
 	pydantic
 	rich
 
 [options.entry_points]
 console_scripts =
```

