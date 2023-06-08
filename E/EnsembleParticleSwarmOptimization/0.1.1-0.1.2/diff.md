# Comparing `tmp/EnsembleParticleSwarmOptimization-0.1.1.tar.gz` & `tmp/EnsembleParticleSwarmOptimization-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnsembleParticleSwarmOptimization-0.1.1.tar", last modified: Mon Jun  5 16:25:59 2023, max compression
+gzip compressed data, was "EnsembleParticleSwarmOptimization-0.1.2.tar", last modified: Thu Jun  8 09:31:47 2023, max compression
```

## Comparing `EnsembleParticleSwarmOptimization-0.1.1.tar` & `EnsembleParticleSwarmOptimization-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-06-05 16:25:59.965747 EnsembleParticleSwarmOptimization-0.1.1/
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-06-05 16:25:59.965747 EnsembleParticleSwarmOptimization-0.1.1/EnsembleParticleSwarmOptimization.egg-info/
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      850 2023-06-05 16:25:59.000000 EnsembleParticleSwarmOptimization-0.1.1/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      431 2023-06-05 16:25:59.000000 EnsembleParticleSwarmOptimization-0.1.1/EnsembleParticleSwarmOptimization.egg-info/SOURCES.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        1 2023-06-05 16:25:59.000000 EnsembleParticleSwarmOptimization-0.1.1/EnsembleParticleSwarmOptimization.egg-info/dependency_links.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       77 2023-06-05 16:25:59.000000 EnsembleParticleSwarmOptimization-0.1.1/EnsembleParticleSwarmOptimization.egg-info/requires.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        5 2023-06-05 16:25:59.000000 EnsembleParticleSwarmOptimization-0.1.1/EnsembleParticleSwarmOptimization.egg-info/top_level.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      850 2023-06-05 16:25:59.965747 EnsembleParticleSwarmOptimization-0.1.1/PKG-INFO
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-06-05 16:25:59.965747 EnsembleParticleSwarmOptimization-0.1.1/PySO/
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    10064 2023-06-05 15:46:22.000000 EnsembleParticleSwarmOptimization-0.1.1/PySO/Clustering_Swarms.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    34011 2023-06-05 16:01:32.000000 EnsembleParticleSwarmOptimization-0.1.1/PySO/HierarchicalSwarmHandler.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    30396 2023-06-02 15:36:36.000000 EnsembleParticleSwarmOptimization-0.1.1/PySO/MWE_Swarm.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     2174 2023-06-02 15:36:36.000000 EnsembleParticleSwarmOptimization-0.1.1/PySO/Model.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     8369 2023-06-02 15:36:36.000000 EnsembleParticleSwarmOptimization-0.1.1/PySO/SwarmHandler.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      288 2023-06-05 16:11:21.000000 EnsembleParticleSwarmOptimization-0.1.1/PySO/__init__.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      212 2023-06-05 16:23:57.000000 EnsembleParticleSwarmOptimization-0.1.1/README.md
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       38 2023-06-05 16:25:59.965747 EnsembleParticleSwarmOptimization-0.1.1/setup.cfg
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      885 2023-06-05 16:11:39.000000 EnsembleParticleSwarmOptimization-0.1.1/setup.py
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-06-08 09:31:47.448766 EnsembleParticleSwarmOptimization-0.1.2/
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-06-08 09:31:47.444766 EnsembleParticleSwarmOptimization-0.1.2/EnsembleParticleSwarmOptimization.egg-info/
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      850 2023-06-08 09:31:47.000000 EnsembleParticleSwarmOptimization-0.1.2/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      431 2023-06-08 09:31:47.000000 EnsembleParticleSwarmOptimization-0.1.2/EnsembleParticleSwarmOptimization.egg-info/SOURCES.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        1 2023-06-08 09:31:47.000000 EnsembleParticleSwarmOptimization-0.1.2/EnsembleParticleSwarmOptimization.egg-info/dependency_links.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       77 2023-06-08 09:31:47.000000 EnsembleParticleSwarmOptimization-0.1.2/EnsembleParticleSwarmOptimization.egg-info/requires.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        5 2023-06-08 09:31:47.000000 EnsembleParticleSwarmOptimization-0.1.2/EnsembleParticleSwarmOptimization.egg-info/top_level.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      850 2023-06-08 09:31:47.448766 EnsembleParticleSwarmOptimization-0.1.2/PKG-INFO
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-06-08 09:31:47.448766 EnsembleParticleSwarmOptimization-0.1.2/PySO/
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    10064 2023-06-05 15:46:22.000000 EnsembleParticleSwarmOptimization-0.1.2/PySO/Clustering_Swarms.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    34011 2023-06-06 10:44:08.000000 EnsembleParticleSwarmOptimization-0.1.2/PySO/HierarchicalSwarmHandler.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    30396 2023-06-02 15:36:36.000000 EnsembleParticleSwarmOptimization-0.1.2/PySO/MWE_Swarm.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     2174 2023-06-02 15:36:36.000000 EnsembleParticleSwarmOptimization-0.1.2/PySO/Model.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     8369 2023-06-02 15:36:36.000000 EnsembleParticleSwarmOptimization-0.1.2/PySO/SwarmHandler.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      288 2023-06-05 16:11:21.000000 EnsembleParticleSwarmOptimization-0.1.2/PySO/__init__.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      212 2023-06-05 16:23:57.000000 EnsembleParticleSwarmOptimization-0.1.2/README.md
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       38 2023-06-08 09:31:47.448766 EnsembleParticleSwarmOptimization-0.1.2/setup.cfg
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      885 2023-06-08 09:21:47.000000 EnsembleParticleSwarmOptimization-0.1.2/setup.py
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.1/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO` & `EnsembleParticleSwarmOptimization-0.1.2/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnsembleParticleSwarmOptimization
-Version: 0.1.1
+Version: 0.1.2
 Summary: Ensemble of particle swarms together with various velocity rules for function optimization
 Home-page: https://github.com/dig07/PySO
 Author: Christopher Moore and Diganta Bandopadhyay
 Author-email: diganta@star.sr.bham.ac.uk
 License: UNKNOWN
 Description: # PySO
         Particle swarm optimizer
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.1/PKG-INFO` & `EnsembleParticleSwarmOptimization-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnsembleParticleSwarmOptimization
-Version: 0.1.1
+Version: 0.1.2
 Summary: Ensemble of particle swarms together with various velocity rules for function optimization
 Home-page: https://github.com/dig07/PySO
 Author: Christopher Moore and Diganta Bandopadhyay
 Author-email: diganta@star.sr.bham.ac.uk
 License: UNKNOWN
 Description: # PySO
         Particle swarm optimizer
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.1/PySO/Clustering_Swarms.py` & `EnsembleParticleSwarmOptimization-0.1.2/PySO/Clustering_Swarms.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.1/PySO/HierarchicalSwarmHandler.py` & `EnsembleParticleSwarmOptimization-0.1.2/PySO/HierarchicalSwarmHandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,39 +12,39 @@
 
 
 
 class HierarchicalSwarmHandler(object):
 
     def __init__(self,
                  Hierarchical_models,
-                 NumSwarms,
-                 NumParticlesPerSwarm,
+                 Numswarms,
+                 Numparticlesperswarm,
                  Omega = 0.6,
-                 PhiP = 0.2,
-                 PhiG = 0.2,
-                 MH_fraction = 0.0,
+                 Phip = 0.2,
+                 Phig = 0.2,
+                 Mh_fraction = 0.0,
                  Swarm_kwargs={},
                  Output = './',
-                 nPeriodicCheckpoint = 10,
+                 Nperiodiccheckpoint = 10,
                  Swarm_names = None,
                  Verbose = False,
-                 SaveEvolution = False,
+                 Saveevolution = False,
                  Maxiter = 1e4,
                  Resume = True,
                  Maximum_number_of_iterations_per_step=400,
                  Minimum_exploration_iterations = 50,
                  Initial_exploration_limit= 150,
-                 clustering_indices = None,
-                 use_func_vals_in_clustering = False,
-                 kick_velocities = True,
-                 fitness_veto_fraction = 0.05,
-                 max_particles_per_swarm = None,
-                 redraw_velocities_at_segmentation = False,
-                 clustering_min_membership = 5,
-                 clustering_max_clusters = 70,
+                 Clustering_indices = None,
+                 Use_func_vals_in_clustering = False,
+                 Kick_velocities = True,
+                 Fitness_veto_fraction = 0.05,
+                 Max_particles_per_swarm = None,
+                 Redraw_velocities_at_segmentation = False,
+                 Clustering_min_membership = 5,
+                 Clustering_max_clusters = 70,
                  Tol = 1.0e-2,
                  Convergence_testing_num_iterations = 50):
         """
 
         REQUIRED INPUTS
         ------
         Hierarchical_models: list,
@@ -59,15 +59,15 @@
         ---------------
         Omega: float or list
             the omega parameter for each hierarhical model, inertial coefficient for velocity updating [defaults to .6]
         PhiP: float or list
             the phi_p parameter for each hierarhical model, cognitive coefficient for velocity updating [defaults to .2]
         PhiG: float or list
             the phi_g parameter for each hierarhical model, social coefficient for velocity updating [defaults to .2]
-        MH_fraction: float
+        Mh_fraction: float
             parameter controlling proportion of velocity rule dictated by MCMC, for each hierarchical model [defaults to 0.]
         Swarm_kwargs: dict
             dictionary of common arguments between all swarms
         Output: str
             folder in which to save output [defaults to './']
         nPeriodicCheckpoint: int
             number of iterations between printing checkpoints [defaults to 10]
@@ -88,15 +88,15 @@
             Minimum number of iterations to be done in each step before stall condition evaluated [defaults to 50]
         Initial_exploration_limit: int
             Minimum number of iterations done in the very first step before stall condition evaluated [defaults to 150]
         clustering_indices: None or list of int
             Parameter position indexes to use for relabelling/clustering step [defaults to all parameters]
         use_func_vals_in_clustering: boolean
             Boolean flag for using function values for clustering or not [defaults to False]
-        kick_velocities: boolean
+        Kick_velocities: boolean
             Boolean flag for reinitialising velocities from position distribution
             on clustering and segmenting [defaults to True]
         fitness_veto_fraction: float
             Fraction of Best swarm position below which we throw away new swarms [defaults to 0.05]
         max_particles_per_swarm: integer
             Maximum number of particles per swarm [defaults to int(total_num_particles/10)]
         redraw_velocities_at_segmentation: Boolean
@@ -112,17 +112,17 @@
         """
         assert len(Hierarchical_models)>1, "Please input multiple models for Hierarchical PSO search"
 
         self.Hierarchical_models = Hierarchical_models
 
         # Ladder for PSO hyper-parameters
         self.Omegas = Omega
