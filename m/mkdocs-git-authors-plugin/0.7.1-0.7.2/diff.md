# Comparing `tmp/mkdocs-git-authors-plugin-0.7.1.tar.gz` & `tmp/mkdocs-git-authors-plugin-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-git-authors-plugin-0.7.1.tar", last modified: Mon May 22 18:11:49 2023, max compression
+gzip compressed data, was "mkdocs-git-authors-plugin-0.7.2.tar", last modified: Thu Jun  8 18:15:48 2023, max compression
```

## Comparing `mkdocs-git-authors-plugin-0.7.1.tar` & `mkdocs-git-authors-plugin-0.7.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:11:49.851965 mkdocs-git-authors-plugin-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-22 18:11:49.851965 mkdocs-git-authors-plugin-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:11:49.851965 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/exclude.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:11:49.851965 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/author.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:11:49.851965 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-22 18:11:49.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-22 18:11:49.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:11:49.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-22 18:11:49.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 18:11:49.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 18:11:49.000000 mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 18:11:49.851965 mkdocs-git-authors-plugin-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-22 18:11:23.000000 mkdocs-git-authors-plugin-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:48.586541 mkdocs-git-authors-plugin-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-08 18:15:19.000000 mkdocs-git-authors-plugin-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-08 18:15:48.586541 mkdocs-git-authors-plugin-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-08 18:15:19.000000 mkdocs-git-authors-plugin-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:48.582541 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:19.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-08 18:15:19.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-08 18:15:19.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/exclude.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:48.586541 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:19.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-08 18:15:19.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/git/author.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-08 18:15:19.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/git/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-08 18:15:19.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-08 18:15:19.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/git/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-08 18:15:19.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/git/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-06-08 18:15:19.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-08 18:15:19.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:48.586541 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-08 18:15:48.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-08 18:15:48.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:15:48.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 18:15:48.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 18:15:48.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 18:15:48.000000 mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:15:48.586541 mkdocs-git-authors-plugin-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-08 18:15:19.000000 mkdocs-git-authors-plugin-0.7.2/setup.py
```

### Comparing `mkdocs-git-authors-plugin-0.7.1/LICENSE` & `mkdocs-git-authors-plugin-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.7.1/PKG-INFO` & `mkdocs-git-authors-plugin-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-git-authors-plugin
-Version: 0.7.1
+Version: 0.7.2
 Summary: Mkdocs plugin to display git authors of a page
 Home-page: https://github.com/timvink/mkdocs-git-authors-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs git contributors committers authors plugin
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocs-git-authors-plugin-0.7.1/README.md` & `mkdocs-git-authors-plugin-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/ci.py` & `mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/ci.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/exclude.py` & `mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/exclude.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/author.py` & `mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/git/author.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/command.py` & `mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/git/command.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/commit.py` & `mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/git/commit.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/page.py` & `mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/git/page.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,34 +14,42 @@
     Results of git blame for a given file.
 
     Stores a list of tuples with a reference to a
     Commit object and a list of consecutive lines
     modified by that commit.
     """
 
-    def __init__(self, repo: Repo, path: Path):
+    def __init__(self, repo: Repo, path: Path, strict: bool):
         """
         Instantiate a Page object
 
         Args:
             repo: Reference to the global Repo instance
             path: Absolute path to the page's Markdown file
         """
         super().__init__(repo)
         self._path = path
         self._sorted = False
         self._total_lines = 0
         self._authors: List[dict] = list()
+        self._strict = strict
+        
         try:
             self._process_git_blame()
         except GitCommandError:
-            logger.warning(
-                "[git-authors-plugin] %s has not been committed yet. Lines are not counted"
-                % path
-            )
+            if self._strict:
+                logger.warning(
+                    "[git-authors-plugin] %s has not been committed yet. Lines are not counted"
+                    % path
+                )
+            else:
+                logger.info(
+                    "[git-authors-plugin] %s has not been committed yet. Lines are not counted"
+                    % path
+                )
 
     def add_total_lines(self, cnt: int = 1):
         """
         Add line(s) to the count of total lines for the page.
 
         Arg:
             cnt: number of lines to add. Default: 1
```

### Comparing `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/git/repo.py` & `mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/git/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
             Page object
         """
         if type(path) == str:
             path = Path(path)
         if not self._pages.get(path):
             from .page import Page
 
-            self._pages[path] = Page(self, path)
+            self._pages[path] = Page(self, path, self.config("strict"))
         return self._pages[path]
 
     def set_config(self, plugin_config):
         """
         Store the plugin configuration in the Repo instance.
 
         Args:
```

### Comparing `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/plugin.py` & `mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         ("show_email_address", config_options.Type(bool, default=True)),
         ("count_empty_lines", config_options.Type(bool, default=True)),
         ("fallback_to_empty", config_options.Type(bool, default=False)),
         ("exclude", config_options.Type(list, default=[])),
         ("enabled", config_options.Type(bool, default=True)),
         ("sort_authors_by", config_options.Type(str, default="name")),
         ("authorship_threshold_percent", config_options.Type(int, default=0)),
+        ("strict", config_options.Type(bool, default=True)),
         # ('sort_authors_by_name', config_options.Type(bool, default=True)),
         # ('sort_reverse', config_options.Type(bool, default=False))
     )
 
     def __init__(self):
         self._repo = None
         self._fallback = False
```

### Comparing `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin/util.py` & `mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/PKG-INFO` & `mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-git-authors-plugin
-Version: 0.7.1
+Version: 0.7.2
 Summary: Mkdocs plugin to display git authors of a page
 Home-page: https://github.com/timvink/mkdocs-git-authors-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs git contributors committers authors plugin
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocs-git-authors-plugin-0.7.1/mkdocs_git_authors_plugin.egg-info/SOURCES.txt` & `mkdocs-git-authors-plugin-0.7.2/mkdocs_git_authors_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-git-authors-plugin-0.7.1/setup.py` & `mkdocs-git-authors-plugin-0.7.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mkdocs-git-authors-plugin",
-    version="0.7.1",
+    version="0.7.2",
     description="Mkdocs plugin to display git authors of a page",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs git contributors committers authors plugin",
     url="https://github.com/timvink/mkdocs-git-authors-plugin",
     author="Tim Vink",
     author_email="vinktim@gmail.com",
```

