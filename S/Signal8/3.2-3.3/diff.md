# Comparing `tmp/Signal8-3.2.tar.gz` & `tmp/Signal8-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-3.2.tar", last modified: Thu Jun  8 18:50:13 2023, max compression
+gzip compressed data, was "Signal8-3.3.tar", last modified: Thu Jun  8 18:55:07 2023, max compression
```

## Comparing `Signal8-3.2.tar` & `Signal8-3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 18:50:13.045873 Signal8-3.2/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-3.2/LICENSE
--rw-rw-rw-   0        0        0     5556 2023-06-08 18:50:13.043870 Signal8-3.2/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2023-06-06 03:52:31.000000 Signal8-3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 18:50:12.948871 Signal8-3.2/Signal8/
--rw-rw-rw-   0        0        0    11046 2023-06-08 18:48:59.000000 Signal8-3.2/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-05 17:11:26.000000 Signal8-3.2/Signal8/__init__.py
--rw-rw-rw-   0        0        0      292 2023-06-08 18:48:15.000000 Signal8-3.2/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-08 18:50:13.037871 Signal8-3.2/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-3.2/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5809 2023-06-06 17:48:52.000000 Signal8-3.2/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2783 2023-06-08 18:19:36.000000 Signal8-3.2/Signal8/utils/npc.py
--rw-rw-rw-   0        0        0     5039 2023-06-05 17:20:08.000000 Signal8-3.2/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-3.2/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12317 2023-06-06 22:01:04.000000 Signal8-3.2/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-3.2/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-08 18:50:13.002870 Signal8-3.2/Signal8.egg-info/
--rw-rw-rw-   0        0        0     5556 2023-06-08 18:50:12.000000 Signal8-3.2/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-08 18:50:12.000000 Signal8-3.2/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 18:50:12.000000 Signal8-3.2/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-08 18:50:12.000000 Signal8-3.2/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 18:50:13.045873 Signal8-3.2/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-08 18:49:16.000000 Signal8-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 18:55:07.207450 Signal8-3.3/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-3.3/LICENSE
+-rw-rw-rw-   0        0        0     5556 2023-06-08 18:55:07.193449 Signal8-3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2023-06-06 03:52:31.000000 Signal8-3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 18:55:07.128451 Signal8-3.3/Signal8/
+-rw-rw-rw-   0        0        0    11051 2023-06-08 18:54:13.000000 Signal8-3.3/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-05 17:11:26.000000 Signal8-3.3/Signal8/__init__.py
+-rw-rw-rw-   0        0        0     1989 2023-06-08 18:53:56.000000 Signal8-3.3/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-08 18:55:07.167451 Signal8-3.3/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-3.3/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5809 2023-06-06 17:48:52.000000 Signal8-3.3/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2783 2023-06-08 18:19:36.000000 Signal8-3.3/Signal8/utils/npc.py
+-rw-rw-rw-   0        0        0     5039 2023-06-05 17:20:08.000000 Signal8-3.3/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-3.3/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12317 2023-06-06 22:01:04.000000 Signal8-3.3/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-3.3/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-08 18:55:07.152452 Signal8-3.3/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     5556 2023-06-08 18:55:06.000000 Signal8-3.3/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-08 18:55:06.000000 Signal8-3.3/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 18:55:06.000000 Signal8-3.3/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-08 18:55:06.000000 Signal8-3.3/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 18:55:07.208450 Signal8-3.3/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-08 18:54:23.000000 Signal8-3.3/setup.py
```

### Comparing `Signal8-3.2/LICENSE` & `Signal8-3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-3.2/PKG-INFO` & `Signal8-3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 3.2
+Version: 3.3
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-3.2/README.md` & `Signal8-3.3/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-3.2/Signal8/Signal8.py` & `Signal8-3.3/Signal8/Signal8.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         sensitivity = 2.0
         while self.scripted_obstacle_running:
             with obstacle.lock:
                 # self.logger.debug(f'{obstacle.name} size: {obstacle.size:}, position: {obstacle.state.p_pos}')
                 action = self._action_callback(obstacle, world)
                 obstacle.action = action * sensitivity
                 obstacle.move()
-            time.sleep(0.5)
+                time.sleep(0.25)
         
     # disaster response: increase obstacle size to resemble increasing size of fire
     # precision farming: move obstacle in a zig-zag pattern to resemble a tractor
     def _action_callback(self, obs, world):
         action = np.zeros(world.dim_p)
         instance = world.problem_instance
         if world.problem_type == 'disaster_response':
```

### Comparing `Signal8-3.2/Signal8/utils/core.py` & `Signal8-3.3/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.2/Signal8/utils/npc.py` & `Signal8-3.3/Signal8/utils/npc.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.2/Signal8/utils/problems.py` & `Signal8-3.3/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.2/Signal8/utils/simple_env.py` & `Signal8-3.3/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.2/Signal8/utils/test_dynamic_obs.py` & `Signal8-3.3/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.2/Signal8.egg-info/PKG-INFO` & `Signal8-3.3/Signal8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 3.2
+Version: 3.3
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-3.2/Signal8.egg-info/SOURCES.txt` & `Signal8-3.3/Signal8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Signal8-3.2/setup.py` & `Signal8-3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="3.2",
+    version="3.3",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

