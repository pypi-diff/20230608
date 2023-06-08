# Comparing `tmp/fer-22.5.0.tar.gz` & `tmp/fer-22.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fer-22.5.0.tar", last modified: Tue Jan 31 14:13:22 2023, max compression
+gzip compressed data, was "dist/fer-22.5.1.tar", last modified: Thu Jun  8 16:27:50 2023, max compression
```

## Comparing `fer-22.5.0.tar` & `fer-22.5.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-01-31 14:13:22.209092 fer-22.5.0/
--rw-r--r--   0 justinshenk   (501) staff       (20)      119 2022-02-21 14:14:23.000000 fer-22.5.0/.flake8
-drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-01-31 14:13:22.173106 fer-22.5.0/.github/
-drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-01-31 14:13:22.184247 fer-22.5.0/.github/workflows/
--rw-r--r--   0 justinshenk   (501) staff       (20)     1382 2022-11-08 10:54:59.000000 fer-22.5.0/.github/workflows/tests.yaml
--rw-r--r--   0 justinshenk   (501) staff       (20)     1233 2021-03-10 20:07:36.000000 fer-22.5.0/.gitignore
--rw-r--r--   0 justinshenk   (501) staff       (20)      208 2022-02-21 14:13:33.000000 fer-22.5.0/.pre-commit-config.yaml
--rw-r--r--   0 justinshenk   (501) staff       (20)     1328 2021-09-22 19:29:54.000000 fer-22.5.0/.travis.yml
--rw-r--r--   0 justinshenk   (501) staff       (20)       36 2021-03-10 20:07:36.000000 fer-22.5.0/AUTHORS
--rw-r--r--   0 justinshenk   (501) staff       (20)      418 2021-09-01 15:40:18.000000 fer-22.5.0/CITATION
--rw-r--r--   0 justinshenk   (501) staff       (20)      675 2021-07-09 09:02:34.000000 fer-22.5.0/Dockerfile
--rw-r--r--   0 justinshenk   (501) staff       (20)     1068 2021-03-10 20:07:36.000000 fer-22.5.0/LICENSE
--rw-r--r--   0 justinshenk   (501) staff       (20)      154 2021-03-10 20:07:36.000000 fer-22.5.0/MANIFEST.in
--rw-r--r--   0 justinshenk   (501) staff       (20)     5766 2023-01-31 14:13:22.209461 fer-22.5.0/PKG-INFO
--rw-r--r--   0 justinshenk   (501) staff       (20)     4781 2022-11-08 10:55:05.000000 fer-22.5.0/README.md
--rw-r--r--   0 justinshenk   (501) staff       (20)     4576 2021-03-26 13:19:38.000000 fer-22.5.0/README.rst
--rw-r--r--   0 justinshenk   (501) staff       (20)     2244 2023-01-31 14:12:44.000000 fer-22.5.0/demo.py
--rw-r--r--   0 justinshenk   (501) staff       (20)      131 2022-02-21 21:23:10.000000 fer-22.5.0/docker-compose.yml
--rw-r--r--   0 justinshenk   (501) staff       (20)     1729 2021-09-22 19:36:36.000000 fer-22.5.0/environment.yml
--rw-r--r--   0 justinshenk   (501) staff       (20)   224583 2021-09-22 19:36:36.000000 fer-22.5.0/fer-video-demo.ipynb
--rw-r--r--   0 justinshenk   (501) staff       (20)    33426 2021-03-10 20:07:36.000000 fer-22.5.0/justin.jpg
--rw-r--r--   0 justinshenk   (501) staff       (20)    11467 2021-03-10 20:07:36.000000 fer-22.5.0/no-faces.jpg
--rw-r--r--   0 justinshenk   (501) staff       (20)      139 2023-01-31 14:13:07.000000 fer-22.5.0/requirements.txt
--rw-r--r--   0 justinshenk   (501) staff       (20)    71411 2021-03-10 20:07:36.000000 fer-22.5.0/result.jpg
--rw-r--r--   0 justinshenk   (501) staff       (20)      131 2023-01-31 14:13:22.210152 fer-22.5.0/setup.cfg
--rw-r--r--   0 justinshenk   (501) staff       (20)     2706 2023-01-31 14:13:07.000000 fer-22.5.0/setup.py
-drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-01-31 14:13:22.173450 fer-22.5.0/src/
-drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-01-31 14:13:22.185809 fer-22.5.0/src/fer/
--rw-r--r--   0 justinshenk   (501) staff       (20)     1630 2023-01-31 14:13:07.000000 fer-22.5.0/src/fer/__init__.py
--rw-r--r--   0 justinshenk   (501) staff       (20)    12702 2023-01-31 14:13:07.000000 fer-22.5.0/src/fer/classes.py
-drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-01-31 14:13:22.195355 fer-22.5.0/src/fer/data/
--rw-r--r--   0 justinshenk   (501) staff       (20)   872856 2021-03-10 20:07:36.000000 fer-22.5.0/src/fer/data/emotion_model.hdf5
--rwxr-xr-x   0 justinshenk   (501) staff       (20)  1254733 2021-03-10 20:07:36.000000 fer-22.5.0/src/fer/data/haarcascade_frontalface_default.xml
--rw-r--r--   0 justinshenk   (501) staff       (20)   729940 2023-01-31 14:13:07.000000 fer-22.5.0/src/fer/data/mmod_human_face_detector.dat
--rw-r--r--   0 justinshenk   (501) staff       (20)      901 2023-01-31 14:13:07.000000 fer-22.5.0/src/fer/emotionsmultilanguage.py
-drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-01-31 14:13:22.197181 fer-22.5.0/src/fer/exceptions/
--rw-r--r--   0 justinshenk   (501) staff       (20)     1222 2021-03-10 20:07:36.000000 fer-22.5.0/src/fer/exceptions/__init__.py
--rw-r--r--   0 justinshenk   (501) staff       (20)    11555 2023-01-31 14:13:07.000000 fer-22.5.0/src/fer/fer.py
--rw-r--r--   0 justinshenk   (501) staff       (20)     3072 2023-01-31 14:13:07.000000 fer-22.5.0/src/fer/utils.py
-drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-01-31 14:13:22.187462 fer-22.5.0/src/fer.egg-info/
--rw-r--r--   0 justinshenk   (501) staff       (20)     5766 2023-01-31 14:13:21.000000 fer-22.5.0/src/fer.egg-info/PKG-INFO
--rw-r--r--   0 justinshenk   (501) staff       (20)      797 2023-01-31 14:13:21.000000 fer-22.5.0/src/fer.egg-info/SOURCES.txt
--rw-r--r--   0 justinshenk   (501) staff       (20)        1 2023-01-31 14:13:21.000000 fer-22.5.0/src/fer.egg-info/dependency_links.txt
--rw-r--r--   0 justinshenk   (501) staff       (20)        1 2021-03-26 12:54:41.000000 fer-22.5.0/src/fer.egg-info/not-zip-safe
--rw-r--r--   0 justinshenk   (501) staff       (20)      170 2023-01-31 14:13:21.000000 fer-22.5.0/src/fer.egg-info/requires.txt
--rw-r--r--   0 justinshenk   (501) staff       (20)        4 2023-01-31 14:13:21.000000 fer-22.5.0/src/fer.egg-info/top_level.txt
-drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-01-31 14:13:22.203001 fer-22.5.0/tests/
--rw-r--r--   0 justinshenk   (501) staff       (20)        0 2021-03-10 20:07:36.000000 fer-22.5.0/tests/__init__.py
--rw-r--r--   0 justinshenk   (501) staff       (20)   556991 2021-03-10 20:07:36.000000 fer-22.5.0/tests/test.mp4
--rw-r--r--   0 justinshenk   (501) staff       (20)     2686 2022-03-13 17:44:40.000000 fer-22.5.0/tests/test_fer.py
--rw-r--r--   0 justinshenk   (501) staff       (20)  1870999 2021-03-10 20:07:36.000000 fer-22.5.0/tests/woman2.mp4
+drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-06-08 16:27:50.066758 fer-22.5.1/
+-rw-r--r--   0 justinshenk   (501) staff       (20)      119 2022-02-21 14:14:23.000000 fer-22.5.1/.flake8
+drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-06-08 16:27:49.995684 fer-22.5.1/.github/
+drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-06-08 16:27:50.025500 fer-22.5.1/.github/workflows/
+-rw-r--r--   0 justinshenk   (501) staff       (20)     1382 2022-11-08 10:54:59.000000 fer-22.5.1/.github/workflows/tests.yaml
+-rw-r--r--   0 justinshenk   (501) staff       (20)     1233 2021-03-10 20:07:36.000000 fer-22.5.1/.gitignore
+-rw-r--r--   0 justinshenk   (501) staff       (20)      208 2022-02-21 14:13:33.000000 fer-22.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 justinshenk   (501) staff       (20)     1328 2021-09-22 19:29:54.000000 fer-22.5.1/.travis.yml
+-rw-r--r--   0 justinshenk   (501) staff       (20)       36 2021-03-10 20:07:36.000000 fer-22.5.1/AUTHORS
+-rw-r--r--   0 justinshenk   (501) staff       (20)      418 2021-09-01 15:40:18.000000 fer-22.5.1/CITATION
+-rw-r--r--   0 justinshenk   (501) staff       (20)      675 2021-07-09 09:02:34.000000 fer-22.5.1/Dockerfile
+-rw-r--r--   0 justinshenk   (501) staff       (20)     1068 2021-03-10 20:07:36.000000 fer-22.5.1/LICENSE
+-rw-r--r--   0 justinshenk   (501) staff       (20)      154 2021-03-10 20:07:36.000000 fer-22.5.1/MANIFEST.in
+-rw-r--r--   0 justinshenk   (501) staff       (20)     5766 2023-06-08 16:27:50.066960 fer-22.5.1/PKG-INFO
+-rw-r--r--   0 justinshenk   (501) staff       (20)     4781 2022-11-08 10:55:05.000000 fer-22.5.1/README.md
+-rw-r--r--   0 justinshenk   (501) staff       (20)     4576 2021-03-26 13:19:38.000000 fer-22.5.1/README.rst
+-rw-r--r--   0 justinshenk   (501) staff       (20)     2244 2023-01-31 14:12:44.000000 fer-22.5.1/demo.py
+-rw-r--r--   0 justinshenk   (501) staff       (20)      131 2022-02-21 21:23:10.000000 fer-22.5.1/docker-compose.yml
+-rw-r--r--   0 justinshenk   (501) staff       (20)     1729 2021-09-22 19:36:36.000000 fer-22.5.1/environment.yml
+-rw-r--r--   0 justinshenk   (501) staff       (20)   224583 2021-09-22 19:36:36.000000 fer-22.5.1/fer-video-demo.ipynb
+-rw-r--r--   0 justinshenk   (501) staff       (20)    33426 2021-03-10 20:07:36.000000 fer-22.5.1/justin.jpg
+-rw-r--r--   0 justinshenk   (501) staff       (20)    11467 2021-03-10 20:07:36.000000 fer-22.5.1/no-faces.jpg
+-rw-r--r--   0 justinshenk   (501) staff       (20)      139 2023-01-31 14:13:07.000000 fer-22.5.1/requirements.txt
+-rw-r--r--   0 justinshenk   (501) staff       (20)    71411 2021-03-10 20:07:36.000000 fer-22.5.1/result.jpg
+-rw-r--r--   0 justinshenk   (501) staff       (20)      131 2023-06-08 16:27:50.067561 fer-22.5.1/setup.cfg
+-rw-r--r--   0 justinshenk   (501) staff       (20)     2785 2023-06-08 16:27:12.000000 fer-22.5.1/setup.py
+drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-06-08 16:27:49.997247 fer-22.5.1/src/
+drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-06-08 16:27:50.031556 fer-22.5.1/src/fer/
+-rw-r--r--   0 justinshenk   (501) staff       (20)     1630 2023-06-08 16:26:29.000000 fer-22.5.1/src/fer/__init__.py
+-rw-r--r--   0 justinshenk   (501) staff       (20)    12702 2023-01-31 14:13:07.000000 fer-22.5.1/src/fer/classes.py
+drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-06-08 16:27:50.048204 fer-22.5.1/src/fer/data/
+-rw-r--r--   0 justinshenk   (501) staff       (20)   872856 2021-03-10 20:07:36.000000 fer-22.5.1/src/fer/data/emotion_model.hdf5
+-rwxr-xr-x   0 justinshenk   (501) staff       (20)  1254733 2021-03-10 20:07:36.000000 fer-22.5.1/src/fer/data/haarcascade_frontalface_default.xml
+-rw-r--r--   0 justinshenk   (501) staff       (20)   729940 2023-01-31 14:13:07.000000 fer-22.5.1/src/fer/data/mmod_human_face_detector.dat
+-rw-r--r--   0 justinshenk   (501) staff       (20)      901 2023-01-31 14:13:07.000000 fer-22.5.1/src/fer/emotionsmultilanguage.py
+drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-06-08 16:27:50.053241 fer-22.5.1/src/fer/exceptions/
+-rw-r--r--   0 justinshenk   (501) staff       (20)     1222 2021-03-10 20:07:36.000000 fer-22.5.1/src/fer/exceptions/__init__.py
+-rw-r--r--   0 justinshenk   (501) staff       (20)    11555 2023-01-31 14:13:07.000000 fer-22.5.1/src/fer/fer.py
+-rw-r--r--   0 justinshenk   (501) staff       (20)     3072 2023-01-31 14:13:07.000000 fer-22.5.1/src/fer/utils.py
+drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-06-08 16:27:50.036878 fer-22.5.1/src/fer.egg-info/
+-rw-r--r--   0 justinshenk   (501) staff       (20)     5766 2023-06-08 16:27:49.000000 fer-22.5.1/src/fer.egg-info/PKG-INFO
+-rw-r--r--   0 justinshenk   (501) staff       (20)      797 2023-06-08 16:27:49.000000 fer-22.5.1/src/fer.egg-info/SOURCES.txt
+-rw-r--r--   0 justinshenk   (501) staff       (20)        1 2023-06-08 16:27:49.000000 fer-22.5.1/src/fer.egg-info/dependency_links.txt
+-rw-r--r--   0 justinshenk   (501) staff       (20)        1 2021-03-26 12:54:41.000000 fer-22.5.1/src/fer.egg-info/not-zip-safe
+-rw-r--r--   0 justinshenk   (501) staff       (20)      221 2023-06-08 16:27:49.000000 fer-22.5.1/src/fer.egg-info/requires.txt
+-rw-r--r--   0 justinshenk   (501) staff       (20)        4 2023-06-08 16:27:49.000000 fer-22.5.1/src/fer.egg-info/top_level.txt
+drwxr-xr-x   0 justinshenk   (501) staff       (20)        0 2023-06-08 16:27:50.059521 fer-22.5.1/tests/
+-rw-r--r--   0 justinshenk   (501) staff       (20)        0 2021-03-10 20:07:36.000000 fer-22.5.1/tests/__init__.py
+-rw-r--r--   0 justinshenk   (501) staff       (20)   556991 2021-03-10 20:07:36.000000 fer-22.5.1/tests/test.mp4
+-rw-r--r--   0 justinshenk   (501) staff       (20)     2686 2022-03-13 17:44:40.000000 fer-22.5.1/tests/test_fer.py
+-rw-r--r--   0 justinshenk   (501) staff       (20)  1870999 2021-03-10 20:07:36.000000 fer-22.5.1/tests/woman2.mp4
```

### Comparing `fer-22.5.0/.github/workflows/tests.yaml` & `fer-22.5.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/.gitignore` & `fer-22.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/.travis.yml` & `fer-22.5.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/Dockerfile` & `fer-22.5.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/LICENSE` & `fer-22.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/PKG-INFO` & `fer-22.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fer
-Version: 22.5.0
+Version: 22.5.1
 Summary: Facial expression recognition from images
 Home-page: https://github.com/justinshenk/fer
 Author: Justin Shenk
 Author-email: shenkjustin@gmail.com
 Maintainer: Justin Shenk
 Maintainer-email: shenkjustin@gmail.com
 License: MIT
