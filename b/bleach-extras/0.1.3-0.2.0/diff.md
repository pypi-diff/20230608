# Comparing `tmp/bleach_extras-0.1.3.tar.gz` & `tmp/bleach_extras-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bleach_extras-0.1.3.tar", last modified: Thu May 19 16:34:30 2022, max compression
+gzip compressed data, was "bleach_extras-0.2.0.tar", last modified: Thu Jun  8 18:51:49 2023, max compression
```

## Comparing `bleach_extras-0.1.3.tar` & `bleach_extras-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2022-05-19 16:34:30.811435 bleach_extras-0.1.3/
--rw-r--r--   0 jvanasco   (501) admin       (80)      689 2022-05-19 16:34:08.000000 bleach_extras-0.1.3/CHANGELOG.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     1487 2018-10-17 03:28:21.000000 bleach_extras-0.1.3/LICENSE
--rw-r--r--   0 jvanasco   (501) admin       (80)      181 2021-03-25 20:58:45.000000 bleach_extras-0.1.3/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)     5272 2022-05-19 16:34:30.811776 bleach_extras-0.1.3/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)     4642 2022-05-19 16:34:08.000000 bleach_extras-0.1.3/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)       48 2020-10-13 15:58:42.000000 bleach_extras-0.1.3/pyproject.toml
--rw-r--r--   0 jvanasco   (501) admin       (80)      365 2022-05-19 16:34:30.813552 bleach_extras-0.1.3/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     1827 2022-05-19 16:34:08.000000 bleach_extras-0.1.3/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2022-05-19 16:34:30.787489 bleach_extras-0.1.3/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2022-05-19 16:34:30.798260 bleach_extras-0.1.3/src/bleach_extras/
--rw-r--r--   0 jvanasco   (501) admin       (80)      522 2022-05-19 16:34:08.000000 bleach_extras-0.1.3/src/bleach_extras/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     6376 2021-12-02 19:32:39.000000 bleach_extras-0.1.3/src/bleach_extras/tag_tree_filter.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2022-05-19 16:34:30.805770 bleach_extras-0.1.3/src/bleach_extras.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)     5272 2022-05-19 16:34:30.000000 bleach_extras-0.1.3/src/bleach_extras.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)      416 2022-05-19 16:34:30.000000 bleach_extras-0.1.3/src/bleach_extras.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2022-05-19 16:34:30.000000 bleach_extras-0.1.3/src/bleach_extras.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 21:00:56.000000 bleach_extras-0.1.3/src/bleach_extras.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)       89 2022-05-19 16:34:30.000000 bleach_extras-0.1.3/src/bleach_extras.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       14 2022-05-19 16:34:30.000000 bleach_extras-0.1.3/src/bleach_extras.egg-info/top_level.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2022-05-19 16:34:30.806588 bleach_extras-0.1.3/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)    17453 2021-12-02 19:32:39.000000 bleach_extras-0.1.3/tests/test_clean.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      169 2022-05-19 16:34:08.000000 bleach_extras-0.1.3/tox.ini
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 18:51:49.413172 bleach_extras-0.2.0/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      739 2023-06-07 22:27:27.000000 bleach_extras-0.2.0/CHANGELOG.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1487 2018-10-17 03:28:21.000000 bleach_extras-0.2.0/LICENSE
+-rw-r--r--   0 jvanasco   (501) admin       (80)      181 2021-03-25 20:58:45.000000 bleach_extras-0.2.0/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)     5477 2023-06-08 18:51:49.413510 bleach_extras-0.2.0/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     4642 2022-05-19 16:34:08.000000 bleach_extras-0.2.0/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)       40 2023-06-07 22:24:46.000000 bleach_extras-0.2.0/pyproject.toml
+-rw-r--r--   0 jvanasco   (501) admin       (80)      365 2023-06-08 18:51:49.415276 bleach_extras-0.2.0/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2082 2023-06-08 18:50:47.000000 bleach_extras-0.2.0/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 18:51:49.389130 bleach_extras-0.2.0/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 18:51:49.401618 bleach_extras-0.2.0/src/bleach_extras/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      522 2023-06-07 22:27:32.000000 bleach_extras-0.2.0/src/bleach_extras/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     7338 2023-06-08 18:11:06.000000 bleach_extras-0.2.0/src/bleach_extras/tag_tree_filter.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 18:51:49.410063 bleach_extras-0.2.0/src/bleach_extras.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     5477 2023-06-08 18:51:49.000000 bleach_extras-0.2.0/src/bleach_extras.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)      416 2023-06-08 18:51:49.000000 bleach_extras-0.2.0/src/bleach_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-08 18:51:49.000000 bleach_extras-0.2.0/src/bleach_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 21:00:56.000000 bleach_extras-0.2.0/src/bleach_extras.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)      109 2023-06-08 18:51:49.000000 bleach_extras-0.2.0/src/bleach_extras.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       14 2023-06-08 18:51:49.000000 bleach_extras-0.2.0/src/bleach_extras.egg-info/top_level.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 18:51:49.411479 bleach_extras-0.2.0/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)    17453 2021-12-02 19:32:39.000000 bleach_extras-0.2.0/tests/test_clean.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      175 2023-06-08 18:16:02.000000 bleach_extras-0.2.0/tox.ini
```

### Comparing `bleach_extras-0.1.3/CHANGELOG.txt` & `bleach_extras-0.2.0/CHANGELOG.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.2.0 | 20230608
+    - drop python 2.6
+    - mpy
+
 0.1.3 | 20220519
 	- version pinning against bleach <5 because of incompatibilities
 	- adjusted github test matrix
 
 0.1.2 | 20210325
 	- packaging fix
