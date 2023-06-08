# Comparing `tmp/metadata_parser-0.9.6.tar.gz` & `tmp/metadata_parser-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/metadata_parser-0.9.6.tar", last modified: Tue May  9 18:13:25 2017, max compression
+gzip compressed data, was "dist/metadata_parser-0.9.7.tar", last modified: Fri May 19 00:39:57 2017, max compression
```

## Comparing `metadata_parser-0.9.6.tar` & `metadata_parser-0.9.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2017-05-09 18:13:25.000000 metadata_parser-0.9.6/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1148 2014-11-26 18:40:26.000000 metadata_parser-0.9.6/LICENSE.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       92 2017-01-16 21:39:29.000000 metadata_parser-0.9.6/MANIFEST.in
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2017-05-09 18:13:25.000000 metadata_parser-0.9.6/metadata_parser/
--rw-r--r--   0 jvanasco   (501) admin       (80)    48268 2017-05-09 18:12:23.000000 metadata_parser-0.9.6/metadata_parser/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     3815 2014-01-19 23:29:11.000000 metadata_parser-0.9.6/metadata_parser/types.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2017-05-09 18:13:25.000000 metadata_parser-0.9.6/metadata_parser.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2017-05-09 18:13:25.000000 metadata_parser-0.9.6/metadata_parser.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       37 2017-05-09 18:13:25.000000 metadata_parser-0.9.6/metadata_parser.egg-info/entry_points.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2017-01-16 21:39:32.000000 metadata_parser-0.9.6/metadata_parser.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)     9930 2017-05-09 18:13:25.000000 metadata_parser-0.9.6/metadata_parser.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       32 2017-05-09 18:13:25.000000 metadata_parser-0.9.6/metadata_parser.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      518 2017-05-09 18:13:25.000000 metadata_parser-0.9.6/metadata_parser.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       22 2017-05-09 18:13:25.000000 metadata_parser-0.9.6/metadata_parser.egg-info/top_level.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     9930 2017-05-09 18:13:25.000000 metadata_parser-0.9.6/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)     7690 2017-03-15 22:13:32.000000 metadata_parser-0.9.6/README.rst
--rw-r--r--   0 jvanasco   (501) admin       (80)       72 2017-05-09 18:13:25.000000 metadata_parser-0.9.6/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     1418 2017-05-09 18:07:08.000000 metadata_parser-0.9.6/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2017-05-09 18:13:25.000000 metadata_parser-0.9.6/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2014-07-14 18:17:30.000000 metadata_parser-0.9.6/tests/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    11172 2017-03-16 18:01:17.000000 metadata_parser-0.9.6/tests/document_parsing.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2017-05-09 18:13:25.000000 metadata_parser-0.9.6/tests/html_scaffolds/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1645 2017-01-17 18:58:57.000000 metadata_parser-0.9.6/tests/html_scaffolds/simple.html
--rw-r--r--   0 jvanasco   (501) admin       (80)      257 2017-01-16 21:27:28.000000 metadata_parser-0.9.6/tests/ip_tracking.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     2528 2017-03-16 00:21:30.000000 metadata_parser-0.9.6/tests/sessions.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    13101 2017-03-07 22:18:35.000000 metadata_parser-0.9.6/tests/url_parsing.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2017-05-19 00:39:57.000000 metadata_parser-0.9.7/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1148 2014-11-26 18:40:26.000000 metadata_parser-0.9.7/LICENSE.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       92 2017-01-16 21:39:29.000000 metadata_parser-0.9.7/MANIFEST.in
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2017-05-19 00:39:57.000000 metadata_parser-0.9.7/metadata_parser/
+-rw-r--r--   0 jvanasco   (501) admin       (80)    50097 2017-05-19 00:38:39.000000 metadata_parser-0.9.7/metadata_parser/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3815 2014-01-19 23:29:11.000000 metadata_parser-0.9.7/metadata_parser/types.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2017-05-19 00:39:57.000000 metadata_parser-0.9.7/metadata_parser.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2017-05-19 00:39:56.000000 metadata_parser-0.9.7/metadata_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       37 2017-05-19 00:39:56.000000 metadata_parser-0.9.7/metadata_parser.egg-info/entry_points.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2017-01-16 21:39:32.000000 metadata_parser-0.9.7/metadata_parser.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)     9930 2017-05-19 00:39:56.000000 metadata_parser-0.9.7/metadata_parser.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)       32 2017-05-19 00:39:56.000000 metadata_parser-0.9.7/metadata_parser.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      518 2017-05-19 00:39:56.000000 metadata_parser-0.9.7/metadata_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       22 2017-05-19 00:39:56.000000 metadata_parser-0.9.7/metadata_parser.egg-info/top_level.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)     9930 2017-05-19 00:39:57.000000 metadata_parser-0.9.7/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     7690 2017-03-15 22:13:32.000000 metadata_parser-0.9.7/README.rst
+-rw-r--r--   0 jvanasco   (501) admin       (80)       72 2017-05-19 00:39:57.000000 metadata_parser-0.9.7/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1418 2017-05-09 18:07:08.000000 metadata_parser-0.9.7/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2017-05-19 00:39:57.000000 metadata_parser-0.9.7/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2014-07-14 18:17:30.000000 metadata_parser-0.9.7/tests/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    11172 2017-03-16 18:01:17.000000 metadata_parser-0.9.7/tests/document_parsing.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2017-05-19 00:39:57.000000 metadata_parser-0.9.7/tests/html_scaffolds/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1645 2017-01-17 18:58:57.000000 metadata_parser-0.9.7/tests/html_scaffolds/simple.html
+-rw-r--r--   0 jvanasco   (501) admin       (80)      257 2017-01-16 21:27:28.000000 metadata_parser-0.9.7/tests/ip_tracking.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2528 2017-03-16 00:21:30.000000 metadata_parser-0.9.7/tests/sessions.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    13894 2017-05-19 00:22:04.000000 metadata_parser-0.9.7/tests/url_parsing.py
```

### Comparing `metadata_parser-0.9.6/LICENSE.txt` & `metadata_parser-0.9.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `metadata_parser-0.9.6/metadata_parser/__init__.py` & `metadata_parser-0.9.7/metadata_parser/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-
 import logging
 log = logging.getLogger(__name__)
 
 
 # ------------------------------------------------------------------------------
 
 
-__VERSION__ = '0.9.6'
+__VERSION__ = '0.9.7'
 
 
 # ------------------------------------------------------------------------------
 
 
 # stdlib
 import datetime
@@ -130,14 +129,34 @@
 
 RE_IPV4_ADDRESS = re.compile(
     r'^(\d{1,3})\.(\d{1,3}).(\d{1,3}).(\d{1,3})$'  # grab 4 octets
 )
 
 RE_ALL_NUMERIC = re.compile("^[\d\.]+$")
 
+# we may need to test general validity of url components
+RE_rfc3986_valid_characters = re.compile("""^[a-z0-9\-\.\_\~\:\/\?\#\[\]\@\!\$\&\'\(\)\*\+\,\;\=\%]+$""", re.I)
+"""
+What is valid in the RFC?
+    # don't need escaping
+    rfc3986_unreserved__noescape = ['a-z', '0-9', ]  
+    
+    # do need escaping
+    rfc3986_unreserved__escape = ['-', '.', '_', '~', ]
+    rfc3986_gen_delims__escape = [":", "/", "?", "#", "[", "]", "@", ]
+    rfc3986_sub_delims__escape = ["!", "$", "&", "'", "(", ")", "*", "+", ",", ";", "=", ]
+    rfc3986_pct_encoded__escape = ["%", ]
+    rfc3986__escape = rfc3986_unreserved__escape  + rfc3986_gen_delims__escape + rfc3986_sub_delims__escape + rfc3986_pct_encoded__escape
+    rfc3986__escaped = re.escape(''.join(rfc3986__escape))
+    rfc3986_chars = ''.join(rfc3986_unreserved__noescape) + rfc3986__escaped
+    print rfc3986_chars
+
+    a-z0-9\-\.\_\~\:\/\?\#\[\]\@\!\$\&\'\(\)\*\+\,\;\=\%
+"""
+    
 
 # ------------------------------------------------------------------------------
 
 
 def encode_ascii(text):
     """
     helper function to force ascii; some edge-cases have unicode line breaks in titles/etc.
@@ -1184,26 +1203,34 @@
         require_public_global=True,
         url_fallback=None,
     ):
         """this was originally part of `get_discrete_url`"""
         canonical = self.get_metadata('canonical', strategy=['page'])
         if not canonical:
             return None
+        # does the canonical have valid characters?
+        # some websites, even BIG PROFESSIONAL ONES, will put html in here.
+        # amateurs.
+        canonical_valid_chars = RE_rfc3986_valid_characters.match(canonical)
+        if not canonical_valid_chars:
+            return None
         if require_public_global:
             if url_fallback is None:
                 # derive a fallback url, and ensure it is valid
                 url_fallback = self.get_fallback_url(require_public_netloc=True,
                                                      allow_localhosts=False,
                                                      )
             if canonical and not is_url_valid(
                 canonical,
                 require_public_netloc=True,
                 allow_localhosts=False,
             ):
                 # try making it absolute
+                
+                
                 canonical = url_to_absolute_url(
                     canonical,
                     url_fallback=url_fallback,
                     require_public_netloc=True,
                     allow_localhosts=False,
                 )
                 if not is_url_valid(
@@ -1220,14 +1247,20 @@
         require_public_global=True,
         url_fallback=None,
     ):
         """this was originally part of `get_discrete_url`"""
         og = self.get_metadata('url', strategy=['og'])
         if not og:
             return None
+        # does the og have valid characters?
+        # some websites, even BIG PROFESSIONAL ONES, will put html in here.
+        # idiots.
+        og_valid_chars = RE_rfc3986_valid_characters.match(og)
+        if not og_valid_chars:
+            return None
         if require_public_global:
             if url_fallback is None:
                 # derive a fallback url, and ensure it is valid
                 url_fallback = self.get_fallback_url(require_public_netloc=True,
                                                      allow_localhosts=False,
                                                      )
             if og and not is_url_valid(
@@ -1329,23 +1362,30 @@
         # `_value` will be our raw value
         _value = self.get_metadata(field, strategy=strategy)
         if not _value:
             return None
 
         # `value` will be our clean value
         # remove whitespace, because some bad blogging platforms add in whitespace by printing elements on multiple lines. d'oh!
+        # this also up data:image and normal links
         value = RE_whitespace.sub('', _value)
 
         # it's possible for an encoded URI to be an image
         # if that is the case, don't return it (this is `get_metadata_LINK`)
-        if value.lower().startswith('data:image/'):
+        if value[:11].lower().startswith('data:image/'):
             if allow_encoded_uri:
                 return value
             return None
 
+        # it is possible for a declared url to not have rfc valid characters
+        # sometimes you'll find HTML documents in here. serious!
+        is_valid_chars = RE_rfc3986_valid_characters.match(value)
+        if not is_valid_chars:
+            return None
+
         if require_public_global:
             _require_public_netloc = True
             _allow_localhosts = False
         else:
             _require_public_netloc = False
             _allow_localhosts = True
```

