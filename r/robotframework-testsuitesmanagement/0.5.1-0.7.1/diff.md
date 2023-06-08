# Comparing `tmp/robotframework-testsuitesmanagement-0.5.1.tar.gz` & `tmp/robotframework-testsuitesmanagement-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\robotframework-testsuitesmanagement-0.5.1.tar", last modified: Tue Jun 28 13:41:07 2022, max compression
+gzip compressed data, was "robotframework-testsuitesmanagement-0.7.1.tar", last modified: Thu Jun  8 14:02:05 2023, max compression
```

## Comparing `robotframework-testsuitesmanagement-0.5.1.tar` & `robotframework-testsuitesmanagement-0.7.1.tar`

### file list

```diff
@@ -1,34 +1,32 @@
-drwxrwxrwx   0        0        0        0 2022-06-28 13:41:07.210021 robotframework-testsuitesmanagement-0.5.1/
--rw-rw-rw-   0        0        0    11356 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/LICENSE
--rw-rw-rw-   0        0        0      117 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     8823 2022-06-28 13:41:07.208068 robotframework-testsuitesmanagement-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     8427 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/README.rst
-drwxrwxrwx   0        0        0        0 2022-06-28 13:41:07.131899 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/
-drwxrwxrwx   0        0        0        0 2022-06-28 13:41:07.148501 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Config/
--rw-rw-rw-   0        0        0    30029 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Config/CConfig.py
--rw-rw-rw-   0        0        0      648 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Config/__init__.py
--rw-rw-rw-   0        0        0     1214 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Config/robot_config.json
--rw-rw-rw-   0        0        0     1083 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Config/robot_schema.json
-drwxrwxrwx   0        0        0        0 2022-06-28 13:41:07.160221 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Keywords/
--rw-rw-rw-   0        0        0      956 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Keywords/COnFailureHandle.py
--rw-rw-rw-   0        0        0     6321 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Keywords/CSetup.py
--rw-rw-rw-   0        0        0      664 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Keywords/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-28 13:41:07.169983 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Utils/
--rw-rw-rw-   0        0        0     1541 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Utils/CStruct.py
-drwxrwxrwx   0        0        0        0 2022-06-28 13:41:07.182680 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Utils/Events/
--rw-rw-rw-   0        0        0      732 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Utils/Events/Event.py
--rw-rw-rw-   0        0        0     1418 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Utils/Events/ScopeEvent.py
--rw-rw-rw-   0        0        0     1372 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Utils/Events/__init__.py
--rw-rw-rw-   0        0        0     4669 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Utils/LibListener.py
--rw-rw-rw-   0        0        0      678 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Utils/__init__.py
--rw-rw-rw-   0        0        0     3576 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/__init__.py
--rw-rw-rw-   0        0        0     1231 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/version.py
-drwxrwxrwx   0        0        0        0 2022-06-28 13:41:07.206115 robotframework-testsuitesmanagement-0.5.1/robotframework_testsuitesmanagement.egg-info/
--rw-rw-rw-   0        0        0     8823 2022-06-28 13:41:05.000000 robotframework-testsuitesmanagement-0.5.1/robotframework_testsuitesmanagement.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1094 2022-06-28 13:41:06.000000 robotframework-testsuitesmanagement-0.5.1/robotframework_testsuitesmanagement.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-28 13:41:05.000000 robotframework-testsuitesmanagement-0.5.1/robotframework_testsuitesmanagement.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2022-06-28 13:41:06.000000 robotframework-testsuitesmanagement-0.5.1/robotframework_testsuitesmanagement.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2022-06-28 13:41:06.000000 robotframework-testsuitesmanagement-0.5.1/robotframework_testsuitesmanagement.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2022-06-28 13:41:06.000000 robotframework-testsuitesmanagement-0.5.1/robotframework_testsuitesmanagement.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-28 13:41:07.210021 robotframework-testsuitesmanagement-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0    10523 2022-05-31 17:56:45.000000 robotframework-testsuitesmanagement-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)    35904 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Config/CConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Keywords/COnFailureHandle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Keywords/CSetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/CStruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/Events/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/Events/Event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/Events/ScopeEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/Events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/LibListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-08 14:02:05.000000 robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-08 14:02:05.000000 robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:02:05.000000 robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 14:02:05.000000 robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 14:02:05.000000 robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 14:02:05.000000 robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:02:05.818161 robotframework-testsuitesmanagement-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-08 13:59:42.000000 robotframework-testsuitesmanagement-0.7.1/setup.py
```

### Comparing `robotframework-testsuitesmanagement-0.5.1/LICENSE` & `robotframework-testsuitesmanagement-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Config/CConfig.py` & `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Config/CConfig.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2022 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,15 +11,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #################################################################################
 #
 # File: CConfig.py
 # Initially created by Mai Dinh Nam Son (RBVH/ECM11) / Nov-2020
-# Base on TML Framework automation concept
+# Based on TML Framework automation concept
 #
 # 2021-06-25: Mai Dinh Nam Son (RBVH/ECM1)
 #   - Adds CJsonDotDict class to convert json to dotdict object
 #   - Converts json config to dotdict config object
 #################################################################################
 
 
@@ -29,74 +29,114 @@
 import ctypes
 import socket
 import json
 import copy
 from jsonschema import validate
 from builtins import staticmethod
 
-from RobotFramework_Testsuites.Utils.CStruct import CStruct
+from RobotFramework_TestsuitesManagement.Utils.CStruct import CStruct
+from PythonExtensionsCollection.String.CString import CString
 
 from JsonPreprocessor import CJsonPreprocessor
 from robot.api import logger
 from robot.version import get_full_version, get_version
 from robot.libraries.BuiltIn import BuiltIn
+from robot.utils.dotdict import DotDict
 import pathlib
+from RobotFramework_TestsuitesManagement.version import VERSION, VERSION_DATE
 
-# This is version information represents for the whole AIO bundle
-# It contains the core robotframework and relative resources such as:
-# testsuitesmanagement, testresultwebapptool, Eclipse for RobotFramework, ...
-# This information is used for Robotframework AIO version control 
-VERSION = "0.5.1"
+INSTALLER_LOCATION = "https://github.com/test-fullautomation/robotframework-testsuitesmanagement/releases"
+BUNDLE_NAME = "RobotFramework_TestsuitesManagement"
+BUNDLE_VERSION = VERSION
+BUNDLE_VERSION_DATE = VERSION_DATE
+
+# Load package context file
+context_filename = "package_context.json"
+context_filepath = os.path.join(os.path.dirname(__file__), context_filename)
+context_config = None
+
+if os.path.isfile(context_filepath):
+    if os.stat(context_filepath).st_size == 0:
+        logger.warn(f"The '{context_filepath}' file is existing but empty.")
+    else:
+        try:
+            with open(context_filepath) as f:
+                context_config = json.load(f)        
+        except Exception as reason:
+            logger.error(f"Cannot load the '{context_filepath}' file. Reason: {reason}")
+            exit(1)
+
+        if ('installer_location' in context_config) and context_config['installer_location']:
+            INSTALLER_LOCATION = context_config['installer_location']
+        if ('bundle_name' in context_config) and context_config['bundle_name']:
+            BUNDLE_NAME = context_config['bundle_name']
+        if ('bundle_version' in context_config) and context_config['bundle_version']:
+            BUNDLE_VERSION = context_config['bundle_version']
+        if ('bundle_version_date' in context_config) and context_config['bundle_version_date']:
+            BUNDLE_VERSION_DATE = context_config['bundle_version_date']
+
+def bundle_version():
+   '''
+This function prints out the package version which is:
+
+- RobotFramework_TestsuitesManagement version when this module is installed
+stand-alone (via `pip` or directly from sourcecode)
+
+- RobotFramework AIO version when this module is bundled with RobotFramework AIO 
+package
+
+**Arguments:**
+
+* No input parameter is required
+
+**Returns:**
+
+* No return variable
+   '''
+   print(f"{BUNDLE_VERSION}")
 
-class dotdict(dict):
+class CConfig():
+    '''
+Defines the properties of configuration and holds the identified config files.
 
-    __setattr__ = dict.__setitem__
-    def __getattr__(self, item):
-        try:
-            return self[item]
-        except KeyError as error:
-            raise AttributeError from error
-    __delattr__ = dict.__delitem__
+The loading configuration method is divided into 4 levels, level1 has the highest priority, Level4 has the lowest priority.
 
+**Level1:** Handed over by command line argument
 
-class CConfig():
-    '''
-Defines the properties of configuration
-Holds the identified config files.
-Level1 is highest priority, Level4 is lowest priority.
+**Level2:** Read from content of json config file
+
+   .. code:: json
+
+      {
+         "default": {
+            "name": "robot_config.jsonp",
+            "path": ".../config/"
+         },
+         "variant_0": {
+            "name": "robot_config.jsonp",
+            "path": ".../config/"
+         },
+         "variant_1": {
+            "name": "robot_config_variant_1.jsonp",
+            "path": ".../config/"
+         },
+            ...
+            ...
+      }
+
+   According to the ``ConfigName``, RobotFramework_TestsuitesManagement will choose the corresponding config file.
+   ``".../config/"`` indicats the relative path to json config file, RobotFramework_TestsuitesManagement will recursively
+   find the ``config`` folder.
+
+**Level3:** Read in testsuite folder: ``/config/robot_config.jsonp``
 
-(remaining content needs to be fixed and restored)
+**Level4:** Read from RobotFramework AIO installation folder:
 
+    ``/RobotFramework/defaultconfig/robot_config.jsonp``
     '''
-    # '''
-# Defines the properties of configuration
-# Holds the identified config files.
-# Level1 is highest priority, Level4 is lowest priority.
-
-# Level1: handed over by command line argument.
-# Level2: read from content of
-                            # {
-                              # "default": {
-                                # "name": "robot_config.json",
-                                # "path": ".../config/"
-                              # },
-                              # "variant_0": {
-                                # "name": "robot_config.json",
-                                # "path": ".../config/"
-                              # },
-                              # "variant_1": {
-                                # "name": "robot_config_variant_1.json",
-                                # "path": ".../config/"
-                              # },
-                                # ...
-                                # ...
-                            # }
-# Level3: read in testsuite folder /config/robot_config.json
-# Level4: read from ROBFW install folder /RobotFramework/defaultconfig/robot_config.json
-    # '''
     ROBOT_LIBRARY_SCOPE = 'GLOBAL'
     __single          = None
     sRootSuiteName    = ''
     bConfigLoaded     = False
     oConfigParams     = {}
     sConfigName       = 'default'
     sProjectName      = None
@@ -107,524 +147,531 @@
     bLoadedCfg        = True
     sLoadedCfgError   = ''
     sTestSuiteCfg     = ''
     sTestCfgFile      = ''
     sTestcasePath     = ''
     sMaxVersion       = ''
     sMinVersion       = ''
