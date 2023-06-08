# Comparing `tmp/warframe.py-0.1.1-py3-none-any.whl.zip` & `tmp/warframe.py-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 18152 bytes, number of entries: 32
+Zip file size: 18143 bytes, number of entries: 32
 -rw-rw-rw-  2.0 fat      131 b- defN 23-Jun-05 20:32 warframe/worldstate/__init__.py
 -rw-rw-rw-  2.0 fat     5643 b- defN 23-Jun-07 15:35 warframe/worldstate/client.py
 -rw-rw-rw-  2.0 fat     1387 b- defN 23-Jun-04 20:34 warframe/worldstate/endpoints.py
 -rw-rw-rw-  2.0 fat      879 b- defN 23-Jun-04 10:32 warframe/worldstate/exceptions.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-28 15:31 warframe/worldstate/worldstate_utils.py
 -rw-rw-rw-  2.0 fat       52 b- defN 23-Jun-04 13:55 warframe/worldstate/common/__init__.py
 -rw-rw-rw-  2.0 fat     1694 b- defN 23-Jun-05 16:27 warframe/worldstate/common/base_objects.py
@@ -22,13 +22,13 @@
 -rw-rw-rw-  2.0 fat     1397 b- defN 23-Jun-04 20:28 warframe/worldstate/models/fissure.py
 -rw-rw-rw-  2.0 fat      610 b- defN 23-Jun-04 10:32 warframe/worldstate/models/flash_sale.py
 -rw-rw-rw-  2.0 fat     1921 b- defN 23-Jun-04 20:35 warframe/worldstate/models/invasion.py
 -rw-rw-rw-  2.0 fat     1542 b- defN 23-Jun-05 16:43 warframe/worldstate/models/mission.py
 -rw-rw-rw-  2.0 fat      405 b- defN 23-Jun-04 10:32 warframe/worldstate/models/orb_vallis.py
 -rw-rw-rw-  2.0 fat      622 b- defN 23-Jun-04 14:01 warframe/worldstate/models/reward.py
 -rw-rw-rw-  2.0 fat     1121 b- defN 23-Jun-04 14:54 warframe/worldstate/models/void_trader.py
--rw-rw-rw-  2.0 fat     1125 b- defN 23-Jun-08 01:43 warframe.py-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2046 b- defN 23-Jun-08 01:43 warframe.py-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-08 01:43 warframe.py-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-08 01:43 warframe.py-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2938 b- defN 23-Jun-08 01:43 warframe.py-0.1.1.dist-info/RECORD
-32 files, 33018 bytes uncompressed, 13310 bytes compressed:  59.7%
+-rw-rw-rw-  2.0 fat     1125 b- defN 23-Jun-08 01:46 warframe.py-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2011 b- defN 23-Jun-08 01:46 warframe.py-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-08 01:46 warframe.py-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-08 01:46 warframe.py-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2938 b- defN 23-Jun-08 01:46 warframe.py-0.1.2.dist-info/RECORD
+32 files, 32983 bytes uncompressed, 13301 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -75,23 +75,23 @@
 
 Filename: warframe/worldstate/models/reward.py
 Comment: 
 
 Filename: warframe/worldstate/models/void_trader.py
 Comment: 
 
-Filename: warframe.py-0.1.1.dist-info/LICENSE
+Filename: warframe.py-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: warframe.py-0.1.1.dist-info/METADATA
+Filename: warframe.py-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: warframe.py-0.1.1.dist-info/WHEEL
+Filename: warframe.py-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: warframe.py-0.1.1.dist-info/top_level.txt
+Filename: warframe.py-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: warframe.py-0.1.1.dist-info/RECORD
+Filename: warframe.py-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `warframe.py-0.1.1.dist-info/LICENSE` & `warframe.py-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `warframe.py-0.1.1.dist-info/METADATA` & `warframe.py-0.1.2.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warframe.py
-Version: 0.1.1
+Version: 0.1.2
 Summary: An asynchronous Python API wrapper for the Warframestat API and (later) the warframe.market API.
 Home-page: https://github.com/WFCD/warframe.py
 Author: Mettwasser
 License: MIT
 Keywords: Warframe API worldstate market wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -55,13 +55,13 @@
 Installing
 ----------
 
 To install the library, use the following command:
 
 .. code-block:: bash
 
-    pip install git+https://github.com/Mettwasser/warframe.git
+    pip install warframe.py
 
 Supported python versions:
 - 3.11
 - 3.10
 - 3.9
```

## Comparing `warframe.py-0.1.1.dist-info/RECORD` & `warframe.py-0.1.2.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 warframe/worldstate/models/fissure.py,sha256=dMvkyUfqgBkgdFdF3qu9n1s_Uq2c-6dwPyMk14GbHRE,1397
 warframe/worldstate/models/flash_sale.py,sha256=WvNpPKCMJmcaaGtjLzSTd4q1vOfZBtLtlLcw1Mr32wE,610
 warframe/worldstate/models/invasion.py,sha256=HTZFhk5L4VoMKWz8I4_D_i8R8vwcRbIYtjzc6C05a9k,1921
 warframe/worldstate/models/mission.py,sha256=0PN1VJymhhnSDdn9LLYWwCqpb9dz1q0Unt05nh6M_Lg,1542
 warframe/worldstate/models/orb_vallis.py,sha256=YeHa-jEA2hYPi-umMKdesFE7EhjA7w2t3cB_WdyAX_8,405
 warframe/worldstate/models/reward.py,sha256=981AJAnAswu0NTRBHXL3kWninGcGvseaYCdziZIKGpQ,622
 warframe/worldstate/models/void_trader.py,sha256=vmRKsMVyv4onokZh2kaBJzfcAwVx8TKvLy0WfnS-EIY,1121
-warframe.py-0.1.1.dist-info/LICENSE,sha256=xXR-dV8ziCSdFcjrmbIiBooDyF-Erz538RTsobauVp8,1125
-warframe.py-0.1.1.dist-info/METADATA,sha256=dzqvk7IKeK7llA5hNT83_SWt85vxj26CL_fcTqnB3OA,2046
-warframe.py-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-warframe.py-0.1.1.dist-info/top_level.txt,sha256=KZ5vYhjaoh3en-QJKMow6f5at-LAzVmj0HiZwM057pQ,9
-warframe.py-0.1.1.dist-info/RECORD,,
+warframe.py-0.1.2.dist-info/LICENSE,sha256=xXR-dV8ziCSdFcjrmbIiBooDyF-Erz538RTsobauVp8,1125
+warframe.py-0.1.2.dist-info/METADATA,sha256=ApXgIUDYY4lwFUBat4KFOyI0EuIeJinlW60oSRnpgK0,2011
+warframe.py-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+warframe.py-0.1.2.dist-info/top_level.txt,sha256=KZ5vYhjaoh3en-QJKMow6f5at-LAzVmj0HiZwM057pQ,9
+warframe.py-0.1.2.dist-info/RECORD,,
```