### Comparing `metadata_parser-0.9.6/metadata_parser/types.txt` & `metadata_parser-0.9.7/metadata_parser/types.txt`

 * *Files identical despite different names*

### Comparing `metadata_parser-0.9.6/metadata_parser.egg-info/PKG-INFO` & `metadata_parser-0.9.7/metadata_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: metadata-parser
-Version: 0.9.6
+Version: 0.9.7
 Summary: A module to parse metadata out of urls and html documents
 Home-page: https://github.com/jvanasco/metadata_parser
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT
 Description: MetadataParser is a python module for pulling metadata out of web documents.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 1.1 Name: metadata-parser Version: 0.9.6 Summary: A module to
+Metadata-Version: 1.1 Name: metadata-parser Version: 0.9.7 Summary: A module to
 parse metadata out of urls and html documents Home-page: https://github.com/
 jvanasco/metadata_parser Author: Jonathan Vanasco Author-email:
 jonathan@findmeon.com License: MIT Description: MetadataParser is a python
 module for pulling metadata out of web documents. It requires BeautifulSoup ,
 and was largely based on Erik River's opengraph module ( https://github.com/
 erikriver/opengraph ). I needed something more aggressive than Erik's module ,
 so had to fork. Installation ============= pip install metadata_parser
```

### Comparing `metadata_parser-0.9.6/metadata_parser.egg-info/SOURCES.txt` & `metadata_parser-0.9.7/metadata_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metadata_parser-0.9.6/PKG-INFO` & `metadata_parser-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: metadata_parser
-Version: 0.9.6
+Version: 0.9.7
 Summary: A module to parse metadata out of urls and html documents
 Home-page: https://github.com/jvanasco/metadata_parser
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT
 Description: MetadataParser is a python module for pulling metadata out of web documents.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 1.1 Name: metadata_parser Version: 0.9.6 Summary: A module to