+    sLocalConfig      = ''
+    lBuitInVariables  = []
     rConfigFiles   = CStruct(
-                                sLevel1 = False,
-                                sLevel2 = False,
-                                sLevel3 = False,
-                                sLevel4 = True   #'.../RobotFramework_Testsuites/Config/robot_config.json'
+                                bLevel1 = False,
+                                bLevel2 = False,
+                                bLevel3 = False,
+                                bLevel4 = True   #'.../RobotFramework_TestsuitesManagement/Config/robot_config.jsonp'
                             )
     
     rMetaData      = CStruct(
                                 sVersionSW = '',
                                 sVersionHW     = '',
                                 sVersionTest   = '',
                                 sROBFWVersion  = get_full_version('Robot Framework')
                             )
     
     # Common configuration parameters 
     sWelcomeString  = None
     sTargetName     = None
-    ddictJson = dotdict()
+    ddictJson = DotDict()
     
     class CJsonDotDict():
         '''
-        The CJsonDotDict class converts json configuration object to dotdict
+The CJsonDotDict class converts json configuration object to dotdict
         '''
-
         def __init__(self):
             self.lTmpParam = ['CConfig.ddictJson']
             
         def __del__(self):
-            CConfig.ddictJson = dotdict()
+            CConfig.ddictJson = DotDict()
             del self.lTmpParam
 
         def dotdictConvert(self, oJson):
             '''
-            Method: dotdictConvert converts json object to dotdict
+This dotdictConvert method converts json object to dotdict.
+
+**Arguments:**
+
+* ``oJson``
+
+   / *Condition*: required / *Type*: dict /
+
+   Json object which want to convert to dotdict.
+
+**Returns:**
+
+* ``CConfig.ddictJson``
 
-            Args:
-                oJson: dict
-            Returns:
-                CConfig.ddictJson: dotdict
+   / *Type*: dotdict /
             '''
             if len(self.lTmpParam) == 1:
                 CConfig.ddictJson.update(oJson)
                 
             for k,v in oJson.items():
                 sExec = ""
                 if isinstance(v, dict):
                     self.lTmpParam.append(k)
                     for i in self.lTmpParam:
                         sExec = i if i==self.lTmpParam[0] else sExec + "." + i
-                    sExec = sExec + " = dotdict(" + str(v) + ")"
+                    sExec = sExec + " = DotDict(" + str(v) + ")"
                     try:
                         exec(sExec, globals())
                     except:
-                        logger.info("Could not convert: %s to dotdict" %(sExec))
+                        logger.info(f"Could not convert: {sExec} to dotdict")
                         pass
                     
                     self.dotdictConvert(v)
                 elif isinstance(v, list):
                     n = 0
                     for item in v:
                         if isinstance(item, dict):
                             self.lTmpParam.append(k+"["+str(n)+"]")
                             for i in self.lTmpParam:
                                 sExec = i if i == self.lTmpParam[0] else sExec + "." + i
-                            sExec = sExec + " = dotdict(" + str(item) + ")"
+                            sExec = sExec + " = DotDict(" + str(item) + ")"
                             try:
                                 exec(sExec, globals())
                             except:
-                                logger.info("Could not convert: %s to dotdict" %(sExec))
+                                logger.info(f"Could not convert: {sExec} to dotdict")
                                 pass
                             
                             self.dotdictConvert(item)
                         n = n+1
             self.lTmpParam = self.lTmpParam[:-1]
             return CConfig.ddictJson
      
-    '''
-    Makes the CConfig class to singleton.
-    Checks to see if a __single exists already for this class
-    Compare class types instead of just looking for None so that subclasses will create
-    their own __single objects. 
-    Args:
-        classtype: type of class
-    Returns:
-        classtype.__single
-    '''
     def __new__(classtype, *args, **kwargs):
+        '''
+Makes the CConfig class to singleton.
+
+Checks to see if a __single exists already for this class. Compare class types instead of just looking
+for None so that subclasses will create their own __single objects.
+        '''
         if classtype != type(classtype.__single):
             classtype.__single = object.__new__(classtype)
         return classtype.__single
 
-    '''
-    Constructor
-    Args:
-        None
-    Returns:
-        None
-    '''
     def __init__(self):
         pass
         
 
     @staticmethod
     def loadCfg(self):
-        if not self.rConfigFiles.sLevel1:
-            if self.rConfigFiles.sLevel2:
-                self.rConfigFiles.sLevel4 = False
-                self.__loadConfigFileLevel2()
+        '''
+This loadCfg method uses to load configuration's parameters from json files.
+
+**Arguments:**
+
+* No input parameter is required
+
+**Returns:**
+
+* No return variable
+        '''
+        bConfigLevel2 = True
+        if not self.rConfigFiles.bLevel1:
+            if self.rConfigFiles.bLevel2:
+                self.rConfigFiles.bLevel4 = False
+                bConfigLevel2 = self.__loadConfigFileLevel2()
             else:
-                bLevel3Check = False
+                if r'${variant}' in BuiltIn().get_variables():
+                    logger.error(f"Not able to get a configuration for variant '{self.sConfigName}' because of a variant configuration file is not available. \n" + \
+                                  "          A variant configuration file must be available when executing robot with configuration level 2. \n")
+                    BuiltIn().unknown('Loading configuration level 2 failed!')
+                    
                 if os.path.isdir(self.sTestcasePath + 'config'):
+                    sConfigFolder = CString.NormalizePath(f"{self.sTestcasePath}/config")
                     sSuiteFileName = BuiltIn().get_variable_value('${SUITE_SOURCE}').split(os.path.sep)[-1:][0]
-                    for file in os.listdir(self.sTestcasePath + 'config'):
-                        if file.split('.')[0] == sSuiteFileName.split('.')[0]:
-                            self.sTestCfgFile = self.sTestcasePath + 'config' + os.path.sep + file
-                            self.rConfigFiles.sLevel4 = False
-                            bLevel3Check = True
-                            break
-                    if not bLevel3Check:
-                        if os.path.isfile(self.sTestcasePath + 'config' + os.path.sep + 'robot_config.json'):
-                            self.sTestCfgFile = self.sTestcasePath + 'config' + os.path.sep + 'robot_config.json'
-                            self.rConfigFiles.sLevel4 = False
-                        else:
-                            self.rConfigFiles.sLevel3 = False
-                            if not self.bConfigLoaded:
-                                #self.rConfigFiles.sLevel4 = True
-                                sDefaultConfig=str(pathlib.Path(__file__).parent.absolute() / "robot_config.json")
-                                self.sTestCfgFile = sDefaultConfig
+                    sJsonFile1 = f"{sConfigFolder}/{sSuiteFileName.split('.')[0]}.jsonp"
+                    sJsonFile2 = f"{sConfigFolder}/{sSuiteFileName.split('.')[0]}.json"
+                    if not os.path.isfile(sJsonFile1) and not os.path.isfile(sJsonFile2):
+                        sJsonFile1    = f"{sConfigFolder}/robot_config.jsonp"
+                        sJsonFile2    = f"{sConfigFolder}/robot_config.json" # still supported alternative extension
+
+                    if os.path.isfile(sJsonFile1) and os.path.isfile(sJsonFile2):
+                        errorMessage = "Configuration file duplicate detected (both extensions: 'jsonp' and 'json')!\n" + \
+                                        f"* file 1: '{sJsonFile1}'\n" + \
+                                        f"* file 2: '{sJsonFile2}'\n" + \
+                                        "Please decide which one to keep and which one to remove. Both together are not allowed."
+                        logger.error(errorMessage)
+                        BuiltIn().unknown("Configuration file duplicate detected (both extensions: 'jsonp' and 'json')!")
+                    elif os.path.isfile(sJsonFile1):
+                        self.sTestCfgFile = sJsonFile1
+                        self.rConfigFiles.bLevel4 = False
+                    elif os.path.isfile(sJsonFile2):
+                        self.sTestCfgFile = sJsonFile2
+                        self.rConfigFiles.bLevel4 = False
+                    else: # meaning: if not os.path.isfile(sJsonFile1) and not os.path.isfile(sJsonFile2)
+                        self.rConfigFiles.bLevel3 = False
+                        if not self.bConfigLoaded:
+                            sDefaultConfig=str(pathlib.Path(__file__).parent.absolute() / "robot_config.jsonp")
+                            self.sTestCfgFile = sDefaultConfig
                 else:
-                    self.rConfigFiles.sLevel3 = False
+                    self.rConfigFiles.bLevel3 = False
                     if not self.bConfigLoaded:
-                        #self.rConfigFiles.sLevel4 = True
-                        sDefaultConfig=str(pathlib.Path(__file__).parent.absolute() / "robot_config.json")
+                        sDefaultConfig=str(pathlib.Path(__file__).parent.absolute() / "robot_config.jsonp")
                         self.sTestCfgFile = sDefaultConfig
 
+            if self.sTestCfgFile != '':                      
+                self.sTestCfgFile = CString.NormalizePath(self.sTestCfgFile)
+
         if self.bConfigLoaded:
-            if self.rConfigFiles.sLevel1:
+            if self.rConfigFiles.bLevel1:
                 return
-            elif not self.rConfigFiles.sLevel2 and not self.rConfigFiles.sLevel3:
+            elif not self.rConfigFiles.bLevel2 and not self.rConfigFiles.bLevel3:
                 return
         
-        if self.rConfigFiles.sLevel1 and self.sTestCfgFile == '':
-            logger.error("The config_file input parameter is empty!!!")
-            raise Exception("The config_file input parameter is empty!!!")
-        elif not (os.path.isfile(self.sTestCfgFile)):
-           raise Exception("Did not find configuration file: '%s'!" % self.sTestCfgFile)
+        if self.rConfigFiles.bLevel1:
+            if self.sConfigName != 'default':
+                errorMessage = "Redundant settings detected in command line: Parameter 'variant' is used together with parameter 'config_file'.\n" + \
+                               "          It is not possible to use both together, because they belong to the same feature (the variant selection).\n" + \
+                               "          Please remove one of them.\n"
+                logger.error(errorMessage)
+                BuiltIn().unknown('Redundant settings detected in command line!')
+
+            if self.sTestCfgFile == '':
+                errorMessage = "The config_file input parameter is empty!!!\n"
+                logger.error(errorMessage)
+                BuiltIn().unknown(errorMessage)
+
+        if not bConfigLevel2:
+            BuiltIn().unknown('Loading configuration level 2 failed!')
+            return
+
+        if not os.path.isfile(self.sTestCfgFile):
+            errorMessage = f"Did not find configuration file: '{self.sTestCfgFile}'!\n"
+            logger.error(errorMessage)
+            BuiltIn().unknown('The configuration file is not found!')
         
         robotCoreData = BuiltIn().get_variables()
         ROBFW_AIO_Data = {}
         for k, v in robotCoreData.items():
             key = re.findall("\s*{\s*(.+)\s*}\s*", k)[0]
             if 'CONFIG' == key:
                 continue
             ROBFW_AIO_Data.update({key:v})
         oJsonPreprocessor = CJsonPreprocessor(syntax="python", currentCfg=ROBFW_AIO_Data)
         try:
             oJsonCfgData = oJsonPreprocessor.jsonLoad(self.sTestCfgFile)
         except Exception as error:
             CConfig.bLoadedCfg = False
