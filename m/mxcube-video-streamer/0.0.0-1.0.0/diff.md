# Comparing `tmp/mxcube_video_streamer-0.0.0.tar.gz` & `tmp/mxcube_video_streamer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxcube_video_streamer-0.0.0.tar", max compression
+gzip compressed data, was "mxcube_video_streamer-1.0.0.tar", max compression
```

## Comparing `mxcube_video_streamer-0.0.0.tar` & `mxcube_video_streamer-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     2637 2023-05-16 08:12:41.872103 mxcube_video_streamer-0.0.0/README.md
--rw-r--r--   0        0        0     1567 2023-06-08 07:08:30.636284 mxcube_video_streamer-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-06 10:38:58.256450 mxcube_video_streamer-0.0.0/video_streamer/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 10:38:58.416494 mxcube_video_streamer-0.0.0/video_streamer/__main__.py
--rw-r--r--   0        0        0        0 2023-03-06 10:38:58.340473 mxcube_video_streamer-0.0.0/video_streamer/core/__init__.py
--rw-r--r--   0        0        0      163 2023-05-22 11:18:09.378453 mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      155 2023-03-06 10:38:58.304463 mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     4618 2023-05-22 11:18:09.394453 mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/camera.cpython-310.pyc
--rw-r--r--   0        0        0     4412 2023-03-06 10:38:58.288459 mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/camera.cpython-37.pyc
--rw-r--r--   0        0        0     1713 2023-05-22 11:18:09.658452 mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0     1534 2023-03-06 10:38:58.272454 mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/config.cpython-37.pyc
--rw-r--r--   0        0        0     1907 2023-03-06 10:38:58.300462 mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/ffmpegstreamer.cpython-310.pyc
--rw-r--r--   0        0        0     4370 2023-05-22 11:18:09.382453 mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/streamer.cpython-310.pyc
--rw-r--r--   0        0        0     3985 2023-03-06 10:38:58.308464 mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/streamer.cpython-37.pyc
--rw-r--r--   0        0        0     1252 2023-05-22 11:18:09.378453 mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/websockethandler.cpython-310.pyc
--rw-r--r--   0        0        0     1219 2023-03-06 10:38:58.280457 mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/websockethandler.cpython-37.pyc
--rw-r--r--   0        0        0     3838 2023-05-16 08:12:41.876103 mxcube_video_streamer-0.0.0/video_streamer/core/camera.py
--rw-r--r--   0        0        0     1137 2023-05-16 08:13:38.448106 mxcube_video_streamer-0.0.0/video_streamer/core/config.py
--rw-r--r--   0        0        0     1336 2023-05-16 08:04:24.344078 mxcube_video_streamer-0.0.0/video_streamer/core/config.py.orig
--rwxr-xr-x   0        0        0    81093 2023-03-06 10:38:58.336472 mxcube_video_streamer-0.0.0/video_streamer/core/fakeimg.jpg
--rw-r--r--   0        0        0     4279 2023-05-16 08:12:41.876103 mxcube_video_streamer-0.0.0/video_streamer/core/streamer.py
--rw-r--r--   0        0        0      653 2023-03-06 10:38:58.356477 mxcube_video_streamer-0.0.0/video_streamer/core/websockethandler.py
--rw-r--r--   0        0        0     3154 2023-05-16 08:12:41.876103 mxcube_video_streamer-0.0.0/video_streamer/main.py
--rw-r--r--   0        0        0     3032 2023-05-16 08:12:41.876103 mxcube_video_streamer-0.0.0/video_streamer/server.py
--rw-r--r--   0        0        0   138464 2023-03-06 10:38:58.404491 mxcube_video_streamer-0.0.0/video_streamer/ui/static/jsmpeg.min.js
--rw-r--r--   0        0        0      121 2023-05-16 08:12:41.876103 mxcube_video_streamer-0.0.0/video_streamer/ui/template/index_mjpeg.html
--rw-r--r--   0        0        0      413 2023-05-16 08:12:41.876103 mxcube_video_streamer-0.0.0/video_streamer/ui/template/index_mpeg1.html
--rw-r--r--   0        0        0   138464 2023-05-16 08:12:41.880103 mxcube_video_streamer-0.0.0/video_streamer/ui/template/jsmpeg.min.js
--rw-r--r--   0        0        0     3747 1970-01-01 00:00:00.000000 mxcube_video_streamer-0.0.0/setup.py
--rw-r--r--   0        0        0     3998 1970-01-01 00:00:00.000000 mxcube_video_streamer-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2637 2023-05-16 08:12:41.872103 mxcube_video_streamer-1.0.0/README.md
+-rw-r--r--   0        0        0     1567 2023-06-08 07:09:09.272239 mxcube_video_streamer-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-06 10:38:58.256450 mxcube_video_streamer-1.0.0/video_streamer/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 10:38:58.416494 mxcube_video_streamer-1.0.0/video_streamer/__main__.py
+-rw-r--r--   0        0        0        0 2023-03-06 10:38:58.340473 mxcube_video_streamer-1.0.0/video_streamer/core/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-22 11:18:09.378453 mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      155 2023-03-06 10:38:58.304463 mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     4618 2023-05-22 11:18:09.394453 mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/camera.cpython-310.pyc
+-rw-r--r--   0        0        0     4412 2023-03-06 10:38:58.288459 mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/camera.cpython-37.pyc
+-rw-r--r--   0        0        0     1713 2023-05-22 11:18:09.658452 mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0     1534 2023-03-06 10:38:58.272454 mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/config.cpython-37.pyc
+-rw-r--r--   0        0        0     1907 2023-03-06 10:38:58.300462 mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/ffmpegstreamer.cpython-310.pyc
+-rw-r--r--   0        0        0     4370 2023-05-22 11:18:09.382453 mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/streamer.cpython-310.pyc
+-rw-r--r--   0        0        0     3985 2023-03-06 10:38:58.308464 mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/streamer.cpython-37.pyc
+-rw-r--r--   0        0        0     1252 2023-05-22 11:18:09.378453 mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/websockethandler.cpython-310.pyc
+-rw-r--r--   0        0        0     1219 2023-03-06 10:38:58.280457 mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/websockethandler.cpython-37.pyc
+-rw-r--r--   0        0        0     3838 2023-05-16 08:12:41.876103 mxcube_video_streamer-1.0.0/video_streamer/core/camera.py
+-rw-r--r--   0        0        0     1137 2023-05-16 08:13:38.448106 mxcube_video_streamer-1.0.0/video_streamer/core/config.py
+-rw-r--r--   0        0        0     1336 2023-05-16 08:04:24.344078 mxcube_video_streamer-1.0.0/video_streamer/core/config.py.orig
+-rwxr-xr-x   0        0        0    81093 2023-03-06 10:38:58.336472 mxcube_video_streamer-1.0.0/video_streamer/core/fakeimg.jpg
+-rw-r--r--   0        0        0     4279 2023-05-16 08:12:41.876103 mxcube_video_streamer-1.0.0/video_streamer/core/streamer.py
+-rw-r--r--   0        0        0      653 2023-03-06 10:38:58.356477 mxcube_video_streamer-1.0.0/video_streamer/core/websockethandler.py
+-rw-r--r--   0        0        0     3154 2023-05-16 08:12:41.876103 mxcube_video_streamer-1.0.0/video_streamer/main.py
+-rw-r--r--   0        0        0     3032 2023-05-16 08:12:41.876103 mxcube_video_streamer-1.0.0/video_streamer/server.py
+-rw-r--r--   0        0        0   138464 2023-03-06 10:38:58.404491 mxcube_video_streamer-1.0.0/video_streamer/ui/static/jsmpeg.min.js
+-rw-r--r--   0        0        0      121 2023-05-16 08:12:41.876103 mxcube_video_streamer-1.0.0/video_streamer/ui/template/index_mjpeg.html
+-rw-r--r--   0        0        0      413 2023-05-16 08:12:41.876103 mxcube_video_streamer-1.0.0/video_streamer/ui/template/index_mpeg1.html
+-rw-r--r--   0        0        0   138464 2023-05-16 08:12:41.880103 mxcube_video_streamer-1.0.0/video_streamer/ui/template/jsmpeg.min.js
+-rw-r--r--   0        0        0     3747 1970-01-01 00:00:00.000000 mxcube_video_streamer-1.0.0/setup.py
+-rw-r--r--   0        0        0     3998 1970-01-01 00:00:00.000000 mxcube_video_streamer-1.0.0/PKG-INFO
```

### Comparing `mxcube_video_streamer-0.0.0/README.md` & `mxcube_video_streamer-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/pyproject.toml` & `mxcube_video_streamer-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mxcube_video_streamer"
-version = "0.0.0"
+version = "1.0.0"
 packages = [{include = "video_streamer"}]
 license = "MIT"
 description = "FastAPI Based video streamer"
 authors = ["Marcus Oskarsson <oscarsso@esrf.fr>"]
 maintainers = [
     "Marcus Oskarsson <oscarsso@esrf.fr>",
 ]
