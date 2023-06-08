# Comparing `tmp/LUASprites-0.0.24.tar.gz` & `tmp/LUASprites-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LUASprites-0.0.24.tar", last modified: Thu Jun  8 20:18:05 2023, max compression
+gzip compressed data, was "LUASprites-0.0.25.tar", last modified: Thu Jun  8 20:25:42 2023, max compression
```

## Comparing `LUASprites-0.0.24.tar` & `LUASprites-0.0.25.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:18:05.447188 LUASprites-0.0.24/
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)     1071 2023-06-08 19:47:22.000000 LUASprites-0.0.24/LICENSE.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)       45 2023-06-08 19:47:22.000000 LUASprites-0.0.24/MANIFEST.in
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      968 2023-06-08 20:18:05.447300 LUASprites-0.0.24/PKG-INFO
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      514 2023-06-08 19:47:22.000000 LUASprites-0.0.24/README.md
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      119 2023-06-08 19:47:22.000000 LUASprites-0.0.24/requirements.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      144 2023-06-08 20:18:05.447548 LUASprites-0.0.24/setup.cfg
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      995 2023-06-08 20:16:23.000000 LUASprites-0.0.24/setup.py
-drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:18:05.444542 LUASprites-0.0.24/src/
-drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:18:05.446705 LUASprites-0.0.24/src/LUASprites.egg-info/
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      968 2023-06-08 20:18:05.000000 LUASprites-0.0.24/src/LUASprites.egg-info/PKG-INFO
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      320 2023-06-08 20:18:05.000000 LUASprites-0.0.24/src/LUASprites.egg-info/SOURCES.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)        1 2023-06-08 20:18:05.000000 LUASprites-0.0.24/src/LUASprites.egg-info/dependency_links.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)       49 2023-06-08 20:18:05.000000 LUASprites-0.0.24/src/LUASprites.egg-info/entry_points.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      119 2023-06-08 20:18:05.000000 LUASprites-0.0.24/src/LUASprites.egg-info/requires.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)       10 2023-06-08 20:18:05.000000 LUASprites-0.0.24/src/LUASprites.egg-info/top_level.txt
-drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:18:05.446901 LUASprites-0.0.24/src/spritegen/
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)    10625 2023-06-08 19:58:42.000000 LUASprites-0.0.24/src/spritegen/cli.py
+drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:25:42.156529 LUASprites-0.0.25/
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)     1071 2023-06-08 19:47:22.000000 LUASprites-0.0.25/LICENSE.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)       45 2023-06-08 19:47:22.000000 LUASprites-0.0.25/MANIFEST.in
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      968 2023-06-08 20:25:42.156591 LUASprites-0.0.25/PKG-INFO
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      514 2023-06-08 19:47:22.000000 LUASprites-0.0.25/README.md
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      119 2023-06-08 19:47:22.000000 LUASprites-0.0.25/requirements.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      144 2023-06-08 20:25:42.156773 LUASprites-0.0.25/setup.cfg
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      995 2023-06-08 20:25:26.000000 LUASprites-0.0.25/setup.py
+drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:25:42.154318 LUASprites-0.0.25/src/
+drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:25:42.156084 LUASprites-0.0.25/src/LUASprites.egg-info/
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      968 2023-06-08 20:25:42.000000 LUASprites-0.0.25/src/LUASprites.egg-info/PKG-INFO
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      320 2023-06-08 20:25:42.000000 LUASprites-0.0.25/src/LUASprites.egg-info/SOURCES.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)        1 2023-06-08 20:25:42.000000 LUASprites-0.0.25/src/LUASprites.egg-info/dependency_links.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)       49 2023-06-08 20:25:42.000000 LUASprites-0.0.25/src/LUASprites.egg-info/entry_points.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      119 2023-06-08 20:25:42.000000 LUASprites-0.0.25/src/LUASprites.egg-info/requires.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)       10 2023-06-08 20:25:42.000000 LUASprites-0.0.25/src/LUASprites.egg-info/top_level.txt
+drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:25:42.156250 LUASprites-0.0.25/src/spritegen/
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)    10636 2023-06-08 20:22:48.000000 LUASprites-0.0.25/src/spritegen/cli.py
```

### Comparing `LUASprites-0.0.24/LICENSE.txt` & `LUASprites-0.0.25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LUASprites-0.0.24/PKG-INFO` & `LUASprites-0.0.25/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LUASprites
-Version: 0.0.24
+Version: 0.0.25
 Summary: Generate spritesheets and lua modules for easy image reference
 Home-page: https://github.com/AJSteinhauser/LUASprites
 Author: AJ Steinhauser
 Author-email: ajsteinhauser11@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `LUASprites-0.0.24/README.md` & `LUASprites-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `LUASprites-0.0.24/setup.py` & `LUASprites-0.0.25/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 
 setup(
     name = 'LUASprites',
-    version = '0.0.24',
+    version = '0.0.25',
     author = 'AJ Steinhauser',
     author_email = 'ajsteinhauser11@gmail.com',
     license = 'MIT License',
     description = 'Generate spritesheets and lua modules for easy image reference',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/AJSteinhauser/LUASprites',
```

### Comparing `LUASprites-0.0.24/src/LUASprites.egg-info/PKG-INFO` & `LUASprites-0.0.25/src/LUASprites.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LUASprites
-Version: 0.0.24
+Version: 0.0.25
 Summary: Generate spritesheets and lua modules for easy image reference
 Home-page: https://github.com/AJSteinhauser/LUASprites
 Author: AJ Steinhauser
 Author-email: ajsteinhauser11@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `LUASprites-0.0.24/src/spritegen/cli.py` & `LUASprites-0.0.25/src/spritegen/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,23 +271,23 @@
             idx = ""
         output += genLuaTableHelper(tree, name, idx)
     return output
         
 # This function goes to a counter api which lets me see how this application is being used and what features are being used most often. No personal data is being sent or anything linkable to yourself
 # Having the usage data allows me to better prioritize what features to update/make better 
 # Please don't spam the api, this is an open source tool and this data helps me tremendously 
-#def usageTrack(usecase):
+def usageTrack(usecase):
+    return 0
     #requests.get('https://api.countapi.xyz/hit/SpriteSheetGenerator_Deploy1/' + usecase)
 
 
 def init():
     print(BANNER)
     usageTrack("start")
 
-
 def main():
     path = getImageFolder()
     init()
     name = getName()
     sprites = loadSprites(path)
     trees = []
     buildTree(trees,sprites)
```

