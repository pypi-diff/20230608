# Comparing `tmp/limacharlie-4.4.7.tar.gz` & `tmp/limacharlie-4.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limacharlie-4.4.7.tar", last modified: Tue May  2 16:50:03 2023, max compression
+gzip compressed data, was "limacharlie-4.4.9.tar", last modified: Sat May 20 00:21:31 2023, max compression
```

## Comparing `limacharlie-4.4.7.tar` & `limacharlie-4.4.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-02 16:50:03.196289 limacharlie-4.4.7/
--rw-r--r--   0 maxime    (1000) maxime    (1000)    11357 2021-03-23 21:34:15.000000 limacharlie-4.4.7/LICENSE
--rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-05-02 16:50:03.196289 limacharlie-4.4.7/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10845 2023-04-28 15:20:27.000000 limacharlie-4.4.7/README.md
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-02 16:50:03.190289 limacharlie-4.4.7/limacharlie/
--rw-r--r--   0 maxime    (1000) maxime    (1000)    50463 2023-04-12 22:28:28.000000 limacharlie-4.4.7/limacharlie/Configs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     3361 2021-03-23 21:34:15.000000 limacharlie-4.4.7/limacharlie/DRCli.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     5057 2023-04-24 15:42:48.000000 limacharlie-4.4.7/limacharlie/Extensions.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    14867 2022-09-03 02:23:38.000000 limacharlie-4.4.7/limacharlie/Firehose.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10160 2023-04-24 16:27:39.000000 limacharlie-4.4.7/limacharlie/Hive.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2643 2021-03-23 21:34:15.000000 limacharlie-4.4.7/limacharlie/Jobs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    15935 2022-11-03 04:20:06.000000 limacharlie-4.4.7/limacharlie/Logs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    53041 2023-05-02 16:49:49.000000 limacharlie-4.4.7/limacharlie/Manager.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2803 2021-03-23 21:34:15.000000 limacharlie-4.4.7/limacharlie/Payloads.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    16039 2023-04-12 23:50:48.000000 limacharlie-4.4.7/limacharlie/Query.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    19246 2023-04-12 23:50:48.000000 limacharlie-4.4.7/limacharlie/Replay.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    12905 2022-11-26 21:02:39.000000 limacharlie-4.4.7/limacharlie/Replicants.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     8981 2023-04-06 18:48:27.000000 limacharlie-4.4.7/limacharlie/Search.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    17540 2023-05-02 16:49:49.000000 limacharlie-4.4.7/limacharlie/Sensor.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    24227 2022-09-23 18:58:57.000000 limacharlie-4.4.7/limacharlie/SpotCheck.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10781 2023-05-01 21:28:43.000000 limacharlie-4.4.7/limacharlie/Spout.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    33649 2021-06-21 23:20:54.000000 limacharlie-4.4.7/limacharlie/Sync.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      970 2021-03-23 21:34:15.000000 limacharlie-4.4.7/limacharlie/Webhook.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2305 2023-05-02 16:49:49.000000 limacharlie-4.4.7/limacharlie/__init__.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    16201 2023-04-30 23:56:52.000000 limacharlie-4.4.7/limacharlie/__main__.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6821 2022-12-01 21:47:34.000000 limacharlie-4.4.7/limacharlie/utils.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-02 16:50:03.192289 limacharlie-4.4.7/limacharlie.egg-info/
--rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-05-02 16:50:03.000000 limacharlie-4.4.7/limacharlie.egg-info/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)      879 2023-05-02 16:50:03.000000 limacharlie-4.4.7/limacharlie.egg-info/SOURCES.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2023-05-02 16:50:03.000000 limacharlie-4.4.7/limacharlie.egg-info/dependency_links.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       58 2023-05-02 16:50:03.000000 limacharlie-4.4.7/limacharlie.egg-info/entry_points.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       43 2023-05-02 16:50:03.000000 limacharlie-4.4.7/limacharlie.egg-info/requires.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       12 2023-05-02 16:50:03.000000 limacharlie-4.4.7/limacharlie.egg-info/top_level.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2021-03-23 21:34:40.000000 limacharlie-4.4.7/limacharlie.egg-info/zip-safe
--rw-r--r--   0 maxime    (1000) maxime    (1000)       79 2023-05-02 16:50:03.197289 limacharlie-4.4.7/setup.cfg
--rw-r--r--   0 maxime    (1000) maxime    (1000)      892 2023-05-02 16:49:49.000000 limacharlie-4.4.7/setup.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-02 16:50:03.195289 limacharlie-4.4.7/tests/
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2394 2021-03-23 21:34:15.000000 limacharlie-4.4.7/tests/test_artifacts.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6000 2022-12-12 23:19:01.000000 limacharlie-4.4.7/tests/test_core.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1415 2021-03-23 21:34:15.000000 limacharlie-4.4.7/tests/test_insight.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      424 2021-03-23 21:34:15.000000 limacharlie-4.4.7/tests/test_replicants.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1327 2021-03-23 21:34:15.000000 limacharlie-4.4.7/tests/test_spout.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6055 2022-09-21 18:43:37.000000 limacharlie-4.4.7/tests/test_sync.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-20 00:21:31.747844 limacharlie-4.4.9/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    11357 2021-03-23 21:34:15.000000 limacharlie-4.4.9/LICENSE
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-05-20 00:21:31.747844 limacharlie-4.4.9/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10845 2023-05-08 23:21:15.000000 limacharlie-4.4.9/README.md
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-20 00:21:31.741844 limacharlie-4.4.9/limacharlie/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    53208 2023-05-18 15:42:53.000000 limacharlie-4.4.9/limacharlie/Configs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     3361 2021-03-23 21:34:15.000000 limacharlie-4.4.9/limacharlie/DRCli.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     5057 2023-05-08 23:21:15.000000 limacharlie-4.4.9/limacharlie/Extensions.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    14867 2022-09-03 02:23:38.000000 limacharlie-4.4.9/limacharlie/Firehose.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10578 2023-05-20 00:20:29.000000 limacharlie-4.4.9/limacharlie/Hive.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2643 2021-03-23 21:34:15.000000 limacharlie-4.4.9/limacharlie/Jobs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    15935 2022-11-03 04:20:06.000000 limacharlie-4.4.9/limacharlie/Logs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    53041 2023-05-08 23:21:15.000000 limacharlie-4.4.9/limacharlie/Manager.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2803 2021-03-23 21:34:15.000000 limacharlie-4.4.9/limacharlie/Payloads.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    16039 2023-05-08 23:21:15.000000 limacharlie-4.4.9/limacharlie/Query.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    19246 2023-05-08 23:21:15.000000 limacharlie-4.4.9/limacharlie/Replay.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    12905 2022-11-26 21:02:39.000000 limacharlie-4.4.9/limacharlie/Replicants.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     8981 2023-05-08 23:21:15.000000 limacharlie-4.4.9/limacharlie/Search.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    17540 2023-05-08 23:21:15.000000 limacharlie-4.4.9/limacharlie/Sensor.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    24227 2022-09-23 18:58:57.000000 limacharlie-4.4.9/limacharlie/SpotCheck.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10781 2023-05-08 23:21:15.000000 limacharlie-4.4.9/limacharlie/Spout.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    33649 2021-06-21 23:20:54.000000 limacharlie-4.4.9/limacharlie/Sync.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      970 2021-03-23 21:34:15.000000 limacharlie-4.4.9/limacharlie/Webhook.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2305 2023-05-20 00:20:29.000000 limacharlie-4.4.9/limacharlie/__init__.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    16201 2023-05-08 23:21:15.000000 limacharlie-4.4.9/limacharlie/__main__.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6821 2022-12-01 21:47:34.000000 limacharlie-4.4.9/limacharlie/utils.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-20 00:21:31.744844 limacharlie-4.4.9/limacharlie.egg-info/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-05-20 00:21:31.000000 limacharlie-4.4.9/limacharlie.egg-info/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      879 2023-05-20 00:21:31.000000 limacharlie-4.4.9/limacharlie.egg-info/SOURCES.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2023-05-20 00:21:31.000000 limacharlie-4.4.9/limacharlie.egg-info/dependency_links.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       58 2023-05-20 00:21:31.000000 limacharlie-4.4.9/limacharlie.egg-info/entry_points.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       43 2023-05-20 00:21:31.000000 limacharlie-4.4.9/limacharlie.egg-info/requires.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       12 2023-05-20 00:21:31.000000 limacharlie-4.4.9/limacharlie.egg-info/top_level.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2021-03-23 21:34:40.000000 limacharlie-4.4.9/limacharlie.egg-info/zip-safe
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       79 2023-05-20 00:21:31.748844 limacharlie-4.4.9/setup.cfg
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      892 2023-05-20 00:20:29.000000 limacharlie-4.4.9/setup.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-20 00:21:31.747844 limacharlie-4.4.9/tests/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2394 2021-03-23 21:34:15.000000 limacharlie-4.4.9/tests/test_artifacts.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6000 2022-12-12 23:19:01.000000 limacharlie-4.4.9/tests/test_core.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     1415 2021-03-23 21:34:15.000000 limacharlie-4.4.9/tests/test_insight.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      424 2021-03-23 21:34:15.000000 limacharlie-4.4.9/tests/test_replicants.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     1327 2021-03-23 21:34:15.000000 limacharlie-4.4.9/tests/test_spout.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6055 2022-09-21 18:43:37.000000 limacharlie-4.4.9/tests/test_sync.py
```

### Comparing `limacharlie-4.4.7/LICENSE` & `limacharlie-4.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/README.md` & `limacharlie-4.4.9/README.md`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/Configs.py` & `limacharlie-4.4.9/limacharlie/Configs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .Manager import Manager
 from .Replicants import Integrity
 from .Replicants import Logging
 from .Replicants import Exfil
 from .utils import _isStringCompat
+from .Extensions import Extension
 
 # Detect if this is Python 2 or 3
 import sys
 _IS_PYTHON_2 = False
 if sys.version_info[ 0 ] < 3:
     _IS_PYTHON_2 = True
 
@@ -126,15 +127,15 @@
     def _getAllOrgConfigValues( self ):
         currentConfigs = {}
         for confName in self._getSupportedOrgConfigs():
             val = self._man.getOrgConfig( confName )
             currentConfigs[ confName ] = val
         return currentConfigs
 
-    def fetch( self, toConfigFile, isRules = False, isFPs = False, isOutputs = False, isIntegrity = False, isArtifact = False, isExfil = False, isResources = False, isOrgConfigs = False, isHives={}, isInstallationKeys = False, isYara = False ):
+    def fetch( self, toConfigFile, isRules = False, isFPs = False, isOutputs = False, isIntegrity = False, isArtifact = False, isExfil = False, isResources = False, isExtensions = False, isOrgConfigs = False, isHives={}, isInstallationKeys = False, isYara = False ):
         '''Retrieves the effective configuration in the cloud to a local config file.
 
         Args:
             toConfigFile (str, dict): the path to the local config file or dict where to store config.
         '''
         if not isinstance( toConfigFile, dict ):
             toConfigFile = os.path.abspath( toConfigFile )
@@ -148,14 +149,15 @@
             try:
                 if self._isUseExtension:
                     data = self._man.extensionRequest( 'ext-infrastructure', 'fetch', {
                         'options' : {
                             'sync_dr' : isRules,
                             'sync_outputs' : isOutputs,
                             'sync_resources' : isResources,
+                            'sync_extensions' : isExtensions,
                             'sync_integrity' : isIntegrity,
                             'sync_fp' : isFPs,
                             'sync_exfil' : isExfil,
                             'sync_artifacts' : isArtifact,
                             'sync_org_values' : isOrgConfigs,
                             'sync_hives' : isHives, # must be map of hive names you want to fetch {"cloud_sensor":true, "fp":true, "dr-service":true, "dr-general": true}
                             'sync_installation_keys' : isInstallationKeys,
@@ -165,14 +167,15 @@
                     asConf = data[ 'data' ][ 'org' ]
                 else:
                     data = self._man.serviceRequest( 'infrastructure-service', {
                         'action' : 'fetch',
                         'sync_dr' : isRules,
                         'sync_outputs' : isOutputs,
                         'sync_resources' : isResources,
+                        'sync_extensions' : isExtensions,
                         'sync_integrity' : isIntegrity,
                         'sync_fp' : isFPs,
                         'sync_exfil' : isExfil,
                         'sync_artifacts' : isArtifact,
                         'sync_org_values' : isOrgConfigs,
                         'sync_hives' : isHives, # must be map of hive names you want to fetch {"cloud_sensor":true, "fp":true, "dr-service":true, "dr-general": true}
                         'sync_installation_keys' : isInstallationKeys,
@@ -272,33 +275,36 @@
             # Translate the replicant entry to service.
             for resType, resources in asConf[ 'resources' ].items():
                 if resType != 'replicant':
                     continue
                 asConf[ 'resources' ][ 'service' ] = asConf[ 'resources' ][ 'replicant' ]
                 asConf[ 'resources' ].pop( 'replicant' )
                 break
+        if isExtensions:
+            asConf[ 'extensions' ] = list( Extension( self._man ).list().keys() )
         if not isinstance( toConfigFile, dict ):
             with open( toConfigFile, 'wb' ) as f:
                 f.write( yaml.safe_dump( asConf, default_flow_style = False, version = (1,1) ).encode() )
 
-    def push( self, fromConfigFile, isForce = False, isDryRun = False, isIgnoreInaccessible = False, isRules = False, isFPs = False, isOutputs = False, isIntegrity = False, isArtifact = False, isExfil = False, isResources = False, isOrgConfigs = False, isHives={}, isInstallationKeys = False, isYara = False, isVerbose = False ):
+    def push( self, fromConfigFile, isForce = False, isDryRun = False, isIgnoreInaccessible = False, isRules = False, isFPs = False, isOutputs = False, isIntegrity = False, isArtifact = False, isExfil = False, isResources = False, isExtensions = False, isOrgConfigs = False, isHives={}, isInstallationKeys = False, isYara = False, isVerbose = False ):
         '''Apply the configuratiion in a local config file to the effective configuration in the cloud.
 
         Args:
             fromConfigFile (str/dict): the path to the config file or dict of a config file content.
             isForce (boolean): if True will remove configurations in the cloud that are not present in the local file.
             isDryRun (boolean): if True will only simulate the effect of a push.
             isIgnoreInaccessible (boolean): if True, ignore inaccessible resources (locked) even when isForce is True.
             isRules (boolean): if True, push D&R rules.
             isFPs (boolean): if True, push False Positive rules.
             isOutputs (boolean): if True, push Outputs.
             isIntegrity (boolean): if True, push Integrity rules.
             isArtifact (boolean): if True, push Artifact rules.
             isExfil (boolean): if True, push Exfil rules.
             isResources (boolean): if True, push Resource subscriptions.
+            isExtensions (boolean): if True, push Extension subscriptions.
             isOrgConfigs (boolean): if True, push Org Configs.
             isHives (dict{"hive_name": true}): only one hive value is requried for sync push to process passed config data, if empty or null no push will occur
             isInstallationKeys (boolean): if True, push Installation Keys.
             isYara (boolean): if True, push Yara rules and sources.
 
         Returns:
             a generator of changes as tuple (changeType, dataType, dataName).
@@ -349,14 +355,15 @@
                         'options' : {
                             'is_dry_run' : isDryRun,
                             'is_force' : isForce,
                             'ignore_inaccessible' : isIgnoreInaccessible,
                             'sync_dr' : isRules,
                             'sync_outputs' : isOutputs,
                             'sync_resources' : isResources,
+                            'sync_extensions' : isExtensions,
                             'sync_integrity' : isIntegrity,
                             'sync_fp' : isFPs,
                             'sync_exfil' : isExfil,
                             'sync_artifacts' : isArtifact,
                             'sync_org_values' : isOrgConfigs,
                             'sync_hives' : isHives,
                             'sync_installation_keys' : isInstallationKeys,
@@ -370,14 +377,15 @@
                         'action' : 'push',
                         'is_force' : isForce,
                         'ignore_inaccessible' : isIgnoreInaccessible,
                         'config' : finalConfig,
                         'sync_dr' : isRules,
                         'sync_outputs' : isOutputs,
                         'sync_resources' : isResources,
+                        'sync_extensions' : isExtensions,
                         'sync_integrity' : isIntegrity,
                         'sync_fp' : isFPs,
                         'sync_exfil' : isExfil,
                         'sync_artifacts' : isArtifact,
                         'sync_org_values' : isOrgConfigs,
                         'sync_hives' : isHives,
                         'sync_installation_keys' : isInstallationKeys,
@@ -420,14 +428,33 @@
                             # Alias replicant to service
                             internalCat = 'service'
                         if resName not in asConf.get( 'resources', {} ).get( internalCat, [] ):
                             fullResName = '%s/%s' % ( cat, resName )
                             if not isDryRun:
                                 self._man.unsubscribeFromResource( fullResName )
                             yield ( '-', 'resource', fullResName )
+        
+        if isExtensions:
+            currentExtensions = list( Extension( self._man ).list() )
+            confExtensions = asConf.get( 'extensions', [] )
+            for ext in confExtensions:
+                if ext in currentExtensions:
+                    yield ( '=', 'extension', ext )
+                else:
+                    if not isDryRun:
+                        Extension( self._man ).subscribe( ext )
+                    yield ( '+', 'resource', fullResName )
+            # Only force "extensions" if it is present in the config.
+            # This avoids unexpected disabling of all configs.
+            if isForce and 'extensions' in asConf:
+                for ext in currentExtensions:
+                    if ext not in asConf.get( 'extensions', [] ):
+                        if not isDryRun:
+                            Extension( self._man ).unsubscribe( ext )
+                        yield ( '-', 'extension', ext )
 
         if isOrgConfigs:
             # Get the current configs, we will try not to push for no reason.
             currentConfigs = self._getAllOrgConfigValues()
 
             # Start by adding the configs with isReplace.
             for confName, confValue in asConf.get( 'org-value', {} ).items():
@@ -858,14 +885,20 @@
                          help = 'if specified, apply Exfil Service from operations' )
     parser.add_argument( '--resources',
                          required = False,
                          default = False,
                          action = 'store_true',
                          dest = 'isResources',
                          help = 'if specified, apply resource subscriptions from operations' )
+    parser.add_argument( '--extensions',
+                         required = False,
+                         default = False,
+                         action = 'store_true',
+                         dest = 'isExtensions',
+                         help = 'if specified, apply extension subscriptions from operations' )
     parser.add_argument( '--org-configs',
                          required = False,
                          default = False,
                          action = 'store_true',
                          dest = 'isOrgConfigs',
                          help = 'if specified, apply org configs from operations' )
     parser.add_argument( '--installation-keys',
@@ -906,14 +939,26 @@
                          help = 'if specified, apply FP rules in the general hive from operations' )
     parser.add_argument( '--hive-cloud-sensor',
                          required = False,
                          default = False,
                          action = 'store_true',
                          dest = 'isHiveCloudSensor',
                          help = 'if specified, apply cloud sensors in hive from operations' )
+    parser.add_argument( '--hive-extension-config',
+                         required = False,
+                         default = False,
+                         action = 'store_true',
+                         dest = 'isHiveExtensionConfig',
+                         help = 'if specified, apply extension configs in hive from operations' )
+    parser.add_argument( '--hive-yara',
+                         required = False,
+                         default = False,
+                         action = 'store_true',
+                         dest = 'isHiveYara',
+                         help = 'if specified, apply yara rules in hive from operations' )
     parser.add_argument( '--all',
                          required = False,
                          default = False,
                          action = 'store_true',
                          dest = 'isAll',
                          help = 'if specified, apply all configs from operations' )
     parser.add_argument( '-c', '--config',
@@ -953,30 +998,35 @@
         'isRules',
         'isFPs',
         'isOutputs',
         'isIntegrity',
         'isArtifact',
         'isExfil',
         'isResources',
+        'isExtensions',
         'isOrgConfigs',
         'isInstallationKeys',
         'isYara',
         'isHiveDRGeneral',
         'isHiveDRManaged',
         'isHiveDRService',
         'isHiveFP',
         'isHiveCloudSensor',
+        'isHiveExtensionConfig',
+        'isHiveYara',
     ]
 
     allHives = {
         'dr-general': True,
         'dr-managed': True,
         'dr-service': True,
         'fp': True,
         'cloud_sensor': True,
+        'extension_config': True,
+        'yara': True,
     }
 
     # If All is enabled, enable all types.
     if args.isAll:
         for k in resTypes:
             setattr( args, k, True )
         setattr( args, 'isHives', allHives )
@@ -997,18 +1047,22 @@
         hives['dr-managed'] = True
     if args.isHiveDRService:
         hives['dr-service'] = True
     if args.isHiveCloudSensor:
         hives['cloud_sensor'] = True
     if args.isHiveFP:
         hives['fp'] = True
+    if args.isHiveExtensionConfig:
+        hives['extension_config'] = True
+    if args.isHiveYara:
+        hives['yara'] = True
 
     s = Configs( oid = args.oid, env = args.environment, isDontUseInfraService = args.isDontUseInfraService, isUseExtension = args.isUseExtension )
 
     if 'fetch' == args.action:
-        s.fetch( args.config, isRules = args.isRules, isFPs = args.isFPs, isOutputs = args.isOutputs, isIntegrity = args.isIntegrity, isArtifact = args.isArtifact, isExfil = args.isExfil, isResources = args.isResources, isOrgConfigs = args.isOrgConfigs, isInstallationKeys = args.isInstallationKeys, isHives = hives, isYara = args.isYara )
+        s.fetch( args.config, isRules = args.isRules, isFPs = args.isFPs, isOutputs = args.isOutputs, isIntegrity = args.isIntegrity, isArtifact = args.isArtifact, isExfil = args.isExfil, isResources = args.isResources, isExtensions = args.isExtensions, isOrgConfigs = args.isOrgConfigs, isInstallationKeys = args.isInstallationKeys, isHives = hives, isYara = args.isYara )
     elif 'push' == args.action:
-        for modification, category, element in s.push( args.config, isForce = args.isForce, isIgnoreInaccessible = args.isIgnoreInaccessible, isDryRun = args.isDryRun, isRules = args.isRules, isFPs = args.isFPs, isOutputs = args.isOutputs, isIntegrity = args.isIntegrity, isArtifact = args.isArtifact, isExfil = args.isExfil, isResources = args.isResources, isOrgConfigs = args.isOrgConfigs, isInstallationKeys = args.isInstallationKeys, isHives = hives, isYara = args.isYara, isVerbose = args.isVerbose ):
+        for modification, category, element in s.push( args.config, isForce = args.isForce, isIgnoreInaccessible = args.isIgnoreInaccessible, isDryRun = args.isDryRun, isRules = args.isRules, isFPs = args.isFPs, isOutputs = args.isOutputs, isIntegrity = args.isIntegrity, isArtifact = args.isArtifact, isExfil = args.isExfil, isResources = args.isResources, isExtensions = args.isExtensions, isOrgConfigs = args.isOrgConfigs, isInstallationKeys = args.isInstallationKeys, isHives = hives, isYara = args.isYara, isVerbose = args.isVerbose ):
             print( '%s %s %s' % ( modification, category, element ) )
 
 if __name__ == '__main__':
     main()
```

