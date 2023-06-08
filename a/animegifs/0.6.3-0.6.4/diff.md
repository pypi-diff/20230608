# Comparing `tmp/animegifs-0.6.3.tar.gz` & `tmp/animegifs-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animegifs-0.6.3.tar", last modified: Tue Jun  6 22:57:06 2023, max compression
+gzip compressed data, was "animegifs-0.6.4.tar", last modified: Thu Jun  8 15:56:03 2023, max compression
```

## Comparing `animegifs-0.6.3.tar` & `animegifs-0.6.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 22:57:06.187573 animegifs-0.6.3/
--rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.6.3/LICENSE
--rw-rw-rw-   0        0        0     3248 2023-06-06 22:57:06.186570 animegifs-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     2464 2023-06-05 17:42:11.000000 animegifs-0.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 22:57:06.168570 animegifs-0.6.3/animegifs/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.6.3/animegifs/__init__.py
--rw-rw-rw-   0        0        0     3388 2023-06-05 16:14:15.000000 animegifs-0.6.3/animegifs/animegifs.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:57:06.184570 animegifs-0.6.3/animegifs/distutils/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.6.3/animegifs/distutils/__init__.py
--rw-rw-rw-   0        0        0     2320 2023-06-06 22:10:28.000000 animegifs-0.6.3/animegifs/distutils/errors.py
--rw-rw-rw-   0        0        0     2011 2023-06-06 22:09:58.000000 animegifs-0.6.3/animegifs/distutils/gifs.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:57:06.179569 animegifs-0.6.3/animegifs.egg-info/
--rw-rw-rw-   0        0        0     3248 2023-06-06 22:57:06.000000 animegifs-0.6.3/animegifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-06-06 22:57:06.000000 animegifs-0.6.3/animegifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 22:57:06.000000 animegifs-0.6.3/animegifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-06 22:57:06.000000 animegifs-0.6.3/animegifs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-06 22:57:06.000000 animegifs-0.6.3/animegifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 22:57:06.188571 animegifs-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1282 2023-06-06 22:09:58.000000 animegifs-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:56:03.451429 animegifs-0.6.4/
+-rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.6.4/LICENSE
+-rw-rw-rw-   0        0        0     3869 2023-06-08 15:56:03.450428 animegifs-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3075 2023-06-08 15:41:36.000000 animegifs-0.6.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 15:56:03.427427 animegifs-0.6.4/animegifs/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.6.4/animegifs/__init__.py
+-rw-rw-rw-   0        0        0     3401 2023-06-08 14:53:25.000000 animegifs-0.6.4/animegifs/animegifs.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:56:03.448431 animegifs-0.6.4/animegifs/distutils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.6.4/animegifs/distutils/__init__.py
+-rw-rw-rw-   0        0        0     2331 2023-06-08 15:47:16.000000 animegifs-0.6.4/animegifs/distutils/errors.py
+-rw-rw-rw-   0        0        0     2026 2023-06-08 14:53:25.000000 animegifs-0.6.4/animegifs/distutils/gifs.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:56:03.438429 animegifs-0.6.4/animegifs.egg-info/
+-rw-rw-rw-   0        0        0     3869 2023-06-08 15:56:03.000000 animegifs-0.6.4/animegifs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-06-08 15:56:03.000000 animegifs-0.6.4/animegifs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 15:56:03.000000 animegifs-0.6.4/animegifs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-08 15:56:03.000000 animegifs-0.6.4/animegifs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-08 15:56:03.000000 animegifs-0.6.4/animegifs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 15:56:03.451429 animegifs-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1282 2023-06-08 14:59:43.000000 animegifs-0.6.4/setup.py
```

### Comparing `animegifs-0.6.3/LICENSE` & `animegifs-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `animegifs-0.6.3/PKG-INFO` & `animegifs-0.6.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,126 +1,115 @@
-Metadata-Version: 2.1
-Name: animegifs
-Version: 0.6.3
-Summary: Get random anime gifs by category.
-Home-page: https://github.com/MarcoSa-2000/animegifs
-Author: Marco-Sa2000
-Author-email: grest0grest@gmail.com
-License: MIT
-Keywords: anime,gif,python,anime-gif,discord
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# animegifs.py
-<p align="center">
-    <a href="https://pypi.org/project/animegifs/">
-    <img src="https://img.shields.io/pypi/dm/animegifs?logo=PyPI&style=for-the-badge" alt="PyPi Downloads"/></a>
-    <a href="https://discord.gg/TKZJ4GJj2z">
-    <img src="https://img.shields.io/discord/856005478789677096?logo=Discord&style=for-the-badge" alt="Discord Server"/></a>
-    <a href="https://pypi.org/project/animegifs/">
-    <img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/MarcoSa-2000/animegifs?style=for-the-badge"></a>
-    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/animegifs?logo=Python&logoColor=%23FFFF00&style=for-the-badge">
-    <img alt="GitHub watchers" src="https://img.shields.io/github/watchers/MarcoSa-2000/animegifs?style=social">
-</p>
-
-Get random anime gifs by category. Use Python (intended (for now) for Discord).
-
-WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all. Version below v0.6 will not have the gifs library updated anymore.
-
-`pip install animegifs`
-
-# HOW TO USE
-```py
-#v0.5.3>
-from animegifs import animegifs
-
-gifs = animegifs.Animegifs()
-
-gif = gifs.get_gif(category) #return the url of the gif.
-```
-
-```py
-#v0.6>
-from animegifs import animegifs
-
-gifs = animegifs.Animegifs()
-
-gif = gifs.get_gif(category) #return the url of the gif.
-mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
-title = gifs.get_animetitle(gif) #get the title of the gif's anime.
-malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page.
-```
-
-**Category list:** 
-
-* Attack
-* Bite
-* Bloodsuck
-* Blush
-* Bonk
-* Brofist
-* Cry
-* Cuddle
-* Dance
-* Disgust
-* Exploding
-* Facedesk
-* Facepalm
-* Flick
-* Flirt
-* Handhold
-* Happy
-* Harass
-* Highfive
-* Hug
-* Icecream
-* Insult
-* Kill
-* Kiss
-* Lick
-* Love
-* Marry
-* Nod
-* Nosebleed
-* Nuzzle
-* Pat
-* Peck
-* Poke
-* Popcorn
-* Pout
-* Punch
-* Punish
-* Run
-* Sad
-* Scared
-* Shoot
-* Shrug
-* Sip
-* Slap
-* Smirk
-* Sorry
-* Spank
-* Stare
-* Tease
-* Threat
-* Tickle
-* Tired
-* Wave
-* Yawn
-
-**Special Category List**
-
-* Random
-* Steal-magic
-
-# Troubleshooting and other
-
-If you encounter an error raise an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues 
-or join the discord server to request new categories, new functions, feedback and even errors.
+# animegifs.py
+<p align="center">
+    <a href="https://pypi.org/project/animegifs/">
+    <img src="https://img.shields.io/pypi/dm/animegifs?logo=PyPI&style=for-the-badge" alt="PyPi Downloads"/></a>
+    <a href="https://discord.gg/TKZJ4GJj2z">
+    <img src="https://img.shields.io/discord/856005478789677096?logo=Discord&style=for-the-badge" alt="Discord Server"/></a>
+    <a href="https://pypi.org/project/animegifs/">
+    <img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/MarcoSa-2000/animegifs?style=for-the-badge"></a>
+    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/animegifs?logo=Python&logoColor=%23FFFF00&style=for-the-badge">
+    <img alt="GitHub watchers" src="https://img.shields.io/github/watchers/MarcoSa-2000/animegifs?style=social">
+</p>
+
+Get random anime gifs by category. Use Python (intended (for now) for Discord).
+
+WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all. Version below v0.6 will not have the gifs library updated anymore.
+
+`pip install animegifs`
+
+# HOW TO USE
+```py
+#v0.5.3>
+from animegifs import animegifs
+
+gifs = animegifs.Animegifs()
+
+gif = gifs.get_gif(category) #return the url of the gif.
+```
+
+```py
+#v0.6>
+from animegifs import animegifs
+
+gifs = animegifs.Animegifs()
+
+gif = gifs.get_gif(category) #gifs.get_gif('hug') and return the url of the gif.
+mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
+title = gifs.get_animetitle(gif) #get the title of the gif's anime.
+malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page.
+```
+
+**Category list:** 
+
+* Attack
+* Bite
+* Bloodsuck
+* Blush
+* Bonk
+* Brofist
+* Cry
+* Cuddle
+* Dance
+* Disgust
+* Exploding
+* Facedesk
+* Facepalm
+* Flick
+* Flirt
+* Handhold
+* Happy
+* Harass
+* Highfive
+* Hug
+* Icecream
+* Insult
+* Kill
+* Kiss
+* Lick
+* Love
+* Marry
+* Nod
+* Nosebleed
+* Nuzzle
+* Pat
+* Peck
+* Poke
+* Popcorn
+* Pout
+* Punch
+* Punish
+* Run
+* Sad
+* Scared
+* Shoot
+* Shrug
+* Sip
+* Slap
+* Smirk
+* Sorry
+* Spank
+* Stare
+* Tease
+* Threat
+* Tickle
+* Tired
+* Wave
+* Yawn
+
+**Special Category List**
+
+* Random
+* Steal-magic
+
+# Troubleshooting and other
+
+If you encounter an error, please raise an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues. 
+Alternatively, you can join my Discord server to request new categories, functions, provide feedback, or report any errors. 
+I do also have a multi-function Discord bot. Feel free to check out the web dashboard here: https://enkidu-app.github.io.
+
+# Copyright
+
+This repository doesn't include any copyrighted material. 
+If you happen to come across any copyrighted content within this repository (but hosted elsewhere) that you own or represent, 
+email me at **grest0grest@gmail.com**. 
+Please provide specific details about the copyrighted material and where it can be found.
+Once I confirm your claim, I'll take immediate action to remove the identified material.
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1 Name: animegifs Version: 0.6.3 Summary: Get random anime
-gifs by category. Home-page: https://github.com/MarcoSa-2000/animegifs Author:
-Marco-Sa2000 Author-email: grest0grest@gmail.com License: MIT Keywords:
-anime,gif,python,anime-gif,discord Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: Microsoft :: Windows Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE # animegifs.py
+# animegifs.py
   [PyPi_Downloads] [Discord_Server] [GitHub_release_(latest_by_date)] [PyPI -
                        Python Version] [GitHub watchers]
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 WIP - updated in time to time. Versions below v0.5.3 aren't expected to work
 flawlessly or at all. Version below v0.6 will not have the gifs library updated
 anymore. `pip install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs
 import animegifs gifs = animegifs.Animegifs() gif = gifs.get_gif(category)
 #return the url of the gif. ``` ```py #v0.6> from animegifs import animegifs
-gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #return the url of
-the gif. mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
-title = gifs.get_animetitle(gif) #get the title of the gif's anime. malid =
-gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page. ```
-**Category list:** * Attack * Bite * Bloodsuck * Blush * Bonk * Brofist * Cry *
-Cuddle * Dance * Disgust * Exploding * Facedesk * Facepalm * Flick * Flirt *
-Handhold * Happy * Harass * Highfive * Hug * Icecream * Insult * Kill * Kiss *
-Lick * Love * Marry * Nod * Nosebleed * Nuzzle * Pat * Peck * Poke * Popcorn *
-Pout * Punch * Punish * Run * Sad * Scared * Shoot * Shrug * Sip * Slap * Smirk
-* Sorry * Spank * Stare * Tease * Threat * Tickle * Tired * Wave * Yawn
-**Special Category List** * Random * Steal-magic # Troubleshooting and other If
-you encounter an error raise an issue on the issue page: https://github.com/
-MarcoSa-2000/animegifs/issues or join the discord server to request new
-categories, new functions, feedback and even errors.
+gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug')
+and return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's
+anime myanimelist page. title = gifs.get_animetitle(gif) #get the title of the
+gif's anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime
+myanimelist page. ``` **Category list:** * Attack * Bite * Bloodsuck * Blush *
+Bonk * Brofist * Cry * Cuddle * Dance * Disgust * Exploding * Facedesk *
+Facepalm * Flick * Flirt * Handhold * Happy * Harass * Highfive * Hug *
+Icecream * Insult * Kill * Kiss * Lick * Love * Marry * Nod * Nosebleed *
+Nuzzle * Pat * Peck * Poke * Popcorn * Pout * Punch * Punish * Run * Sad *
+Scared * Shoot * Shrug * Sip * Slap * Smirk * Sorry * Spank * Stare * Tease *
+Threat * Tickle * Tired * Wave * Yawn **Special Category List** * Random *
+Steal-magic # Troubleshooting and other If you encounter an error, please raise
+an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues.
+Alternatively, you can join my Discord server to request new categories,
+functions, provide feedback, or report any errors. I do also have a multi-
+function Discord bot. Feel free to check out the web dashboard here: https://
+enkidu-app.github.io. # Copyright This repository doesn't include any
+copyrighted material. If you happen to come across any copyrighted content
+within this repository (but hosted elsewhere) that you own or represent, email
+me at **grest0grest@gmail.com**. Please provide specific details about the
+copyrighted material and where it can be found. Once I confirm your claim, I'll
+take immediate action to remove the identified material.
```

### Comparing `animegifs-0.6.3/animegifs/animegifs.py` & `animegifs-0.6.4/animegifs/animegifs.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         Args:
             category (str): Valid categories: attack, bite, bloodsuck, blush, bonk,
                 brofist, cry, cuddle, dance, disgust, exploding, facedesk, facepalm, flick, flirt,
                 handhold, happy, harass, highfive, hug, icecream, insult, kill, kiss,
                 lick, love, marry, nod, nosebleed, nuzzle, pat, peck, poke, popcorn, pout,
                 punch, punish, random, run, sad, scared, shoot, shrug, sip, slap, smirk,