-            CConfig.sLoadedCfgError = str(error)
-            logger.error("Loading of JSON configuration file failed! Reason: %s" %(CConfig.sLoadedCfgError))
+            CConfig.sLoadedCfgError = ''
+            for item in str(error).split(': \''):
+                CConfig.sLoadedCfgError += f"{item}\n                  "
+            logger.error(f"Loading of JSON configuration file failed! \n          Reason: {CConfig.sLoadedCfgError}")
+            BuiltIn().unknown('Loading of JSON configuration file failed!')
             raise Exception
 
+        if self.sLocalConfig != '':
+            try:
+                oLocalConfig = oJsonPreprocessor.jsonLoad(CString.NormalizePath(self.sLocalConfig))
+            except Exception as error:
+                CConfig.bLoadedCfg = False
+                CConfig.sLoadedCfgError = str(error)
+                logger.error(f"Loading local config failed! Reason: {CConfig.sLoadedCfgError}\n")
+                BuiltIn().unknown('Loading local config failed!')
+                raise Exception
+            
+            def __loadLocalConfig(oLocalConfig):
+                tmpDict = copy.deepcopy(oLocalConfig)
+                for k, v in tmpDict.items():
+                    if re.match('.*\${\s*', k):
+                        del oLocalConfig[k]
+                    elif isinstance(v, dict):
+                        __loadLocalConfig(oLocalConfig)
+                oJsonCfgData.update(oLocalConfig)
+            __loadLocalConfig(oLocalConfig)
+
         bJsonSchema = True    
         try:
-            sSchemaFile=str(pathlib.Path(__file__).parent.absolute() / "robot_schema.json")
+            sSchemaFile=str(pathlib.Path(__file__).parent.absolute() / "configuration_schema.json")
             with open(sSchemaFile) as f:
                 oJsonSchemaCfg = json.load(f)
         except Exception as err:
             bJsonSchema = False
-            logger.error("Could not parse configuration json schema file: '%s'" % str(err))
+            logger.error(f"Could not parse configuration JSON schema file: '{str(err)}'\n")
+            BuiltIn().unknown('Parse JSON schema file failed!')
     
         if bJsonSchema:
             try:
                 validate(instance=oJsonCfgData, schema=oJsonSchemaCfg)
             except Exception as error:
                 if error.validator == 'additionalProperties':
-                    logger.error("Verification against json schema failed: '%s'" %(error.message))
-                    logger.error("Additional properties are not allowed! \n \
-                    Please put the additional params to 'preprocessor': { 'definitions' : {...} or 'params': { 'global': {...}")
-                    raise Exception("Verification against json schema failed: '%s'" %(error.message))
+                    logger.error(f"Verification against JSON schema failed: '{error.message}'\n" + \
+                                 "          Please put the additional params into 'params': { 'global': {...} \n")
                 elif error.validator == 'required':
-                    logger.error("The parameter %s, but it's not set in JSON configuration file." % (error.message))
-                    raise Exception("The parameter %s, but it's missing in JSON configuration file." % (error.message))
+                    logger.error(f"The parameter {error.message} in configuration file {self.sTestCfgFile}.\n")
                 else:
                     errParam = error.path.pop()
-                    logger.error("Parameter '%s' in JSON configuration file is not allowed due to: %s" % (errParam, error.message))
-                    raise Exception("Parameter '%s' in JSON configuration file is not allowed due to: %s" % (errParam, error.message))
+                    logger.error(f"Parameter '{errParam}' with invalid value found in JSON configuration file! \n" + \
+                                 f"          {error.message}\n")
+                BuiltIn().unknown('JSON schema validation failed!')
             
         self.sProjectName = oJsonCfgData['Project']
         self.sTargetName = oJsonCfgData['TargetName']
         self.sWelcomeString = oJsonCfgData['WelcomeString']
-        if ("Maximum_version" in oJsonCfgData):
+        if ("Maximum_version" in oJsonCfgData) and oJsonCfgData["Maximum_version"] != None:
             self.sMaxVersion = oJsonCfgData["Maximum_version"]
-        if ("Minimum_version" in oJsonCfgData):
+        if ("Minimum_version" in oJsonCfgData) and oJsonCfgData["Minimum_version"] != None:
             self.sMinVersion = oJsonCfgData["Minimum_version"]
 
+        suiteMetadata = BuiltIn().get_variables()['&{SUITE_METADATA}']
         # Set metadata at top level
         BuiltIn().set_suite_metadata("project", self.sProjectName, top=True)
-        BuiltIn().set_suite_metadata("version_sw", self.rMetaData.sVersionSW, top=True)
-        BuiltIn().set_suite_metadata("version_hw", self.rMetaData.sVersionHW, top=True)
-        BuiltIn().set_suite_metadata("version_test", self.rMetaData.sVersionTest, top=True)
         BuiltIn().set_suite_metadata("machine", self.__getMachineName(), top=True)
         BuiltIn().set_suite_metadata("tester", self.__getUserName(), top=True)
         BuiltIn().set_suite_metadata("testtool", self.rMetaData.sROBFWVersion, top=True)
-        BuiltIn().set_suite_metadata("version", VERSION, top=True)
+        BuiltIn().set_suite_metadata("bundle_version", BUNDLE_VERSION, top=True)
+        if "version_sw" in suiteMetadata and self.rMetaData.sVersionSW == '':
+            pass
+        else:
+            BuiltIn().set_suite_metadata("version_sw", self.rMetaData.sVersionSW, top=True)
+        if "version_hw" in suiteMetadata and self.rMetaData.sVersionHW == '':
+            pass
+        else:
+            BuiltIn().set_suite_metadata("version_hw", self.rMetaData.sVersionHW, top=True)
+        if "version_test" in suiteMetadata and self.rMetaData.sVersionTest == '':
+            pass
+        else:
+            BuiltIn().set_suite_metadata("version_test", self.rMetaData.sVersionTest, top=True)
         
         CConfig.oConfigParams = copy.deepcopy(oJsonCfgData)
         
         self.__updateGlobalVariable()
         try:    
             del oJsonCfgData['params']['global']
         except:
             pass  
         
-        try:
-            del oJsonCfgData['preprocessor']['definitions']
-        except:
-            pass 
+        # try:
+        #     del oJsonCfgData['preprocessor']['definitions']
+        # except:
+        #     pass 
         
         bDotdict = False
         dotdictObj = CConfig.CJsonDotDict()
         try:
             jsonDotdict = dotdictObj.dotdictConvert(oJsonCfgData)
             bDotdict = True
         except:
-            logger.info("Could not convert json config to dotdict!!!")
+            logger.info("Could not convert JSON config to dotdict!!!")
             pass
         del dotdictObj
         
         if bDotdict:
             BuiltIn().set_global_variable("${CONFIG}", jsonDotdict)
         else:
             BuiltIn().set_global_variable("${CONFIG}",oJsonCfgData)
         self.bConfigLoaded = True
+
+        if len(oJsonPreprocessor.lUpdatedParams) > 0:
+            for param in oJsonPreprocessor.lUpdatedParams:
+                logger.info(f"The parameter '{param}' is updated")
         
-    def updateCfg(sUpdateCfgFile):
+    def __setGlobalVariable(self, key, value):
         '''
-        staticmethod updateParams: This method updates preprocessor, global or local params base on
-                     ROBFW local config or any json config file according to purpose of
-                     specific testsuite.
-
-        Args:
-            sUpdateCfgFile: str
-        Returns:
-            None              
+This method set RobotFramework AIO global variable from config object.
+
+**Arguments:**
+
+* ``key``
+
+   / *Condition*: required / *Type*: string /
+
+   key is set as global variable of RobotFramework AIO, user can call ${<key>} in test script.
+
+* ``value``
+
+   / *Condition*: required / *Type*: <variant datatypes> /
+
+**Returns:**
+
+* No return variable
         '''
-        oJsonPreprocessor = CJsonPreprocessor(syntax="python", currentCfg=CConfig.oConfigParams)
-        try:
-            oUpdateParams = oJsonPreprocessor.jsonLoad(sUpdateCfgFile)
-        except Exception as error:
-            CConfig.bLoadedCfg = False
-            CConfig.sLoadedCfgError = str(error)
-            logger.error("Loading of JSON configuration file failed! Reason: %s" %(CConfig.sLoadedCfgError))
-            raise Exception
-            
-        if bool(oUpdateParams):
-            CConfig.oConfigParams.update(oUpdateParams)
-        oTmpJsonCfgData = copy.deepcopy(CConfig.oConfigParams)
-        try:    
-            del oTmpJsonCfgData['params']['global']
-        except:
-            pass  
-        
-        try:
-            del oTmpJsonCfgData['preprocessor']['definitions']
-        except:
-            pass
-        
-        BuiltIn().set_global_variable("${CONFIG}", oTmpJsonCfgData)
-        del oTmpJsonCfgData
-        CConfig.__updateGlobalVariable(CConfig)
-        
-    '''
-    private __setGlobalVariable: This method set Robot global variable from config object
-    Args:
-        key: string
-        value: value of key
-    Returns:
-        None
-    '''
-    def __setGlobalVariable(self, key, value):
         k = key
         v = value
         if isinstance(v, dict):
             bDotdict = False
             dotdictObj = CConfig.CJsonDotDict()
             try:
                 jsonDotdict = dotdictObj.dotdictConvert(v)
                 bDotdict = True
             except:
-                logger.info("Could not convert json config to dotdict!!!")
+                logger.info("Could not convert JSON config to dotdict!!!")
                 pass
             del dotdictObj
             if bDotdict:
-                BuiltIn().set_global_variable("${%s}" % k.strip(), jsonDotdict)
+                BuiltIn().set_global_variable(f"${{{k.strip()}}}", jsonDotdict)
             else:
-                BuiltIn().set_global_variable("${%s}" % k.strip(), v)
+                BuiltIn().set_global_variable(f"${{{k.strip()}}}", v)
         elif isinstance(v, list):
             tmpList = []
             for item in v:
                 if isinstance(item, dict):
                     bDotdict = False
                     dotdictObj = CConfig.CJsonDotDict()
                     try:
                         jsonDotdict = dotdictObj.dotdictConvert(item)
                         bDotdict = True
                     except:
-                        logger.info("Could not convert json config to dotdict!!!")
+                        logger.info("Could not convert JSON config to dotdict!!!")
                         pass
                     if bDotdict:
                         tmpList.append(jsonDotdict)
                     else:
                         tmpList.append(item)
                 else:
                     tmpList.append(item)
-            BuiltIn().set_global_variable("${%s}" % k.strip(), tmpList)
+            BuiltIn().set_global_variable(f"${{{k.strip()}}}", tmpList)
         else:         
-            BuiltIn().set_global_variable("${%s}" % k.strip(), v)
+            BuiltIn().set_global_variable(f"${{{k.strip()}}}", v)
             
-    '''
-    private __updateGlobalVariable: This method updates preprocessor and global params to global variable
-                                    of ROBFW
-    Args:
-        None
-    Returns:
-        None
-    '''
     def __updateGlobalVariable(self):
