# Comparing `tmp/openepd-0.8.0.tar.gz` & `tmp/openepd-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-0.8.0.tar", max compression
+gzip compressed data, was "openepd-0.8.1.tar", max compression
```

## Comparing `openepd-0.8.0.tar` & `openepd-0.8.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-06-08 16:40:32.104392 openepd-0.8.0/LICENSE
--rw-r--r--   0        0        0     2841 2023-06-08 16:40:32.104392 openepd-0.8.0/README.md
--rw-r--r--   0        0        0     3051 2023-06-08 16:40:32.104392 openepd-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      837 2023-06-08 16:40:32.104392 openepd-0.8.0/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2023-06-08 16:40:32.104392 openepd-0.8.0/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2023-06-08 16:40:32.104392 openepd-0.8.0/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     2841 2023-06-08 16:40:32.104392 openepd-0.8.0/src/openepd/model/base.py
--rw-r--r--   0        0        0     4512 2023-06-08 16:40:32.104392 openepd-0.8.0/src/openepd/model/common.py
--rw-r--r--   0        0        0    12291 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/model/epd.py
--rw-r--r--   0        0        0    11551 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     3813 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/model/org.py
--rw-r--r--   0        0        0     2889 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/model/pcr.py
--rw-r--r--   0        0        0     1137 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/model/specs/__init__.py
--rw-r--r--   0        0        0     3342 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/model/specs/concrete.py
--rw-r--r--   0        0        0     1519 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/model/standard.py
--rw-r--r--   0        0        0        0 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/py.typed
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-08 17:16:28.921051 openepd-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2841 2023-06-08 17:16:28.921051 openepd-0.8.1/README.md
+-rw-r--r--   0        0        0     3051 2023-06-08 17:16:28.921051 openepd-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-06-08 17:16:28.921051 openepd-0.8.1/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2023-06-08 17:16:28.921051 openepd-0.8.1/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2023-06-08 17:16:28.921051 openepd-0.8.1/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     2841 2023-06-08 17:16:28.921051 openepd-0.8.1/src/openepd/model/base.py
+-rw-r--r--   0        0        0     4545 2023-06-08 17:16:28.921051 openepd-0.8.1/src/openepd/model/common.py
+-rw-r--r--   0        0        0    12291 2023-06-08 17:16:28.921051 openepd-0.8.1/src/openepd/model/epd.py
+-rw-r--r--   0        0        0    11551 2023-06-08 17:16:28.921051 openepd-0.8.1/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     3813 2023-06-08 17:16:28.921051 openepd-0.8.1/src/openepd/model/org.py
+-rw-r--r--   0        0        0     2889 2023-06-08 17:16:28.921051 openepd-0.8.1/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0     1137 2023-06-08 17:16:28.921051 openepd-0.8.1/src/openepd/model/specs/__init__.py
+-rw-r--r--   0        0        0     3342 2023-06-08 17:16:28.921051 openepd-0.8.1/src/openepd/model/specs/concrete.py
+-rw-r--r--   0        0        0     1519 2023-06-08 17:16:28.921051 openepd-0.8.1/src/openepd/model/standard.py
+-rw-r--r--   0        0        0        0 2023-06-08 17:16:28.921051 openepd-0.8.1/src/openepd/py.typed
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.8.1/PKG-INFO
```

### Comparing `openepd-0.8.0/LICENSE` & `openepd-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-0.8.0/README.md` & `openepd-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `openepd-0.8.0/pyproject.toml` & `openepd-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openepd"
-version = "0.8.0"
+version = "0.8.1"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <support@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
@@ -52,15 +52,15 @@
 types-deprecated = ">=1.2.9"
 
 [tool.poetry.extras]
 #xml = ["lxml"]
 
 
 [tool.commitizen]
-version = "0.8.0"
+version = "0.8.1"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/openepd/__version__.py",
 ]
```

### Comparing `openepd-0.8.0/src/openepd/__init__.py` & `openepd-0.8.1/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.8.0/src/openepd/__version__.py` & `openepd-0.8.1/src/openepd/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.8.0"
+VERSION = "0.8.1"
```

### Comparing `openepd-0.8.0/src/openepd/model/__init__.py` & `openepd-0.8.1/src/openepd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.8.0/src/openepd/model/base.py` & `openepd-0.8.1/src/openepd/model/base.py`

 * *Files identical despite different names*

### Comparing `openepd-0.8.0/src/openepd/model/common.py` & `openepd-0.8.1/src/openepd/model/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from typing import Annotated, Any
 
 import pydantic as pyd
-from pydantic import root_validator
+from pydantic import BaseModel, root_validator
 
 from openepd.model.base import BaseOpenEpdSchema
 
 
 class Amount(BaseOpenEpdSchema):
     """A value-and-unit pairing for amounts that do not have an uncertainty."""
 
@@ -69,15 +69,15 @@
     link: pyd.AnyUrl | None = pyd.Field(
         description="Link to this object's OpenEPD declaration. "
         "An OpenIndustryEPD or OpenLCI link is also acceptable.",
         default=None,
     )
 
 
-class WithAttachmentsMixin:
+class WithAttachmentsMixin(BaseModel):
     """Mixin for objects that can have attachments."""
 
     attachments: dict[Annotated[str, pyd.Field(max_length=200)], pyd.AnyUrl] | None = pyd.Field(
         description="Dict of URLs relevant to this entry",
         example={
             "Contact Us": "https://www.c-change-labs.com/en/contact-us/",
             "LinkedIn": "https://www.linkedin.com/company/c-change-labs/",
@@ -93,15 +93,15 @@
 
     def set_attachment_if_any(self, name: str, url: str | None):
         """Set an attachment if url is not None."""
         if url is not None:
             self.set_attachment(name, url)
 
 
-class WithAltIdsMixin:
+class WithAltIdsMixin(BaseModel):
     """Mixin for objects that can have alt_ids."""
 
     alt_ids: dict[Annotated[str, pyd.Field(max_length=200)], str] | None = pyd.Field(
         description="Dict identifiers for this entry.",
         example={
             "oekobau.dat": "bdda4364-451f-4df2-a68b-5912469ee4c9",
         },
```

### Comparing `openepd-0.8.0/src/openepd/model/epd.py` & `openepd-0.8.1/src/openepd/model/epd.py`

 * *Files identical despite different names*

### Comparing `openepd-0.8.0/src/openepd/model/lcia.py` & `openepd-0.8.1/src/openepd/model/lcia.py`

 * *Files identical despite different names*

### Comparing `openepd-0.8.0/src/openepd/model/org.py` & `openepd-0.8.1/src/openepd/model/org.py`

 * *Files identical despite different names*

### Comparing `openepd-0.8.0/src/openepd/model/pcr.py` & `openepd-0.8.1/src/openepd/model/pcr.py`

 * *Files identical despite different names*

### Comparing `openepd-0.8.0/src/openepd/model/specs/__init__.py` & `openepd-0.8.1/src/openepd/model/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.8.0/src/openepd/model/specs/concrete.py` & `openepd-0.8.1/src/openepd/model/specs/concrete.py`

 * *Files identical despite different names*

### Comparing `openepd-0.8.0/src/openepd/model/standard.py` & `openepd-0.8.1/src/openepd/model/standard.py`

 * *Files identical despite different names*

### Comparing `openepd-0.8.0/PKG-INFO` & `openepd-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python library to work with OpenEPD format
 Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: support@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openepd Version: 0.8.0 Summary: Python library to
+Metadata-Version: 2.1 Name: openepd Version: 0.8.1 Summary: Python library to
 work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: support@c-change-labs.com
 Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