-                sorry, spank, stare, tease, threat, tickle, tired, wave, yawn.
+                sorry, spank, stare, steal-magic, tease, threat, tickle, tired, wave, yawn.
 
         Returns:
             gif: gif (url) -> str
         """
         if type(category) is int:
             raise errors.CategoryIntegral(category)
         if category.lower() in gifs.gifs_name_list:
```

### Comparing `animegifs-0.6.3/animegifs/distutils/errors.py` & `animegifs-0.6.4/animegifs/distutils/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,16 @@
     def __init__(self, gif, error="Method not yet available for this gif."):
         self.gif = gif
         self.error = error
         super().__init__(self.error)
 
 class AuthTimeout(Exception):
     """
-    Authentication request timed out. Probably status 504 on server side. Check your connection too.
+    Authentication request timed out. Probably status error 504 on server side.
+    Check your connection too.
     """
 
     def __init__(self, exc, error="Authentication request timed out."):
         self.exc = exc
         self.error = error
         super().__init__(self.error)
```

### Comparing `animegifs-0.6.3/animegifs/distutils/gifs.py` & `animegifs-0.6.4/animegifs/distutils/gifs.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                   'icecream', 'insult',
                   'kill', 'kiss',
                   'lick', 'love',
                   'marry',
                   'nod', 'nosebleed', 'nuzzle',
                   'pat', 'peck', 'poke', 'popcorn', 'pout', 'punch', 'punish',
                   'random', 'run',
-                  'sad', 'scared', 'shoot', 'shrug', 'sip', 'slap', 'smirk', 'sorry', 'spank', 'stare',
+                  'sad', 'scared', 'shoot', 'shrug', 'sip', 'slap', 'smirk', 'sorry', 'spank', 'stare', 'steal-magic',
                   'tease', 'threat', 'tickle', 'tired',
                   'wave',
                   'yawn']
 
 def authentication():
     try:
         response = requests.post("https://enkidu-app-5a3qq2fqya-uc.a.run.app/key1", timeout=100)
```

### Comparing `animegifs-0.6.3/animegifs.egg-info/PKG-INFO` & `animegifs-0.6.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.6.3
+Version: 0.6.4
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif,discord
 Classifier: Programming Language :: Python :: 3.8
@@ -48,15 +48,15 @@
 
 ```py
 #v0.6>
 from animegifs import animegifs
 
 gifs = animegifs.Animegifs()
 
-gif = gifs.get_gif(category) #return the url of the gif.
+gif = gifs.get_gif(category) #gifs.get_gif('hug') and return the url of the gif.
 mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
 title = gifs.get_animetitle(gif) #get the title of the gif's anime.
 malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page.
 ```
 
 **Category list:** 
 
@@ -118,9 +118,18 @@
 **Special Category List**
 
 * Random
 * Steal-magic
 
 # Troubleshooting and other
 
-If you encounter an error raise an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues 
-or join the discord server to request new categories, new functions, feedback and even errors.
+If you encounter an error, please raise an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues. 
+Alternatively, you can join my Discord server to request new categories, functions, provide feedback, or report any errors. 
+I do also have a multi-function Discord bot. Feel free to check out the web dashboard here: https://enkidu-app.github.io.
+
+# Copyright
+
+This repository doesn't include any copyrighted material. 
+If you happen to come across any copyrighted content within this repository (but hosted elsewhere) that you own or represent, 
+email me at **grest0grest@gmail.com**. 
+Please provide specific details about the copyrighted material and where it can be found.
+Once I confirm your claim, I'll take immediate action to remove the identified material.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: animegifs Version: 0.6.3 Summary: Get random anime
+Metadata-Version: 2.1 Name: animegifs Version: 0.6.4 Summary: Get random anime
 gifs by category. Home-page: https://github.com/MarcoSa-2000/animegifs Author:
 Marco-Sa2000 Author-email: grest0grest@gmail.com License: MIT Keywords:
 anime,gif,python,anime-gif,discord Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: Microsoft :: Windows Requires-Python: >=3.8 Description-
@@ -11,21 +11,29 @@
                        Python Version] [GitHub watchers]
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 WIP - updated in time to time. Versions below v0.5.3 aren't expected to work
 flawlessly or at all. Version below v0.6 will not have the gifs library updated
 anymore. `pip install animegifs` # HOW TO USE ```py #v0.5.3> from animegifs
 import animegifs gifs = animegifs.Animegifs() gif = gifs.get_gif(category)
 #return the url of the gif. ``` ```py #v0.6> from animegifs import animegifs
-gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #return the url of
-the gif. mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
-title = gifs.get_animetitle(gif) #get the title of the gif's anime. malid =
-gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page. ```
-**Category list:** * Attack * Bite * Bloodsuck * Blush * Bonk * Brofist * Cry *
-Cuddle * Dance * Disgust * Exploding * Facedesk * Facepalm * Flick * Flirt *
-Handhold * Happy * Harass * Highfive * Hug * Icecream * Insult * Kill * Kiss *
-Lick * Love * Marry * Nod * Nosebleed * Nuzzle * Pat * Peck * Poke * Popcorn *
-Pout * Punch * Punish * Run * Sad * Scared * Shoot * Shrug * Sip * Slap * Smirk
-* Sorry * Spank * Stare * Tease * Threat * Tickle * Tired * Wave * Yawn
-**Special Category List** * Random * Steal-magic # Troubleshooting and other If
-you encounter an error raise an issue on the issue page: https://github.com/
-MarcoSa-2000/animegifs/issues or join the discord server to request new
-categories, new functions, feedback and even errors.
+gifs = animegifs.Animegifs() gif = gifs.get_gif(category) #gifs.get_gif('hug')
+and return the url of the gif. mal = gifs.get_mal(gif) #get url of the gif's
+anime myanimelist page. title = gifs.get_animetitle(gif) #get the title of the
+gif's anime. malid = gifs.get_malId(gif) #get the ID of the gif's anime
+myanimelist page. ``` **Category list:** * Attack * Bite * Bloodsuck * Blush *
+Bonk * Brofist * Cry * Cuddle * Dance * Disgust * Exploding * Facedesk *
+Facepalm * Flick * Flirt * Handhold * Happy * Harass * Highfive * Hug *
+Icecream * Insult * Kill * Kiss * Lick * Love * Marry * Nod * Nosebleed *
+Nuzzle * Pat * Peck * Poke * Popcorn * Pout * Punch * Punish * Run * Sad *
+Scared * Shoot * Shrug * Sip * Slap * Smirk * Sorry * Spank * Stare * Tease *
+Threat * Tickle * Tired * Wave * Yawn **Special Category List** * Random *
+Steal-magic # Troubleshooting and other If you encounter an error, please raise
+an issue on the issue page: https://github.com/MarcoSa-2000/animegifs/issues.
+Alternatively, you can join my Discord server to request new categories,
+functions, provide feedback, or report any errors. I do also have a multi-
+function Discord bot. Feel free to check out the web dashboard here: https://
+enkidu-app.github.io. # Copyright This repository doesn't include any
+copyrighted material. If you happen to come across any copyrighted content
+within this repository (but hosted elsewhere) that you own or represent, email
+me at **grest0grest@gmail.com**. Please provide specific details about the
+copyrighted material and where it can be found. Once I confirm your claim, I'll
+take immediate action to remove the identified material.
```

### Comparing `animegifs-0.6.3/setup.py` & `animegifs-0.6.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 LONG_DESCRIPTION = long_description
-VERSION = '0.6.3'
+VERSION = '0.6.4'
 
 setup(
     name='animegifs',
     package_dir={"anime_gifs": "animegifs"},
     packages=["animegifs", "animegifs.distutils"],
     version=VERSION,
     description='Get random anime gifs by category.',
```

