# Comparing `tmp/ratinabox-1.7.0.tar.gz` & `tmp/ratinabox-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratinabox-1.7.0.tar", last modified: Tue Jun  6 19:29:57 2023, max compression
+gzip compressed data, was "ratinabox-1.7.1.tar", last modified: Thu Jun  8 18:05:35 2023, max compression
```

## Comparing `ratinabox-1.7.0.tar` & `ratinabox-1.7.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-06 19:29:57.689907 ratinabox-1.7.0/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.7.0/LICENSE
--rw-r--r--   0 tomgeorge   (501) staff       (20)    27991 2023-06-06 19:29:57.690044 ratinabox-1.7.0/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)    27271 2023-06-06 19:12:00.000000 ratinabox-1.7.0/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.7.0/pyproject.toml
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-06 19:29:57.682410 ratinabox-1.7.0/ratinabox/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    43768 2023-05-25 16:57:08.000000 ratinabox-1.7.0/ratinabox/Agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    32568 2023-04-27 09:08:29.000000 ratinabox-1.7.0/ratinabox/Environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    88673 2023-06-06 19:27:47.000000 ratinabox-1.7.0/ratinabox/Neurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.7.0/ratinabox/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3986 2023-05-25 16:50:19.000000 ratinabox-1.7.0/ratinabox/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-06 19:29:57.685087 ratinabox-1.7.0/ratinabox/contribs/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     8800 2023-04-23 10:24:42.000000 ratinabox-1.7.0/ratinabox/contribs/FieldOfViewNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     5782 2023-04-23 10:24:42.000000 ratinabox-1.7.0/ratinabox/contribs/PhasePrecessingPlaceCells.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3930 2023-04-23 10:24:42.000000 ratinabox-1.7.0/ratinabox/contribs/PlaneWaveNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.7.0/ratinabox/contribs/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.7.0/ratinabox/contribs/STDPFeedForwardLayer.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3402 2023-04-24 16:38:06.000000 ratinabox-1.7.0/ratinabox/contribs/SuccessorFeatures.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    56348 2023-06-06 18:34:59.000000 ratinabox-1.7.0/ratinabox/contribs/TaskEnvironment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    15029 2023-04-23 10:24:42.000000 ratinabox-1.7.0/ratinabox/contribs/ThetaSequenceAgent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7522 2023-04-24 16:38:06.000000 ratinabox-1.7.0/ratinabox/contribs/ValueNeuron.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.7.0/ratinabox/contribs/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-06 19:29:57.686185 ratinabox-1.7.0/ratinabox/data/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.7.0/ratinabox/data/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.7.0/ratinabox/data/__init__.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.7.0/ratinabox/data/rat.png
--rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.7.0/ratinabox/data/sargolini.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.7.0/ratinabox/data/tanni.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)    34824 2023-06-06 13:51:08.000000 ratinabox-1.7.0/ratinabox/utils.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-06 19:29:57.683367 ratinabox-1.7.0/ratinabox.egg-info/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    27991 2023-06-06 19:29:57.000000 ratinabox-1.7.0/ratinabox.egg-info/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)      945 2023-06-06 19:29:57.000000 ratinabox-1.7.0/ratinabox.egg-info/SOURCES.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-06-06 19:29:57.000000 ratinabox-1.7.0/ratinabox.egg-info/dependency_links.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       91 2023-06-06 19:29:57.000000 ratinabox-1.7.0/ratinabox.egg-info/requires.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-06-06 19:29:57.000000 ratinabox-1.7.0/ratinabox.egg-info/top_level.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)      979 2023-06-06 19:29:57.690381 ratinabox-1.7.0/setup.cfg
--rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.7.0/setup.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-06 19:29:57.689776 ratinabox-1.7.0/tests/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-04-12 13:21:00.000000 ratinabox-1.7.0/tests/test_advanced.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.7.0/tests/test_agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.7.0/tests/test_environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.7.0/tests/test_neurons.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-08 18:05:35.467378 ratinabox-1.7.1/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.7.1/LICENSE
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    27991 2023-06-08 18:05:35.467519 ratinabox-1.7.1/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    27271 2023-06-06 19:12:00.000000 ratinabox-1.7.1/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.7.1/pyproject.toml
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-08 18:05:35.459916 ratinabox-1.7.1/ratinabox/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    43878 2023-06-08 14:45:53.000000 ratinabox-1.7.1/ratinabox/Agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    32568 2023-04-27 09:08:29.000000 ratinabox-1.7.1/ratinabox/Environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    90154 2023-06-08 17:46:51.000000 ratinabox-1.7.1/ratinabox/Neurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.7.1/ratinabox/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3986 2023-05-25 16:50:19.000000 ratinabox-1.7.1/ratinabox/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-08 18:05:35.462377 ratinabox-1.7.1/ratinabox/contribs/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     8800 2023-04-23 10:24:42.000000 ratinabox-1.7.1/ratinabox/contribs/FieldOfViewNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     5782 2023-04-23 10:24:42.000000 ratinabox-1.7.1/ratinabox/contribs/PhasePrecessingPlaceCells.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3930 2023-04-23 10:24:42.000000 ratinabox-1.7.1/ratinabox/contribs/PlaneWaveNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.7.1/ratinabox/contribs/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.7.1/ratinabox/contribs/STDPFeedForwardLayer.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3402 2023-04-24 16:38:06.000000 ratinabox-1.7.1/ratinabox/contribs/SuccessorFeatures.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    56431 2023-06-07 01:12:00.000000 ratinabox-1.7.1/ratinabox/contribs/TaskEnvironment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    15029 2023-04-23 10:24:42.000000 ratinabox-1.7.1/ratinabox/contribs/ThetaSequenceAgent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7522 2023-04-24 16:38:06.000000 ratinabox-1.7.1/ratinabox/contribs/ValueNeuron.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.7.1/ratinabox/contribs/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-08 18:05:35.463802 ratinabox-1.7.1/ratinabox/data/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.7.1/ratinabox/data/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.7.1/ratinabox/data/__init__.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.7.1/ratinabox/data/rat.png
+-rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.7.1/ratinabox/data/sargolini.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.7.1/ratinabox/data/tanni.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    34818 2023-06-07 17:48:54.000000 ratinabox-1.7.1/ratinabox/utils.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-08 18:05:35.460822 ratinabox-1.7.1/ratinabox.egg-info/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    27991 2023-06-08 18:05:35.000000 ratinabox-1.7.1/ratinabox.egg-info/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      967 2023-06-08 18:05:35.000000 ratinabox-1.7.1/ratinabox.egg-info/SOURCES.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-06-08 18:05:35.000000 ratinabox-1.7.1/ratinabox.egg-info/dependency_links.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       91 2023-06-08 18:05:35.000000 ratinabox-1.7.1/ratinabox.egg-info/requires.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-06-08 18:05:35.000000 ratinabox-1.7.1/ratinabox.egg-info/top_level.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      979 2023-06-08 18:05:35.467872 ratinabox-1.7.1/setup.cfg
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.7.1/setup.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-06-08 18:05:35.467232 ratinabox-1.7.1/tests/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-04-12 13:21:00.000000 ratinabox-1.7.1/tests/test_advanced.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.7.1/tests/test_agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.7.1/tests/test_environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.7.1/tests/test_neurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3649 2023-06-08 14:57:09.000000 ratinabox-1.7.1/tests/test_taskenv.py
```

### Comparing `ratinabox-1.7.0/LICENSE` & `ratinabox-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/PKG-INFO` & `ratinabox-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.7.0
+Version: 1.7.1
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
```

### Comparing `ratinabox-1.7.0/README.md` & `ratinabox-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/Agent.py` & `ratinabox-1.7.1/ratinabox/Agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,17 @@
         # initialise history dataframes
         self.history = {}
         self.history["t"] = []
         self.history["pos"] = []
         self.history["vel"] = []
         self.history["rot_vel"] = []
 