-        try:
-            for k,v in self.oConfigParams['preprocessor']['definitions'].items():
-                try:
-                    self.__setGlobalVariable(k, v)
-                except:
-                    logger.info("The parameter %s is updated" %k.strip())
-                    continue
-        except:
-            pass
+        '''
+This method updates preprocessor and global params to global variable of RobotFramework AIO.
+
+**Arguments:**
+
+* No input parameter is required
+
+**Returns:**
+
+* No return variable
+        '''
+        # try:
+        #     for k,v in self.oConfigParams['preprocessor']['definitions'].items():
+        #         if k in self.lBuitInVariables:
+        #             continue
+        #         try:
+        #             self.__setGlobalVariable(k, v)
+        #         except:
+        #             continue
+        # except:
+        #     pass
         
         try:
             for k,v in self.oConfigParams['params']['global'].items():
+                if k in self.lBuitInVariables:
+                    continue
                 try:
                     self.__setGlobalVariable(k, v)
                 except:
-                    logger.info("The parameter %s is updated" %k.strip())
                     continue
         except:
             pass  
         
-    '''
-    Destructor
-    Args:
-        None
-    Returns:
-        None
-    '''
     def __del__(self):
+        '''
+This destructor method.
+
+**Arguments:**
+
+* No input parameter is required
+
+**Returns:**
+
+* No return variable
+        '''
         pass
     
-    '''
-    private __loadConfigFileLevel2: loads config in case rConfigFiles.sLevel2 == True
-    Args:
-        None
-    Returns:
-        sTestCfgFile: string
-    '''
-    def __loadConfigFileLevel2(self):
+    def __loadConfigFileLevel2(self) -> bool:
+        '''
+This __loadConfigFileLevel2 method loads configuration in case rConfigFiles.bLevel2 == True.
+
+**Arguments:**
+
+* No input parameter is required
+
+**Returns:**
+
+* No return variable
+        '''
         
         oJsonPreprocessor = CJsonPreprocessor(syntax="python")
         try:
-            oSuiteConfig = oJsonPreprocessor.jsonLoad(self.sTestSuiteCfg)
+            oSuiteConfig = oJsonPreprocessor.jsonLoad(CString.NormalizePath(self.sTestSuiteCfg))
         except Exception as error:
             CConfig.bLoadedCfg = False
-            CConfig.sLoadedCfgError = str(error)
-            logger.error("Loading of JSON configuration file failed! Reason: %s" %(CConfig.sLoadedCfgError))
-            raise Exception
-        
+            CConfig.sLoadedCfgError = ''
+            for item in str(error).split(': \''):
+                CConfig.sLoadedCfgError += f"{item}\n                  "
+            logger.error(f"Loading of JSON configuration file failed! \n          Reason: {CConfig.sLoadedCfgError}\n")
+            return False
+        sListOfVariants = '\n'
+        for item in list(oSuiteConfig.keys()):
+            sListOfVariants = sListOfVariants + f"            - '{item}' \n"
+        if not re.match(r'^[a-zA-Z0-9.\u0080-\U0010FFFF\_\-\:@\$]+$', self.sConfigName):
+            CConfig.sLoadedCfgError = "Testsuite management - Loading configuration level 2 failed! \n" + \
+                                      f"          The variant name '{self.sConfigName}' is invalid. \n" + \
+                                      f"          Please find the suitable variant in this list: {sListOfVariants}\n"
+            logger.error(CConfig.sLoadedCfgError)
+            return False
+
+        if self.sConfigName not in oSuiteConfig:
+            CConfig.sLoadedCfgError = "Testsuite management - Loading configuration level 2 failed! \n" + \
+                                     f"          The variant '{self.sConfigName}' is not defined in '{os.path.abspath(self.sTestSuiteCfg)}' \n" + \
+                                     f"          Please find the suitable variant in this list: {sListOfVariants}\n"
+            logger.error(CConfig.sLoadedCfgError)
+            return False
+
         try:
-            defualtCfg = oSuiteConfig['default']['name']
+            self.sTestCfgFile = oSuiteConfig[self.sConfigName]['name']
+            sTestCfgDir = oSuiteConfig[self.sConfigName]['path']
         except:
-            logger.error("Testsuite management is in configuration level2.")
-            logger.error("The file '%s' has no default config or wrong testsuite config format for level 2" %(self.sTestSuiteCfg))
-            logger.error("Testsuite will run with default config file: %s " %(self.sTestCfgFile))
-            return
-        
-        self.sTestCfgFile = oSuiteConfig[self.sConfigName]['name']
-        sTestCfgDir = oSuiteConfig[self.sConfigName]['path']
+            CConfig.sLoadedCfgError = "Testsuite management - Loading configuration level 2 failed! \n" + \
+                                     "          The 'name' or 'path' property is not defined for the variant" + \
+                                    f"'{self.sConfigName}' in '{os.path.abspath(self.sTestSuiteCfg)}'\n"
+            logger.error(CConfig.sLoadedCfgError)
+            return False
+        if self.sTestCfgFile.strip() == '':
+            CConfig.sLoadedCfgError = "Testsuite management - Loading configuration level 2 failed! \n" + \
+                                      f"          The configuration file name of variant '{self.sConfigName}' " + \
+                                      f"must not be empty in '{os.path.abspath(self.sTestSuiteCfg)}'\n"
+            logger.error(CConfig.sLoadedCfgError)
+            return False
             
         if sTestCfgDir.startswith('.../'):
             sTestCfgDirStart = sTestCfgDir
             sTestCfgDir = sTestCfgDir[4:]
-            if os.path.exists(self.sCalcAbsPath(self, './' + sTestCfgDir)):
+            if os.path.exists(CString.NormalizePath('./' + sTestCfgDir)):
                 sTestCfgDir = './' + sTestCfgDir
             else:
                 bFoundTestCfgDir = False
+                sCheckCfgDir = ''
                 for i in range(0, 30):
                     sTestCfgDir = '../' + sTestCfgDir
-                    if os.path.exists(self.sCalcAbsPath(self, sTestCfgDir)):
+                    if sCheckCfgDir == CString.NormalizePath(sTestCfgDir):
+                        break
+                    else:
+                        sCheckCfgDir = CString.NormalizePath(sTestCfgDir)
+                    if os.path.exists(sCheckCfgDir):
                         bFoundTestCfgDir = True
                         break
                 if bFoundTestCfgDir == False:
-                    raise Exception('Could not find out config directory: %s' %(sTestCfgDirStart))
+                    CConfig.sLoadedCfgError = "Testsuite management - Loading configuration level 2 failed! \n" + \
+                                             f"          Could not find out config directory: '{sTestCfgDirStart}'"
+                    logger.error(CConfig.sLoadedCfgError)
+                    return False
                 
-        self.sTestCfgFile = sTestCfgDir + self.sTestCfgFile    
+        self.sTestCfgFile = sTestCfgDir + self.sTestCfgFile
+        return True
     
     @staticmethod
-    def sCalcAbsPath(self, relativePath):
-        '''
-        Staticmethod: sCalcAbsPath
-
-        Args:
-            relativePath: String
-        Returns:
-            absolutePath: String
-        '''
-        sCurDir = os.curdir
-        os.chdir(self.sTestcasePath)
-        absolutePath = os.path.abspath(os.path.relpath(relativePath, os.path.curdir))
-        os.chdir(sCurDir)
-        
-        return absolutePath
-        
-    @staticmethod
-    def sNormalizePath(sPath):
-        '''
-
-staticmethod sNormalizePath:
-
-(remaining content needs to be fixed and restored)
-
+    def __getMachineName():
         '''
-        # '''
-
-# staticmethod sNormalizePath:
-
-# - UNC paths
+This __getMachineName method gets current machine name which is running the test.
 
-    # e.g. \\hi-z4939\ccstg\....
+**Arguments:**
 
-# - escape sequences in windows paths
+* No input parameter is required
 
-    # e.g. c:\robottest\tuner   \t will be interpreted as tab, the result
-    # after processing it with an regexp would be
+**Returns:**
 
-    # c:\robottest   uner
+* ``sMachineName``
 
-# In order to solve this problems any slash will be replaced from backslash
-# to slash, only the two UNC backslashes must be kept if contained.
-
-# Args:
-
-    # sPath: string
-
-# Returns:
-
-    # sNPath: string
-
-        # '''
-        if sPath.strip()=='':
-            return ''
-        
-        if platform.system().lower()!="windows":
-            sPath=re.sub("%(.*?)%","${\\1}",sPath)
-        sNPath=os.path.normpath(os.path.expandvars(sPath.strip()))
-        sNPath=Config.__mkslash(sNPath)
-        
-        return sNPath
-
-    '''
-    staticmethod: __mkslash: Make all backslashes to slash, but mask
-                  UNC indicator \\ before and restore after.
-    Args:
-        sPath: string
-    Returns:
-        sNPath: string
-    '''
-    @staticmethod
-    def __mkslash(sPath):
-        if sPath.strip()=='':
-            return ''
-        
-        sNPath=re.sub(r"\\\\",r"#!#!#",sPath.strip())
-        sNPath=re.sub(r"\\",r"/",sNPath)
-        sNPath=re.sub(r"#!#!#",r"\\\\",sNPath)
-        
-        return sNPath
-        
-    '''
-    Private Method: __read reads data from a XML object
-    Args:
-        oXMLTree: XML object
-        sPath: string
-        sDefault: string
-    Results:
-        sResult: string
-    '''
-    @staticmethod
-    def __read(oXMLTree, sPath, sDefault=None):
-        sResult = oXMLTree.xpath(sPath)[0].strip() if len(oXMLTree.xpath(sPath))>0 else sDefault
-        return sResult
-    
-    '''
-    Private Method: __getMachineName gets current machine name which is running the test.
-    Args:
-        None
-    Returns:
-        sMachineName: string
-    '''
-    @staticmethod
-    def __getMachineName():
+   / *Type*: string /
+        '''
         sMachineName = ''
         # Allows windows system access only in windows systems
         if platform.system().lower()!="windows":
             try:
                 sMachineName = socket.gethostname()
             except Exception(reason):
                 pass
@@ -632,23 +679,29 @@
             try:
                 sMachineName = os.getenv("COMPUTERNAME",'')
             except:
                 pass
             
         return sMachineName
     
-    '''
-    Private method: __getUserName gets current account name login to run the test
-    Args:
-        None
-    Returns:
-        sUserName: string
-    '''
     @staticmethod
     def __getUserName():
+        '''
+This __getUserName method gets current account name login to run the test.
+
+**Arguments:**
+
+* No input parameter is required
+
+**Returns:**
+
+* ``sUserName``
+
+   / *Type*: string /
+        '''
         sUserName = ''
         # Allows windows system access only in windows systems
         if platform.system().lower()!="windows":
             try:
                 sUserName = os.getenv("USER","")
             except:
                 pass
@@ -664,60 +717,134 @@
                 GetUserNameEx(NameDisplay, nameBuffer, size)
                 sUserName = nameBuffer.value
             except:
                 pass
         
         return sUserName
     
-    def verifyRbfwVersion(self):
+    def verifyVersion(self):
         '''
