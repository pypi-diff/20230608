# Comparing `tmp/Signal8-2.9.tar.gz` & `tmp/Signal8-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-2.9.tar", last modified: Tue Jun  6 22:07:51 2023, max compression
+gzip compressed data, was "Signal8-3.0.tar", last modified: Thu Jun  8 18:24:23 2023, max compression
```

## Comparing `Signal8-2.9.tar` & `Signal8-3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 22:07:51.629105 Signal8-2.9/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-2.9/LICENSE
--rw-rw-rw-   0        0        0     5556 2023-06-06 22:07:51.627104 Signal8-2.9/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2023-06-06 03:52:31.000000 Signal8-2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 22:07:51.484102 Signal8-2.9/Signal8/
--rw-rw-rw-   0        0        0    11051 2023-06-06 22:06:46.000000 Signal8-2.9/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-05 17:11:26.000000 Signal8-2.9/Signal8/__init__.py
--rw-rw-rw-   0        0        0      268 2023-06-06 22:03:30.000000 Signal8-2.9/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:07:51.619105 Signal8-2.9/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-2.9/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5809 2023-06-06 17:48:52.000000 Signal8-2.9/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2811 2023-06-06 21:50:32.000000 Signal8-2.9/Signal8/utils/npc.py
--rw-rw-rw-   0        0        0     5039 2023-06-05 17:20:08.000000 Signal8-2.9/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-2.9/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12317 2023-06-06 22:01:04.000000 Signal8-2.9/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1746 2023-06-01 20:02:00.000000 Signal8-2.9/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-06 22:07:51.536105 Signal8-2.9/Signal8.egg-info/
--rw-rw-rw-   0        0        0     5556 2023-06-06 22:07:51.000000 Signal8-2.9/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-06-06 22:07:51.000000 Signal8-2.9/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 22:07:51.000000 Signal8-2.9/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-06 22:07:51.000000 Signal8-2.9/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 22:07:51.629105 Signal8-2.9/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-06 22:06:58.000000 Signal8-2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 18:24:23.901306 Signal8-3.0/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-3.0/LICENSE
+-rw-rw-rw-   0        0        0     5556 2023-06-08 18:24:23.898307 Signal8-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2023-06-06 03:52:31.000000 Signal8-3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 18:24:23.754052 Signal8-3.0/Signal8/
+-rw-rw-rw-   0        0        0    11049 2023-06-08 18:17:47.000000 Signal8-3.0/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-05 17:11:26.000000 Signal8-3.0/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      268 2023-06-06 22:03:30.000000 Signal8-3.0/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-08 18:24:23.891304 Signal8-3.0/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-3.0/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5809 2023-06-06 17:48:52.000000 Signal8-3.0/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2783 2023-06-08 18:19:36.000000 Signal8-3.0/Signal8/utils/npc.py
+-rw-rw-rw-   0        0        0     5039 2023-06-05 17:20:08.000000 Signal8-3.0/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-3.0/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12317 2023-06-06 22:01:04.000000 Signal8-3.0/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1746 2023-06-01 20:02:00.000000 Signal8-3.0/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-08 18:24:23.831305 Signal8-3.0/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     5556 2023-06-08 18:24:22.000000 Signal8-3.0/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-08 18:24:22.000000 Signal8-3.0/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 18:24:22.000000 Signal8-3.0/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-08 18:24:22.000000 Signal8-3.0/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 18:24:23.902309 Signal8-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-08 18:23:42.000000 Signal8-3.0/setup.py
```

### Comparing `Signal8-2.9/LICENSE` & `Signal8-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-2.9/PKG-INFO` & `Signal8-3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 2.9
+Version: 3.0
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-2.9/README.md` & `Signal8-3.0/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-2.9/Signal8/Signal8.py` & `Signal8-3.0/Signal8/Signal8.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         return np.concatenate((agent_pos, agent_vel, np.concatenate(observed_obstacles, axis=0), observed_goal))
             
     # Run a thread for each scripted obstacle
     def run_scripted_obstacle(self, world, obstacle):
         sensitivity = 2.0
         while self.scripted_obstacle_running:
             with obstacle.lock:
-                # self.logger.debug(f'{obstacle.name} size: {obstacle.size:}, position: {obstacle.state.p_pos}')
+                self.logger.debug(f'{obstacle.name} size: {obstacle.size:}, position: {obstacle.state.p_pos}')
                 action = self._action_callback(obstacle, world)
                 obstacle.action = action * sensitivity
                 obstacle.move()
                 time.sleep(0.25)
         
     # disaster response: increase obstacle size to resemble increasing size of fire
     # precision farming: move obstacle in a zig-zag pattern to resemble a tractor
```

### Comparing `Signal8-2.9/Signal8/utils/core.py` & `Signal8-3.0/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.9/Signal8/utils/npc.py` & `Signal8-3.0/Signal8/utils/npc.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     
     def get_scripted_action(self, obs, instance_num):
         destination = self.farming_instances[instance_num]['destination']
         direction = self.farming_instances[instance_num]['direction']
         bounds = self.farming_instances[instance_num]['bounds']
         
         action = np.array([0, 0])
-        with obs.lock:
-            x, y, = obs.state.p_pos
+        x, y, = obs.state.p_pos
         
         if self.status == 'moving_to_destination':
             if np.allclose([x, y], destination, atol=0.05):
                 self.status = 'zigzagging'
                 self.direction = direction
             else:
                 action = self._move_towards_point(x, y, destination)
```

### Comparing `Signal8-2.9/Signal8/utils/problems.py` & `Signal8-3.0/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.9/Signal8/utils/simple_env.py` & `Signal8-3.0/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.9/Signal8/utils/test_dynamic_obs.py` & `Signal8-3.0/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-2.9/Signal8.egg-info/PKG-INFO` & `Signal8-3.0/Signal8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 2.9
+Version: 3.0
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-2.9/Signal8.egg-info/SOURCES.txt` & `Signal8-3.0/Signal8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Signal8-2.9/setup.py` & `Signal8-3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="2.9",
+    version="3.0",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

