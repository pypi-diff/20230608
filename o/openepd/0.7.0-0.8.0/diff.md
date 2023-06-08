# Comparing `tmp/openepd-0.7.0.tar.gz` & `tmp/openepd-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-0.7.0.tar", max compression
+gzip compressed data, was "openepd-0.8.0.tar", max compression
```

## Comparing `openepd-0.7.0.tar` & `openepd-0.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-06-07 09:51:04.050774 openepd-0.7.0/LICENSE
--rw-r--r--   0        0        0     2841 2023-06-07 09:51:04.050774 openepd-0.7.0/README.md
--rw-r--r--   0        0        0     3051 2023-06-07 09:51:04.050774 openepd-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      837 2023-06-07 09:51:04.050774 openepd-0.7.0/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2023-06-07 09:51:04.050774 openepd-0.7.0/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2023-06-07 09:51:04.050774 openepd-0.7.0/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     2613 2023-06-07 09:51:04.050774 openepd-0.7.0/src/openepd/model/base.py
--rw-r--r--   0        0        0     3365 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/common.py
--rw-r--r--   0        0        0    12201 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/epd.py
--rw-r--r--   0        0        0    11266 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     3811 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/org.py
--rw-r--r--   0        0        0     2855 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/pcr.py
--rw-r--r--   0        0        0     1137 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/specs/__init__.py
--rw-r--r--   0        0        0     3342 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/specs/concrete.py
--rw-r--r--   0        0        0     1519 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/model/standard.py
--rw-r--r--   0        0        0        0 2023-06-07 09:51:04.054774 openepd-0.7.0/src/openepd/py.typed
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-08 16:40:32.104392 openepd-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2841 2023-06-08 16:40:32.104392 openepd-0.8.0/README.md
+-rw-r--r--   0        0        0     3051 2023-06-08 16:40:32.104392 openepd-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-06-08 16:40:32.104392 openepd-0.8.0/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2023-06-08 16:40:32.104392 openepd-0.8.0/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2023-06-08 16:40:32.104392 openepd-0.8.0/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     2841 2023-06-08 16:40:32.104392 openepd-0.8.0/src/openepd/model/base.py
+-rw-r--r--   0        0        0     4512 2023-06-08 16:40:32.104392 openepd-0.8.0/src/openepd/model/common.py
+-rw-r--r--   0        0        0    12291 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/model/epd.py
+-rw-r--r--   0        0        0    11551 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     3813 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/model/org.py
+-rw-r--r--   0        0        0     2889 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0     1137 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/model/specs/__init__.py
+-rw-r--r--   0        0        0     3342 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/model/specs/concrete.py
+-rw-r--r--   0        0        0     1519 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/model/standard.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:40:32.108392 openepd-0.8.0/src/openepd/py.typed
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.8.0/PKG-INFO
```

### Comparing `openepd-0.7.0/LICENSE` & `openepd-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-0.7.0/README.md` & `openepd-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `openepd-0.7.0/pyproject.toml` & `openepd-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openepd"
-version = "0.7.0"
+version = "0.8.0"
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
-version = "0.7.0"
+version = "0.8.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/openepd/__version__.py",
 ]
```

### Comparing `openepd-0.7.0/src/openepd/__init__.py` & `openepd-0.8.0/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.7.0/src/openepd/__version__.py` & `openepd-0.8.0/src/openepd/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.7.0"
+VERSION = "0.8.0"
```

### Comparing `openepd-0.7.0/src/openepd/model/__init__.py` & `openepd-0.8.0/src/openepd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.7.0/src/openepd/model/base.py` & `openepd-0.8.0/src/openepd/model/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,14 +40,19 @@
 
     def set_ext_field(self, key: str, value: AnySerializable) -> None:
         """Add an extension field to the model."""
         if self.ext is None:
             self.ext = {}
         self.ext[key] = value
 
+    def set_ext_field_if_any(self, key: str, value: AnySerializable) -> None:
+        """Add an extension field to the model if the value is not None."""
+        if value is not None:
+            self.set_ext_field(key, value)
+
     def get_ext_field(self, key: str, default: AnySerializable = None) -> AnySerializable | None:
         """Get an extension field from the model."""
         if self.ext is None:
             return default
         return self.ext.get(key, default)
 
     @classmethod
