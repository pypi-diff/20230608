# Comparing `tmp/e-models-1.3.2.tar.gz` & `tmp/e-models-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.3.2.tar", last modified: Fri May 19 18:49:17 2023, max compression
+gzip compressed data, was "e-models-1.3.3.tar", last modified: Thu Jun  8 13:46:59 2023, max compression
```

## Comparing `e-models-1.3.2.tar` & `e-models-1.3.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-19 18:49:17.846984 e-models-1.3.2/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.3.2/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3270 2023-05-19 18:49:17.846984 e-models-1.3.2/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2730 2023-04-19 14:03:12.000000 e-models-1.3.2/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-19 18:49:17.842984 e-models-1.3.2/e_models.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3270 2023-05-19 18:49:17.000000 e-models-1.3.2/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      471 2023-05-19 18:49:17.000000 e-models-1.3.2/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-05-19 18:49:17.000000 e-models-1.3.2/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        7 2023-05-19 18:49:17.000000 e-models-1.3.2/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-05-19 18:49:17.000000 e-models-1.3.2/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-19 18:49:17.846984 e-models-1.3.2/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2023-05-19 18:48:44.000000 e-models-1.3.2/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-05-04 18:51:26.000000 e-models-1.3.2/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-19 18:49:17.846984 e-models-1.3.2/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    34290 2023-05-19 18:47:14.000000 e-models-1.3.2/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.3.2/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.3.2/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.3.2/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.3.2/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.3.2/emodels/py.typed
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6744 2023-05-19 17:09:55.000000 e-models-1.3.2/emodels/scrapyutils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.3.2/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-05-19 18:49:17.846984 e-models-1.3.2/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      907 2023-05-19 18:48:49.000000 e-models-1.3.2/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-19 18:49:17.846984 e-models-1.3.2/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3915 2023-05-19 18:19:41.000000 e-models-1.3.2/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7435 2023-05-04 18:49:39.000000 e-models-1.3.2/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-08 13:46:59.465554 e-models-1.3.3/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.3.3/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3468 2023-06-08 13:46:59.465554 e-models-1.3.3/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2928 2023-06-01 14:06:43.000000 e-models-1.3.3/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-08 13:46:59.461554 e-models-1.3.3/e_models.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3468 2023-06-08 13:46:59.000000 e-models-1.3.3/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      471 2023-06-08 13:46:59.000000 e-models-1.3.3/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-06-08 13:46:59.000000 e-models-1.3.3/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        7 2023-06-08 13:46:59.000000 e-models-1.3.3/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-06-08 13:46:59.000000 e-models-1.3.3/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-08 13:46:59.461554 e-models-1.3.3/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2023-06-08 13:46:29.000000 e-models-1.3.3/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-05-04 18:51:26.000000 e-models-1.3.3/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-08 13:46:59.465554 e-models-1.3.3/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35296 2023-06-08 13:46:29.000000 e-models-1.3.3/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.3.3/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.3.3/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.3.3/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.3.3/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.3.3/emodels/py.typed
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6744 2023-05-19 17:09:55.000000 e-models-1.3.3/emodels/scrapyutils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.3.3/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-06-08 13:46:59.465554 e-models-1.3.3/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      907 2023-06-08 13:46:29.000000 e-models-1.3.3/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-06-08 13:46:59.465554 e-models-1.3.3/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4951 2023-06-08 13:41:24.000000 e-models-1.3.3/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7435 2023-05-04 18:49:39.000000 e-models-1.3.3/tests/test_scrapyutils.py
```

### Comparing `e-models-1.3.2/LICENSE` & `e-models-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.3.2/PKG-INFO` & `e-models-1.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.3.2
+Version: 1.3.3
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -31,14 +31,15 @@
 
 scrapyutils module provides two classes, one for extending `scrapy.http.TextResponse` and another for
 extending `scrapy.loader.ItemLoader`. The extensions provide methods that:
 
 1. Allow to extract item data in the text (markdown) domain instead of the html source domain.
 2. The main purpose of this approach is the generation of datasets suitable for training transformer models for text extraction (aka extractive question answering, EQA)
 3. As a secondary objective, it provides an alternative approach to xpath and css selectors for extraction of data from the html source, that may be more suitable and readable for humans.