-        Validate the current robotframework version with maximum and minimum 
-        version (if provided in the configuration file).
-        In case the current version is not between min and max version, then
-        the execution of testsuite is terminated with "unknown" state
+This verifyVersion validates the current package version with maximum and 
+minimum version (if provided in the configuration file).
+
+The package version is:
+
+- RobotFramework_TestsuitesManagement version when this module is installed
+stand-alone (via `pip` or directly from sourcecode)
+
+- RobotFramework AIO version when this module is bundled with RobotFramework AIO 
+package
+
+In case the current version is not between min and max version, then the 
+execution of testsuite is terminated with "unknown" state
+
+**Arguments:**
+
+* No input parameter is required
+
+**Returns:**
+
+* No return variable
         '''
-        sCurrentVersion = VERSION
+        sCurrentVersion = BUNDLE_VERSION
         tCurrentVersion = CConfig.tupleVersion(sCurrentVersion)
         
         # Verify format of provided min and max versions then parse to tuples
         tMinVersion = None
         tMaxVersion = None
+        if self.sMinVersion.strip() == '' and self.sMaxVersion.strip() == '':
+            logger.info(f"Running without {BUNDLE_NAME} version check!")
+            return
         if self.sMinVersion != '':
             tMinVersion = CConfig.tupleVersion(self.sMinVersion)
         if self.sMaxVersion != '':
             tMaxVersion = CConfig.tupleVersion(self.sMaxVersion)
-
+        bVersionCheck = True
         if tMinVersion and tMaxVersion and (tMinVersion > tMaxVersion):
             self.versioncontrol_error('wrong_minmax', self.sMinVersion, self.sMaxVersion)
-
+            bVersionCheck = False
         if tMinVersion and not CConfig.bValidateMinVersion(tCurrentVersion, tMinVersion):
             self.versioncontrol_error('conflict_min', self.sMinVersion, sCurrentVersion)
-
+            bVersionCheck = False
         if tMaxVersion and not CConfig.bValidateMaxVersion(tCurrentVersion, tMaxVersion):
             self.versioncontrol_error('conflict_max', self.sMaxVersion, sCurrentVersion)
+            bVersionCheck = False
+
+        if bVersionCheck:
+            logger.info(f"{BUNDLE_NAME} version check passed!")
 
     @staticmethod
     def bValidateMinVersion(tCurrentVersion, tMinVersion):
         '''
-        Validate current version with required minimun version.
+This bValidateMinVersion validates the current version with required minimun version.
+
+**Arguments:**
+
+* ``tCurrentVersion``
+
+  / *Condition*: required / *Type*: tuple /
+
+  Current package version.
+
+* ``tMinVersion``
+
+  / *Condition*: required / *Type*: tuple /
+
+  The minimum version of package.
+
+**Returns:**
+
+* ``True`` or ``False``
         '''
         return tCurrentVersion >= tMinVersion
 
     @staticmethod
     def bValidateMaxVersion(tCurrentVersion, tMaxVersion):
         '''
-        Validate current version with required maximun version.
+This bValidateMaxVersion validates the current version with required minimun version.
+
+**Arguments:**
+
+* ``tCurrentVersion``
+
+  / *Condition*: required / *Type*: tuple /
+
+  Current package version.
+
+* ``tMinVersion``
+
+  / *Condition*: required / *Type*: tuple /
+
+  The minimum version of package.
+
+**Returns:**
+
+* ``True or False``
         '''
         return tCurrentVersion <= tMaxVersion
 
     @staticmethod
     def bValidateSubVersion(sVersion):
         '''
-        Validate the format of provided sub version and parse it into sub tuple
-        for version comparision.
+This bValidateSubVersion validates the format of provided sub version and parse 
+it into sub tuple for version comparision.
+
+**Arguments:**
+
+* ``sVersion``
+
+  / *Condition*: required / *Type*: string /
+
+  The version of package.
+
+**Returns:**
+
+* ``lSubVersion``
+
+  / *Type*: tuple /
         '''
         lSubVersion = [0,0,0]
         oMatch = re.match(r"^(\d+)(?:-?(a|b|rc)(\d*))?$", sVersion)
         if oMatch:
             lSubVersion[0] = int(oMatch.group(1))
             # a < b < rc < released (without any character)
             if oMatch.group(2):
@@ -738,66 +865,102 @@
             return tuple(lSubVersion)
         else:
             raise Exception("Wrong format in version info")
             
     @staticmethod
     def tupleVersion(sVersion):
         '''
-Return a tuple which contains the (major, minor, patch) version.
+This tupleVersion returns a tuple which contains the (major, minor, patch) version.
+
+In case minor/patch version is missing, it is set to 0.
+E.g: "1" is transformed to "1.0.0" and "1.1" is transformed to "1.1.0"
+            
+This tupleVersion also support version which contains Alpha (a), Beta (b) or 
+Release candidate (rc): E.g: "1.2rc3", "1.2.1b1", ...
+
+**Arguments:**
+
+* ``sVersion``
+
+  / *Condition*: required / *Type*: string /
+
+  The version of package.
+
+**Returns:**
+
+* ``lVersion``
+
+  / *Type*: tuple /
+
+  A tuple which contains the (major, minor, patch) version.
 
-(remaining content needs to be fixed and restored)
 
         '''
-        # '''
-        # Return a tuple which contains the (major, minor, patch) version.
-          # - In case minor/patch version is missing, it is set to 0.
-            # E.g: 1   => 1.0.0
-                 # 1.1 => 1.1.0
-          # - Support version contains Alpha (a), Beta (b) or Release candidate (rc):
-            # E.g: 1.2rc3, 1.2.1b1, ...
-        # '''
         lVersion = sVersion.split(".")
         if len(lVersion) == 1:
             lVersion.extend(["0", "0"])
         elif len(lVersion) == 2:
             lVersion.append("0")
         elif len(lVersion) >= 3:
             # Just ignore and remove the remaining 
             lVersion = lVersion[:3]
         try:
             # verify the version info is a number
             return tuple(map(lambda x: CConfig.bValidateSubVersion(x), lVersion))
         except Exception:
-            BuiltIn().fatal_error("Provided version '%s' is not a correct version format."%sVersion)
+            BuiltIn().fatal_error(f"Provided version '{sVersion}' is not a correct version format.")
 
     def versioncontrol_error(self, reason, version1, version2):
         '''
-        Wrapper version control error log:
-        Log error message of version control due to reason and set to unknown state.
-        `reason` can only be "conflict_min", "conflict_max" and "wrong_minmax".
+Wrapper version control error log:
+
+Log error message of version control due to reason and set to unknown state.
+
+**Arguments:**
+
+* ``reason``
+
+  / *Condition*: required / *Type*: string /
+
+  ``reason`` can only be ``conflict_min``, ``conflict_max`` and ``wrong_minmax``.
+
+* ``version1``
+
+  / *Condition*: required / *Type*: string /
+
+* ``version2``
+
+  / *Condition*: required / *Type*: string /
+
+**Returns:**
+
+* No return variable
         '''
-        sLocation = "\\\\bosch.com\\dfsrb\\DfsDE\\DIV\\CM\\DI\\Projects\\Common\\RobotFramework\\Releases"
+
         header = ""
         detail = ""
         if reason=="conflict_min":
             header = "Version conflict."
-            detail = f"\nThe configuration requires minimum Robotframework version '{version1}'"
-            detail +=f"\nbut the installed Robotframework version is older         '{version2}'"
+            detail = f"\nThe test execution requires minimum {BUNDLE_NAME} version '{version1}'"
+            detail +=f"\nbut the installed {BUNDLE_NAME} version is older          '{version2}'"
         elif reason=="conflict_max":
             header = "Version conflict."
-            detail = f"\nThe configuration requires maximum Robotframework version '{version1}'"
-            detail +=f"\nbut the installed Robotframework version is younger       '{version2}'"
+            detail = f"\nThe test execution requires maximum {BUNDLE_NAME} version '{version1}'"
+            detail +=f"\nbut the installed {BUNDLE_NAME} version is younger        '{version2}'"
         elif reason=="wrong_minmax":
             header = "Wrong use of max/min version control in configuration."
-            detail = f"\nThe configured minimum Robotframework version                 '{version1}'"
-            detail +=f"\nis younger than the configured maximum Robotframework version '{version2}'"
+            detail = f"\nThe configured minimum {BUNDLE_NAME} version                 '{version1}'"
+            detail +=f"\nis younger than the configured maximum {BUNDLE_NAME} version '{version2}'"
             detail +="\nPlease correct the values of 'Maximum_version', 'Minimum_version' in config file"
         else:
             return
         
         BuiltIn().log(f"{header}" +
         f"\nTestsuite : {BuiltIn().get_variable_value('${SUITE SOURCE}')}" +
         f"\nconfig    : {self.sTestCfgFile}" +
         f"\n{detail}\n"
-        "\nPlease install the required RobotFramework AIO version." +
-        f"\nYou can find an installer here: {sLocation}\n", "ERROR")
-        BuiltIn().unknown()        
+        f"\nPlease install the required {BUNDLE_NAME} version." +
+        f"\nYou can find an installer here: {INSTALLER_LOCATION}\n", "ERROR")
+        BuiltIn().unknown('Version control error!!!')
+
+if __name__ == "__main__":
+    bundle_version()
```

### Comparing `robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Config/__init__.py` & `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2022 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from .CConfig import CConfig, VERSION
+from .CConfig import CConfig, bundle_version, BUNDLE_VERSION
```

### Comparing `robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Keywords/COnFailureHandle.py` & `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Keywords/COnFailureHandle.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2022 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,12 +17,12 @@
 
 class COnFailureHandle():
     
     @not_keyword
     def is_noney(self, item):
         return item is None or is_string(item) and item.upper() == 'NONE'
     
-    @keyword
-    def register_keyword_run_on_failure(self, keyword):
-        '''
-        TBD
-        '''
+    # @keyword
+    # def register_keyword_run_on_failure(self, keyword):
+    #     '''
+    #     TBD
+    #     '''
```

### Comparing `robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Keywords/CSetup.py` & `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Keywords/CSetup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,137 +1,200 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2022 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import copy
+import os
 
-import RobotFramework_Testsuites
+import RobotFramework_TestsuitesManagement
 from robot.api.deco import keyword
 from robot.api import logger
 
-from RobotFramework_Testsuites.Config import CConfig
+from RobotFramework_TestsuitesManagement.Config import CConfig
 
 from lxml import etree
 
 from robot.libraries.BuiltIn import BuiltIn
 
 
 
 
 class CSetupKeywords(object):
     '''
-    Definition setup keywords
+This CSetupKeywords class uses to define the setup keywords which are using in suite setup and teardown of
+robot test script.
+
+``Testsuite Setup`` keyword loads the RobotFramework AIO configuration, checks the version of RobotFramework AIO,
+and logs out the basic information of the robot run.
+
+``Testsuite Teardown`` keyword currently do nothing, it's defined here for future requirements.
+
+``Testcase Setup`` keyword currently do nothing, it's defined here for future requirements.
+
+``Testcase Teardown`` keyword currently do nothing, it's defined here for future requirements.
     '''
 
     @keyword
     def testsuite_setup(self, sTestsuiteCfgFile=''):