+        self.Neurons = []  # each new Neurons class belonging to this Agent will append itself to this list
+
+
         # time and runID
         self.t = 0
         self.distance_travelled = 0
         self.average_measured_speed = max(self.speed_mean, self.speed_std)
         self.use_imported_trajectory = False
 
         # motion model stufff
```

### Comparing `ratinabox-1.7.0/ratinabox/Environment.py` & `ratinabox-1.7.1/ratinabox/Environment.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/Neurons.py` & `ratinabox-1.7.1/ratinabox/Neurons.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         Args:
             params (dict, optional). Defaults to {}.
 
         Typically you will not actually initialise a Neurons() class, instead you will initialised by one of it's subclasses.
         """
 
         self.Agent = Agent
+        self.Agent.Neurons.append(self)
 
         self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
 
         utils.update_class_params(self, self.params, get_all_defaults=True)
         utils.check_params(self, params.keys())
 
@@ -449,15 +450,15 @@
 
             if spikes is True:
                 for i, ax_ in enumerate(axes):
                     pos_where_spiked = pos[spike_data[chosen_neurons[i], :]]
                     ax_.scatter(
                         pos_where_spiked[:, 0],
                         pos_where_spiked[:, 1],
-                        s=3,
+                        s=5,
                         linewidth=0,
                         alpha=0.7,
                         zorder=1.2,
                         color=(self.color or "C1"),
                     )
 
         # PLOT 1D
@@ -854,43 +855,47 @@
 class GridCells(Neurons):
     """The GridCells class defines a population of GridCells. This class is a subclass of Neurons() and inherits it properties/plotting functions.
 
     Must be initialised with an Agent and a 'params' dictionary.
 
     GridCells defines a set of 'n' grid cells with random orientations, grid scales and offsets (these can be set non-randomly of course). Grids are modelled as the rectified sum of three cosine waves at 60 degrees to each other.
 
