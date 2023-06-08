# Comparing `tmp/ask-sdk-core-1.8.0.tar.gz` & `tmp/ask-sdk-core-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ask-sdk-core-1.8.0.tar", last modified: Thu Feb 28 01:25:24 2019, max compression
+gzip compressed data, was "dist/ask-sdk-core-1.9.0.tar", last modified: Tue Mar 19 12:00:52 2019, max compression
```

## Comparing `ask-sdk-core-1.8.0.tar` & `ask-sdk-core-1.9.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-02-28 01:25:24.000000 ask-sdk-core-1.8.0/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2536 2019-02-28 01:25:24.000000 ask-sdk-core-1.8.0/CHANGELOG.rst
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       69 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/requirements.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       67 2019-02-28 01:25:24.000000 ask-sdk-core-1.8.0/setup.cfg
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      107 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/MANIFEST.in
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1853 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/README.rst
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-02-28 01:25:24.000000 ask-sdk-core-1.8.0/ask_sdk_core/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    14865 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/ask_sdk_core/serialize.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4128 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/ask_sdk_core/handler_input.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1205 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/ask_sdk_core/exceptions.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      593 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/ask_sdk_core/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8169 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/ask_sdk_core/attributes_manager.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)    12364 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/ask_sdk_core/response_helper.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5884 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/ask_sdk_core/api_client.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-02-28 01:25:24.000000 ask-sdk-core-1.8.0/ask_sdk_core/dispatch_components/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2450 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/ask_sdk_core/dispatch_components/exception_components.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3876 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/ask_sdk_core/dispatch_components/request_components.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      871 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/ask_sdk_core/dispatch_components/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     9166 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/ask_sdk_core/skill.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1142 2019-02-28 01:25:24.000000 ask-sdk-core-1.8.0/ask_sdk_core/__version__.py
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-02-28 01:25:24.000000 ask-sdk-core-1.8.0/ask_sdk_core/utils/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8227 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/ask_sdk_core/utils/viewport.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      835 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/ask_sdk_core/utils/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3571 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/ask_sdk_core/utils/predicate.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4509 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/ask_sdk_core/skill_builder.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6594 2019-02-28 01:25:24.000000 ask-sdk-core-1.8.0/PKG-INFO
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-02-28 01:25:24.000000 ask-sdk-core-1.8.0/ask_sdk_core.egg-info/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      819 2019-02-28 01:25:24.000000 ask-sdk-core-1.8.0/ask_sdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-02-28 01:25:24.000000 ask-sdk-core-1.8.0/ask_sdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       13 2019-02-28 01:25:24.000000 ask-sdk-core-1.8.0/ask_sdk_core.egg-info/top_level.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-02-28 01:25:24.000000 ask-sdk-core-1.8.0/ask_sdk_core.egg-info/not-zip-safe
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6594 2019-02-28 01:25:24.000000 ask-sdk-core-1.8.0/ask_sdk_core.egg-info/PKG-INFO
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       69 2019-02-28 01:25:24.000000 ask-sdk-core-1.8.0/ask_sdk_core.egg-info/requires.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2144 2019-02-28 01:25:20.000000 ask-sdk-core-1.8.0/setup.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-19 12:00:52.000000 ask-sdk-core-1.9.0/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2697 2019-03-19 12:00:52.000000 ask-sdk-core-1.9.0/CHANGELOG.rst
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       69 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/requirements.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       67 2019-03-19 12:00:52.000000 ask-sdk-core-1.9.0/setup.cfg
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      107 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/MANIFEST.in
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1853 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/README.rst
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-19 12:00:52.000000 ask-sdk-core-1.9.0/ask_sdk_core/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    14865 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/serialize.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4128 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/handler_input.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1205 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/exceptions.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      593 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8169 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/attributes_manager.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    12364 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/response_helper.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     5884 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/api_client.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-19 12:00:52.000000 ask-sdk-core-1.9.0/ask_sdk_core/dispatch_components/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2450 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/dispatch_components/exception_components.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3876 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/dispatch_components/request_components.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      871 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/dispatch_components/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     9166 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/skill.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1142 2019-03-19 12:00:52.000000 ask-sdk-core-1.9.0/ask_sdk_core/__version__.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-19 12:00:52.000000 ask-sdk-core-1.9.0/ask_sdk_core/utils/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)    12717 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/utils/request_util.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     8232 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/utils/viewport.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1086 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/utils/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     3571 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/utils/predicate.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4509 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/ask_sdk_core/skill_builder.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6819 2019-03-19 12:00:52.000000 ask-sdk-core-1.9.0/PKG-INFO
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-19 12:00:52.000000 ask-sdk-core-1.9.0/ask_sdk_core.egg-info/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      854 2019-03-19 12:00:52.000000 ask-sdk-core-1.9.0/ask_sdk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-03-19 12:00:52.000000 ask-sdk-core-1.9.0/ask_sdk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       13 2019-03-19 12:00:52.000000 ask-sdk-core-1.9.0/ask_sdk_core.egg-info/top_level.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-03-19 12:00:52.000000 ask-sdk-core-1.9.0/ask_sdk_core.egg-info/not-zip-safe
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6819 2019-03-19 12:00:52.000000 ask-sdk-core-1.9.0/ask_sdk_core.egg-info/PKG-INFO
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       69 2019-03-19 12:00:52.000000 ask-sdk-core-1.9.0/ask_sdk_core.egg-info/requires.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2144 2019-03-19 12:00:48.000000 ask-sdk-core-1.9.0/setup.py
```

### Comparing `ask-sdk-core-1.8.0/CHANGELOG.rst` & `ask-sdk-core-1.9.0/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -95,7 +95,15 @@
 1.8.0
 ~~~~~~~
 
 This release contains the following changes : 
 
 - Allow Default API Client to invoke Alexa APIs that require other than 'application/json' body type.
 