-        if not RobotFramework_Testsuites.CTestsuitesCfg.oConfig.bLoadedCfg:
-            BuiltIn().unknown("Loading of %s" %(CConfig.sLoadedCfgError))
+        '''
+This testsuite_setup defines the ``Testsuite Setup`` which is used to loads the RobotFramework AIO configuration,
+checks the version of RobotFramework AIO, and logs out the basic information of the robot run.
+
+**Arguments:**
+
+* ``sTestsuiteCfgFile``
+
+  / *Condition*: required / *Type*: string /
+
+  ``sTestsuiteCfgFile=''`` and variable ``config_file`` is not set RobotFramework AIO will check for configuration
+  level 3, and level 4.
+
+  ``sTestsuiteCfgFile`` is set with a <json_config_file_path> and variable ``config_file`` is not set RobotFramework AIO 
+  will load configuration level 2.
+
+**Returns:**
+
+* No return variable
+        '''
+        if not RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.bLoadedCfg:
+            BuiltIn().unknown(CConfig.sLoadedCfgError)
             return
         else:
-            if not RobotFramework_Testsuites.CTestsuitesCfg.oConfig.rConfigFiles.sLevel1:
+            if not RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel1:
                 if sTestsuiteCfgFile != '':
-                    RobotFramework_Testsuites.CTestsuitesCfg.oConfig.rConfigFiles.sLevel2 = True
-                    RobotFramework_Testsuites.CTestsuitesCfg.oConfig.rConfigFiles.sLevel4 = False
-                    RobotFramework_Testsuites.CTestsuitesCfg.oConfig.sTestSuiteCfg = sTestsuiteCfgFile
-                    try:
-                        RobotFramework_Testsuites.CTestsuitesCfg.oConfig.loadCfg(RobotFramework_Testsuites.CTestsuitesCfg.oConfig)
-                    except Exception as error:
-                        BuiltIn().unknown("Loading of %s" %(CConfig.sLoadedCfgError))
+                    RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel2 = True
+                    RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel4 = False
+                    RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestSuiteCfg = os.path.abspath(sTestsuiteCfgFile)
+                    RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.loadCfg(RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig)
                 else:
-                    RobotFramework_Testsuites.CTestsuitesCfg.oConfig.rConfigFiles.sLevel3 = True
-                    RobotFramework_Testsuites.CTestsuitesCfg.oConfig.rConfigFiles.sLevel4 = False
-                    try:
-                        RobotFramework_Testsuites.CTestsuitesCfg.oConfig.loadCfg(RobotFramework_Testsuites.CTestsuitesCfg.oConfig)
-                    except Exception as error:
-                        BuiltIn().unknown("Loading of %s" %(CConfig.sLoadedCfgError))
-            else:
-                logger.warn('The configuration level 1 is set for this Robot run! \nThe configuration \"%s\" is using as highest priority' \
-                    %(RobotFramework_Testsuites.CTestsuitesCfg.oConfig.sTestCfgFile))
-
-        if RobotFramework_Testsuites.CTestsuitesCfg.oConfig.rConfigFiles.sLevel1:
-            logger.info('Running with configuration level: 1')
-        elif RobotFramework_Testsuites.CTestsuitesCfg.oConfig.rConfigFiles.sLevel2:
-            logger.info('Running with configuration level: 2')
-            if RobotFramework_Testsuites.CTestsuitesCfg.oConfig.bConfigLoaded:
-                logger.info("The parameters in \"%s\" will be added into configuration object" \
-                    %(RobotFramework_Testsuites.CTestsuitesCfg.oConfig.sTestCfgFile))
-        elif RobotFramework_Testsuites.CTestsuitesCfg.oConfig.rConfigFiles.sLevel3:
-            logger.info('Running with configuration level: 3')
-            if RobotFramework_Testsuites.CTestsuitesCfg.oConfig.bConfigLoaded:
-                logger.info("The parameters in \"%s\" will be added into configuration object" \
-                    %(RobotFramework_Testsuites.CTestsuitesCfg.oConfig.sTestCfgFile))
+                    RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel3 = True
+                    RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel4 = False
+                    RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.loadCfg(RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig)
+            # else:
+            #     logger.warn(f"Running with configuration level 1! \nSelected configuration file '{RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestCfgFile}'")
+
+        if RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel1:
+            logger.info('Running with configuration level 1')
+        elif RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel2:
+            logger.info('Running with configuration level 2')
+            if RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.bConfigLoaded:
+                logger.info(f"Parameters loaded from '{RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestCfgFile}'")
+        elif RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.rConfigFiles.bLevel3:
+            logger.info('Running with configuration level 3')
+            if RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.bConfigLoaded:
+                logger.info(f"Parameters loaded from '{RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestCfgFile}'")
         else:
-            logger.info('Running with configuration level: 4')
+            logger.warn(f"Running with configuration level 4! \nSelected configuration file '{RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestCfgFile}'")
 
-        RobotFramework_Testsuites.CTestsuitesCfg.oConfig.verifyRbfwVersion()
-        logger.info('Suite Path: %s' %(RobotFramework_Testsuites.CTestsuitesCfg.oConfig.sTestcasePath))
-        logger.info('CfgFile Path: %s' %(RobotFramework_Testsuites.CTestsuitesCfg.oConfig.sTestCfgFile))
-        logger.info('Suite Count: %s' %(RobotFramework_Testsuites.CTestsuitesCfg.oConfig.iSuiteCount))
-        logger.info('Total testcases in TestSuite "%s" is: %s' %( \
-            RobotFramework_Testsuites.CTestsuitesCfg.oConfig.sRootSuiteName, \
-            RobotFramework_Testsuites.CTestsuitesCfg.oConfig.iTotalTestcases))
+        RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.verifyVersion()
+        logger.info(f"Suite Path: '{RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestcasePath}'")
+        logger.info(f"CfgFile Path: '{RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sTestCfgFile}'")
+        if RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sLocalConfig != '':
+            logger.info(f"Local config file: '{RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.sLocalConfig}'")
+        logger.info(f"Number of test suites: {RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.iSuiteCount}")
+        logger.info(f"Total number of testcases: {RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.iTotalTestcases}")
         
     @keyword
     def testsuite_teardown(self):
+        '''
+This testsuite_teardown defines the ``Testsuite Teardown`` keyword, currently this keyword does nothing,
+it's defined here for future requirements.
+        '''
         logger.info('testsuite_teardown: Will be implemented later')
         
     @keyword
     def testcase_setup(self):
-        logger.info('Test Count: %s' %(RobotFramework_Testsuites.CTestsuitesCfg.oConfig.iTestCount))
+        '''
+This testcase_setup defines the ``Testcase Setup`` keyword, currently this keyword does nothing,
+it's defined here for future requirements.
+        '''
+        logger.info(f"Test Count: {RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.iTestCount}")
         
     @keyword
     def testcase_teardown(self):
+        '''
+This testcase_teardown defines the ``Testcase Teardown`` keyword, currently this keyword does nothing,
+it's defined here for future requirements.
+        '''
         logger.info('testcase_teardown: Will be implemented later')
         
-    @keyword
-    def update_config(self, sCfgFile):
-        CConfig.updateCfg(sCfgFile)
-        
 class CGeneralKeywords(object):
     '''
-    Definition setup keywords
+This CGeneralKeywords class defines the keywords which will be using in RobotFramework AIO test script.
+
+``Get Config`` keyword gets the current config object of robot run.
+
+``Load Json`` keyword loads json file then return json object.
+
+In case new robot keyword is required, it will be defined and implemented in this class.
     '''
      
     @keyword
     def get_config(self):
         '''
-        oConfigParams: is the dictionary consist of some configuration params which 
-        are return to user from get_config_params keyword
+This get_config defines the ``Get Config`` keyword gets the current config object of RobotFramework AIO.
+
+**Arguments:**
+
+* No parameter is required
+
+**Returns:**
+
+* ``oConfig.oConfigParams``
+
+  / *Type*: json /
         '''
-        return copy.deepcopy(RobotFramework_Testsuites.CTestsuitesCfg.oConfig.oConfigParams)
+        return copy.deepcopy(RobotFramework_TestsuitesManagement.CTestsuitesCfg.oConfig.oConfigParams)
     
     @keyword
     def load_json(self, jsonfile, level=1, variant='default'):
         '''
-        This keyword uses to load json file then return json object.
-           - Level = 1 -> loads the content of jsonfile.
-           - level != 1 -> loads the json file which is set with variant (likes loading
-             config level2)
+Loads a json file and returns a json object.
+
+**Arguments:**
+
+* ``jsonfile``
+
+  / *Condition*: required / *Type*: string /
+
+  The path of Json configuration file.
+
+* ``level``
+
+  / *Condition*: required / *Type*: int /
+
+  Level = 1 -> loads the content of jsonfile.
+
+  level != 1 -> loads the json file which is set with variant (likes loading config level2)
+
+**Returns:**
+
+* ``oJsonData``
+
+  / *Type*: json /
         '''
         import os
         from os.path import abspath, dirname
         from JsonPreprocessor import CJsonPreprocessor
         jsonFileDir = dirname(abspath(jsonfile))
         oJsonPreprocessor = CJsonPreprocessor()
         if level == 1:
             oJsonData = oJsonPreprocessor.jsonLoad(jsonfile)
             return oJsonData
         else:
             oJsonFristLevel = oJsonPreprocessor.jsonLoad(jsonfile)
             if variant not in oJsonFristLevel:
-                logger.error('The variant: %s is not correct' % variant)
+                logger.error(f"The variant: {variant} is not correct!\n")
                 return {}
             jsonFileLoaded = jsonFileDir + oJsonFristLevel[variant]['path'] + '/' + oJsonFristLevel[variant]['name']
             oJsonData = oJsonPreprocessor.jsonLoad(jsonFileLoaded)
             return oJsonData
-
```

### Comparing `robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Keywords/__init__.py` & `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2022 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from .CSetup import CSetupKeywords, CGeneralKeywords
+
+from .LibListener import LibListener
+from .CStruct import CStruct
```

### Comparing `robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Utils/CStruct.py` & `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/CStruct.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2022 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,32 +16,34 @@
 # File: CStruct.py
 # Initially created by Mai Dinh Nam Son (RBVH/ECM11) / Dec-2020
 # Base on file lib\Misc\CStruct.py of TML Framework (Author: Pollerspoeck Thomas)
 #
 #
 #################################################################################
 
-'''
-This class provides the "struct" functionality of "C/C++" in python.
-It simply helps to organize data which belongs logically together.
-
-Usage: oStruct=CStruct(attribute_1=value_1, ... attribute_n=value_n)
-       oStruct.attribute_1="....."
-'''
+# '''
+# This class provides the "struct" functionality of "C/C++" in python.
+# It simply helps to organize data which belongs logically together.
+
+# Usage: oStruct=CStruct(attribute_1=value_1, ... attribute_n=value_n)
+       # oStruct.attribute_1="....."
+# '''
 
 class CStruct:
     '''
-    Constructor __init__ creates the given attributes dynamically at runtime.
+This ``CStruct`` class creates the given attributes dynamically at runtime.
+    '''
 