```

### Comparing `openepd-0.7.0/src/openepd/model/common.py` & `openepd-0.8.0/src/openepd/model/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -80,7 +80,41 @@
         description="Dict of URLs relevant to this entry",
         example={
             "Contact Us": "https://www.c-change-labs.com/en/contact-us/",
             "LinkedIn": "https://www.linkedin.com/company/c-change-labs/",
         },
         default=None,
     )
+
+    def set_attachment(self, name: str, url: str):
+        """Set an attachment."""
+        if self.attachments is None:
+            self.attachments = {}  # type: ignore
+        self.attachments[name] = url  # type: ignore
+
+    def set_attachment_if_any(self, name: str, url: str | None):
+        """Set an attachment if url is not None."""
+        if url is not None:
+            self.set_attachment(name, url)
+
+
+class WithAltIdsMixin:
+    """Mixin for objects that can have alt_ids."""
+
+    alt_ids: dict[Annotated[str, pyd.Field(max_length=200)], str] | None = pyd.Field(
+        description="Dict identifiers for this entry.",
+        example={
+            "oekobau.dat": "bdda4364-451f-4df2-a68b-5912469ee4c9",
+        },
+        default=None,
+    )
+
+    def set_alt_id(self, domain_name: str, value: str):
+        """Set an alt_id."""
+        if self.alt_ids is None:
+            self.alt_ids = {}
+        self.alt_ids[domain_name] = value
+
+    def set_alt_id_if_any(self, domain_name: str, value: str | None):
+        """Set an alt_id if value is not None."""
+        if value is not None:
+            self.set_alt_id(domain_name, value)
```

### Comparing `openepd-0.7.0/src/openepd/model/epd.py` & `openepd-0.8.0/src/openepd/model/epd.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 #
 import datetime
 from typing import Annotated, Literal
 
 import pydantic as pyd
 
 from openepd.model.base import BaseOpenEpdSchema
-from openepd.model.common import Amount, Ingredient
+from openepd.model.common import Amount, Ingredient, WithAltIdsMixin, WithAttachmentsMixin
 from openepd.model.lcia import ImpactSet, OutputFlowSet, ResourceUseSet
 from openepd.model.org import Org, Plant
 from openepd.model.pcr import Pcr
 from openepd.model.specs import Specs
 from openepd.model.standard import Standard
 
 
-class Epd(BaseOpenEpdSchema):
+class Epd(WithAttachmentsMixin, WithAltIdsMixin, BaseOpenEpdSchema):
     """Represent an EPD."""
 
     # TODO: Add validator for open-xpd-uuid on this field
     id: str = pyd.Field(
         description="The unique ID for this EPD.  To ensure global uniqueness, should be registered at "
         "open-xpd-uuid.cqd.io/register or a coordinating registry.",
         example="1u7zsed8",
@@ -51,15 +51,15 @@
         max_length=200, description="Unique stock keeping identifier assigned by manufacturer"
     )
     product_description: str | None = pyd.Field(
         max_length=2000,
         description="1-paragraph description of product. " "Supports plain text or github flavored markdown.",
     )
     # TODO: add product_alt_names? E.g. ILCD has a list of synonymous names