+Metadata-Version: 1.1 Name: metadata_parser Version: 0.9.7 Summary: A module to
 parse metadata out of urls and html documents Home-page: https://github.com/
 jvanasco/metadata_parser Author: Jonathan Vanasco Author-email:
 jonathan@findmeon.com License: MIT Description: MetadataParser is a python
 module for pulling metadata out of web documents. It requires BeautifulSoup ,
 and was largely based on Erik River's opengraph module ( https://github.com/
 erikriver/opengraph ). I needed something more aggressive than Erik's module ,
 so had to fork. Installation ============= pip install metadata_parser
```

### Comparing `metadata_parser-0.9.6/README.rst` & `metadata_parser-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `metadata_parser-0.9.6/setup.py` & `metadata_parser-0.9.7/setup.py`

 * *Files identical despite different names*

### Comparing `metadata_parser-0.9.6/tests/document_parsing.py` & `metadata_parser-0.9.7/tests/document_parsing.py`

 * *Files identical despite different names*

### Comparing `metadata_parser-0.9.6/tests/html_scaffolds/simple.html` & `metadata_parser-0.9.7/tests/html_scaffolds/simple.html`

 * *Files identical despite different names*

### Comparing `metadata_parser-0.9.6/tests/sessions.py` & `metadata_parser-0.9.7/tests/sessions.py`

 * *Files identical despite different names*