-    To initialise grid cells you specify three things: (i) params['gridscale'], (ii) params['orientation'] and (iii) params['phase_offset']. These are all sampled from a distribution (specified as, e.g. params['phase_offset_distribution']) and then used to calculate the firing rate of each grid cell. For each of these there quantities the value you specify parameterises the distribution from which it is sampled. For example params['gridscale':0.45,'gridscale_distribution':'uniform'] will pull gridscales from a uniform distribution between 0 and 0.45m. The 'delta' distribution means a constant will be taken. For all three of these you can optionally just pass an array of length GridCells.n (in which case the corresponding distribution parameter is ignored). This array is set a the value for each grid cell.
+    To initialise grid cells you specify three things: (i) params['gridscale'], (ii) params['orientation'] and (iii) params['phase_offset']. These are all sampled from a distribution (specified as, e.g. params['phase_offset_distribution']) and then used to calculate the firing rate of each grid cell. For each of these there quantities the value you specify parameterises the distribution from which it is sampled. For example params['gridscale':0.5,'gridscale_distribution':'uniform'] will pull gridscales from a uniform distribution between 0.5*gridscale (=0.25m) and 1.5*gridscale (=0.75m) The 'delta' distribution means a constant will be taken. For all three of these you can optionally just pass an array of length GridCells.n (in which case the corresponding distribution parameter is ignored). This array is set a the value for each grid cell.
+
+    params['description'] gives the place cells model being used. Currently either rectified sum of three cosines "three_rectified_cosines" or a shifted sum of three cosines "three_shifted_cosines" (which is similar, just a little softer at the edges, see Solstad et al. 2006)
 
     List of functions:
         • get_state()
         • set_phase_offsets()
 
 
     default_params = {
             "n": 10,
-            "gridscale": 0.45, 
+            "gridscale": 0.5,
             "gridscale_distribution": "uniform",
-            "orientation": None, 
+            "orientation": None,
             "orientation_distribution": "uniform",
             "phase_offset": True,
             "phase_offset_distribution": "uniform",
+            "description":"three_rectified_cosines",
             "min_fr": 0,
             "max_fr": 1,
             "name": "GridCells",
         }
     """
 
     default_params = {
         "n": 10,
-        "gridscale": 0.50, 
+        "gridscale": 0.50,
         "gridscale_distribution": "rayleigh",
-        "orientation": None, 
+        "orientation": None,
         "orientation_distribution": "uniform",
-        "phase_offset": True,
+        "phase_offset": None,
         "phase_offset_distribution": "uniform",
+        "description": "three_rectified_cosines",  # can also be "three_shifted_cosines" as in Solstad 2006 Eq. (2)
         "min_fr": 0,
         "max_fr": 1,
         "name": "GridCells",
     }
 
     def __init__(self, Agent, params={}):
         """Initialise GridCells(), takes as input a parameter dictionary. Any values not provided by the params dictionary are taken from a default dictionary below.