```

### Comparing `fer-22.5.0/README.md` & `fer-22.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/README.rst` & `fer-22.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/demo.py` & `fer-22.5.1/demo.py`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/environment.yml` & `fer-22.5.1/environment.yml`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/fer-video-demo.ipynb` & `fer-22.5.1/fer-video-demo.ipynb`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/justin.jpg` & `fer-22.5.1/justin.jpg`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/no-faces.jpg` & `fer-22.5.1/no-faces.jpg`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/result.jpg` & `fer-22.5.1/result.jpg`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/setup.py` & `fer-22.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,19 @@
 INSTALL_REQUIRES = [
     "matplotlib",
     "opencv-contrib-python",
     "keras>=2.0.0",
     "pandas",
     "requests",
     "facenet-pytorch",
-    "tqdm",
+    "tqdm>=4.62.1",
+    "moviepy",
+    "facenet-pytorch",
+    "ffmpeg==1.4",
+    "Pillow",
 ]
 
 EXTRAS_REQUIRE = {"docs": ["sphinx"], "tests": ["coverage", "pytest"]}
 EXTRAS_REQUIRE["dev"] = (
     EXTRAS_REQUIRE["tests"] + EXTRAS_REQUIRE["docs"] + ["wheel", "pre-commit"]
 )
```

### Comparing `fer-22.5.0/src/fer/__init__.py` & `fer-22.5.1/src/fer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 from .classes import Video
 from .fer import FER
 
 log = logging.getLogger("fer")
 log.setLevel(logging.INFO)
 
