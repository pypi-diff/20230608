# Comparing `tmp/streamlit-disqus-darkmode-0.11.tar.gz` & `tmp/streamlit-disqus-darkmode-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-disqus-darkmode-0.11.tar", last modified: Thu Jun  8 16:55:57 2023, max compression
+gzip compressed data, was "streamlit-disqus-darkmode-0.12.tar", last modified: Thu Jun  8 16:59:28 2023, max compression
```

## Comparing `streamlit-disqus-darkmode-0.11.tar` & `streamlit-disqus-darkmode-0.12.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 16:55:57.904797 streamlit-disqus-darkmode-0.11/
--rw-rw-rw-   0        0        0     1093 2023-06-08 16:21:18.000000 streamlit-disqus-darkmode-0.11/LICENSE
--rw-rw-rw-   0        0        0       48 2023-06-08 16:21:18.000000 streamlit-disqus-darkmode-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     1272 2023-06-08 16:55:57.904797 streamlit-disqus-darkmode-0.11/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-06-08 16:49:46.000000 streamlit-disqus-darkmode-0.11/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 16:55:57.904797 streamlit-disqus-darkmode-0.11/setup.cfg
--rw-rw-rw-   0        0        0      654 2023-06-08 16:55:28.000000 streamlit-disqus-darkmode-0.11/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:55:57.890796 streamlit-disqus-darkmode-0.11/streamlit_disqus/
--rw-rw-rw-   0        0        0     1757 2023-06-08 16:49:26.000000 streamlit-disqus-darkmode-0.11/streamlit_disqus/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:55:57.903798 streamlit-disqus-darkmode-0.11/streamlit_disqus_darkmode.egg-info/
--rw-rw-rw-   0        0        0     1272 2023-06-08 16:55:57.000000 streamlit-disqus-darkmode-0.11/streamlit_disqus_darkmode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-06-08 16:55:57.000000 streamlit-disqus-darkmode-0.11/streamlit_disqus_darkmode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 16:55:57.000000 streamlit-disqus-darkmode-0.11/streamlit_disqus_darkmode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-08 16:55:57.000000 streamlit-disqus-darkmode-0.11/streamlit_disqus_darkmode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-08 16:55:57.000000 streamlit-disqus-darkmode-0.11/streamlit_disqus_darkmode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 16:59:28.437417 streamlit-disqus-darkmode-0.12/
+-rw-rw-rw-   0        0        0     1093 2023-06-08 16:21:18.000000 streamlit-disqus-darkmode-0.12/LICENSE
+-rw-rw-rw-   0        0        0       48 2023-06-08 16:21:18.000000 streamlit-disqus-darkmode-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     1272 2023-06-08 16:59:28.437417 streamlit-disqus-darkmode-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-06-08 16:49:46.000000 streamlit-disqus-darkmode-0.12/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-08 16:59:28.437417 streamlit-disqus-darkmode-0.12/setup.cfg
+-rw-rw-rw-   0        0        0      654 2023-06-08 16:59:09.000000 streamlit-disqus-darkmode-0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:59:28.418418 streamlit-disqus-darkmode-0.12/streamlit_disqus_darkmode/
+-rw-rw-rw-   0        0        0     1757 2023-06-08 16:49:26.000000 streamlit-disqus-darkmode-0.12/streamlit_disqus_darkmode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:59:28.435416 streamlit-disqus-darkmode-0.12/streamlit_disqus_darkmode.egg-info/
+-rw-rw-rw-   0        0        0     1272 2023-06-08 16:59:28.000000 streamlit-disqus-darkmode-0.12/streamlit_disqus_darkmode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-06-08 16:59:28.000000 streamlit-disqus-darkmode-0.12/streamlit_disqus_darkmode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 16:59:28.000000 streamlit-disqus-darkmode-0.12/streamlit_disqus_darkmode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-08 16:59:28.000000 streamlit-disqus-darkmode-0.12/streamlit_disqus_darkmode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-08 16:59:28.000000 streamlit-disqus-darkmode-0.12/streamlit_disqus_darkmode.egg-info/top_level.txt
```

### Comparing `streamlit-disqus-darkmode-0.11/LICENSE` & `streamlit-disqus-darkmode-0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-disqus-darkmode-0.11/PKG-INFO` & `streamlit-disqus-darkmode-0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-disqus-darkmode
-Version: 0.11
+Version: 0.12
 Summary: A streamlit component to embed Disqus in your applications.
 Home-page: https://github.com/leonfresh/streamlit-disqus-darkmode
 Author: leonfresh
 Author-email: 
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-disqus-darkmode-0.11/README.md` & `streamlit-disqus-darkmode-0.12/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-disqus-darkmode-0.11/setup.py` & `streamlit-disqus-darkmode-0.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 
 README = (Path(__file__).parent/"README.md").read_text()
 
 setuptools.setup(
     name="streamlit-disqus-darkmode",
-    version="0.11",
+    version="0.12",
     author="leonfresh",
     author_email="",
     description="A streamlit component to embed Disqus in your applications.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/leonfresh/streamlit-disqus-darkmode",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-disqus-darkmode-0.11/streamlit_disqus/__init__.py` & `streamlit-disqus-darkmode-0.12/streamlit_disqus_darkmode/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-disqus-darkmode-0.11/streamlit_disqus_darkmode.egg-info/PKG-INFO` & `streamlit-disqus-darkmode-0.12/streamlit_disqus_darkmode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-disqus-darkmode
-Version: 0.11
+Version: 0.12
 Summary: A streamlit component to embed Disqus in your applications.
 Home-page: https://github.com/leonfresh/streamlit-disqus-darkmode
 Author: leonfresh
 Author-email: 
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