@@ -900,63 +905,91 @@
 
         self.Agent = Agent
 
         self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
 
         # deprecation warnings
-        if ("random_gridscales" in self.params) or ("random_orientations" in self.params) or ("random_phase_offsets" in self.params):
-            warnings.warn("the GridCell API has changed slightly, 'random_gridscales', 'random_orientations' and 'random_phase_offsets' are no longer accepted as parameters. Please use 'gridscale','gridscale_distribution','orientation','orientation_distribution','phase_offset' and 'phase_offset_distribution' instead. See docstring or 1.7.0 release notes for instructions.")
+        if (
+            ("random_gridscales" in self.params)
+            or ("random_orientations" in self.params)
+            or ("random_phase_offsets" in self.params)
+        ):
+            warnings.warn(
+                "the GridCell API has changed slightly, 'random_gridscales', 'random_orientations' and 'random_phase_offsets' are no longer accepted as parameters. Please use 'gridscale','gridscale_distribution','orientation','orientation_distribution','phase_offset' and 'phase_offset_distribution' instead. See docstring or 1.7.0 release notes for instructions."
+            )
 
         # Initialise the gridscales
-        if hasattr(self.params["gridscale"],"__len__"):
+        if hasattr(self.params["gridscale"], "__len__"):
             self.gridscales = np.array(self.params["gridscale"])
-            self.params['n'] = len(self.gridscales)
-        else: 
-            if self.params['gridscale_distribution'] == "uniform":
-                self.gridscales = np.random.uniform(0, self.params["gridscale"], self.params["n"])
-            elif self.params['gridscale_distribution'] == "rayleigh":
-                self.gridscales = np.random.rayleigh(scale=self.params["gridscale"], size=self.params["n"])
-            elif self.params['gridscale_distribution'] == "delta":
+            self.params["n"] = len(self.gridscales)
+        else:
+            if self.params["gridscale_distribution"] == "uniform":
+                self.gridscales = np.random.uniform(
+                    0.5 * self.params["gridscale"],
+                    1.5 * self.params["gridscale"],
+                    self.params["n"],
+                )
+            elif self.params["gridscale_distribution"] == "rayleigh":
+                self.gridscales = np.random.rayleigh(
+                    scale=self.params["gridscale"], size=self.params["n"]
+                )
+            elif self.params["gridscale_distribution"] == "logarithmic":
+                [low, high] = list(self.params["gridscale"])
+                self.gridscales = np.logspace(
+                    np.log10(low), np.log10(high), num=self.params["n"], base=10
+                )
+            elif self.params["gridscale_distribution"] == "delta":
                 self.gridscales = np.ones(self.params["n"]) * self.params["gridscale"]
             else:
                 raise ValueError("gridscale distribution not recognised")
-        
+
         # Initialise Neurons parent class
         super().__init__(Agent, self.params)
 
-
-        #Initialise phase offsets for each grid cell
-        if hasattr(self.params["phase_offset"],"__len__") and len(np.array(self.params['phase_offset']).shape) == 2:
+        # Initialise phase offsets for each grid cell
+        if (
+            hasattr(self.params["phase_offset"], "__len__")
+            and len(np.array(self.params["phase_offset"]).shape) == 2
+        ):
             self.phase_offsets = np.array(self.params["phase_offset"])