-    Args:
+    def __init__(self, *args, **kwargs):
+        '''
+The constructor __init__ creates the given attributes dynamically at runtime.
 
-        Attributes to be created with the initial value
+**Arguments:**
 
-    Returns:
+Attributes to be created with the initial value.
 
-        Accessible attributes
-    '''
+**Returns:**
 
-    def __init__(self, *args, **kwargs):
+Accessible attributes.
+        '''
         for k, v in kwargs.items():
             setattr(self, k, v)
-
```

### Comparing `robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Utils/Events/Event.py` & `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/Events/Event.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2022 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,8 +16,7 @@
 
 
 class Event(object):
     
     @abc.abstractmethod
     def trigger(self, *args, **kwargs):
         pass
-
```

### Comparing `robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Utils/Events/ScopeEvent.py` & `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/Events/ScopeEvent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2022 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -36,9 +36,7 @@
             
        
 class ScopeStart(ScopeEvent):
     name = 'scope_start'
     
 class ScopeEnd(ScopeEvent):
     name = 'scope_end'
-            
-
```

### Comparing `robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Utils/Events/__init__.py` & `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Utils/Events/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2022 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -32,8 +32,8 @@
         if event.name == event_name:
             event.trigger(*args, **kwargs)
             
 def register_event(event):
     for registered_event in _registered_events:
         if event.name == registered_event.name:
             raise AttributeError('An event with the name ' + event.name + ' already exists.')
-    _registered_events.append(event)
+    _registered_events.append(event)
```

### Comparing `robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/Utils/__init__.py` & `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/Keywords/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2022 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-
-from .LibListener import LibListener
-from .CStruct import CStruct
+from .CSetup import CSetupKeywords, CGeneralKeywords
```

### Comparing `robotframework-testsuitesmanagement-0.5.1/RobotFramework_Testsuites/__init__.py` & `robotframework-testsuitesmanagement-0.7.1/RobotFramework_TestsuitesManagement/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2022 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,98 +17,98 @@
 from robot.errors import DataError
 from robot.libraries.BuiltIn import BuiltIn
 from robot.utils import is_string
 from robot.utils.importer import Importer
 
 from robotlibcore import DynamicCore
 
-from RobotFramework_Testsuites.Utils import LibListener
-from RobotFramework_Testsuites.Keywords import (CSetupKeywords, CGeneralKeywords)
-from RobotFramework_Testsuites.Config import VERSION
-
-__version__ = '0.0.1'
+from RobotFramework_TestsuitesManagement.Utils import LibListener
+from RobotFramework_TestsuitesManagement.Keywords import (CSetupKeywords, CGeneralKeywords)
+from RobotFramework_TestsuitesManagement.Config import BUNDLE_VERSION as VERSION
 
 
-class RobotFramework_Testsuites(DynamicCore):
-    '''
-    RobotFramework_Testsuites is the Bosch testing library for Robot Framework.
-    RobotFramework_Testsuites control peripheral devices, tools and target under testing.
-    '''
+class RobotFramework_TestsuitesManagement(DynamicCore):
+    # '''
+    # **Class: RobotFramework_TestsuitesManagement**
+
+       # RobotFramework_TestsuitesManagement is the Bosch testing library for Robot Framework.
+
+       # RobotFramework_TestsuitesManagement control peripheral devices, tools and target under testing.
+    # '''
     ROBOT_LIBRARY_SCOPE = 'GLOBAL'
-    ROBOT_LIBRARY_VERSION = __version__
+    ROBOT_LIBRARY_VERSION = VERSION
     
-    '''
-    Constructor
-    Args:
-        None
-    Returns:
-        None
-    '''
+    # '''
+    # Constructor
+    # Args:
+        # None
+    # Returns:
+        # None
+    # '''
     def __init__(self, timeout=10.0):
         self.timeout = timeout
         self._running_on_failure_keyword = False
         self.run_on_failure_keyword = None # will update later 
         libraries = [CSetupKeywords(), CGeneralKeywords()]
         self.ROBOT_LIBRARY_LISTENER = LibListener()
         self._running_keyword = None
         DynamicCore.__init__(self, libraries)
     
-    '''
-    Method: run_keyword
-    Args:
-        name: string
-    Returns:
-        DynamicCore.run_keyword
-    '''
+    # '''
+    # Method: run_keyword
+    # Args:
+        # name: string
+    # Returns:
+        # DynamicCore.run_keyword
+    # '''
     def run_keyword(self, name, args, kwargs):
         try:
             return DynamicCore.run_keyword(self, name, args, kwargs)
         except Exception:
             self.failure_occurred()
             raise
         
-    '''
-    Method: get_keyword_tags
-    Args:
-        name: String
-    Returns:
-        tags
-    '''
+    # '''
+    # Method: get_keyword_tags
+    # Args:
+        # name: String
+    # Returns:
+        # tags
+    # '''
     def get_keyword_tags(self, name):
         tags = list(DynamicCore.get_keyword_tags(self, name))
         return tags
         
-    '''
-    Method: get_keyword_documentation
-    Args:
-        name: string
-    Returns:
-        DynamicCore.get_keyword_documentation
-    '''
+    # '''
+    # Method: get_keyword_documentation
+    # Args:
+        # name: string
+    # Returns:
+        # DynamicCore.get_keyword_documentation
+    # '''
     def get_keyword_documentation(self, name):
         return DynamicCore.get_keyword_documentation(self, name)
     
-    '''
-    Method: failure_occurred is executed when RobotFramework_Testsuites keyword fails.
-    By default, executes the registered run-on-failure keyword. RobotFramework_Testsuites can 
-    overwrite this hook method in case provides custom functionality instead.
-    Args:
-        None
-    Returns:
-        None
-    '''        
+    # '''
+    # Method: failure_occurred is executed when RobotFramework_TestsuitesManagement keyword fails.
+    # By default, executes the registered run-on-failure keyword. RobotFramework_TestsuitesManagement can 
+    # overwrite this hook method in case provides custom functionality instead.
+    # Args:
+        # None
+    # Returns:
+        # None
+    # '''        
     def failure_occurred(self):
         if self._running_on_failure_keyword or not self.run_on_failure_keyword:
             return None
         try:
             self._running_on_failure_keyword = True
             BuiltIn().run_keyword(self.run_on_failure_keyword)
         except Exception as error:
-            logger.warn("Keyword '%s' could not be run on failure: '%s'"
-                        % (self.run_on_failure_keyword, error))
+            logger.warn(f"Keyword '{self.run_on_failure_keyword}' could not be run on failure: '{error}'")
         finally:
             self._running_on_failure_keyword = False
 
 class CTestsuitesCfg():
     oConfig = None
     
     def __init__(self):
```

### Comparing `robotframework-testsuitesmanagement-0.5.1/robotframework_testsuitesmanagement.egg-info/SOURCES.txt` & `robotframework-testsuitesmanagement-0.7.1/robotframework_testsuitesmanagement.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
-RobotFramework_Testsuites/__init__.py
-RobotFramework_Testsuites/version.py
-RobotFramework_Testsuites/Config/CConfig.py
-RobotFramework_Testsuites/Config/__init__.py
-RobotFramework_Testsuites/Config/robot_config.json
-RobotFramework_Testsuites/Config/robot_schema.json
-RobotFramework_Testsuites/Keywords/COnFailureHandle.py
-RobotFramework_Testsuites/Keywords/CSetup.py
-RobotFramework_Testsuites/Keywords/__init__.py
-RobotFramework_Testsuites/Utils/CStruct.py
-RobotFramework_Testsuites/Utils/LibListener.py
-RobotFramework_Testsuites/Utils/__init__.py
-RobotFramework_Testsuites/Utils/Events/Event.py
-RobotFramework_Testsuites/Utils/Events/ScopeEvent.py
-RobotFramework_Testsuites/Utils/Events/__init__.py
+RobotFramework_TestsuitesManagement/__init__.py
+RobotFramework_TestsuitesManagement/version.py
+RobotFramework_TestsuitesManagement/Config/CConfig.py
+RobotFramework_TestsuitesManagement/Config/__init__.py
+RobotFramework_TestsuitesManagement/Keywords/COnFailureHandle.py
+RobotFramework_TestsuitesManagement/Keywords/CSetup.py
+RobotFramework_TestsuitesManagement/Keywords/__init__.py
+RobotFramework_TestsuitesManagement/Utils/CStruct.py
+RobotFramework_TestsuitesManagement/Utils/LibListener.py
+RobotFramework_TestsuitesManagement/Utils/__init__.py
+RobotFramework_TestsuitesManagement/Utils/Events/Event.py
+RobotFramework_TestsuitesManagement/Utils/Events/ScopeEvent.py
+RobotFramework_TestsuitesManagement/Utils/Events/__init__.py
 robotframework_testsuitesmanagement.egg-info/PKG-INFO
 robotframework_testsuitesmanagement.egg-info/SOURCES.txt
 robotframework_testsuitesmanagement.egg-info/dependency_links.txt
 robotframework_testsuitesmanagement.egg-info/entry_points.txt
 robotframework_testsuitesmanagement.egg-info/requires.txt
 robotframework_testsuitesmanagement.egg-info/top_level.txt
```

### Comparing `robotframework-testsuitesmanagement-0.5.1/setup.py` & `robotframework-testsuitesmanagement-0.7.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 #
 # **************************************************************************************************************
 #
 # setup.py
 #
 # XC-CT/ECA3-Queckenstedt
 #
-# Extends the standard setuptools installation by adding the documentation in HTML format
+# Extends the standard setuptools installation by adding the documentation in PDF format
 # (requires installation mode) and tidying up some folders.
 #
 # !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 #
-# This script deletes folders (as defined in config.CConfig, depending on the position of this script):
+# This script deletes folders (as defined in config.CRepositoryConfig, depending on the position of this script):
 # - previous builds within this repository
 # - previous installations within
 #   * <Python installation>\Lib\site-packages (Windows)
 #   * <Python installation>/../lib/python3.9/site-packages (Linux)
 #
 # before the build and the installation start again!
 #
@@ -40,55 +40,43 @@
 # --------------------------------------------------------------------------------------------------------------
 #
 # * Hints:
 #
 # The usual
 #    packages = setuptools.find_packages(),
 # is replaced by