-        self.PhiPs = PhiP
-        self.PhiGs = PhiG
-        self.MH_fractions = MH_fraction
+        self.PhiPs = Phip
+        self.PhiGs = Phig
+        self.MH_fractions = Mh_fraction
 
         # If PSO hyper-parameters are only a float, replicate them for each step in the ladder
         if type(self.Omegas) == float:
             self.Omegas = [self.Omegas] * len(self.Hierarchical_models)
             self.PhiPs = [self.PhiPs] * len(self.Hierarchical_models)
             self.PhiGs = [self.PhiGs] * len(self.Hierarchical_models)
             self.MH_fractions = [self.MH_fractions] * len(self.Hierarchical_models)
@@ -132,31 +132,31 @@
         # Parameter names
         self.Model_axis_names = self.Hierarchical_models[1].names
 
 
         # Number of dimensions
         self.Ndim = len(self.Model_axis_names)
 
-        self.NumSwarms = NumSwarms
+        self.NumSwarms = Numswarms
 
         # NOTE THIS NAME IS MISLEADING, this is just the total size of the initial swarm
-        self.NumParticlesPerSwarm = NumParticlesPerSwarm
+        self.NumParticlesPerSwarm = Numparticlesperswarm
 
         # Common parameters for all swarms
         self.Swarm_kwargs = Swarm_kwargs
 
