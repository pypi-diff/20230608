# Comparing `tmp/htmlmeta_hub-0.4.1.tar.gz` & `tmp/htmlmeta_hub-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/htmlmeta_hub-0.4.1.tar", last modified: Fri Mar 26 00:35:14 2021, max compression
+gzip compressed data, was "htmlmeta_hub-0.5.0.tar", last modified: Thu Jun  8 19:34:11 2023, max compression
```

## Comparing `htmlmeta_hub-0.4.1.tar` & `htmlmeta_hub-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-26 00:35:14.000000 htmlmeta_hub-0.4.1/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1353 2021-03-26 00:34:29.000000 htmlmeta_hub-0.4.1/CHANGES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     1181 2012-02-06 23:47:22.000000 htmlmeta_hub-0.4.1/LICENSE.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      200 2021-03-26 00:34:16.000000 htmlmeta_hub-0.4.1/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)     2828 2021-03-26 00:35:14.000000 htmlmeta_hub-0.4.1/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       48 2020-10-14 16:22:13.000000 htmlmeta_hub-0.4.1/pyproject.toml
--rw-r--r--   0 jvanasco   (501) admin       (80)     1711 2020-10-20 20:01:02.000000 htmlmeta_hub-0.4.1/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)       69 2021-03-26 00:35:14.000000 htmlmeta_hub-0.4.1/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     1627 2021-03-26 00:35:00.000000 htmlmeta_hub-0.4.1/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-26 00:35:14.000000 htmlmeta_hub-0.4.1/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-26 00:35:14.000000 htmlmeta_hub-0.4.1/src/htmlmeta_hub/
--rw-r--r--   0 jvanasco   (501) admin       (80)     6672 2021-03-26 00:34:24.000000 htmlmeta_hub-0.4.1/src/htmlmeta_hub/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      386 2020-10-20 19:58:38.000000 htmlmeta_hub-0.4.1/src/htmlmeta_hub/pyramid_helpers.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-26 00:35:14.000000 htmlmeta_hub-0.4.1/src/htmlmeta_hub.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-26 00:35:13.000000 htmlmeta_hub-0.4.1/src/htmlmeta_hub.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-26 00:35:13.000000 htmlmeta_hub-0.4.1/src/htmlmeta_hub.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)     2828 2021-03-26 00:35:13.000000 htmlmeta_hub-0.4.1/src/htmlmeta_hub.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       52 2021-03-26 00:35:13.000000 htmlmeta_hub-0.4.1/src/htmlmeta_hub.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      452 2021-03-26 00:35:13.000000 htmlmeta_hub-0.4.1/src/htmlmeta_hub.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       13 2021-03-26 00:35:13.000000 htmlmeta_hub-0.4.1/src/htmlmeta_hub.egg-info/top_level.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-26 00:35:14.000000 htmlmeta_hub-0.4.1/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)     2792 2020-10-20 20:00:43.000000 htmlmeta_hub-0.4.1/tests/test_core.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1133 2020-10-20 20:00:43.000000 htmlmeta_hub-0.4.1/tests/test_pyramid_integration.py
--rw-r--r--   0 jvanasco   (501) admin       (80)       46 2019-04-26 20:43:20.000000 htmlmeta_hub-0.4.1/TODO.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      132 2020-10-14 16:22:33.000000 htmlmeta_hub-0.4.1/tox.ini
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 19:34:11.584887 htmlmeta_hub-0.5.0/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1395 2023-06-08 19:33:54.000000 htmlmeta_hub-0.5.0/CHANGES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1181 2012-02-06 23:47:22.000000 htmlmeta_hub-0.5.0/LICENSE.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      200 2021-03-26 00:34:16.000000 htmlmeta_hub-0.5.0/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2605 2023-06-08 19:34:11.585207 htmlmeta_hub-0.5.0/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1711 2020-10-20 20:01:02.000000 htmlmeta_hub-0.5.0/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)       46 2019-04-26 20:43:20.000000 htmlmeta_hub-0.5.0/TODO.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       40 2023-06-08 19:33:54.000000 htmlmeta_hub-0.5.0/pyproject.toml
+-rw-r--r--   0 jvanasco   (501) admin       (80)      248 2023-06-08 19:34:11.587300 htmlmeta_hub-0.5.0/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1926 2023-06-08 19:33:54.000000 htmlmeta_hub-0.5.0/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 19:34:11.539721 htmlmeta_hub-0.5.0/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 19:34:11.566963 htmlmeta_hub-0.5.0/src/htmlmeta_hub/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     6903 2023-06-08 19:33:54.000000 htmlmeta_hub-0.5.0/src/htmlmeta_hub/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-05-12 23:18:09.000000 htmlmeta_hub-0.5.0/src/htmlmeta_hub/py.typed
+-rw-r--r--   0 jvanasco   (501) admin       (80)      685 2023-05-12 23:18:09.000000 htmlmeta_hub-0.5.0/src/htmlmeta_hub/pyramid_helpers.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 19:34:11.575735 htmlmeta_hub-0.5.0/src/htmlmeta_hub.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2605 2023-06-08 19:34:11.000000 htmlmeta_hub-0.5.0/src/htmlmeta_hub.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)      496 2023-06-08 19:34:11.000000 htmlmeta_hub-0.5.0/src/htmlmeta_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-08 19:34:11.000000 htmlmeta_hub-0.5.0/src/htmlmeta_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-26 00:35:13.000000 htmlmeta_hub-0.5.0/src/htmlmeta_hub.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)       53 2023-06-08 19:34:11.000000 htmlmeta_hub-0.5.0/src/htmlmeta_hub.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       13 2023-06-08 19:34:11.000000 htmlmeta_hub-0.5.0/src/htmlmeta_hub.egg-info/top_level.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 19:34:11.580910 htmlmeta_hub-0.5.0/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-05-12 23:18:09.000000 htmlmeta_hub-0.5.0/tests/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2746 2023-05-12 23:18:09.000000 htmlmeta_hub-0.5.0/tests/test_core.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1104 2023-05-12 23:18:09.000000 htmlmeta_hub-0.5.0/tests/test_pyramid_integration.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-05-12 23:18:09.000000 htmlmeta_hub-0.5.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `htmlmeta_hub-0.4.1/CHANGES.txt` & `htmlmeta_hub-0.5.0/CHANGES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 unreleased
+    *
+
+0.5.0
+    * typing
+    * drop py27
 
 0.4.1
 	* packaging fixes
 
 0.4.0
 	* packaging fixes
 	* removed `htmlmeta_setup` from pyramid_helpers; use the `includeme` instead
```