```

### Comparing `bleach_extras-0.1.3/LICENSE` & `bleach_extras-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bleach_extras-0.1.3/PKG-INFO` & `bleach_extras-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: bleach_extras
-Version: 0.1.3
-Summary: some extensions for bleach
-Home-page: http://github.com/jvanasco/bleach_extras
-Author: Jonathan Vanasco
-Author-email: jonathan@findmeon.com
-License: MIT License
-Keywords: bleach html-sanitizing
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
 ![Python package](https://github.com/jvanasco/bleach_extras/workflows/Python%20package/badge.svg)
 
 `bleach_extras` is a package of *unofficial* "extras" and utilities paired for
 use with the `bleach` library.
 
 The first utility is `TagTreeFilter` which is utilized by `clean_strip_content`
 and `cleaner_factory__strip_content`.
@@ -116,9 +97,7 @@
 	class IFrameFilter2(bleach_extras.TagTreeFilter):
 		tags_strip_content = ('script', 'style', 'iframe')
 		tag_replace_string = "&lt;unsafe garbage/&gt;"
 
 	print bleach_extras.clean_strip_content(dangerous2, tags=['div', ], filters=[IFrameFilter2, ])
 	# foo.<div>1&amp;lt;unsafe garbage/&amp;gt;2</div>.bar
 
-
-
```

#### html2text {}

```diff
@@ -1,26 +1,18 @@
-Metadata-Version: 2.1 Name: bleach_extras Version: 0.1.3 Summary: some
-extensions for bleach Home-page: http://github.com/jvanasco/bleach_extras
-Author: Jonathan Vanasco Author-email: jonathan@findmeon.com License: MIT
-License Keywords: bleach html-sanitizing Platform: UNKNOWN Classifier: License
-:: OSI Approved :: MIT License Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Intended Audience
-:: Developers Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*,
-!=3.4.*, !=3.5.* Description-Content-Type: text/markdown Provides-Extra:
-testing License-File: LICENSE ![Python package](https://github.com/jvanasco/
-bleach_extras/workflows/Python%20package/badge.svg) `bleach_extras` is a
-package of *unofficial* "extras" and utilities paired for use with the `bleach`
-library. The first utility is `TagTreeFilter` which is utilized by
-`clean_strip_content` and `cleaner_factory__strip_content`. # Compatability
-`bleach_extras` currently requires `bleach>=3.2.1` and `bleach<5`. Earlier
-versions of `bleach` have security concerns; latter versions are not compatible
-due to API changes (future support is planned). # `TagTreeFilter`,
-`clean_strip_content`, `cleaner_factory__strip_content` `clean_strip_content`
-is paired to `bleach.clean`; the only intended difference is to support the
-concept of stripping the content tree of tags -- not just the tagÂ node itself.
+![Python package](https://github.com/jvanasco/bleach_extras/workflows/
+Python%20package/badge.svg) `bleach_extras` is a package of *unofficial*
+"extras" and utilities paired for use with the `bleach` library. The first
+utility is `TagTreeFilter` which is utilized by `clean_strip_content` and
+`cleaner_factory__strip_content`. # Compatability `bleach_extras` currently
+requires `bleach>=3.2.1` and `bleach<5`. Earlier versions of `bleach` have
+security concerns; latter versions are not compatible due to API changes
+(future support is planned). # `TagTreeFilter`, `clean_strip_content`,
+`cleaner_factory__strip_content` `clean_strip_content` is paired to
+`bleach.clean`; the only intended difference is to support the concept of
+stripping the content tree of tags -- not just the tagÂ node itself.
 `cleaner_factory__strip_content` is a factory function used to create
 configured `bleach.Cleaner` instances. `bleach` has a `strip` flag that toggles
 the behavior of "unsafe" tags: `strip = False` will render the tags as escaped
 HTML encodings, such as this replacement: - foo.
 1
 2
 .bar + foo.
```

### Comparing `bleach_extras-0.1.3/README.md` & `bleach_extras-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: bleach_extras
+Version: 0.2.0
+Summary: some extensions for bleach
+Home-page: http://github.com/jvanasco/bleach_extras
+Author: Jonathan Vanasco
+Author-email: jonathan@findmeon.com
+License: MIT License
+Keywords: bleach html-sanitizing
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Developers
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE
+
 ![Python package](https://github.com/jvanasco/bleach_extras/workflows/Python%20package/badge.svg)
 
 `bleach_extras` is a package of *unofficial* "extras" and utilities paired for
 use with the `bleach` library.
 
 The first utility is `TagTreeFilter` which is utilized by `clean_strip_content`
 and `cleaner_factory__strip_content`.
```

#### html2text {}

```diff
@@ -1,8 +1,19 @@
-![Python package](https://github.com/jvanasco/bleach_extras/workflows/
+Metadata-Version: 2.1 Name: bleach_extras Version: 0.2.0 Summary: some
+extensions for bleach Home-page: http://github.com/jvanasco/bleach_extras
+Author: Jonathan Vanasco Author-email: jonathan@findmeon.com License: MIT
+License Keywords: bleach html-sanitizing Classifier: License :: OSI Approved ::
+MIT License Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Intended Audience :: Developers
+Description-Content-Type: text/markdown Provides-Extra: testing License-File:
+LICENSE ![Python package](https://github.com/jvanasco/bleach_extras/workflows/
 Python%20package/badge.svg) `bleach_extras` is a package of *unofficial*
 "extras" and utilities paired for use with the `bleach` library. The first
 utility is `TagTreeFilter` which is utilized by `clean_strip_content` and
 `cleaner_factory__strip_content`. # Compatability `bleach_extras` currently
 requires `bleach>=3.2.1` and `bleach<5`. Earlier versions of `bleach` have
 security concerns; latter versions are not compatible due to API changes
 (future support is planned). # `TagTreeFilter`, `clean_strip_content`,
```

### Comparing `bleach_extras-0.1.3/setup.py` & `bleach_extras-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 tests_require = ["pytest>=3.0.0"]
 testing_extras = (
     install_requires
     + tests_require
     + [
         "pytest-wholenodeid",
         "flake8",
+        "mypy",
         "tox",
+        "types-bleach<5",
     ]
 )
 
 
 def get_version():
     fn = os.path.join("src", "bleach_extras", "__init__.py")
     vsre = r"""^__version__ = ['"]([^'"]*)['"]"""
@@ -49,20 +51,25 @@
     keywords="bleach html-sanitizing",
     test_suite="tests",
     packages=find_packages(
         where="src",
     ),
     package_dir={"": "src"},
     include_package_data=True,
-    python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*",
     install_requires=install_requires,
     tests_require=tests_require,
     extras_require={
         "testing": testing_extras,
     },
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Intended Audience :: Developers",
     ],
 )
```

### Comparing `bleach_extras-0.1.3/src/bleach_extras/__init__.py` & `bleach_extras-0.2.0/src/bleach_extras/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 from .tag_tree_filter import TAG_TREE_TAGS  # noqa: F401
 from .tag_tree_filter import TagTreeFilter  # noqa: F401
 
 # ==============================================================================
 
 
 # yyyymmdd
-__releasedate__ = "20220519"
+__releasedate__ = "20230608"
 # x.y.z or x.y.z.dev0 -- semver
-__version__ = "0.1.3"
+__version__ = "0.2.0"
 VERSION = parse_version(__version__)
```

### Comparing `bleach_extras-0.1.3/src/bleach_extras/tag_tree_filter.py` & `bleach_extras-0.2.0/src/bleach_extras/tag_tree_filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,24 @@
+# stdlib
+from typing import Any
+from typing import Callable
+from typing import Container
+from typing import Dict
+from typing import Iterable
+from typing import List
+from typing import Optional
+from typing import Union
+
+# pypi
 from bleach.html5lib_shim import Filter
 from bleach.sanitizer import ALLOWED_ATTRIBUTES
 from bleach.sanitizer import ALLOWED_PROTOCOLS
-from bleach.sanitizer import ALLOWED_STYLES
+from bleach.sanitizer import ALLOWED_STYLES  # type: ignore[attr-defined]  # stubs are 5+
 from bleach.sanitizer import ALLOWED_TAGS
 from bleach.sanitizer import Cleaner
-from six import text_type
 
 
 # ==============================================================================
 
 
 TAG_TREE_TAGS = ("script", "style")
 
@@ -28,33 +38,36 @@
     tags_strip_content = TAG_TREE_TAGS
     _tags_strip_content = None  # memoized on __init__
 
     "if defined in a subclass, a string to replace the content with."
     tag_replace_string = None
     _tag_replace = None  # memoized on __init__
 
-    def __init__(self, source):
+    def __init__(
+        self,
+        source: Any,
+    ):
         """
         Creates a TagTreeFilter instance.
 
         This instance will strip the tag and the content tree of tags appearing
         in ``tags_strip_content``.
 
-        :arg Treewalker source: stream
+        :arg source: the source token stream
         """
         if not self.tags_strip_content:
             raise ValueError("must have `tags_strip_content` on the class")
         self._tags_strip_content = [t.lower() for t in self.tags_strip_content]
         if self.tag_replace_string is not None:
             self._tag_replace = {
-                "data": text_type(self.tag_replace_string),
+                "data": self.tag_replace_string,
                 "type": "Characters",
             }
         self._in_strip_content = 0
-        return super(TagTreeFilter, self).__init__(source)
+        return super(TagTreeFilter, self).__init__(source)  # type: ignore[call-arg]  # stubs are 5+
 
     def __iter__(self):
         for token in Filter.__iter__(self):
             _name = token.get("name", "").lower()
             if _name in self._tags_strip_content:
                 if token.get("type") == "StartTag":
                     self._in_strip_content += 1
@@ -66,23 +79,29 @@
                     if self._in_strip_content:
                         yield self._tag_replace
                 continue
             yield token
 
 
 def clean_strip_content(
-    text,
-    tags=ALLOWED_TAGS,
-    attributes=ALLOWED_ATTRIBUTES,
-    styles=ALLOWED_STYLES,
-    protocols=ALLOWED_PROTOCOLS,
-    strip=False,
-    strip_comments=True,
-    filters=None,
-):
+    text: str,
+    tags: Iterable[str] = ALLOWED_TAGS,
+    attributes: Union[
+        Callable[[str, str, str], bool],
+        Dict[str, Union[List[str], Callable[[str, str, str], bool]]],
+        Dict[str, List[str]],
+        Dict[str, Callable[[str, str, str], bool]],
+        List[str],
+    ] = ALLOWED_ATTRIBUTES,
+    styles: Container[str] = ALLOWED_STYLES,
+    protocols: Container[str] = ALLOWED_PROTOCOLS,
+    strip: bool = False,
+    strip_comments: bool = True,
+    filters: Optional[Any] = None,
+) -> str:
     """
     Clean an HTML fragment of malicious content and return it
 
     This function is paired to `bleach.clean` and the only intended difference
     is to support the concept of stripping the content of tags, and not just the
     tag itself.
 
@@ -139,22 +158,28 @@
         strip_comments=strip_comments,
         filters=filters,
     )
     return cleaner.clean(text)
 
 
 def cleaner_factory__strip_content(
-    tags=ALLOWED_TAGS,
-    attributes=ALLOWED_ATTRIBUTES,
-    styles=ALLOWED_STYLES,
-    protocols=ALLOWED_PROTOCOLS,
-    strip=False,
-    strip_comments=True,
-    filters=None,
-):
+    tags: Iterable[str] = ALLOWED_TAGS,
+    attributes: Union[
+        Callable[[str, str, str], bool],
+        Dict[str, Union[List[str], Callable[[str, str, str], bool]]],
+        Dict[str, List[str]],
+        Dict[str, Callable[[str, str, str], bool]],
+        List[str],
+    ] = ALLOWED_ATTRIBUTES,
+    styles: Container[str] = ALLOWED_STYLES,
+    protocols: Container[str] = ALLOWED_PROTOCOLS,
+    strip: bool = False,
+    strip_comments: bool = True,
+    filters: Optional[Any] = None,
+) -> Cleaner:
     """
     Factory for building a ``bleach.Cleaner`` instance designed to
     strip content.
 
     The accepts the same arguments as ``clean_strip_content`` except for the
     initial `text` argument.