+4. In many situations, and specially when there is not an id or a class to spot accurately the text, the expresion in terms of regular expressions in the domain of markdown is usually much simpler.
 
 Usage:
 
 Instead of subclass your item loaders from `scrapy.loader.ItemLoader`, use `emodels.scrapyutils.ExtractItemLoader`. This action will not affect the working of itemloaders and will enable the properties just
 described above. In addition, in order to save the collected extraction data, it is required to set the environment variable `EMODELS_SAVE_EXTRACT_ITEMS` to 1. The collected
 extraction data will be stored at `<user home folder>/.datasets/items/<item class name>/<sequence number>.jl.gz`. The base folder `<user home folder>/.datasets` is the default one. You can
 customize it via the environment variable `EMODELS_DIR`.
```

### Comparing `e-models-1.3.2/README.md` & `e-models-1.3.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 scrapyutils module provides two classes, one for extending `scrapy.http.TextResponse` and another for
 extending `scrapy.loader.ItemLoader`. The extensions provide methods that:
 
 1. Allow to extract item data in the text (markdown) domain instead of the html source domain.
 2. The main purpose of this approach is the generation of datasets suitable for training transformer models for text extraction (aka extractive question answering, EQA)
 3. As a secondary objective, it provides an alternative approach to xpath and css selectors for extraction of data from the html source, that may be more suitable and readable for humans.
+4. In many situations, and specially when there is not an id or a class to spot accurately the text, the expresion in terms of regular expressions in the domain of markdown is usually much simpler.
 
 Usage:
 
 Instead of subclass your item loaders from `scrapy.loader.ItemLoader`, use `emodels.scrapyutils.ExtractItemLoader`. This action will not affect the working of itemloaders and will enable the properties just
 described above. In addition, in order to save the collected extraction data, it is required to set the environment variable `EMODELS_SAVE_EXTRACT_ITEMS` to 1. The collected
 extraction data will be stored at `<user home folder>/.datasets/items/<item class name>/<sequence number>.jl.gz`. The base folder `<user home folder>/.datasets` is the default one. You can
 customize it via the environment variable `EMODELS_DIR`.
```

### Comparing `e-models-1.3.2/e_models.egg-info/PKG-INFO` & `e-models-1.3.3/e_models.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.3.2
+Version: 1.3.3
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -31,14 +31,15 @@
 
 scrapyutils module provides two classes, one for extending `scrapy.http.TextResponse` and another for
 extending `scrapy.loader.ItemLoader`. The extensions provide methods that:
 
 1. Allow to extract item data in the text (markdown) domain instead of the html source domain.
 2. The main purpose of this approach is the generation of datasets suitable for training transformer models for text extraction (aka extractive question answering, EQA)
 3. As a secondary objective, it provides an alternative approach to xpath and css selectors for extraction of data from the html source, that may be more suitable and readable for humans.
+4. In many situations, and specially when there is not an id or a class to spot accurately the text, the expresion in terms of regular expressions in the domain of markdown is usually much simpler.
 
 Usage:
 
 Instead of subclass your item loaders from `scrapy.loader.ItemLoader`, use `emodels.scrapyutils.ExtractItemLoader`. This action will not affect the working of itemloaders and will enable the properties just
 described above. In addition, in order to save the collected extraction data, it is required to set the environment variable `EMODELS_SAVE_EXTRACT_ITEMS` to 1. The collected
 extraction data will be stored at `<user home folder>/.datasets/items/<item class name>/<sequence number>.jl.gz`. The base folder `<user home folder>/.datasets` is the default one. You can
 customize it via the environment variable `EMODELS_DIR`.
```

### Comparing `e-models-1.3.2/emodels/html2text/__init__.py` & `e-models-1.3.3/emodels/html2text/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,17 +130,17 @@
         self.abbr_list = {}  # type: Dict[str, str]
         self.baseurl = baseurl
         self.stressed = False
         self.preceding_stressed = False
         self.preceding_data = ""
         self.current_tag = ""
         self.ids = ids