-        self.nPeriodicCheckpoint = nPeriodicCheckpoint
+        self.nPeriodicCheckpoint = Nperiodiccheckpoint
 
         self.BestKnownEnsemblePoint = np.zeros(self.Ndim)
         self.BestKnownEnsembleValue = None
         self.BestCurrentSwarm = None
 
         self.Verbose = Verbose
 
-        self.SaveEvolution = SaveEvolution
+        self.SaveEvolution = Saveevolution
 
         # Refering to the hierarchical steps
         self.Maximum_number_of_iterations_per_step = Maximum_number_of_iterations_per_step
 
         # Minimum number of iterations the swarms will conduct before they evaluate the stall condition
         self.Minimum_exploration_iterations = Minimum_exploration_iterations
 
@@ -173,33 +173,33 @@
         self.Output = Output
 
         # If we have given then swarm names, otherwise default to numbered list
         self.Swarm_names = Swarm_names
         if self.Swarm_names == None: self.Swarm_names = np.arange(self.NumSwarms) # Defaults to numbered list of swarms
 
         # If the clustering is done only in certain parameters, otherwise cluster in all dimensions (Not including objective function value)
-        self.clustering_indices  = clustering_indices
+        self.clustering_indices  = Clustering_indices
         if self.clustering_indices == None: self.clustering_indices = np.arange(self.Ndim) # Use all parameters by default in clustering
 
         # If the objective function value is to be used in the clustering process.