-    product_classes: dict[str, str] = pyd.Field(
+    product_classes: dict[str, str | list[str]] = pyd.Field(
         description="List of classifications, including Masterformat and UNSPC", default_factory=dict
     )
     product_image_small: pyd.AnyUrl | None = pyd.Field(
         description="Pointer to image illustrating the product, which is no more than 200x200 pixels", default=None
     )
     product_image: pyd.AnyUrl | None = pyd.Field(
         description="pointer to image illustrating the product no more than 10MB", default=None
```

### Comparing `openepd-0.7.0/src/openepd/model/lcia.py` & `openepd-0.8.0/src/openepd/model/lcia.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,19 @@
         "emissions). All related emissions for native forests are included under this category. "
         "Uptake for native forests is set to 0 kgCO2 for EN15804.",
     )
     gwp_nonCO2: ScopeSet | None = pyd.Field(
         alias="gwp-nonCO2",
         description="GWP from non-CO2, non-fossil sources, such as livestock-sourced CH4 and agricultural N2O.",
     )
+    gwp_fossil: ScopeSet | None = pyd.Field(
+        alias="gwp-fossil",
+        description="Climate change effects due to greenhouse gas emissions originating from the oxidation or "
+        "reduction of fossil fuels or materials containing fossil carbon. [Source: EN15804]",
+    )
 
 
 class ResourceUseSet(BaseOpenEpdSchema):
     """A set of resource use indicators, such as RPRec, RPRm, etc."""
 
     RPRec: ScopeSet | None = pyd.Field(
         description="Renewable primary resources used as energy carrier (fuel). "
```

### Comparing `openepd-0.7.0/src/openepd/model/org.py` & `openepd-0.8.0/src/openepd/model/org.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 #  Find out more at www.BuildingTransparency.org
 #
 from typing import Annotated, Optional
 
 import pydantic as pyd
 
 from openepd.model.base import BaseOpenEpdSchema
-from openepd.model.common import WithAttachmentsMixin
+from openepd.model.common import WithAltIdsMixin, WithAttachmentsMixin
 
 
 class Contact(BaseOpenEpdSchema):  # TODO: NEW Object, not in the spec
     """Contact information of a person or organization."""
 
     email: pyd.EmailStr | None = pyd.Field(description="Email", example="contact@c-change-labs.com", default=None)
     phone: str | None = pyd.Field(description="Phone number", example="+15263327352", default=None)
     website: pyd.AnyUrl | None = pyd.Field(
         description="Url of the website", example="http://buildingtransparency.org", default=None
     )
     address: str | None = pyd.Field(description="Address", example="123 Main St, San Francisco, CA 94105", default=None)
 
 
-class Org(WithAttachmentsMixin, BaseOpenEpdSchema):  # TODO: NEW Identifiable field, not in the spec
+class Org(WithAttachmentsMixin, WithAltIdsMixin, BaseOpenEpdSchema):
     """Represent an organization."""
 
     web_domain: str = pyd.Field(
         description="A web domain owned by organization. Typically is the org's home website address",
     )
     name: str = pyd.Field(max_length=200, description="Common name for organization", example="C Change Labs")
     alt_names: Annotated[list[str], pyd.conlist(pyd.constr(max_length=200), max_items=255)] | None = pyd.Field(
@@ -54,15 +54,15 @@
     subsidiaries: Annotated[list[str], pyd.conlist(pyd.constr(max_length=200), max_items=255)] | None = pyd.Field(
         description="Organizations controlled by this organization",
         example=["cqd.io", "supplychaincarbonpricing.org"],
         default=None,
     )
 
 
-class Plant(WithAttachmentsMixin, BaseOpenEpdSchema):
+class Plant(WithAttachmentsMixin, WithAltIdsMixin, BaseOpenEpdSchema):
     """Represent a manufacturing plant."""
 
     # TODO: Add proper validator
     id: str = pyd.Field(
         description="Plus code (aka Open Location Code) of plant's location and "
         "owner's web domain joined with `.`(dot).",
         example="865P2W3V+3W.interface.com",
```

### Comparing `openepd-0.7.0/src/openepd/model/pcr.py` & `openepd-0.8.0/src/openepd/model/pcr.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 #
 import datetime
 from typing import Optional
 
 import pydantic as pyd
 
 from openepd.model.base import BaseOpenEpdSchema
-from openepd.model.common import WithAttachmentsMixin
+from openepd.model.common import WithAltIdsMixin, WithAttachmentsMixin
 from openepd.model.org import Org
 
 
-class Pcr(WithAttachmentsMixin, BaseOpenEpdSchema):
+class Pcr(WithAttachmentsMixin, WithAltIdsMixin, BaseOpenEpdSchema):
     """Represent a PCR (Product Category Rules)."""
 
     id: str = pyd.Field(
         description="The unique ID for this PCR.  To ensure global uniqueness, should be registered "
         "at open-xpd-uuid.cqd.io/register or a coordinating registry.",
         example="ec3xpgq2",
     )
```

### Comparing `openepd-0.7.0/src/openepd/model/specs/__init__.py` & `openepd-0.8.0/src/openepd/model/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.7.0/src/openepd/model/specs/concrete.py` & `openepd-0.8.0/src/openepd/model/specs/concrete.py`

 * *Files identical despite different names*

### Comparing `openepd-0.7.0/src/openepd/model/standard.py` & `openepd-0.8.0/src/openepd/model/standard.py`

 * *Files identical despite different names*

### Comparing `openepd-0.7.0/PKG-INFO` & `openepd-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 0.7.0
+Version: 0.8.0
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
-Metadata-Version: 2.1 Name: openepd Version: 0.7.0 Summary: Python library to
+Metadata-Version: 2.1 Name: openepd Version: 0.8.0 Summary: Python library to
 work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: support@c-change-labs.com
 Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

