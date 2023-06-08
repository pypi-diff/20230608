# Comparing `tmp/LUASprites-0.0.23.tar.gz` & `tmp/LUASprites-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LUASprites-0.0.23.tar", last modified: Sun Aug 21 21:15:00 2022, max compression
+gzip compressed data, was "LUASprites-0.0.24.tar", last modified: Thu Jun  8 20:18:05 2023, max compression
```

## Comparing `LUASprites-0.0.23.tar` & `LUASprites-0.0.24.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2022-08-21 21:15:00.312153 LUASprites-0.0.23/
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)     1071 2022-08-19 16:38:07.000000 LUASprites-0.0.23/LICENSE.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)       45 2022-08-21 13:36:56.000000 LUASprites-0.0.23/MANIFEST.in
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      968 2022-08-21 21:15:00.312214 LUASprites-0.0.23/PKG-INFO
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      514 2022-08-20 20:23:04.000000 LUASprites-0.0.23/README.md
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      119 2022-08-21 21:05:31.000000 LUASprites-0.0.23/requirements.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      144 2022-08-21 21:15:00.312397 LUASprites-0.0.23/setup.cfg
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      996 2022-08-21 21:14:39.000000 LUASprites-0.0.23/setup.py
-drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2022-08-21 21:15:00.310496 LUASprites-0.0.23/src/
-drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2022-08-21 21:15:00.311746 LUASprites-0.0.23/src/LUASprites.egg-info/
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      968 2022-08-21 21:15:00.000000 LUASprites-0.0.23/src/LUASprites.egg-info/PKG-INFO
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      320 2022-08-21 21:15:00.000000 LUASprites-0.0.23/src/LUASprites.egg-info/SOURCES.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)        1 2022-08-21 21:15:00.000000 LUASprites-0.0.23/src/LUASprites.egg-info/dependency_links.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)       50 2022-08-21 21:15:00.000000 LUASprites-0.0.23/src/LUASprites.egg-info/entry_points.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)      119 2022-08-21 21:15:00.000000 LUASprites-0.0.23/src/LUASprites.egg-info/requires.txt
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)       10 2022-08-21 21:15:00.000000 LUASprites-0.0.23/src/LUASprites.egg-info/top_level.txt
-drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2022-08-21 21:15:00.311922 LUASprites-0.0.23/src/spritegen/
--rw-r--r--   0 ajsteinhauser   (501) staff       (20)    10623 2022-08-21 21:12:52.000000 LUASprites-0.0.23/src/spritegen/cli.py
+drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:18:05.447188 LUASprites-0.0.24/
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)     1071 2023-06-08 19:47:22.000000 LUASprites-0.0.24/LICENSE.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)       45 2023-06-08 19:47:22.000000 LUASprites-0.0.24/MANIFEST.in
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      968 2023-06-08 20:18:05.447300 LUASprites-0.0.24/PKG-INFO
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      514 2023-06-08 19:47:22.000000 LUASprites-0.0.24/README.md
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      119 2023-06-08 19:47:22.000000 LUASprites-0.0.24/requirements.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      144 2023-06-08 20:18:05.447548 LUASprites-0.0.24/setup.cfg
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      995 2023-06-08 20:16:23.000000 LUASprites-0.0.24/setup.py
+drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:18:05.444542 LUASprites-0.0.24/src/
+drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:18:05.446705 LUASprites-0.0.24/src/LUASprites.egg-info/
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      968 2023-06-08 20:18:05.000000 LUASprites-0.0.24/src/LUASprites.egg-info/PKG-INFO
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      320 2023-06-08 20:18:05.000000 LUASprites-0.0.24/src/LUASprites.egg-info/SOURCES.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)        1 2023-06-08 20:18:05.000000 LUASprites-0.0.24/src/LUASprites.egg-info/dependency_links.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)       49 2023-06-08 20:18:05.000000 LUASprites-0.0.24/src/LUASprites.egg-info/entry_points.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)      119 2023-06-08 20:18:05.000000 LUASprites-0.0.24/src/LUASprites.egg-info/requires.txt
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)       10 2023-06-08 20:18:05.000000 LUASprites-0.0.24/src/LUASprites.egg-info/top_level.txt
+drwxr-xr-x   0 ajsteinhauser   (501) staff       (20)        0 2023-06-08 20:18:05.446901 LUASprites-0.0.24/src/spritegen/
+-rw-r--r--   0 ajsteinhauser   (501) staff       (20)    10625 2023-06-08 19:58:42.000000 LUASprites-0.0.24/src/spritegen/cli.py
```

### Comparing `LUASprites-0.0.23/LICENSE.txt` & `LUASprites-0.0.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LUASprites-0.0.23/PKG-INFO` & `LUASprites-0.0.24/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LUASprites
-Version: 0.0.23
+Version: 0.0.24
 Summary: Generate spritesheets and lua modules for easy image reference
 Home-page: https://github.com/AJSteinhauser/LUASprites
 Author: AJ Steinhauser
 Author-email: ajsteinhauser11@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `LUASprites-0.0.23/README.md` & `LUASprites-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `LUASprites-0.0.23/setup.py` & `LUASprites-0.0.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 
 setup(
     name = 'LUASprites',
-    version = '0.0.23',
+    version = '0.0.24',
     author = 'AJ Steinhauser',
     author_email = 'ajsteinhauser11@gmail.com',
     license = 'MIT License',
     description = 'Generate spritesheets and lua modules for easy image reference',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/AJSteinhauser/LUASprites',
@@ -23,10 +23,10 @@
     python_requires='>=3.7',
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
     ],
     entry_points = '''
         [console_scripts]
-        luasprites=spritegen.cli:main
+        luasprite=spritegen.cli:main
     '''
 )
```

### Comparing `LUASprites-0.0.23/src/LUASprites.egg-info/PKG-INFO` & `LUASprites-0.0.24/src/LUASprites.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LUASprites
-Version: 0.0.23
+Version: 0.0.24
 Summary: Generate spritesheets and lua modules for easy image reference
 Home-page: https://github.com/AJSteinhauser/LUASprites
 Author: AJ Steinhauser
 Author-email: ajsteinhauser11@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
```

### Comparing `LUASprites-0.0.23/src/spritegen/cli.py` & `LUASprites-0.0.24/src/spritegen/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,16 +271,16 @@
             idx = ""
         output += genLuaTableHelper(tree, name, idx)
     return output
         
 # This function goes to a counter api which lets me see how this application is being used and what features are being used most often. No personal data is being sent or anything linkable to yourself
 # Having the usage data allows me to better prioritize what features to update/make better 
 # Please don't spam the api, this is an open source tool and this data helps me tremendously 
-def usageTrack(usecase):
-    requests.get('https://api.countapi.xyz/hit/SpriteSheetGenerator_Deploy1/' + usecase)
+#def usageTrack(usecase):
+    #requests.get('https://api.countapi.xyz/hit/SpriteSheetGenerator_Deploy1/' + usecase)
 
 
 def init():
     print(BANNER)
     usageTrack("start")
```