### Comparing `htmlmeta_hub-0.4.1/LICENSE.txt` & `htmlmeta_hub-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `htmlmeta_hub-0.4.1/PKG-INFO` & `htmlmeta_hub-0.5.0/src/htmlmeta_hub.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,83 @@
 Metadata-Version: 2.1
-Name: htmlmeta_hub
-Version: 0.4.1
+Name: htmlmeta-hub
+Version: 0.5.0
 Summary: Lightweight support for managing metadata on webpages.
 Home-page: https://github.com/jvanasco/htmlmeta_hub
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT
-Description: htmlmeta_hub
-        ============
-        
-        Build Status: ![Python package](https://github.com/jvanasco/htmlmeta_hub/workflows/Python%20package/badge.svg)
-        
-        `htmlmeta_hub` offers lightweight support for managing metadata on webpages.
-        
-        This package simply and conveniently manages a dict of "metadata"", and renders
-        it appropriately.
-        
-        There are helpers for the Pyramid framework which will attach the metdata object
-        to a request, allowing you to build up metadata throughtout the request cycle
-        and then finally render.
-        
-        A typical way to use this package in the Pyramid framework:
-        
-        
-        Include this package in your application's  `__init__.py`:
-        
-        	def main(global_config, **settings):
-        		...
-        		# custom htmlmeta
-        		config.include("htmlmeta_hub.pyramid_helpers")
-        
-        
-        If you are using "class based views", you can set some default metadata in a core
-        handler:
-        
-        	class Handler(object):
-        		def __init__(self,request):
-        			self.request = request
-        			# set some defaults
-        			self.reqesut.htmlmeta.set_many(\
-        				title="MyApp",
-        				description="awesome",
-        				keywords="fun!",
-        			)
-        
-        and then you can add specific metadata in each view's handler:
-        
-        	class ContentPage(Handler):
-        		def view(self):
-        		    content= ...
-        			self.request.htmlmeta.set('title', content.title)
-        			self.request.htmlmeta.set('description', content.description)
-        
-        In a template, such as this `page.mako` example, you can access specific bits of
-        the metadata, or render an entire payload:
-        
-        	<title>${request.htmlmeta.get('title')|n}</title>
-        	${request.htmlmeta.as_html()|n}
-        
-        
-        Pyramid helpers existed until version `0.3.x` but were dropped in favor of the
-        `@reify` request method offered by the `config.include` method.
-        
-        Pylons helpers existed until version `0.1.2` but were dropped.
-        
-        
-        
 Keywords: metadata html web pyramid
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Pyramid
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE.txt
+
+htmlmeta_hub
+============
+
+Build Status: ![Python package](https://github.com/jvanasco/htmlmeta_hub/workflows/Python%20package/badge.svg)
+
+`htmlmeta_hub` offers lightweight support for managing metadata on webpages.
+
+This package simply and conveniently manages a dict of "metadata"", and renders
+it appropriately.
+
+There are helpers for the Pyramid framework which will attach the metdata object
+to a request, allowing you to build up metadata throughtout the request cycle
+and then finally render.
+
+A typical way to use this package in the Pyramid framework:
+
+
+Include this package in your application's  `__init__.py`:
+
+	def main(global_config, **settings):
+		...
+		# custom htmlmeta
+		config.include("htmlmeta_hub.pyramid_helpers")
+
+
+If you are using "class based views", you can set some default metadata in a core
+handler:
+
+	class Handler(object):
+		def __init__(self,request):
+			self.request = request
+			# set some defaults
+			self.reqesut.htmlmeta.set_many(\
+				title="MyApp",
+				description="awesome",
+				keywords="fun!",
+			)
+
+and then you can add specific metadata in each view's handler:
+
+	class ContentPage(Handler):
+		def view(self):
+		    content= ...
+			self.request.htmlmeta.set('title', content.title)
+			self.request.htmlmeta.set('description', content.description)
+
+In a template, such as this `page.mako` example, you can access specific bits of
+the metadata, or render an entire payload:
+
+	<title>${request.htmlmeta.get('title')|n}</title>
+	${request.htmlmeta.as_html()|n}
+
+
+Pyramid helpers existed until version `0.3.x` but were dropped in favor of the
+`@reify` request method offered by the `config.include` method.
+
+Pylons helpers existed until version `0.1.2` but were dropped.
+
+
```

### Comparing `htmlmeta_hub-0.4.1/README.md` & `htmlmeta_hub-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `htmlmeta_hub-0.4.1/setup.py` & `htmlmeta_hub-0.5.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 with open(os.path.join(HERE, "README.md")) as f:
     long_description = f.read()
 
 # store version in the init.py
 with open(os.path.join(HERE, "src", "htmlmeta_hub", "__init__.py")) as v_file:
     VERSION = re.compile(r'.*__VERSION__ = "(.*?)"', re.S).match(v_file.read()).group(1)
 
-requires = ["metadata_utils>=0.0.2"]
+requires = ["metadata_utils>=0.2.0"]
 tests_require = [
-    "six",
+    "mypy",
     "pyramid",
     "pytest",
 ]
 testing_extras = tests_require + []
 
 
 setup(
@@ -37,24 +37,30 @@
     author_email="jonathan@findmeon.com",
     zip_safe=False,
     keywords="metadata html web pyramid",
     packages=find_packages(
         where="src",
     ),
     package_dir={"": "src"},
+    package_data={"htmlmeta_hub": ["py.typed"]},
     include_package_data=True,
-    test_suite="tests",
     classifiers=[
         "Intended Audience :: Developers",
         "Framework :: Pyramid",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
     ],
     license="MIT",
     install_requires=requires,
     tests_require=tests_require,
     extras_require={
         "testing": testing_extras,
     },
+    test_suite="tests",
 )
```

### Comparing `htmlmeta_hub-0.4.1/src/htmlmeta_hub/__init__.py` & `htmlmeta_hub-0.5.0/src/htmlmeta_hub/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+# stdlib
+from typing import Dict
+from typing import Optional
+
+# local
 from metadata_utils import html_attribute_escape
 
 
-__VERSION__ = "0.4.1"
+__VERSION__ = "0.5.0"
 
 
 # ==============================================================================
 
 
 _http_equivs = ("content-type", "expires", "refresh")
 _link_rels = ("canonical", "link")
 
 
 class HtmlMetaHub(object):
-    data_struct = None
+    data_struct: Dict[str, Dict]
 
     def __init__(self, **kwargs):
         """Sets up self.data_struct dict which we use for storage of metadata.
 
         This package is rather silly, but it affords a consistent way to manage metadata across multiple projects.
         """
         self.data_struct = {
@@ -24,156 +29,156 @@
             "name": {},
             "other": {},
             "link": {},
             "_multi": {},  # private namespace for setmulti
         }
         self.set_many(**kwargs)
 
-    def set_http_equiv(self, key, value):
+    def set_http_equiv(self, key: str, value: str):
         self.data_struct["http-equiv"][key] = value
 
-    def set_link(self, rel, value):
+    def set_link(self, rel: str, value: str):
         self.data_struct["link"][rel] = value
 
-    def set_name(self, key, value):
+    def set_name(self, key: str, value: str):
         self.data_struct["name"][key] = value
 
-    def set_other(self, key, value):
+    def set_other(self, key: str, value: str):
         self.data_struct["other"][key] = value
 
-    def set(self, key, value):
+    def set(self, key: str, value: str):
         """set uses (k,v) as there exists valid meta names which are not kwarg safe"""
         if key.lower() in _http_equivs:
             self.data_struct["http-equiv"][key] = value
         elif key.lower() in _link_rels:
             self.data_struct["link"][key] = value
         else:
             self.data_struct["name"][key] = value
 
     def set_many(self, **kwargs):
-        """ set simply iterates over the **kwargs; here for legacy compatibility"""
+        """set simply iterates over the **kwargs; here for legacy compatibility"""
         for key, value in kwargs.items():
             self.set(key, value)
 
-    def get(self, key):
+    def get(self, key: str) -> Optional[str]:
         if key.lower() in _http_equivs:
             return self.data_struct["http-equiv"].get(key, None)
         elif key.lower() in _link_rels:
             return self.data_struct["link"].get(key, None)
         else:
             return self.data_struct["name"].get(key, None)
 
-    def unset(self, key):
+    def unset(self, key: str):
         if key.lower() in _http_equivs:
             if key in self.data_struct["http-equiv"]:
                 del self.data_struct["http-equiv"][key]
         elif key.lower() in _link_rels:
             if key in self.data_struct["link"]:
                 del self.data_struct["link"][key]
         else:
             if key in self.data_struct["name"]:
                 del self.data_struct["name"][key]
 
     # --------------------------------------------------------------------------
     # these are used for multile items.
     # sometimes you'll have several 'authors' in a link
 
-    def _hasmulti(self, section, key, value):
+    def _hasmulti(self, section: str, key: str, value: str) -> bool:
         if section in self.data_struct["_multi"]:
             if key in self.data_struct["_multi"][section]:
                 if value in self.data_struct["_multi"][section][key]:
                     return True
         return False
 
-    def _setmulti(self, section, key, value):
+    def _setmulti(self, section: str, key: str, value: str):
         if section not in self.data_struct["_multi"]:
             self.data_struct["_multi"][section] = {}
         if key not in self.data_struct["_multi"][section]:
             self.data_struct["_multi"][section][key] = []
         if not self._hasmulti(section, key, value):
             self.data_struct["_multi"][section][key].append(value)
 
-    def _unsetmulti(self, section, key, value):
+    def _unsetmulti(self, section: str, key: str, value: str):
         if self._hasmulti(section, key, value):
             self.data_struct["_multi"][section][key] = [
                 i for i in self.data_struct["_multi"][section][key] if i != value
             ]
 
-    def _clearmulti(self, section, key):
+    def _clearmulti(self, section: str, key: str):
         if section in self.data_struct["_multi"]:
             if key in self.data_struct["_multi"][section]:
                 del self.data_struct["_multi"][section][key]
 
-    def setmulti_link(self, key, value):
+    def setmulti_link(self, key: str, value: str):
         """sets a value for a non-unique key"""
         self._setmulti("link", key, value)
 
-    def unsetmulti_link(self, key, value):
+    def unsetmulti_link(self, key: str, value: str):
         """unsets a value for a non-unique key"""
         self._unsetmulti("link", key, value)
 
-    def clearmulti_link(self, key):
+    def clearmulti_link(self, key: str):
         """clears a value for a non-unique key"""
         self._clearmulti("link", key)
 
     # --------------------------------------------------------------------------
 
-    def as_html(self):
+    def as_html(self) -> str:
         """helper function. prints out metadata for you.
 
         You'd probably call it like this in a Mako template:
             <head>
                 ${meta.as_html()|n}
             </head>
 
         Notice that you have to escape under Mako.   For more information on mako escape options - http://www.makotemplates.org/docs/filtering.html
         """
         output = []
         _others = self.data_struct["other"].items()
         _equivs = self.data_struct["http-equiv"].items()
         _others_2 = []
         _equivs_2 = []
-        for (k, v) in _others:
+        for k, v in _others:
             if k.lower() == "charset":
                 output.append(
-                    u"""<meta %s="%s"/>"""
+                    """<meta %s="%s"/>"""
                     % (html_attribute_escape(k), html_attribute_escape(v))
                 )
             else:
                 _others_2.append((k, v))
-        for (k, v) in _equivs:
+        for k, v in _equivs:
             if "charset" in v.lower():
                 output.append(
-                    u"""<meta http-equiv="%s" content="%s"/>"""
+                    """<meta http-equiv="%s" content="%s"/>"""
                     % (html_attribute_escape(k), html_attribute_escape(v))
                 )
             else:
                 _equivs_2.append((k, v))
-        for (k, v) in _equivs_2:
+        for k, v in _equivs_2:
             output.append(
-                u"""<meta http-equiv="%s" content="%s"/>"""
+                """<meta http-equiv="%s" content="%s"/>"""
                 % (html_attribute_escape(k), html_attribute_escape(v))
             )
-        for (k, v) in self.data_struct["name"].items():
+        for k, v in self.data_struct["name"].items():
             output.append(
-                u"""<meta name="%s" content="%s"/>"""
+                """<meta name="%s" content="%s"/>"""
                 % (html_attribute_escape(k), html_attribute_escape(v))
             )
-        for (k, v) in _others_2:
+        for k, v in _others_2:
             output.append(
-                u"""<meta %s="%s"/>"""
+                """<meta %s="%s"/>"""
                 % (html_attribute_escape(k), html_attribute_escape(v))
             )
-        for (rel, v) in self.data_struct["link"].items():
+        for rel, v in self.data_struct["link"].items():
             output.append(
-                u"""<link rel="%s" href="%s"/>"""
+                """<link rel="%s" href="%s"/>"""
                 % (html_attribute_escape(rel), html_attribute_escape(v))
             )
         if self.data_struct["_multi"]:
             if "link" in self.data_struct["_multi"]:
                 for rel in self.data_struct["_multi"]["link"]:
                     for v in self.data_struct["_multi"]["link"][rel]:
                         output.append(
-                            u"""<link rel="%s" href="%s"/>"""
+                            """<link rel="%s" href="%s"/>"""
                             % (html_attribute_escape(rel), html_attribute_escape(v))
                         )
-        return u"\n".join(output)
+        return "\n".join(output)
```

### Comparing `htmlmeta_hub-0.4.1/src/htmlmeta_hub.egg-info/PKG-INFO` & `htmlmeta_hub-0.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,83 @@
 Metadata-Version: 2.1
-Name: htmlmeta-hub
-Version: 0.4.1
+Name: htmlmeta_hub
+Version: 0.5.0
 Summary: Lightweight support for managing metadata on webpages.
 Home-page: https://github.com/jvanasco/htmlmeta_hub
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT
-Description: htmlmeta_hub
-        ============
-        
-        Build Status: ![Python package](https://github.com/jvanasco/htmlmeta_hub/workflows/Python%20package/badge.svg)
-        
-        `htmlmeta_hub` offers lightweight support for managing metadata on webpages.
-        
-        This package simply and conveniently manages a dict of "metadata"", and renders
-        it appropriately.
-        
-        There are helpers for the Pyramid framework which will attach the metdata object
-        to a request, allowing you to build up metadata throughtout the request cycle
-        and then finally render.
-        
-        A typical way to use this package in the Pyramid framework:
-        
-        
-        Include this package in your application's  `__init__.py`:
-        
-        	def main(global_config, **settings):
-        		...
-        		# custom htmlmeta
-        		config.include("htmlmeta_hub.pyramid_helpers")
-        
-        
-        If you are using "class based views", you can set some default metadata in a core
-        handler:
-        
-        	class Handler(object):
-        		def __init__(self,request):
-        			self.request = request
-        			# set some defaults
-        			self.reqesut.htmlmeta.set_many(\
-        				title="MyApp",
-        				description="awesome",
-        				keywords="fun!",
-        			)
-        
-        and then you can add specific metadata in each view's handler:
-        
-        	class ContentPage(Handler):
-        		def view(self):
-        		    content= ...
-        			self.request.htmlmeta.set('title', content.title)
-        			self.request.htmlmeta.set('description', content.description)
-        
-        In a template, such as this `page.mako` example, you can access specific bits of
-        the metadata, or render an entire payload:
-        
-        	<title>${request.htmlmeta.get('title')|n}</title>
-        	${request.htmlmeta.as_html()|n}
-        
-        
-        Pyramid helpers existed until version `0.3.x` but were dropped in favor of the
-        `@reify` request method offered by the `config.include` method.
-        
-        Pylons helpers existed until version `0.1.2` but were dropped.
-        
-        
-        
 Keywords: metadata html web pyramid
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Pyramid
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE.txt
+
+htmlmeta_hub
+============
+
+Build Status: ![Python package](https://github.com/jvanasco/htmlmeta_hub/workflows/Python%20package/badge.svg)
+
+`htmlmeta_hub` offers lightweight support for managing metadata on webpages.
+
+This package simply and conveniently manages a dict of "metadata"", and renders
+it appropriately.
+
+There are helpers for the Pyramid framework which will attach the metdata object
+to a request, allowing you to build up metadata throughtout the request cycle
+and then finally render.
+
+A typical way to use this package in the Pyramid framework:
+
+
+Include this package in your application's  `__init__.py`:
+
+	def main(global_config, **settings):
+		...
+		# custom htmlmeta
+		config.include("htmlmeta_hub.pyramid_helpers")
+
+
+If you are using "class based views", you can set some default metadata in a core
+handler:
+
+	class Handler(object):
+		def __init__(self,request):
+			self.request = request
+			# set some defaults
+			self.reqesut.htmlmeta.set_many(\
+				title="MyApp",
+				description="awesome",
+				keywords="fun!",
+			)
+
+and then you can add specific metadata in each view's handler:
+
+	class ContentPage(Handler):
+		def view(self):
+		    content= ...
+			self.request.htmlmeta.set('title', content.title)
+			self.request.htmlmeta.set('description', content.description)
+
+In a template, such as this `page.mako` example, you can access specific bits of
+the metadata, or render an entire payload:
+
+	<title>${request.htmlmeta.get('title')|n}</title>
+	${request.htmlmeta.as_html()|n}
+
+
+Pyramid helpers existed until version `0.3.x` but were dropped in favor of the
+`@reify` request method offered by the `config.include` method.
+
+Pylons helpers existed until version `0.1.2` but were dropped.
+
+
```

### Comparing `htmlmeta_hub-0.4.1/tests/test_core.py` & `htmlmeta_hub-0.5.0/tests/test_core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # -*- coding: utf-8 -*-
 # stdlib
 import re
 import unittest
 
-# pypi
-import six
-
 # local package for testing
 import htmlmeta_hub
 
 
 # ==============================================================================
 
 # regexes to test against
@@ -22,60 +19,60 @@
 
 
 class TestCore(unittest.TestCase):
     def test_basic(self):
         a = htmlmeta_hub.HtmlMetaHub()
         a.set_http_equiv("refresh", "15")
         a.set_name("description", "awesome")
-        a.set_name("title", u"greeñ")  # test unicode values
+        a.set_name("title", "greeñ")  # test unicode values
         a.set("content-type", "text/html;charset=UTF-8")
         a.set_other("charset", "utf8")
         b = a.get("description")
         a.unset("description")
         b = a.as_html()
         self.assertEqual(
             b,
-            u"""<meta charset="utf8"/>
+            """<meta charset="utf8"/>
 <meta http-equiv="content-type" content="text/html;charset=UTF-8"/>
 <meta http-equiv="refresh" content="15"/>
 <meta name="title" content="greeñ"/>""",
         )
 
     def test_set_http_equiv_1(self):
         a = htmlmeta_hub.HtmlMetaHub()
         a.set_http_equiv("refresh", "15")
         b = a.as_html()
-        six.assertRegex(self, b, re_refresh_15)
+        self.assertRegex(b, re_refresh_15)
 
     def test_set_http_equiv_2(self):
         a = htmlmeta_hub.HtmlMetaHub()
         a.set("refresh", "15")
         b = a.as_html()
-        six.assertRegex(self, b, re_refresh_15)
+        self.assertRegex(b, re_refresh_15)
 
     def test_unset_http_equiv_2(self):
         a = htmlmeta_hub.HtmlMetaHub()
         a.set("refresh", "15")
         b = a.as_html()
-        six.assertRegex(self, b, re_refresh_15)
+        self.assertRegex(b, re_refresh_15)
         a.unset("refresh")
         b = a.as_html()
         self.assertNotRegexpMatches(b, re_refresh_15)
 
     def test_set_other(self):
         a = htmlmeta_hub.HtmlMetaHub()
         a.set_other("charset", "utf8")
         b = a.as_html()
-        six.assertRegex(self, b, re_other_charset)
+        self.assertRegex(b, re_other_charset)
 
     def test_set_link(self):
         a = htmlmeta_hub.HtmlMetaHub()
         a.set_link("canonical", "http://www.w3.org")
         b = a.as_html()
-        six.assertRegex(self, b, re_link)
+        self.assertRegex(b, re_link)
 
 
 class TestMulti(unittest.TestCase):
     def test_basic(self):
         a = htmlmeta_hub.HtmlMetaHub()
         a.setmulti_link("author", "Jonathan")
         a.setmulti_link("author", "Lindsey")
```

### Comparing `htmlmeta_hub-0.4.1/tests/test_pyramid_integration.py` & `htmlmeta_hub-0.5.0/tests/test_pyramid_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # -*- coding: utf-8 -*-
 # stdlib
-import re
 import unittest
 
-# pypi
-import six
-
 # pyramid testing requirements
 from pyramid import testing
 from pyramid.interfaces import IRequestExtensions
 
 # local package for testing
 import htmlmeta_hub
 import htmlmeta_hub.pyramid_helpers
```