-        self.current_id: List[str | None] = []
+        self.current_id: List[Tuple[str, bool | None]] = []
         self.classes = classes
-        self.current_class: List[str | None] = []
+        self.current_class: List[Tuple[str, bool | None]] = []
         self.within_table_row = 0
 
         config.UNIFIABLE["nbsp"] = "&nbsp_place_holder;"
 
     def feed(self, data: str) -> None:
         data = data.replace("</' + 'script>", "</ignore>")
         super().feed(data)
@@ -184,21 +184,21 @@
 
     def handle_entityref(self, c: str) -> None:
         result = unormalize("NFKC", html_unescape("&" + c))
         if result:
             return self.handle_data(result, True)
 
     def handle_starttag(self, tag: str, attrs: List[Tuple[str, Optional[str]]]) -> None:
-        attrid = dict(attrs).get("itemprop", "")
+        attrid = (dict(attrs).get("itemprop") or "").strip()
         if not attrid:
-            attrid = dict(attrs).get("id", "")
-        self.current_id.append(attrid)
+            attrid = (dict(attrs).get("id") or "").strip()
+        self.current_id.append((attrid, None))
 
-        attrclass = dict(attrs).get("class", "").strip()
-        self.current_class.append(attrclass)
+        attrclass = (dict(attrs).get("class") or "").strip()
+        self.current_class.append((attrclass, None))
 
         self.handle_tag(tag, dict(attrs), start=True)
 
     def handle_endtag(self, tag: str) -> None:
         if self.current_id:
             self.current_id.pop()
         if self.current_class:
@@ -823,22 +823,43 @@
                 self.maybe_automatic_link = None
                 self.empty_link = False
 
         if not self.code and not self.pre and not entity_char:
             data = escape_md_section(data, snob=self.escape_snob)
         self.preceding_data = data
         self.o(data, puredata=True)
-        if self.ids and rawdata and self.current_id and not self.cdata_elem:
-            attrid = self.current_id[-1]
-            if attrid:
-                self.out(f" <!--#{attrid}-->")
-        if self.classes and rawdata and self.current_class and not self.cdata_elem:
-            attrclass = self.current_class[-1]
-            if attrclass:
-                self.out(f" <!--.{attrclass}-->")
+
+        if self.ids and self.current_id and not self.cdata_elem:
+            attrid, delayed_attrid = self.current_id[-1]
+            if rawdata:
+                if attrid:
+                    self.out(f" <!--#{attrid}-->")
+                elif len(self.current_id) > 1:
+                    a, d = self.current_id[-2]
+                    if d:
+                        self.out(f" <!--#{a}-->")
+                        self.current_id = self.current_id[:-2] + [(a, False), self.current_id[-1]]
+            elif attrid and delayed_attrid is None:
+
+                self.current_id.pop()
+                self.current_id.append((attrid, True))
+
+        if self.classes and self.current_class and not self.cdata_elem:
+            attrclass, delayed_attrclass = self.current_class[-1]
+            if rawdata:
+                if attrclass:
+                    self.out(f" <!--.{attrclass}-->")
+                elif len(self.current_class) > 1:
+                    a, d = self.current_class[-2]
+                    if d:
+                        self.out(f" <!--.{a}-->")
+                        self.current_class = self.current_class[:-2] + [(a, False), self.current_class[-1]]
+            elif attrclass and delayed_attrclass is None:
+                self.current_class.pop()
+                self.current_class.append((attrclass, True))
 
     def charref(self, name: str) -> str:
         if name[0] in ["x", "X"]:
             c = int(name[1:], 16)
         else:
             c = int(name)
```

### Comparing `e-models-1.3.2/emodels/html2text/config.py` & `e-models-1.3.3/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.3.2/emodels/html2text/utils.py` & `e-models-1.3.3/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.3.2/emodels/scrapyutils.py` & `e-models-1.3.3/emodels/scrapyutils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.3.2/setup.py` & `e-models-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.3.2',
+    version      = '1.3.3',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
```

### Comparing `e-models-1.3.2/tests/test_scrapyutils.py` & `e-models-1.3.3/tests/test_scrapyutils.py`

 * *Files identical despite different names*