### Comparing `metadata_parser-0.9.6/tests/url_parsing.py` & `metadata_parser-0.9.7/tests/url_parsing.py`

 * *Files 8% similar despite different names*

```diff
@@ -112,14 +112,39 @@
     'https://example_com/one',
     'https://999.999.999.999/',
     'https://999.999.999.999.999/',
     'https://999.999.999.999.999:8080:8080',
 ]
 
 
+RFC_REGEX_VALID = ["""http://user:password@one.example.com/foo/bar;one=two&three=four?foo=bar&biz=bash#foo""",
+                   ]
+
+RFC_REGEX_INVALID = ["""</p><br /><p>Then l""",
+                     """ccurl" style="display:none;" """,
+                   ]
+
+
+class TestUrlRfcValid(unittest.TestCase):
+    """
+    python -m unittest tests.url_parsing.TestUrlRfcValid
+
+    Ensures URLs contain rfc valid components
+    """
+    def test_urls_valid(self):
+        for i in RFC_REGEX_VALID:
+            matched = metadata_parser.RE_rfc3986_valid_characters.match(i)
+            self.assertTrue(matched)
+
+    def test_urls_invalid(self):
+        for i in RFC_REGEX_INVALID:
+            matched = metadata_parser.RE_rfc3986_valid_characters.match(i)
+            self.assertTrue(matched is None)
+
+
 class TestUrlParsing(unittest.TestCase):
     """
     python -m unittest tests.url_parsing.TestUrls
 
     Ensures URLs are parsed correctly as valid/invalid
     """
     def test_urls_valid(self):
```