-#    packages = [str(oRepositoryConfig.Get('sPackageName')), ],
-# to avoid that also config.CConfig() and config.CExtendedSetup() are part of the distribution.
-# CConfig and CExtendedSetup() are only repository internal helper.
+#    packages = [str(oRepositoryConfig.Get('PACKAGENAME')), ],
+# to avoid that also config.CRepositoryConfig() and additions.CExtendedSetup() are part of the distribution.
+# CRepositoryConfig and CExtendedSetup() are only repository internal helper.
 #
 # * Known issues:
 #
 #   - setuptools do not properly update an existing package installation under <Python installation>\Lib\site-packages\<package name>!
 #     > Files modified manually within installation folder, are still modified after repeated execution of setuptools.
 #     > Files added manually within installation folder, are still present there after repeated execution of setuptools.
 #     > Only files deleted manually within installation folder, are are restored there after repeated execution of setuptools.
 #   - No such issues with <Python installation>\Lib\site-packages\<package name>-<versions>.egg-info.
 #   - Solution: explicit deletion of all previous output (all documentation-, build- and installation-folder, except the egg-info folder)
 #     (see 'delete_previous_build()' and 'delete_previous_installation()')
 #
 # --------------------------------------------------------------------------------------------------------------
 #
-# 11.03.2022 / XC-CT/ECA3-Queckenstedt
-# 'package_dir' added
-#
-# 07.03.2022 / XC-CT/ECA3-Queckenstedt
-# Fixed 'packages' listing and the installation of additional files (json)
-#
-# 22.02.2022 / XC-CT/ECA3-Queckenstedt
-# "sdist bdist_wheel" maintenance: some steps moved from inside 'ExtendedInstallCommand' to outside
-#
-# 11.10.2021 / XC-CI1/ECA3-Queckenstedt
-# Fixed computation order of readme files together with long_description
-# 
-# 30.09.2021 / XC-CI1/ECA3-Queckenstedt
-# Added wrapper for error messages
-# 
-# Initial version 08/2021
+# 29.06.2022
 #
 # --------------------------------------------------------------------------------------------------------------
 
 import os, sys, platform, shlex, subprocess
 import setuptools
 from setuptools.command.install import install
 
-from config.CConfig import CConfig # providing repository and environment specific information
-from config.CExtendedSetup import CExtendedSetup # providing functions to support the extended setup process
+# prefer the repository local version of all additional libraries (instead of the installed version under site-packages)
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "./additions")))
+
+from config.CRepositoryConfig import CRepositoryConfig # providing repository and environment specific information
+from additions.CExtendedSetup import CExtendedSetup # providing functions to support the extended setup process
 
 import colorama as col
 
 col.init(autoreset=True)
 
 COLBR = col.Style.BRIGHT + col.Fore.RED
 COLBY = col.Style.BRIGHT + col.Fore.YELLOW
@@ -110,50 +98,28 @@
 class ExtendedInstallCommand(install):
     """Extended setup for installation mode."""
 
     def run(self):
 
         listCmdArgs = sys.argv
         if ( ('install' in listCmdArgs) or ('build' in listCmdArgs) or ('sdist' in listCmdArgs) or ('bdist_wheel' in listCmdArgs) ):
-            print()
-            print(COLBY + "Extended setup step 4/5: install.run(self)") # creates the build folder .\build
-            print()
             install.run(self)
-            print()
-            if 'bdist_wheel' in listCmdArgs:
-                print(COLBY + "Extended setup step 5/5: Add html documentation to local wheel folder inside build")
-                print()
-                nReturn = oExtendedSetup.add_htmldoc_to_wheel()
-                if nReturn != SUCCESS:
-                    return nReturn
-                print()
-            else:
-                print(COLBY + "Extended setup step 5/5: Add html documentation to package installation folder") # (./doc/_build/html to <Python installation>\Lib\site-packages\<package name>_doc)
-                print()
-                nReturn = oExtendedSetup.add_htmldoc_to_installation()
-                if nReturn != SUCCESS:
-                    return nReturn
-                print()
-            print(COLBG + "Extended installation done")
-            print()
-
         return SUCCESS
 
 # eof class ExtendedInstallCommand(install):
 
 # --------------------------------------------------------------------------------------------------------------
 
 # -- Even in case of other command line parameters than 'install' or 'build' are used we need the following objects.
 #    (Without repository configuration commands like '--author-email' would not be possible)
 
 # -- setting up the repository configuration
 oRepositoryConfig = None
-sReferencePath = os.path.dirname(os.path.abspath(sys.argv[0]))
 try:
-    oRepositoryConfig = CConfig(sReferencePath)
+    oRepositoryConfig = CRepositoryConfig(os.path.abspath(sys.argv[0]))
 except Exception as ex:
     print()
     printexception(str(ex))
     print()
     sys.exit(ERROR)
 
 # -- setting up the extended setup
@@ -173,77 +139,97 @@
 listCmdArgs = sys.argv
 if ( ('install' in listCmdArgs) or ('build' in listCmdArgs) or ('sdist' in listCmdArgs) or ('bdist_wheel' in listCmdArgs) ):
     print()
     print(COLBY + "Entering extended installation")
     print()
 
     print(COLBY + "Extended setup step 1/5: Calling the documentation builder")
-    # (previously called inside ExtendedInstallCommand - but this is too late, because the content of the initially
-    # generated or updated README file is already needed for the long_description below.)
     print()
-    nReturn = oExtendedSetup.gen_doc()
+
+    nReturn = oExtendedSetup.genpackagedoc()
     if nReturn != SUCCESS:
         sys.exit(nReturn)
 
-    print(COLBY + "Extended setup step 2/5: Deleting previous setup outputs (build, dist, <package name>.egg-info within repository)")
+    print(COLBY + "Extended setup step 2/5: Converting the repository README")
+    print()
+
+    nReturn = oExtendedSetup.convert_repo_readme()
+    if nReturn != SUCCESS:
+        sys.exit(nReturn)
+
+    print(COLBY + "Extended setup step 3/5: Deleting previous setup outputs (build, dist, <package name>.egg-info within repository)")
     print()
     nReturn = oExtendedSetup.delete_previous_build()
     if nReturn != SUCCESS:
         sys.exit(nReturn)
 
-    if not 'bdist_wheel' in listCmdArgs:
+    if ( ('bdist_wheel' in listCmdArgs) or ('build' in listCmdArgs) ):
+        print()
+        print(COLBY + "Skipping extended setup step 4/5: Deleting previous package installation folder within site-packages")
+        print()
+    else:
         print()
-        print(COLBY + "Extended setup step 3/5: Deleting previous package installation folder within site-packages") # (<package name> and <package name>_doc under <Python installation>\Lib\site-packages
+        print(COLBY + "Extended setup step 4/5: Deleting previous package installation folder within site-packages") # (<package name> and <package name>_doc under <Python installation>\Lib\site-packages
         print()
         nReturn = oExtendedSetup.delete_previous_installation()
         if nReturn != SUCCESS:
             sys.exit(nReturn)
 
-    with open("README.md", "r", encoding="utf-8") as fh:
+    README_MD = str(oRepositoryConfig.Get('README_MD'))
+    with open(README_MD, "r", encoding="utf-8") as fh:
         long_description = fh.read()
-    print()
+    fh.close()
 
 
 # --------------------------------------------------------------------------------------------------------------
 
-# This also handles the printing of help to console and therefore must be called in every case.
-# And therefore all variables and objects must exist (even in case of the values are not used).
+# -- the 'setup' itself
+
+print(COLBY + "Extended setup step 5/5: install.run(self)")
+print()
+
 setuptools.setup(
-    name         = str(oRepositoryConfig.Get('sPackageName')),
-    version      = str(oRepositoryConfig.Get('sVersion')),
-    author       = str(oRepositoryConfig.Get('sAuthor')),
-    author_email = str(oRepositoryConfig.Get('sAuthorEMail')),
-    description  = str(oRepositoryConfig.Get('sDescription')),
+    name         = str(oRepositoryConfig.Get('REPOSITORYNAME')),
+    version      = str(oRepositoryConfig.Get('PACKAGEVERSION')),
+    author       = str(oRepositoryConfig.Get('AUTHOR')),
+    author_email = str(oRepositoryConfig.Get('AUTHOREMAIL')),
+    description  = str(oRepositoryConfig.Get('DESCRIPTION')),
     long_description = long_description,
-    long_description_content_type = str(oRepositoryConfig.Get('sLongDescriptionContentType')),
-    url = str(oRepositoryConfig.Get('sURL')),
+    long_description_content_type = str(oRepositoryConfig.Get('LONGDESCRIPTIONCONTENTTYPE')),
+    url = str(oRepositoryConfig.Get('URL')),
 
-    packages = [str(oRepositoryConfig.Get('sImportName')),
-                str(oRepositoryConfig.Get('sImportName')) + ".Config",
-                str(oRepositoryConfig.Get('sImportName')) + ".Keywords",
-                str(oRepositoryConfig.Get('sImportName')) + ".Utils",
-                str(oRepositoryConfig.Get('sImportName')) + ".Utils.Events"],
+    packages = [str(oRepositoryConfig.Get('PACKAGENAME')),
+                str(oRepositoryConfig.Get('PACKAGENAME')) + ".Config",
+                str(oRepositoryConfig.Get('PACKAGENAME')) + ".Keywords",
+                str(oRepositoryConfig.Get('PACKAGENAME')) + ".Utils",
+                str(oRepositoryConfig.Get('PACKAGENAME')) + ".Utils.Events"],
 
-    package_dir = {str(oRepositoryConfig.Get('sPackageName')) : str(oRepositoryConfig.Get('sImportName'))},
+    package_dir = {str(oRepositoryConfig.Get('REPOSITORYNAME')) : str(oRepositoryConfig.Get('PACKAGENAME'))},
 
     include_package_data = True,
 
     classifiers = [
-        str(oRepositoryConfig.Get('sProgrammingLanguage')),
-        str(oRepositoryConfig.Get('sLicence')),
-        str(oRepositoryConfig.Get('sOperatingSystem')),
-        str(oRepositoryConfig.Get('sDevelopmentStatus')),
-        str(oRepositoryConfig.Get('sIntendedAudience')),
-        str(oRepositoryConfig.Get('sTopic')),
+        str(oRepositoryConfig.Get('PROGRAMMINGLANGUAGE')),
+        str(oRepositoryConfig.Get('LICENCE')),
+        str(oRepositoryConfig.Get('OPERATINGSYSTEM')),
+        str(oRepositoryConfig.Get('DEVELOPMENTSTATUS')),
+        str(oRepositoryConfig.Get('INTENDEDAUDIENCE')),
+        str(oRepositoryConfig.Get('TOPIC')),
     ],
-    python_requires = str(oRepositoryConfig.Get('sPythonRequires')),
+    python_requires = str(oRepositoryConfig.Get('PYTHONREQUIRES')),
     cmdclass={
         'install': ExtendedInstallCommand,
     },
-    install_requires = oRepositoryConfig.Get('arInstallRequires'),
+    install_requires = oRepositoryConfig.Get('INSTALLREQUIRES'),
     entry_points={
-        'console_scripts': oRepositoryConfig.Get('arConsoleScripts'),
-    }
+        'console_scripts': oRepositoryConfig.Get('CONSOLESCRIPTS'),
+    },
+    package_data={f"{oRepositoryConfig.Get('PACKAGENAME')}" : oRepositoryConfig.Get('PACKAGEDATA')},
 )
+# --------------------------------------------------------------------------------------------------------------
+
+print()
+print(COLBG + "Extended installation done")
+print()
 
 # --------------------------------------------------------------------------------------------------------------
```