-            assert len(self.phase_offsets) == self.params["n"], "number of phase offsets supplied incompatible with number of neurons"
+            assert (
+                len(self.phase_offsets) == self.params["n"]
+            ), "number of phase offsets supplied incompatible with number of neurons"
         else:
-            if self.params['phase_offset_distribution'] == "uniform":
-                self.phase_offsets = np.random.uniform(0, 2*np.pi, size=(self.params["n"],2))
-            elif self.params['phase_offset_distribution'] == "delta":
-                phase_offset = self.params["phase_offset"] or np.array([0,0])
-                self.phase_offsets = np.ones((self.params["n"],2)) * np.array(phase_offset)
-            elif self.params['phase_offset_distribution'] == "grid":
+            if self.params["phase_offset_distribution"] == "uniform":
+                self.phase_offsets = np.random.uniform(
+                    0, 2 * np.pi, size=(self.params["n"], 2)
+                )
+            elif self.params["phase_offset_distribution"] == "delta":
+                phase_offset = self.params["phase_offset"] or np.array([0, 0])
+                self.phase_offsets = np.ones((self.params["n"], 2)) * np.array(
+                    phase_offset
+                )
+            elif self.params["phase_offset_distribution"] == "grid":
                 self.phase_offsets = self.set_phase_offsets_on_grid()
             else:
                 raise ValueError("phase offset distribution not recognised")
-        
-        #Initialise orientations for each grid cell
-        if hasattr(self.params["orientation"],"__len__"):
+
+        # Initialise orientations for each grid cell
+        if hasattr(self.params["orientation"], "__len__"):
             self.orientations = np.array(self.params["orientation"])
-            assert len(self.orientations) == self.params["n"], "number of orientations supplied incompatible with number of neurons"
+            assert (
+                len(self.orientations) == self.params["n"]
+            ), "number of orientations supplied incompatible with number of neurons"
         else:
-            if self.params['orientation_distribution'] == "uniform":
-                self.orientations = np.random.uniform(0, 2*np.pi, size=(self.params["n"],))
-            elif self.params['orientation_distribution'] == "delta":
+            if self.params["orientation_distribution"] == "uniform":
+                self.orientations = np.random.uniform(
+                    0, 2 * np.pi, size=(self.params["n"],)
+                )
+            elif self.params["orientation_distribution"] == "delta":
                 orientation = self.params["orientation"] or 0
                 self.orientations = np.ones(self.params["n"]) * orientation
             else:
                 raise ValueError("orientation distribution not recognised")
-        
 
         # Initialise grid cells
         assert (
             self.Agent.Environment.dimensionality == "2D"
         ), "grid cells only available in 2D"
 
         w = []
@@ -988,50 +1021,54 @@
         else:
             pos = kwargs["pos"]
         pos = np.array(pos)
         pos = pos.reshape(-1, pos.shape[-1])
 
         # grid cells are modelled as the thresholded sum of three cosines all at 60 degree offsets
         # vectors to grids cells "centred" at their (random) phase offsets
-        origin = self.gridscales.reshape(-1,1)*self.phase_offsets/(2*np.pi)
-        vecs = utils.get_vectors_between(
-            origin, pos
-        )  # shape = (N_cells,N_pos,2)
+        origin = self.gridscales.reshape(-1, 1) * self.phase_offsets / (2 * np.pi)
+        vecs = utils.get_vectors_between(origin, pos)  # shape = (N_cells,N_pos,2)
         w1 = np.tile(np.expand_dims(self.w[:, 0, :], axis=1), reps=(1, pos.shape[0], 1))
         w2 = np.tile(np.expand_dims(self.w[:, 1, :], axis=1), reps=(1, pos.shape[0], 1))
         w3 = np.tile(np.expand_dims(self.w[:, 2, :], axis=1), reps=(1, pos.shape[0], 1))
         gridscales = np.tile(
             np.expand_dims(self.gridscales, axis=1), reps=(1, pos.shape[0])
         )
         phi_1 = ((2 * np.pi) / gridscales) * (vecs * w1).sum(axis=-1)
         phi_2 = ((2 * np.pi) / gridscales) * (vecs * w2).sum(axis=-1)
         phi_3 = ((2 * np.pi) / gridscales) * (vecs * w3).sum(axis=-1)