-__version__ = "22.5.0"
+__version__ = "22.5.1"
 
 __title__ = "fer"
 __description__ = "Facial expression recognition from images"
 __url__ = "https://github.com/justinshenk/fer"
 __uri__ = __url__
 __doc__ = __description__ + " <" + __url__ + ">"
```

### Comparing `fer-22.5.0/src/fer/classes.py` & `fer-22.5.1/src/fer/classes.py`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/src/fer/data/emotion_model.hdf5` & `fer-22.5.1/src/fer/data/emotion_model.hdf5`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/src/fer/data/haarcascade_frontalface_default.xml` & `fer-22.5.1/src/fer/data/haarcascade_frontalface_default.xml`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/src/fer/data/mmod_human_face_detector.dat` & `fer-22.5.1/src/fer/data/mmod_human_face_detector.dat`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/src/fer/emotionsmultilanguage.py` & `fer-22.5.1/src/fer/emotionsmultilanguage.py`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/src/fer/exceptions/__init__.py` & `fer-22.5.1/src/fer/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/src/fer/fer.py` & `fer-22.5.1/src/fer/fer.py`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/src/fer/utils.py` & `fer-22.5.1/src/fer/utils.py`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/src/fer.egg-info/PKG-INFO` & `fer-22.5.1/src/fer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fer
-Version: 22.5.0
+Version: 22.5.1
 Summary: Facial expression recognition from images
 Home-page: https://github.com/justinshenk/fer
 Author: Justin Shenk
 Author-email: shenkjustin@gmail.com
 Maintainer: Justin Shenk
 Maintainer-email: shenkjustin@gmail.com
 License: MIT
```

### Comparing `fer-22.5.0/src/fer.egg-info/SOURCES.txt` & `fer-22.5.1/src/fer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/tests/test.mp4` & `fer-22.5.1/tests/test.mp4`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/tests/test_fer.py` & `fer-22.5.1/tests/test_fer.py`

 * *Files identical despite different names*

### Comparing `fer-22.5.0/tests/woman2.mp4` & `fer-22.5.1/tests/woman2.mp4`

 * *Files identical despite different names*