### Comparing `limacharlie-4.4.7/limacharlie/DRCli.py` & `limacharlie-4.4.9/limacharlie/DRCli.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/Extensions.py` & `limacharlie-4.4.9/limacharlie/Extensions.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/Firehose.py` & `limacharlie-4.4.9/limacharlie/Firehose.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/Hive.py` & `limacharlie-4.4.9/limacharlie/Hive.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,16 @@
     }
 
     if args.data is not None:
         if args.data == '-':
             data = "\n".join( sys.stdin.readlines() )
         else:
             data = open( args.data, 'rb' ).read().decode()
+        if args.dataKey is not None:
+            data = json.dumps( { args.dataKey : data } )
         data = json.loads( data )
         record[ 'data' ] = data
 
     usrMtd = {}
     if args.expiry is not None:
         usrMtd[ 'expiry' ] = args.expiry
     if args.enabled is not None:
@@ -242,14 +244,20 @@
 
     parser.add_argument( '-d', '--data',
                          default = None,
                          required = False,
                          dest = 'data',
                          help = 'file containing the JSON data for the record, or "-" for stdin.' )
 
+    parser.add_argument( '-dk', '--data-key',
+                         default = None,
+                         required = False,
+                         dest = 'dataKey',
+                         help = 'some hives expect data to be located within a specific key of the json data, wrap the --data content in this key.' )
+
     parser.add_argument( '-pk', '--partition-key',
                          default = None,
                          required = False,
                          dest = 'partitionKey',
                          help = 'the partition key to use instead of the default OID.' )
 
     parser.add_argument( '--etag',
```

### Comparing `limacharlie-4.4.7/limacharlie/Jobs.py` & `limacharlie-4.4.9/limacharlie/Jobs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/Logs.py` & `limacharlie-4.4.9/limacharlie/Logs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/Manager.py` & `limacharlie-4.4.9/limacharlie/Manager.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/Payloads.py` & `limacharlie-4.4.9/limacharlie/Payloads.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/Query.py` & `limacharlie-4.4.9/limacharlie/Query.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/Replay.py` & `limacharlie-4.4.9/limacharlie/Replay.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/Replicants.py` & `limacharlie-4.4.9/limacharlie/Replicants.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/Search.py` & `limacharlie-4.4.9/limacharlie/Search.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/Sensor.py` & `limacharlie-4.4.9/limacharlie/Sensor.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/SpotCheck.py` & `limacharlie-4.4.9/limacharlie/SpotCheck.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/Spout.py` & `limacharlie-4.4.9/limacharlie/Spout.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/Sync.py` & `limacharlie-4.4.9/limacharlie/Sync.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/Webhook.py` & `limacharlie-4.4.9/limacharlie/Webhook.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/__init__.py` & `limacharlie-4.4.9/limacharlie/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """limacharlie API for limacharlie.io"""
 
-__version__ = "4.4.7"
+__version__ = "4.4.9"
 __author__ = "Maxime Lamothe-Brassard ( Refraction Point, Inc )"
 __author_email__ = "maxime@refractionpoint.com"
 __license__ = "Apache v2"
 __copyright__ = "Copyright (c) 2020 Refraction Point, Inc"
 
 # Global API Credentials
 import os
```

### Comparing `limacharlie-4.4.7/limacharlie/__main__.py` & `limacharlie-4.4.9/limacharlie/__main__.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie/utils.py` & `limacharlie-4.4.9/limacharlie/utils.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/limacharlie.egg-info/SOURCES.txt` & `limacharlie-4.4.9/limacharlie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/setup.py` & `limacharlie-4.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "4.4.7"
+__version__ = "4.4.9"
 __author__ = "Maxime Lamothe-Brassard ( Refraction Point, Inc )"
 __author_email__ = "maxime@refractionpoint.com"
 __license__ = "Apache v2"
 __copyright__ = "Copyright (c) 2020 Refraction Point, Inc"
 
 setup( name = 'limacharlie',
        version = __version__,
```

### Comparing `limacharlie-4.4.7/tests/test_artifacts.py` & `limacharlie-4.4.9/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/tests/test_core.py` & `limacharlie-4.4.9/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/tests/test_insight.py` & `limacharlie-4.4.9/tests/test_insight.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/tests/test_spout.py` & `limacharlie-4.4.9/tests/test_spout.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.7/tests/test_sync.py` & `limacharlie-4.4.9/tests/test_sync.py`

 * *Files identical despite different names*