-        firingrate = (1 / 3) * ((np.cos(phi_1) + np.cos(phi_2) + np.cos(phi_3)))
-        firingrate[firingrate < 0] = 0
+
+        if self.description == "three_rectified_cosines":
+            firingrate = (1 / 3) * ((np.cos(phi_1) + np.cos(phi_2) + np.cos(phi_3)))
+            firingrate[firingrate < 0] = 0
+        elif self.description == "three_shifted_cosines":
+            firingrate = (2 / 3) * (
+                (1 / 3) * (np.cos(phi_1) + np.cos(phi_2) + np.cos(phi_3)) + (1 / 2)
+            )
 
         firingrate = (
             firingrate * (self.max_fr - self.min_fr) + self.min_fr
         )  # scales from being between [0,1] to [min_fr, max_fr]
         return firingrate
 
     def set_phase_offsets_on_grid(self):
         """Set non-random phase_offsets. Most offsets (n_on_grid, the largest square numer before self.n) will tile a grid of 0 to 2pi in x and 0 to 2pi in y, while the remainings (cell number: n - n_on_grid) are random."""
         n_x = int(np.sqrt(self.n))
         n_y = self.n // n_x
         n_remaining = self.n - n_x * n_y
 
-        dx = 2*np.pi / n_x
-        dy = 2*np.pi / n_y
+        dx = 2 * np.pi / n_x
+        dy = 2 * np.pi / n_y
 
         grid = np.mgrid[
-            (0 + dx / 2) : (2*np.pi - dx / 2) : (n_x * 1j),
-            (0 + dy / 2) : (2*np.pi - dy / 2) : (n_y * 1j),
+            (0 + dx / 2) : (2 * np.pi - dx / 2) : (n_x * 1j),
+            (0 + dy / 2) : (2 * np.pi - dy / 2) : (n_y * 1j),
         ]
         grid = grid.reshape(2, -1).T
-        remaining = np.random.uniform(0, 2*np.pi, size=(n_remaining, 2))
+        remaining = np.random.uniform(0, 2 * np.pi, size=(n_remaining, 2))
 
         all_offsets = np.vstack([grid, remaining])
 
         return all_offsets
 
 
 class BoundaryVectorCells(Neurons):
@@ -1914,15 +1951,15 @@
         else:
             V = np.zeros((self.n, kwargs["pos"].shape[0]))
 
         for inputlayer in self.inputs.values():
             w = inputlayer["w"]
             if evaluate_at == "last":
                 I = inputlayer["layer"].firingrate
-            else:  # kick can down the road let input layer decide how to evaluate the firingrate. this is core to feedforward layer as this recursive call will backprop through the upstraem layers until it reaches a "core" (e.g. place cells) layer which will then evaluate the firingrate. 
+            else:  # kick can down the road let input layer decide how to evaluate the firingrate. this is core to feedforward layer as this recursive call will backprop through the upstraem layers until it reaches a "core" (e.g. place cells) layer which will then evaluate the firingrate.
                 I = inputlayer["layer"].get_state(evaluate_at, **kwargs)
             inputlayer["I_temp"] = I
             V += np.matmul(w, I)
 
         biases = self.biases
         if biases.shape != V.shape:
             biases = biases.reshape((-1, 1))