+
+
+1.9.0
+~~~~~~~
+
+This release includes the following : 
+
+- Request utility methods which makes it easier to retrieve common properties from an incoming request.
```

### Comparing `ask-sdk-core-1.8.0/README.rst` & `ask-sdk-core-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/serialize.py` & `ask-sdk-core-1.9.0/ask_sdk_core/serialize.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/handler_input.py` & `ask-sdk-core-1.9.0/ask_sdk_core/handler_input.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/exceptions.py` & `ask-sdk-core-1.9.0/ask_sdk_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/__init__.py` & `ask-sdk-core-1.9.0/ask_sdk_core/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/attributes_manager.py` & `ask-sdk-core-1.9.0/ask_sdk_core/attributes_manager.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/response_helper.py` & `ask-sdk-core-1.9.0/ask_sdk_core/response_helper.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/api_client.py` & `ask-sdk-core-1.9.0/ask_sdk_core/api_client.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/dispatch_components/exception_components.py` & `ask-sdk-core-1.9.0/ask_sdk_core/dispatch_components/exception_components.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/dispatch_components/request_components.py` & `ask-sdk-core-1.9.0/ask_sdk_core/dispatch_components/request_components.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/dispatch_components/__init__.py` & `ask-sdk-core-1.9.0/ask_sdk_core/dispatch_components/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/skill.py` & `ask-sdk-core-1.9.0/ask_sdk_core/skill.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/__version__.py` & `ask-sdk-core-1.9.0/ask_sdk_core/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # License.
 #
 
 __pip_package_name__ = 'ask-sdk-core'
 __description__ = ('The ASK SDK Core package provides core Alexa Skills Kit '
                    'functionality, for building Alexa Skills.')
 __url__ = 'https://github.com/alexa/alexa-skills-kit-sdk-for-python'
-__version__ = '1.8.0'
+__version__ = '1.9.0'
 __author__ = 'Alexa Skills Kit'
 __author_email__ = 'ask-sdk-dynamic@amazon.com'
 __license__ = 'Apache 2.0'
 __keywords__ = ['ASK SDK', 'Alexa Skills Kit', 'Alexa', 'Core']
 __install_requires__ = ["requests", "python_dateutil",
                         "ask-sdk-model>=1.0.0", "ask-sdk-runtime>=1.1.0"]
```

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/utils/viewport.py` & `ask-sdk-core-1.9.0/ask_sdk_core/utils/viewport.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
 def get_orientation(width, height):
     # type: (int, int) -> Orientation
     """Get viewport orientation from given width and height.
 
     :type width: int
     :type height: int
-    :return viewport orientation enum
+    :return: viewport orientation enum
     :rtype: Orientation
     """
     if width > height:
         return Orientation.LANDSCAPE
     elif width < height:
         return Orientation.PORTRAIT
     else:
@@ -99,15 +99,15 @@
 
 
 def get_size(size):
     # type: (int) -> Size
     """Get viewport size from given size.
 
     :type size: int
-    :return viewport size enum
+    :return: viewport size enum
     :rtype: Size
     """
     if size in range(0, 600):
         return Size.XSMALL
     elif size in range(600, 960):
         return Size.SMALL
     elif size in range(960, 1280):
@@ -121,15 +121,15 @@
 
 
 def get_dpi_group(dpi):
     # type: (int) -> Density
     """Get viewport density group from given dpi.
 
     :type dpi: int
-    :return viewport density group enum
+    :return: viewport density group enum
     :rtype: Density
     """
     if dpi in range(0, 121):
         return Density.XLOW
     elif dpi in range(121, 161):
         return Density.LOW
     elif dpi in range(161, 241):
@@ -153,16 +153,16 @@
 
     If there is no `viewport`
     value in `request_envelope.context`, then an
     `ViewportProfile.UNKNOWN_VIEWPORT_PROFILE` is returned.
 
     :param request_envelope: The alexa request envelope object
     :type request_envelope: ask_sdk_model.request_envelope.RequestEnvelope
-    :return Calculated Viewport Profile enum
-    :rtype ViewportProfile
+    :return: Calculated Viewport Profile enum
+    :rtype: ViewportProfile
     """
     viewport_state = request_envelope.context.viewport
     if viewport_state:
         shape = viewport_state.shape
         current_pixel_width = int(viewport_state.current_pixel_width)
         current_pixel_height = int(viewport_state.current_pixel_height)
         dpi = int(viewport_state.dpi)
```

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/utils/__init__.py` & `ask-sdk-core-1.9.0/ask_sdk_core/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,13 +14,18 @@
 # OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the
 # License.
 #
 import sys
 
 from ..__version__ import __version__