```

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/camera.cpython-310.pyc` & `mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/camera.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/camera.cpython-37.pyc` & `mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/camera.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/config.cpython-310.pyc` & `mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/config.cpython-37.pyc` & `mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/config.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/ffmpegstreamer.cpython-310.pyc` & `mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/ffmpegstreamer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/streamer.cpython-310.pyc` & `mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/streamer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/streamer.cpython-37.pyc` & `mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/streamer.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/websockethandler.cpython-310.pyc` & `mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/websockethandler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/core/__pycache__/websockethandler.cpython-37.pyc` & `mxcube_video_streamer-1.0.0/video_streamer/core/__pycache__/websockethandler.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/core/camera.py` & `mxcube_video_streamer-1.0.0/video_streamer/core/camera.py`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/core/config.py` & `mxcube_video_streamer-1.0.0/video_streamer/core/config.py`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/core/config.py.orig` & `mxcube_video_streamer-1.0.0/video_streamer/core/config.py.orig`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/core/fakeimg.jpg` & `mxcube_video_streamer-1.0.0/video_streamer/core/fakeimg.jpg`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/core/streamer.py` & `mxcube_video_streamer-1.0.0/video_streamer/core/streamer.py`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/core/websockethandler.py` & `mxcube_video_streamer-1.0.0/video_streamer/core/websockethandler.py`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/main.py` & `mxcube_video_streamer-1.0.0/video_streamer/main.py`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/server.py` & `mxcube_video_streamer-1.0.0/video_streamer/server.py`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/ui/static/jsmpeg.min.js` & `mxcube_video_streamer-1.0.0/video_streamer/ui/static/jsmpeg.min.js`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/video_streamer/ui/template/jsmpeg.min.js` & `mxcube_video_streamer-1.0.0/video_streamer/ui/template/jsmpeg.min.js`

 * *Files identical despite different names*

### Comparing `mxcube_video_streamer-0.0.0/setup.py` & `mxcube_video_streamer-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'websockets>=10.4,<11.0']
 
 entry_points = \
 {'console_scripts': ['video-streamer = video_streamer.main:run']}
 
 setup_kwargs = {
     'name': 'mxcube-video-streamer',
-    'version': '0.0.0',
+    'version': '1.0.0',
     'description': 'FastAPI Based video streamer',
     'long_description': '# video-streamer\nVideo streamer to be used with MXCuBE. The streamer currently suports streaming from Tango (Lima) devices but can be extened to used with other camera solutons aswell. The output streams are either MJPEG or MPEG1.\n\n![Screenshot from 2023-03-03 14-36-02](https://user-images.githubusercontent.com/4331447/222733892-c7d3af26-26ca-4a3c-b9f4-ab56fc91e390.png)\n\n### Installation\n\n```\ngit clone https://github.com/mxcube/video-streamer.git\ncd video-streamer\n\n# optional \nconda env create -f conda-environment.yml\n\n# For development\npip install -e .\n\n# For usage \npip install .\n```\n\n### Usage\n```\nusage: video-streamer [-h] [-c CONFIG_FILE_PATH] [-tu TANGO_URI] [-hs HOST] [-p PORT] [-q QUALITY] [-s SIZE] [-of OUTPUT_FORMAT] [-id HASH] [-d]\n\nmxcube-web Backend server command line utility.\n\noptions:\n  -h, --help            show this help message and exit\n  -c CONFIG_FILE_PATH, --config CONFIG_FILE_PATH\n                        Configuration file path\n  -tu TANGO_URI, --tango-uri TANGO_URI\n                        Tango device URI\n  -hs HOST, --host HOST\n                        Host name to listen on for incomming client connections defualt (0.0.0.0)\n  -p PORT, --port PORT  Port\n  -q QUALITY, --quality QUALITY\n                        Compresion rate/quality\n  -s SIZE, --size SIZE  size\n  -of OUTPUT_FORMAT, --output-format OUTPUT_FORMAT\n                        output format, MPEG1 or MJPEG1\n  -id HASH, --id HASH   Sream id\n  -d, --debug           Debug true or false\n```\n\nThere is the possibility to use a configuration file instead of command line arguments. All  command line arguments except debug are ignored if a config file is used. The configuration  file also makes it possible to configure several sources while the command line only allows  configuration of a single source.\n\n### Example command line (for testing):\n```\nvideo-streamer -d -of MPEG1 -tu test\n```\n\n#### Example configuration file (config.json):\nThe configuration file format is JSON. A test image is used when the input_uri is set to "test". The example below creates one MPEG1 stream and one MJPEG stream from the test image. There is a defualt test/demo UI to see the video stream on http://localhost:[port]/ui. In example below case:\n  \n MPEG1: http://localhost:8000/ui\n \n MJPEG: http://localhost:8001/ui\n\n\n```\nvideo-streamer -c config.json\n\nconfig.json:\n{\n    "sources": {\n        "0.0.0.0:8000": {\n            "input_uri": "test",\n            "quality": 4,\n            "format": "MPEG1"\n        },\n        "0.0.0.0:8000": {\n            "input_uri": "test",\n            "quality": 4,\n            "format": "MJPEG"\n        }\n    }\n}\n```\n  \n',
     'author': 'Marcus Oskarsson',
     'author_email': 'oscarsso@esrf.fr',
     'maintainer': 'Marcus Oskarsson',
     'maintainer_email': 'oscarsso@esrf.fr',
     'url': 'http://github.com/mxcube/fast-api-streamer',
```

### Comparing `mxcube_video_streamer-0.0.0/PKG-INFO` & `mxcube_video_streamer-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxcube-video-streamer
-Version: 0.0.0
+Version: 1.0.0
 Summary: FastAPI Based video streamer
 Home-page: http://github.com/mxcube/fast-api-streamer
 License: MIT
 Keywords: mxcube,fast-api-streamer,video_streamer,mxcubeweb
 Author: Marcus Oskarsson
 Author-email: oscarsso@esrf.fr
 Maintainer: Marcus Oskarsson
```