-        self.use_func_vals_in_clustering = use_func_vals_in_clustering
+        self.use_func_vals_in_clustering = Use_func_vals_in_clustering
 
         # If true, draw new velocities from the new swarms particle positions using a normal distribution [ DEFAULTS TO TRUE ]
         # If false, use previous particle velocities
-        self.kick_velocities = kick_velocities
+        self.kick_velocities = Kick_velocities
 
         # If true, draw new velocities from the new swarms particle positions using a uniform distribution [ DEFAULTS TO FALSE ]
         # If false, use previous particle velocities
-        self.redraw_velocities_at_segmentation = redraw_velocities_at_segmentation
+        self.redraw_velocities_at_segmentation = Redraw_velocities_at_segmentation
 
         # self.fitness_veto_fraction * best_objective_function_Val below which we throw swarms away (reassign particles to other swarms)
-        self.fitness_veto_fraction = fitness_veto_fraction
+        self.fitness_veto_fraction = Fitness_veto_fraction
 
         # Maximum particles per swarm, defaults to total particles over 10
-        self.max_particles_per_swarm = max_particles_per_swarm
+        self.max_particles_per_swarm = Max_particles_per_swarm
         if self.max_particles_per_swarm == None: self.max_particles_per_swarm = int(self.NumParticlesPerSwarm/10)
 
         # Initialise swarms
         self.InitialiseSwarms()
 
         # frozen swarms are temporarily held in this dict
         self.frozen_swarms = {}
@@ -210,16 +210,16 @@
         # Boolean variable to indicate if all swarms at the current level have stalled
         self.AllStalled = False
 
         # Variable to check if all swarms have finishing iterating on the last hierarchical model.
         self.swarm_stepping_done = False
 
         # Clustering parameters (See docstrings)
-        self.clustering_min_membership = clustering_min_membership
-        self.clustering_max_clusters = clustering_max_clusters
+        self.clustering_min_membership = Clustering_min_membership
+        self.clustering_max_clusters = Clustering_max_clusters
 
         # RESUME FUNCTIONALITY UNTESTED TODO: TEST
         resume_file = os.path.join(self.Output, "PySO_resume.pkl")
 
         # Stall testing parameters
         self.Tol = Tol
         self.Convergence_testing_num_iterations = Convergence_testing_num_iterations
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.1/PySO/MWE_Swarm.py` & `EnsembleParticleSwarmOptimization-0.1.2/PySO/MWE_Swarm.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.1/PySO/Model.py` & `EnsembleParticleSwarmOptimization-0.1.2/PySO/Model.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.1/PySO/SwarmHandler.py` & `EnsembleParticleSwarmOptimization-0.1.2/PySO/SwarmHandler.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.1/setup.py` & `EnsembleParticleSwarmOptimization-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="EnsembleParticleSwarmOptimization",
-    version="0.1.1",
+    version="0.1.2",
     author="Christopher Moore and Diganta Bandopadhyay",
     author_email="diganta@star.sr.bham.ac.uk",
     description="Ensemble of particle swarms together with various velocity rules for function optimization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dig07/PySO",
     packages=setuptools.find_packages(),
```

