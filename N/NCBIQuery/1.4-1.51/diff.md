# Comparing `tmp/NCBIQuery-1.4.tar.gz` & `tmp/NCBIQuery-1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NCBIQuery-1.4.tar", last modified: Thu Apr 27 19:46:06 2023, max compression
+gzip compressed data, was "NCBIQuery-1.51.tar", last modified: Thu Jun  8 20:00:04 2023, max compression
```

## Comparing `NCBIQuery-1.4.tar` & `NCBIQuery-1.51.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:46:06.445273 NCBIQuery-1.4/
--rw-r--r--   0 root         (0) root         (0)     1064 2023-04-18 18:58:13.000000 NCBIQuery-1.4/LICENSE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:46:06.445273 NCBIQuery-1.4/NCBIQuery/
--rw-r--r--   0 root         (0) root         (0)     2349 2023-04-27 19:41:51.000000 NCBIQuery-1.4/NCBIQuery/NCBIQuery.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-04-18 18:58:13.000000 NCBIQuery-1.4/NCBIQuery/__init__.py
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-27 19:43:19.000000 NCBIQuery-1.4/NCBIQuery/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 19:46:06.445273 NCBIQuery-1.4/NCBIQuery.egg-info/
--rw-r--r--   0 root         (0) root         (0)      254 2023-04-27 19:46:06.000000 NCBIQuery-1.4/NCBIQuery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      269 2023-04-27 19:46:06.000000 NCBIQuery-1.4/NCBIQuery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 19:46:06.000000 NCBIQuery-1.4/NCBIQuery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-27 19:46:06.000000 NCBIQuery-1.4/NCBIQuery.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-27 19:46:06.000000 NCBIQuery-1.4/NCBIQuery.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      254 2023-04-27 19:46:06.445273 NCBIQuery-1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2279 2023-04-27 19:42:06.000000 NCBIQuery-1.4/README.md
--rw-r--r--   0 root         (0) root         (0)       95 2023-04-27 19:46:06.445273 NCBIQuery-1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      425 2023-04-18 18:58:13.000000 NCBIQuery-1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:00:04.246648 NCBIQuery-1.51/
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-04-18 18:58:13.000000 NCBIQuery-1.51/LICENSE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:00:04.246648 NCBIQuery-1.51/NCBIQuery/
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-06-08 18:48:06.000000 NCBIQuery-1.51/NCBIQuery/NCBIQuery.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-18 18:58:13.000000 NCBIQuery-1.51/NCBIQuery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-08 19:59:56.000000 NCBIQuery-1.51/NCBIQuery/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:00:04.246648 NCBIQuery-1.51/NCBIQuery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      255 2023-06-08 20:00:04.000000 NCBIQuery-1.51/NCBIQuery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-08 20:00:04.000000 NCBIQuery-1.51/NCBIQuery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 20:00:04.000000 NCBIQuery-1.51/NCBIQuery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 20:00:04.000000 NCBIQuery-1.51/NCBIQuery.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 20:00:04.000000 NCBIQuery-1.51/NCBIQuery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      255 2023-06-08 20:00:04.246648 NCBIQuery-1.51/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-04-27 19:42:06.000000 NCBIQuery-1.51/README.md
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-08 20:00:04.246648 NCBIQuery-1.51/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      425 2023-04-18 18:58:13.000000 NCBIQuery-1.51/setup.py
```

### Comparing `NCBIQuery-1.4/LICENSE.md` & `NCBIQuery-1.51/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NCBIQuery-1.4/NCBIQuery/NCBIQuery.py` & `NCBIQuery-1.51/NCBIQuery/NCBIQuery.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,19 +36,19 @@
         et = ET.fromstring(res)
         return et
     if not isinstance(search_ids, list):
         search_ids = [search_ids]
     article_abstracts = []
     article_infos = get_article_info(search_ids)
     for article in article_infos:
+        abstract = ''
         for child in article.iter('*'):
             if child.tag == 'AbstractText':
                 if child.text is not None:
-                    article_abstracts.append(child.text)
-                else:
-                    article_abstracts.append('')
+                    abstract = child.text
                 break
+        article_abstracts.append(abstract)
     return article_abstracts
 
 def query_abstract(db='pubmed', search_field_tags='tw', contents='', retmax=10000):
     search_ids = query_id(db, search_field_tags, contents, retmax)
     return id_abstract(search_ids, db)
```

### Comparing `NCBIQuery-1.4/README.md` & `NCBIQuery-1.51/README.md`

 * *Files identical despite different names*