```

### Comparing `ratinabox-1.7.0/ratinabox/README.md` & `ratinabox-1.7.1/ratinabox/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/__init__.py` & `ratinabox-1.7.1/ratinabox/__init__.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/contribs/FieldOfViewNeurons.py` & `ratinabox-1.7.1/ratinabox/contribs/FieldOfViewNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/contribs/PhasePrecessingPlaceCells.py` & `ratinabox-1.7.1/ratinabox/contribs/PhasePrecessingPlaceCells.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/contribs/PlaneWaveNeurons.py` & `ratinabox-1.7.1/ratinabox/contribs/PlaneWaveNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/contribs/README.md` & `ratinabox-1.7.1/ratinabox/contribs/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/contribs/STDPFeedForwardLayer.py` & `ratinabox-1.7.1/ratinabox/contribs/STDPFeedForwardLayer.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/contribs/SuccessorFeatures.py` & `ratinabox-1.7.1/ratinabox/contribs/SuccessorFeatures.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/contribs/TaskEnvironment.py` & `ratinabox-1.7.1/ratinabox/contribs/TaskEnvironment.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,16 +361,17 @@
         for reward_cache in self.reward_caches.values():
             reward_cache.update()
 
         # Udpate the environment, which can add new rewards to caches
         self.update(*pos, **kws)
 
         # If any terminal agents, remove from set of active agents
+        truncations = self._dict(self._is_truncated_state())
         for agent, term in self._dict(self._is_terminal_state()).items():
-            if term and agent in self.agents:
+            if term and agent in self.agents or truncations[agent]:
                 self.agents.remove(agent)
         
         # Return the next state, reward, whether the state is terminal,
         return (self.get_observation(), 
                 self.get_reward(), 
                 self._dict(self._is_terminal_state()),
                 self._dict(self._is_truncated_state()),
```

### Comparing `ratinabox-1.7.0/ratinabox/contribs/ThetaSequenceAgent.py` & `ratinabox-1.7.1/ratinabox/contribs/ThetaSequenceAgent.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/contribs/ValueNeuron.py` & `ratinabox-1.7.1/ratinabox/contribs/ValueNeuron.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/data/README.md` & `ratinabox-1.7.1/ratinabox/data/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/data/rat.png` & `ratinabox-1.7.1/ratinabox/data/rat.png`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/data/sargolini.npz` & `ratinabox-1.7.1/ratinabox/data/sargolini.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/data/tanni.npz` & `ratinabox-1.7.1/ratinabox/data/tanni.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/ratinabox/utils.py` & `ratinabox-1.7.1/ratinabox/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,15 +542,15 @@
     return fig, ax
 
 
 def save_figure(
     fig,
     save_title="",
     fig_save_types=["png", "svg"],
-    anim_save_types=["mp4", "gif"],
+    anim_save_types=["mp4",],
     save=True,
 ):
     """
     Saves a figure in a dated-folder with the current time appended to save_title, as both '.png' and '.svg'. Same for animations but as ".gif" and ".mp4".
     This function can be used by anyone...just pass a fig object and it will be saved in the right place.
 
     Args:
```

### Comparing `ratinabox-1.7.0/ratinabox.egg-info/PKG-INFO` & `ratinabox-1.7.1/ratinabox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.7.0
+Version: 1.7.1
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
```

### Comparing `ratinabox-1.7.0/ratinabox.egg-info/SOURCES.txt` & `ratinabox-1.7.1/ratinabox.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 ratinabox/data/__init__.py
 ratinabox/data/rat.png
 ratinabox/data/sargolini.npz
 ratinabox/data/tanni.npz
 tests/test_advanced.py
 tests/test_agent.py
 tests/test_environment.py
-tests/test_neurons.py
+tests/test_neurons.py
+tests/test_taskenv.py
```

### Comparing `ratinabox-1.7.0/setup.cfg` & `ratinabox-1.7.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ratinabox
-version = 1.7.0
+version = 1.7.1
 author = Tom George
 author_email = tomgeorge1@btinternet.com
 project_urls = 
 	Documentation = https://github.com/TomGeorge1234/RatInABox
 	Source = https://github.com/TomGeorge1234/RatInABox
 	Tracker = https://github.com/TomGeorge1234/RatInABox/issues
 description = RatInABox: A package for simulating motion and ephys data in continuous environments
```

### Comparing `ratinabox-1.7.0/tests/test_advanced.py` & `ratinabox-1.7.1/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.7.0/tests/test_environment.py` & `ratinabox-1.7.1/tests/test_environment.py`

 * *Files identical despite different names*