-from .predicate import is_canfulfill_intent_name, is_intent_name, is_request_type
+from .predicate import (
+    is_canfulfill_intent_name, is_intent_name, is_request_type)
 from ask_sdk_runtime.utils import user_agent_info
+from .request_util import (
+    get_slot, get_slot_value, get_account_linking_access_token,
+    get_api_access_token, get_device_id, get_dialog_state, get_intent_name,
+    get_locale, get_request_type, is_new_session, get_supported_interfaces)
 
 
 SDK_VERSION = __version__
 RESPONSE_FORMAT_VERSION = "1.0"
```

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/utils/predicate.py` & `ask-sdk-core-1.9.0/ask_sdk_core/utils/predicate.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core/skill_builder.py` & `ask-sdk-core-1.9.0/ask_sdk_core/skill_builder.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-core-1.8.0/PKG-INFO` & `ask-sdk-core-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ask-sdk-core
-Version: 1.8.0
+Version: 1.9.0
 Summary: The ASK SDK Core package provides core Alexa Skills Kit functionality, for building Alexa Skills.
 Home-page: https://github.com/alexa/alexa-skills-kit-sdk-for-python
 Author: Alexa Skills Kit
 Author-email: ask-sdk-dynamic@amazon.com
 License: Apache 2.0
 Description: ====================================================
         ASK SDK Core - Base components of Python ASK SDK
@@ -158,14 +158,22 @@
         ~~~~~~~
         
         This release contains the following changes : 
         
         - Allow Default API Client to invoke Alexa APIs that require other than 'application/json' body type.
         
         
+        
+        1.9.0
+        ~~~~~~~
+        
+        This release includes the following : 
+        
+        - Request utility methods which makes it easier to retrieve common properties from an incoming request.
+        
 Keywords: ASK SDK,Alexa Skills Kit,Alexa,Core
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core.egg-info/SOURCES.txt` & `ask-sdk-core-1.9.0/ask_sdk_core.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 ask_sdk_core.egg-info/requires.txt
 ask_sdk_core.egg-info/top_level.txt
 ask_sdk_core/dispatch_components/__init__.py
 ask_sdk_core/dispatch_components/exception_components.py
 ask_sdk_core/dispatch_components/request_components.py
 ask_sdk_core/utils/__init__.py
 ask_sdk_core/utils/predicate.py
+ask_sdk_core/utils/request_util.py
 ask_sdk_core/utils/viewport.py
```

### Comparing `ask-sdk-core-1.8.0/ask_sdk_core.egg-info/PKG-INFO` & `ask-sdk-core-1.9.0/ask_sdk_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ask-sdk-core
-Version: 1.8.0
+Version: 1.9.0
 Summary: The ASK SDK Core package provides core Alexa Skills Kit functionality, for building Alexa Skills.
 Home-page: https://github.com/alexa/alexa-skills-kit-sdk-for-python
 Author: Alexa Skills Kit
 Author-email: ask-sdk-dynamic@amazon.com
 License: Apache 2.0
 Description: ====================================================
         ASK SDK Core - Base components of Python ASK SDK
@@ -158,14 +158,22 @@
         ~~~~~~~
         
         This release contains the following changes : 
         
         - Allow Default API Client to invoke Alexa APIs that require other than 'application/json' body type.
         
         
+        
+        1.9.0
+        ~~~~~~~
+        
+        This release includes the following : 
+        
+        - Request utility methods which makes it easier to retrieve common properties from an incoming request.
+        
 Keywords: ASK SDK,Alexa Skills Kit,Alexa,Core
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `ask-sdk-core-1.8.0/setup.py` & `ask-sdk-core-1.9.0/setup.py`

 * *Files identical despite different names*