```

### Comparing `bleach_extras-0.1.3/src/bleach_extras.egg-info/PKG-INFO` & `bleach_extras-0.2.0/src/bleach_extras.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: bleach-extras
-Version: 0.1.3
+Version: 0.2.0
 Summary: some extensions for bleach
 Home-page: http://github.com/jvanasco/bleach_extras
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT License
 Keywords: bleach html-sanitizing
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 ![Python package](https://github.com/jvanasco/bleach_extras/workflows/Python%20package/badge.svg)
 
 `bleach_extras` is a package of *unofficial* "extras" and utilities paired for
@@ -116,9 +120,7 @@
 	class IFrameFilter2(bleach_extras.TagTreeFilter):
 		tags_strip_content = ('script', 'style', 'iframe')
 		tag_replace_string = "&lt;unsafe garbage/&gt;"
 
 	print bleach_extras.clean_strip_content(dangerous2, tags=['div', ], filters=[IFrameFilter2, ])
 	# foo.<div>1&amp;lt;unsafe garbage/&amp;gt;2</div>.bar
 
-
-
```

#### html2text {}

```diff
@@ -1,26 +1,29 @@
-Metadata-Version: 2.1 Name: bleach-extras Version: 0.1.3 Summary: some
+Metadata-Version: 2.1 Name: bleach-extras Version: 0.2.0 Summary: some
 extensions for bleach Home-page: http://github.com/jvanasco/bleach_extras
 Author: Jonathan Vanasco Author-email: jonathan@findmeon.com License: MIT
-License Keywords: bleach html-sanitizing Platform: UNKNOWN Classifier: License
-:: OSI Approved :: MIT License Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Intended Audience
-:: Developers Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*,
-!=3.4.*, !=3.5.* Description-Content-Type: text/markdown Provides-Extra:
-testing License-File: LICENSE ![Python package](https://github.com/jvanasco/
-bleach_extras/workflows/Python%20package/badge.svg) `bleach_extras` is a
-package of *unofficial* "extras" and utilities paired for use with the `bleach`
-library. The first utility is `TagTreeFilter` which is utilized by
-`clean_strip_content` and `cleaner_factory__strip_content`. # Compatability
-`bleach_extras` currently requires `bleach>=3.2.1` and `bleach<5`. Earlier
-versions of `bleach` have security concerns; latter versions are not compatible
-due to API changes (future support is planned). # `TagTreeFilter`,
-`clean_strip_content`, `cleaner_factory__strip_content` `clean_strip_content`
-is paired to `bleach.clean`; the only intended difference is to support the
-concept of stripping the content tree of tags -- not just the tagÂ node itself.
+License Keywords: bleach html-sanitizing Classifier: License :: OSI Approved ::
+MIT License Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Intended Audience :: Developers
+Description-Content-Type: text/markdown Provides-Extra: testing License-File:
+LICENSE ![Python package](https://github.com/jvanasco/bleach_extras/workflows/
+Python%20package/badge.svg) `bleach_extras` is a package of *unofficial*
+"extras" and utilities paired for use with the `bleach` library. The first
+utility is `TagTreeFilter` which is utilized by `clean_strip_content` and
+`cleaner_factory__strip_content`. # Compatability `bleach_extras` currently
+requires `bleach>=3.2.1` and `bleach<5`. Earlier versions of `bleach` have
+security concerns; latter versions are not compatible due to API changes
+(future support is planned). # `TagTreeFilter`, `clean_strip_content`,
+`cleaner_factory__strip_content` `clean_strip_content` is paired to
+`bleach.clean`; the only intended difference is to support the concept of
+stripping the content tree of tags -- not just the tagÂ node itself.
 `cleaner_factory__strip_content` is a factory function used to create
 configured `bleach.Cleaner` instances. `bleach` has a `strip` flag that toggles
 the behavior of "unsafe" tags: `strip = False` will render the tags as escaped
 HTML encodings, such as this replacement: - foo.
 1
 2
 .bar + foo.
```

### Comparing `bleach_extras-0.1.3/tests/test_clean.py` & `bleach_extras-0.2.0/tests/test_clean.py`

 * *Files identical despite different names*

