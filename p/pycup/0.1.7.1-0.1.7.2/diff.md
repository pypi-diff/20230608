# Comparing `tmp/pycup-0.1.7.1.tar.gz` & `tmp/pycup-0.1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pycup-0.1.7.1.tar", last modified: Tue Jun  6 07:15:25 2023, max compression
+gzip compressed data, was "dist\pycup-0.1.7.2.tar", last modified: Thu Jun  8 11:39:14 2023, max compression
```

## Comparing `pycup-0.1.7.1.tar` & `pycup-0.1.7.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 07:15:25.190031 pycup-0.1.7.1/
--rw-rw-rw-   0        0        0     6368 2023-06-06 07:15:25.189930 pycup-0.1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     5112 2023-06-05 15:14:54.000000 pycup-0.1.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 07:15:25.173926 pycup-0.1.7.1/pycup/
--rw-rw-rw-   0        0        0    17161 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/GLUE.py
--rw-rw-rw-   0        0        0    38271 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/GWO.py
--rw-rw-rw-   0        0        0    32971 2023-06-05 15:19:02.000000 pycup-0.1.7.1/pycup/MFO.py
--rw-rw-rw-   0        0        0    14600 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/MODE.py
--rw-rw-rw-   0        0        0    25532 2023-06-06 07:13:42.000000 pycup-0.1.7.1/pycup/MOMFO.py
--rw-rw-rw-   0        0        0    24212 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/MOPSO.py
--rw-rw-rw-   0        0        0    14937 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/NSGA2.py
--rw-rw-rw-   0        0        0    19287 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/PESTclasses.py
--rw-rw-rw-   0        0        0    35498 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/PSO.py
--rw-rw-rw-   0        0        0    15659 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/Reslib.py
--rw-rw-rw-   0        0        0    30073 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/SCA.py
--rw-rw-rw-   0        0        0    32941 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/SOA.py
--rw-rw-rw-   0        0        0    32160 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/SSA.py
--rw-rw-rw-   0        0        0     5757 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/TOPSIS.py
--rw-rw-rw-   0        0        0    33343 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/TSA.py
--rw-rw-rw-   0        0        0    32912 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/WOA.py
--rw-rw-rw-   0        0        0      975 2023-06-05 14:17:37.000000 pycup-0.1.7.1/pycup/__init__.py
--rw-rw-rw-   0        0        0    10042 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/calc_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:15:25.186508 pycup-0.1.7.1/pycup/document/
--rw-rw-rw-   0        0        0   826264 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/document/Documentation.pdf
--rw-rw-rw-   0        0        0     4027 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/evaluation_metrics.py
--rw-rw-rw-   0        0        0    53886 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/integrate.py
--rw-rw-rw-   0        0        0     7263 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/multi_jobs.py
--rw-rw-rw-   0        0        0   125519 2023-06-06 07:11:27.000000 pycup-0.1.7.1/pycup/plot.py
--rw-rw-rw-   0        0        0      460 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/progress_bar.py
--rw-rw-rw-   0        0        0    10352 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/sampling.py
--rw-rw-rw-   0        0        0    19081 2023-06-05 14:17:37.000000 pycup-0.1.7.1/pycup/save.py
--rw-rw-rw-   0        0        0     2068 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/template.py
--rw-rw-rw-   0        0        0        0 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/test.py
--rw-rw-rw-   0        0        0     6055 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/test_functions.py
--rw-rw-rw-   0        0        0    69170 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/uncertainty_analysis_fun.py
--rw-rw-rw-   0        0        0    17048 2023-06-05 14:05:02.000000 pycup-0.1.7.1/pycup/utilize.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:15:25.182928 pycup-0.1.7.1/pycup.egg-info/
--rw-rw-rw-   0        0        0     6368 2023-06-06 07:15:25.000000 pycup-0.1.7.1/pycup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      705 2023-06-06 07:15:25.000000 pycup-0.1.7.1/pycup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 07:15:25.000000 pycup-0.1.7.1/pycup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-06 07:15:25.000000 pycup-0.1.7.1/pycup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-06 07:15:25.000000 pycup-0.1.7.1/pycup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 07:15:25.190031 pycup-0.1.7.1/setup.cfg
--rw-rw-rw-   0        0        0      955 2023-06-06 07:13:42.000000 pycup-0.1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:39:14.444435 pycup-0.1.7.2/
+-rw-rw-rw-   0        0        0     6695 2023-06-08 11:39:14.443433 pycup-0.1.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5431 2023-06-08 11:38:11.000000 pycup-0.1.7.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:39:14.428431 pycup-0.1.7.2/pycup/
+-rw-rw-rw-   0        0        0    17161 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/GLUE.py
+-rw-rw-rw-   0        0        0    38271 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/GWO.py
+-rw-rw-rw-   0        0        0    35573 2023-06-08 11:31:10.000000 pycup-0.1.7.2/pycup/MFO.py
+-rw-rw-rw-   0        0        0    14600 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/MODE.py
+-rw-rw-rw-   0        0        0    26848 2023-06-08 03:47:05.000000 pycup-0.1.7.2/pycup/MOMFO.py
+-rw-rw-rw-   0        0        0    24212 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/MOPSO.py
+-rw-rw-rw-   0        0        0    14937 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/NSGA2.py
+-rw-rw-rw-   0        0        0    19287 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/PESTclasses.py
+-rw-rw-rw-   0        0        0    35498 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/PSO.py
+-rw-rw-rw-   0        0        0    15659 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/Reslib.py
+-rw-rw-rw-   0        0        0    30073 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/SCA.py
+-rw-rw-rw-   0        0        0    32941 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/SOA.py
+-rw-rw-rw-   0        0        0    32160 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/SSA.py
+-rw-rw-rw-   0        0        0     5757 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/TOPSIS.py
+-rw-rw-rw-   0        0        0    33343 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/TSA.py
+-rw-rw-rw-   0        0        0    32912 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/WOA.py
+-rw-rw-rw-   0        0        0      975 2023-06-05 14:17:37.000000 pycup-0.1.7.2/pycup/__init__.py
+-rw-rw-rw-   0        0        0    10042 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/calc_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:39:14.439433 pycup-0.1.7.2/pycup/document/
+-rw-rw-rw-   0        0        0   826264 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/document/Documentation.pdf
+-rw-rw-rw-   0        0        0     4027 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/evaluation_metrics.py
+-rw-rw-rw-   0        0        0    53886 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/integrate.py
+-rw-rw-rw-   0        0        0     7263 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/multi_jobs.py
+-rw-rw-rw-   0        0        0   125519 2023-06-06 07:11:27.000000 pycup-0.1.7.2/pycup/plot.py
+-rw-rw-rw-   0        0        0      460 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/progress_bar.py
+-rw-rw-rw-   0        0        0    10352 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/sampling.py
+-rw-rw-rw-   0        0        0    19233 2023-06-08 03:47:05.000000 pycup-0.1.7.2/pycup/save.py
+-rw-rw-rw-   0        0        0     2068 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/template.py
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/test.py
+-rw-rw-rw-   0        0        0     6055 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/test_functions.py
+-rw-rw-rw-   0        0        0    69170 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/uncertainty_analysis_fun.py
+-rw-rw-rw-   0        0        0    17048 2023-06-05 14:05:02.000000 pycup-0.1.7.2/pycup/utilize.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:39:14.436432 pycup-0.1.7.2/pycup.egg-info/
+-rw-rw-rw-   0        0        0     6695 2023-06-08 11:39:14.000000 pycup-0.1.7.2/pycup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-06-08 11:39:14.000000 pycup-0.1.7.2/pycup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:39:14.000000 pycup-0.1.7.2/pycup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-08 11:39:14.000000 pycup-0.1.7.2/pycup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-08 11:39:14.000000 pycup-0.1.7.2/pycup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:39:14.444435 pycup-0.1.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      955 2023-06-08 03:47:05.000000 pycup-0.1.7.2/setup.py
```

### Comparing `pycup-0.1.7.1/PKG-INFO` & `pycup-0.1.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycup
-Version: 0.1.7.1
+Version: 0.1.7.2
 Summary: An auto-calibration tool for environmental models based on heuristic algorithms and uncertainty estimation theory.
 Home-page: https://github.com/QianyangWang/PyCUP
 Author: Qianyang Wang
 Author-email: wqy07010944@hotmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/QianyangWang/PyCUP/DOCUMENT
 Project-URL: Source, https://github.com/QianyangWang/PyCUP/pycup
@@ -12,15 +12,16 @@
         
         <img src="https://img.shields.io/badge/Version-0.1.7-brightgreen" /><img src="https://img.shields.io/badge/Language-Python-blue" />	
         
         This is an open-source package designed for (environmental) model calibration and uncertainty analysis. The current version is the very first version, we welcome all comments, suggestions, and improvements.
         
         ## v 0.1.7 Update
         
-        A new superior algorithm MOMFO (multi-objective moth-flame optimizer)  based on archive and crowding distance non-domination sort, and its elite-opposition improved version (EO-MOMFO) have been designed and provided in the new version. The elite opposition mechanism was modified based on the concept of non-domination and was embedded for updating the flame population of MOMFO. The implemented MOMFO has a similar principle as the current literature, although with some differences in details, while the elite-opposition version is original in this package.
+        1.  A new superior algorithm MOMFO (multi-objective moth-flame optimizer)  based on archive and crowding distance non-domination sort, and its elite-opposition improved version (EO-MOMFO) have been designed and provided in the new version. The elite opposition mechanism was modified based on the concept of non-domination and was embedded for updating the flame population of MOMFO. The implemented MOMFO has a similar principle as the current literature, although with some differences in details, while the elite-opposition version is original in this package.
+        1.  A "Mode" variable for MFO and MOMFO for switching the flame updating mechanism has been provided. A "Mode" value of 0 is for Mirjalili's original version, while a "Mode" value of 1 (default) is my modification. Details about the differences will be given in the upcoming algorithm introduction documentations.
         
         ## What does it have
         
         ### (1) For model calibration/optimization
         
         1. Single-objective heuristic algorithms including PSO, GWO, MFO, SOA, SCA, SSA, TSA, and WOA.
         2. Multi-objective heuristic algorithms including MOPSO, MODE, and NSGA-II.
```

### Comparing `pycup-0.1.7.1/README.md` & `pycup-0.1.7.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 <img src="https://img.shields.io/badge/Version-0.1.7-brightgreen" /><img src="https://img.shields.io/badge/Language-Python-blue" />	
 
 This is an open-source package designed for (environmental) model calibration and uncertainty analysis. The current version is the very first version, we welcome all comments, suggestions, and improvements.
 
 ## v 0.1.7 Update
 
-A new superior algorithm MOMFO (multi-objective moth-flame optimizer)  based on archive and crowding distance non-domination sort, and its elite-opposition improved version (EO-MOMFO) have been designed and provided in the new version. The elite opposition mechanism was modified based on the concept of non-domination and was embedded for updating the flame population of MOMFO. The implemented MOMFO has a similar principle as the current literature, although with some differences in details, while the elite-opposition version is original in this package.
+1.  A new superior algorithm MOMFO (multi-objective moth-flame optimizer)  based on archive and crowding distance non-domination sort, and its elite-opposition improved version (EO-MOMFO) have been designed and provided in the new version. The elite opposition mechanism was modified based on the concept of non-domination and was embedded for updating the flame population of MOMFO. The implemented MOMFO has a similar principle as the current literature, although with some differences in details, while the elite-opposition version is original in this package.
+1.  A "Mode" variable for MFO and MOMFO for switching the flame updating mechanism has been provided. A "Mode" value of 0 is for Mirjalili's original version, while a "Mode" value of 1 (default) is my modification. Details about the differences will be given in the upcoming algorithm introduction documentations.
 
 ## What does it have
 
 ### (1) For model calibration/optimization
 
 1. Single-objective heuristic algorithms including PSO, GWO, MFO, SOA, SCA, SSA, TSA, and WOA.
 2. Multi-objective heuristic algorithms including MOPSO, MODE, and NSGA-II.
```

### Comparing `pycup-0.1.7.1/pycup/GLUE.py` & `pycup-0.1.7.2/pycup/GLUE.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/GWO.py` & `pycup-0.1.7.2/pycup/GWO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/MFO.py` & `pycup-0.1.7.2/pycup/MFO.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .calc_utils import BorderChecker,SortFitness,SortPosition,check_listitem,record_check,record_checkMV
 from .calc_utils import CalculateFitness,CalculateFitnessMP,CalculateFitness_MV,CalculateFitnessMP_MV
 
 Sampling = "LHS"
 EliteOppoSwitch = True
 OppoFactor = 0.1
 BorderCheckMethod = "rebound"
+Mode = 1 # The switch for the flame generation mechanism, 0: Mirjalili's original version, 1: My version
 
 
 def initial(pop, dim, ub, lb):
     """
     lhs sampling based initialization
     :argument
     pop: population size -> int
@@ -124,37 +125,39 @@
         hr = []
         X, lb, ub = initial(pop, dim, ub, lb)
         fitness,res = CalculateFitness(X, fun,1, args)
         hr.append(res)
         hs.append(copy.copy(X))
         hf.append(copy.copy(fitness))
         Progress_Bar.update(len(hf))
-        #X_previous = copy.copy(X)
-        #fitness_previous = copy.copy(fitness)
-        #res_previous = copy.copy(res)
         fitnessS, sortIndex = SortFitness(fitness)
         # in the first iteration, the flame is the sorted population
         Xs = SortPosition(X, sortIndex)
+        # X t-1
+        Xp = copy.copy(X)
+        fitnessP = copy.copy(fitness)
         GbestScore = copy.copy(fitnessS[0])
         GbestPosition = np.zeros([1, dim])
         GbestPosition[0, :] = copy.copy(Xs[0, :])
         Curve = np.zeros([MaxIter, 1])
         record = save.SwarmRecord(pop=pop,dim=dim,lb=lb,ub=ub,hf=hf,hs=hs,hr=hr,
                          GbestPosition=GbestPosition,GbestScore=GbestScore,Curve=Curve,X=X,fitness=fitness,iteration=0,
-                         Xs=Xs,fitnessS=fitnessS)
+                         Xs=Xs,fitnessS=fitnessS,Xp=Xp,fitnessP=fitnessP)
         record.save()
     else:
         record = save.SwarmRecord.load(RecordPath)
         hs = record.hs
         hf = record.hf
         hr = record.hr
         X = record.X
         Xs = record.Xs
+        Xp = record.Xp
         fitnessS = record.fitnessS
         fitness = record.fitness
+        fitnessP = record.fitnessP
         GbestScore = record.GbestScore
         GbestPosition = record.GbestPosition
         Curve = record.Curve
         iter = record.iteration
         a_lb = record.lb
         a_ub = record.ub
         a_pop = record.pop
@@ -182,24 +185,34 @@
                     r = (a - 1) * random.random() + 1
                     X[i, j] = distance_to_flame * np.exp(b * r) * np.cos(r * 2 * math.pi) + Xs[Flame_no-1, j]
 
 
         X = checker.BorderCheck(X, ub, lb, pop, dim)
         fitness, res = CalculateFitness(X, fun,1, args)
 
-        # merge the flame and moth
-        fitnessM = np.concatenate([fitnessS,fitness],axis=0)
-        Xm = np.concatenate([Xs,X],axis=0)
+        # merge the moth t-1 (mode = 0)/ flame (mode = 1) and moth
+        if Mode == 0:
+            # Mirjalili's original version
+            Xm = np.concatenate([Xp, X], axis=0)
+            fitnessM = np.concatenate([fitnessP, fitness], axis=0)
+        elif Mode == 1:
+            # My version: Remain the historical local/global optimums, v1 and v2 will be the same in iteration 0 and 1
+            # This modification can guide the moths always using the historical optima, instead of loosing them as in mode 1
+            Xm = np.concatenate([Xs,X],axis=0)
+            fitnessM = np.concatenate([fitnessS, fitness], axis=0)
+        else:
+            raise NotImplementedError("The mode should be 0 or 1.")
         fitnessM, sortIndexM = SortFitness(fitnessM)
         Xm = SortPosition(Xm, sortIndexM)
         # update the Xs (flame population)
         Xs = Xm[0:Flame_no,:]
         fitnessS = fitnessM[0:Flame_no]
 
-
+        Xp = copy.copy(X)
+        fitnessP = copy.copy(fitness)
         X2file = copy.copy(X)
         fitness2file = copy.copy(fitness)
         res2file = copy.copy(res)
         if EliteOppoSwitch:
 
             EliteNumber = int(np.ceil(Xs.shape[0] * OppoFactor))
             if EliteNumber > 0:
@@ -229,15 +242,15 @@
             GbestScore = copy.copy(fitnessS[0])
             GbestPosition[0, :] = copy.copy(Xs[0, :])
         Curve[t] = GbestScore
         Progress_Bar.update(len(hf))
 
         record = save.SwarmRecord(pop=pop,dim=dim,lb=lb,ub=ub,hf=hf,hs=hs,hr=hr,
                          GbestPosition=GbestPosition,GbestScore=GbestScore,Curve=Curve,X=X,fitness=fitness,iteration=t+1,
-                         Xs=Xs,fitnessS=fitnessS)
+                         Xs=Xs,fitnessS=fitnessS,Xp=Xp,fitnessP=fitnessP)
         record.save()
 
     print("")  # for progress bar
     if Reslib.UseResObject:
         hr = Reslib.ResultDataPackage(l_result=hr,method_info="Algorithm")
     raw_saver = save.RawDataSaver(hs, hf, hr, GbestScore, GbestPosition, Curve)
     raw_saver.save(save.raw_path)
@@ -304,30 +317,35 @@
         fitness, res = CalculateFitnessMP(X, fun,1,n_jobs, args)
         hr.append(res)
         hs.append(copy.copy(X))
         hf.append(copy.copy(fitness))
         Progress_Bar.update(len(hf))
         fitnessS, sortIndex = SortFitness(fitness)
         Xs = SortPosition(X, sortIndex)
+        # X t-1
+        Xp = copy.copy(X)
+        fitnessP = copy.copy(fitness)
         GbestScore = copy.copy(fitnessS[0])
         GbestPosition = np.zeros([1, dim])
         GbestPosition[0, :] = copy.copy(Xs[0, :])
         Curve = np.zeros([MaxIter, 1])
         record = save.SwarmRecord(pop=pop,dim=dim,lb=lb,ub=ub,hf=hf,hs=hs,hr=hr,
                          GbestPosition=GbestPosition,GbestScore=GbestScore,Curve=Curve,X=X,fitness=fitness,iteration=0,
-                         Xs=Xs,fitnessS=fitnessS)
+                         Xs=Xs,fitnessS=fitnessS,Xp=Xp,fitnessP=fitnessP)
         record.save()
     else:
         record = save.SwarmRecord.load(RecordPath)
         hs = record.hs
         hf = record.hf
         hr = record.hr
         X = record.X
         Xs = record.Xs
+        Xp = record.Xp
         fitnessS = record.fitnessS
+        fitnessP = record.fitnessP
         fitness = record.fitness
         GbestScore = record.GbestScore
         GbestPosition = record.GbestPosition
         Curve = record.Curve
         iter = record.iteration
         a_lb = record.lb
         a_ub = record.ub
@@ -354,22 +372,33 @@
                     distance_to_flame = np.abs(Xs[Flame_no - 1, j] - X[i, j])
                     b = 1
                     r = (a - 1) * random.random() + 1
                     X[i, j] = distance_to_flame * np.exp(b * r) * np.cos(r * 2 * math.pi) + Xs[Flame_no - 1, j]
 
         X = checker.BorderCheck(X, ub, lb, pop, dim)
         fitness, res = CalculateFitnessMP(X, fun,1,n_jobs, args)
-        fitnessM = np.concatenate([fitnessS, fitness], axis=0)
-        Xm = np.concatenate([Xs, X], axis=0)
+        # merge the moth t-1 (mode = 0)/ flame (mode = 1) and moth
+        if Mode == 0:
+            # Mirjalili's original version
+            Xm = np.concatenate([Xp, X], axis=0)
+            fitnessM = np.concatenate([fitnessP, fitness], axis=0)
+        elif Mode == 1:
+            # My version: Remain the historical local optimums
+            Xm = np.concatenate([Xs,X],axis=0)
+            fitnessM = np.concatenate([fitnessS, fitness], axis=0)
+        else:
+            raise NotImplementedError("The mode should be 0 or 1.")
         fitnessM, sortIndexM = SortFitness(fitnessM)
         Xm = SortPosition(Xm, sortIndexM)
         # update the Xs
         Xs = Xm[0:Flame_no, :]
         fitnessS = fitnessM[0:Flame_no]
 
+        Xp = copy.copy(X)
+        fitnessP = copy.copy(fitness)
         X2file = copy.copy(X)
         fitness2file = copy.copy(fitness)
         res2file = copy.copy(res)
         if EliteOppoSwitch:
 
             EliteNumber = int(np.ceil(Xs.shape[0] * OppoFactor))
             if EliteNumber > 0:
@@ -399,15 +428,15 @@
             GbestScore = copy.copy(fitnessS[0])
             GbestPosition[0, :] = copy.copy(Xs[0, :])
         Curve[t] = GbestScore
         Progress_Bar.update(len(hf))
 
         record = save.SwarmRecord(pop=pop,dim=dim,lb=lb,ub=ub,hf=hf,hs=hs,hr=hr,
                          GbestPosition=GbestPosition,GbestScore=GbestScore,Curve=Curve,X=X,fitness=fitness,iteration=t+1,
-                         Xs=Xs,fitnessS=fitnessS)
+                         Xs=Xs,fitnessS=fitnessS,Xp=Xp,fitnessP=fitnessP)
         record.save()
 
     print("")  # for progress bar
     if Reslib.UseResObject:
         hr = Reslib.ResultDataPackage(l_result=hr,method_info="Algorithm")
     raw_saver = save.RawDataSaver(hs, hf, hr, GbestScore, GbestPosition, Curve)
     raw_saver.save(save.raw_path)
@@ -459,14 +488,17 @@
         hfs = [[] for i in range(num_var)]
         hrs = [[] for i in range(num_var)]
 
         X, lbs, ubs = initial_MV(pop, dims, ubs, lbs)
         fitness,res = CalculateFitness_MV(X, fun, args)
         Xs = copy.copy(X)
         fitnessS = copy.copy(fitness)
+        # X t-1
+        Xp = copy.copy(X)
+        fitnessP = copy.copy(fitness)
         for i in range(num_var):
             hrs[i].append(res[i])
             hss[i].append(copy.copy(X[i]))
             hfs[i].append(copy.copy(fitness[i]))
         Progress_Bar.update(len(hfs[0]))
 
         for n in range(num_var):
@@ -476,24 +508,26 @@
         GbestScore = [copy.copy(fitnessS[n][0]) for n in range(num_var)]
         GbestPosition = [np.zeros([1, dims[n]]) for n in range(num_var)]
         for n in range(num_var):
             GbestPosition[n][0, :] = copy.copy(Xs[n][0, :])
         Curve = [np.zeros([MaxIter, 1]) for i in range(num_var)]
         record = save.SwarmRecord(pop=pop,dim=dims,lb=lbs,ub=ubs,hf=hfs,hs=hss,hr=hrs,
                          GbestPosition=GbestPosition,GbestScore=GbestScore,Curve=Curve,X=X,fitness=fitness,iteration=0,
-                         Xs=Xs,fitnessS=fitnessS)
+                         Xs=Xs,fitnessS=fitnessS,Xp=Xp,fitnessP=fitnessP)
         record.save()
     else:
         record = save.SwarmRecord.load(RecordPath)
         hss = record.hs
         hfs = record.hf
         hrs = record.hr
         X = record.X
         Xs = record.Xs
+        Xp = record.Xp
         fitnessS = record.fitnessS
+        fitnessP = record.fitnessP
         fitness = record.fitness
         GbestScore = record.GbestScore
         GbestPosition = record.GbestPosition
         Curve = record.Curve
         iter = record.iteration
         a_lb = record.lb
         a_ub = record.ub
@@ -524,22 +558,30 @@
                         X[n][i, j] = distance_to_flame * np.exp(b * r) * np.cos(r * 2 * math.pi) + Xs[n][Flame_no-1, j]
 
         for n in range(num_var):
             X[n] = checker.BorderCheck(X[n], ubs[n], lbs[n], pop, dims[n])
         fitness, res = CalculateFitness_MV(X, fun, args)
 
         for n in range(num_var):
-            fitnessM = np.concatenate([fitnessS[n],fitness[n]],axis=0)
-            Xm = np.concatenate([Xs[n],X[n]],axis=0)
+            if Mode == 0:
+                fitnessM = np.concatenate([fitnessP[n],fitness[n]],axis=0)
+                Xm = np.concatenate([Xp[n],X[n]],axis=0)
+            elif Mode == 1:
+                fitnessM = np.concatenate([fitnessS[n],fitness[n]],axis=0)
+                Xm = np.concatenate([Xs[n],X[n]],axis=0)
+            else:
+                raise NotImplementedError("The mode should be 0 or 1.")
             fitnessM, sortIndexM = SortFitness(fitnessM)
             Xm = SortPosition(Xm, sortIndexM)
             # update the Xs
             Xs[n] = Xm[0:Flame_no,:]
             fitnessS[n] = fitnessM[0:Flame_no]
 
+        Xp = copy.copy(X)
+        fitnessP = copy.copy(fitness)
         X2file = copy.copy(X)
         fitness2file = copy.copy(fitness)
         res2file = copy.copy(res)
         if EliteOppoSwitch:
 
             EliteNumber = int(np.ceil(Xs[0].shape[0] * OppoFactor))
             if EliteNumber > 0:
@@ -574,15 +616,15 @@
                 GbestScore[n] = copy.copy(fitnessS[n][0])
                 GbestPosition[n][0, :] = copy.copy(Xs[n][0, :])
             Curve[n][t] = GbestScore[n]
         Progress_Bar.update(len(hfs[0]))
 
         record = save.SwarmRecord(pop=pop,dim=dims,lb=lbs,ub=ubs,hf=hfs,hs=hss,hr=hrs,
                          GbestPosition=GbestPosition,GbestScore=GbestScore,Curve=Curve,X=X,fitness=fitness,iteration=t+1,
-                         Xs=Xs,fitnessS=fitnessS)
+                         Xs=Xs,fitnessS=fitnessS,Xp=Xp,fitnessP=fitnessP)
         record.save()
 
     print("")  # for progress bar
     for n in range(num_var):
 
         if len(save.raw_pathMV) == len(hss):
             save.raw_path = save.raw_pathMV[n]
@@ -641,14 +683,17 @@
         hss = [[] for i in range(num_var)]
         hfs = [[] for i in range(num_var)]
         hrs = [[] for i in range(num_var)]
         X, lbs, ubs = initial_MV(pop, dims, ubs, lbs)
         fitness,res = CalculateFitnessMP_MV(X, fun,n_jobs, args)
         Xs = copy.copy(X)
         fitnessS = copy.copy(fitness)
+        # X t-1
+        Xp = copy.copy(X)
+        fitnessP = copy.copy(fitness)
         for i in range(num_var):
             hrs[i].append(res[i])
             hss[i].append(copy.copy(X[i]))
             hfs[i].append(copy.copy(fitness[i]))
         Progress_Bar.update(len(hfs[0]))
 
         for n in range(num_var):
@@ -658,25 +703,27 @@
         GbestScore = [copy.copy(fitnessS[n][0]) for n in range(num_var)]
         GbestPosition = [np.zeros([1, dims[n]]) for n in range(num_var)]
         for n in range(num_var):
             GbestPosition[n][0, :] = copy.copy(Xs[n][0, :])
         Curve = [np.zeros([MaxIter, 1]) for i in range(num_var)]
         record = save.SwarmRecord(pop=pop,dim=dims,lb=lbs,ub=ubs,hf=hfs,hs=hss,hr=hrs,
                          GbestPosition=GbestPosition,GbestScore=GbestScore,Curve=Curve,X=X,fitness=fitness,iteration=0,
-                         Xs=Xs,fitnessS=fitnessS)
+                         Xs=Xs,fitnessS=fitnessS,Xp=Xp,fitnessP=fitnessP)
         record.save()
     else:
         record = save.SwarmRecord.load(RecordPath)
         hss = record.hs
         hfs = record.hf
         hrs = record.hr
         X = record.X
         Xs = record.Xs
+        Xp = record.Xp
         fitnessS = record.fitnessS
         fitness = record.fitness
+        fitnessP = record.fitnessP
         GbestScore = record.GbestScore
         GbestPosition = record.GbestPosition
         Curve = record.Curve
         iter = record.iteration
         a_lb = record.lb
         a_ub = record.ub
         a_pop = record.pop
@@ -706,22 +753,30 @@
                         X[n][i, j] = distance_to_flame * np.exp(b * r) * np.cos(r * 2 * math.pi) + Xs[n][Flame_no-1, j]
 
         for n in range(num_var):
             X[n] = checker.BorderCheck(X[n], ubs[n], lbs[n], pop, dims[n])
         fitness, res = CalculateFitnessMP_MV(X, fun,n_jobs, args)
 
         for n in range(num_var):
-            fitnessM = np.concatenate([fitnessS[n],fitness[n]],axis=0)
-            Xm = np.concatenate([Xs[n],X[n]],axis=0)
+            if Mode == 0:
+                fitnessM = np.concatenate([fitnessP[n],fitness[n]],axis=0)
+                Xm = np.concatenate([Xp[n],X[n]],axis=0)
+            elif Mode == 1:
+                fitnessM = np.concatenate([fitnessS[n],fitness[n]],axis=0)
+                Xm = np.concatenate([Xs[n],X[n]],axis=0)
+            else:
+                raise NotImplementedError("The mode should be 0 or 1.")
             fitnessM, sortIndexM = SortFitness(fitnessM)
             Xm = SortPosition(Xm, sortIndexM)
             # update the Xs
             Xs[n] = Xm[0:Flame_no,:]
             fitnessS[n] = fitnessM[0:Flame_no]
 
+        Xp = copy.copy(X)
+        fitnessP = copy.copy(fitness)
         X2file = copy.copy(X)
         fitness2file = copy.copy(fitness)
         res2file = copy.copy(res)
         if EliteOppoSwitch:
 
             EliteNumber = int(np.ceil(Xs[0].shape[0] * OppoFactor))
             if EliteNumber > 0:
@@ -756,15 +811,15 @@
                 GbestScore[n] = copy.copy(fitnessS[n][0])
                 GbestPosition[n][0, :] = copy.copy(Xs[n][0, :])
             Curve[n][t] = GbestScore[n]
         Progress_Bar.update(len(hfs[0]))
 
         record = save.SwarmRecord(pop=pop,dim=dims,lb=lbs,ub=ubs,hf=hfs,hs=hss,hr=hrs,
                          GbestPosition=GbestPosition,GbestScore=GbestScore,Curve=Curve,X=X,fitness=fitness,iteration=t+1,
-                         Xs=Xs,fitnessS=fitnessS)
+                         Xs=Xs,fitnessS=fitnessS,Xp=Xp,fitnessP=fitnessP)
         record.save()
 
     print("")  # for progress bar
     for n in range(num_var):
 
         if len(save.raw_pathMV) == len(hss):
             save.raw_path = save.raw_pathMV[n]
```

### Comparing `pycup-0.1.7.1/pycup/MODE.py` & `pycup-0.1.7.2/pycup/MODE.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/MOMFO.py` & `pycup-0.1.7.2/pycup/MOMFO.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .calc_utils import BorderChecker,SortFitness,SortPosition,check_listitem,record_check,record_checkMV
 from .calc_utils import CalculateFitness,CalculateFitnessMP,CalculateFitness_MV,CalculateFitnessMP_MV
 from collections import Counter
 Sampling = "LHS"
 EliteOppoSwitch = True
 OppoFactor = 0.1
 BorderCheckMethod = "rebound"
+Mode = 0
 
 
 def nonDominationSort(X, fitness):
 
     pop = X.shape[0]
     nF = fitness.shape[1]
     ranks = np.zeros(pop, dtype=np.int32)
@@ -330,14 +331,17 @@
     if not RecordPath:
         iter = 0
         hs = []
         hf = []
         hr = []
         X, lb, ub = initial(pop, dim, ub, lb)
         fitness,res = CalculateFitness(X, fun,n_obj, args)
+        # X t-1
+        Xp = copy.copy(X)
+        fitnessP = copy.copy(fitness)
         hr.append(res)
         hs.append(copy.copy(X))
         hf.append(copy.copy(fitness))
         Progress_Bar.update(len(hf))
 
         # initialize the archive set
         archive, arFits,arRes = getNonDominationPops(X, fitness,res)
@@ -345,29 +349,31 @@
         # the first iteration use the sorted X as the flame
         ranks = nonDominationSort(X, fitness)
         distances = crowdingDistanceSort(X, fitness, ranks)
         #Xs, fitnessS = select1(pop, X, fitness, ranks, distances)
         Xs, fitnessS = rank_distance_sort(X, fitness, ranks, distances)
         record = save.MOswarmRecord(pop=pop,dim=dim,lb=lb,ub=ub,hf=hf,hs=hs,hr=hr,
                          X=X,fitness=fitness,iteration=0,
-                         Xs=Xs,fitnessS=fitnessS,n_obj=n_obj)
+                         Xs=Xs,fitnessS=fitnessS,Xp=Xp,fitnessP=fitnessP,archive=archive,arFits=arFits,arRes=arRes,n_obj=n_obj)
         record.save()
 
     else:
         record = save.SwarmRecord.load(RecordPath)
         hs = record.hs
         hf = record.hf
         hr = record.hr
         archive = record.archive
         arFits = record.arFits
         arRes = record.arRes
         X = record.X
         Xs = record.Xs
+        Xp = record.Xp
         fitnessS = record.fitnessS
         fitness = record.fitness
+        fitnessP = record.fitnessP
         iter = record.iteration
         a_lb = record.lb
         a_ub = record.ub
         a_pop = record.pop
         a_dim = record.dim
         same = record_check(pop,dim,lb,ub,a_pop,a_dim,a_lb,a_ub)
         if not same:
@@ -394,24 +400,34 @@
 
 
         X = checker.BorderCheck(X, ub, lb, pop, dim)
         fitness, res = CalculateFitness(X, fun,n_obj, args)
         archive, arFits,arRes = updateArchive(X, fitness,res, archive, arFits,arRes)
         archive, arFits,arRes = checkArchive(archive, arFits,arRes, nAr, M)
         # merge the flame and moth
-        fitnessM = np.concatenate([fitnessS,fitness],axis=0)
-        Xm = np.concatenate([Xs,X],axis=0)
+        if Mode == 0:
+            # Mirjalili's original version
+            fitnessM = np.concatenate([fitnessP, fitness], axis=0)
+            Xm = np.concatenate([Xp, X], axis=0)
+        elif Mode == 1:
+            # My version: Remain the historical local optimums, v1 and v2 will be the same in iteration 0 and 1
+            fitnessM = np.concatenate([fitnessS,fitness],axis=0)
+            Xm = np.concatenate([Xs,X],axis=0)
+        else:
+            raise NotImplementedError("The mode should be 0 or 1.")
         ranks = nonDominationSort(Xm, fitnessM)
         distances = crowdingDistanceSort(Xm, fitnessM, ranks)
         #Xm, fitnessM = select1(Xm.shape[0], Xm, fitnessM, ranks, distances)
         Xm, fitnessM = rank_distance_sort(Xm, fitnessM, ranks, distances)
         # update the Xs (flame population)
         Xs = Xm[0:Flame_no,:]
         fitnessS = fitnessM[0:Flame_no]
 
+        Xp = copy.copy(X)
+        fitnessP = copy.copy(fitness)
         X2file = copy.copy(X)
         fitness2file = copy.copy(fitness)
         res2file = copy.copy(res)
         if EliteOppoSwitch:
 
             EliteNumber = int(np.ceil(Xs.shape[0] * OppoFactor))
             if EliteNumber > 0:
@@ -427,15 +443,14 @@
                     isDom = sum(isDom1) >= 1 and sum(isDom2) == n_obj
                     if isDom:
                         fitnessS[j] = copy.copy(fitOppo[j])
                         Xs[j, :] = copy.copy(XOppo[j, :])
 
                 ranks = nonDominationSort(Xs, fitnessS)
                 distances = crowdingDistanceSort(Xs, fitnessS, ranks)
-                #Xs, fitnessS = select1(Xs.shape[0], Xs, fitnessS, ranks, distances)
                 Xs, fitnessS = rank_distance_sort(Xs, fitnessS, ranks, distances)
                 X2file = np.concatenate([X2file, XOppo], axis=0)
                 fitness2file = np.concatenate([fitness2file, fitOppo], axis=0)
                 res2file = np.concatenate([res2file, resOppo], axis=0)
 
                 archive, arFits, arRes = updateArchive(XOppo, fitOppo, resOppo, archive, arFits, arRes)
                 archive, arFits, arRes = checkArchive(archive, arFits, arRes, nAr, M)
@@ -445,15 +460,15 @@
         hf.append(fitness2file)
 
 
         Progress_Bar.update(len(hf))
 
         record = save.MOswarmRecord(pop=pop,dim=dim,lb=lb,ub=ub,hf=hf,hs=hs,hr=hr,
                          X=X,fitness=fitness,iteration=t+1,
-                         Xs=Xs,fitnessS=fitnessS,archive=archive,arFits=arFits,arRes=arRes,n_obj=n_obj)
+                         Xs=Xs,fitnessS=fitnessS,Xp=Xp,fitnessP=fitnessP,archive=archive,arFits=arFits,arRes=arRes,n_obj=n_obj)
         record.save()
 
     paretoPops, paretoFits, paretoRes = getNonDominationPops(archive, arFits, arRes)
     print("")  # for progress bar
 
     if Reslib.UseResObject:
         hr = Reslib.ResultDataPackage(l_result=hr,method_info="Algorithm")
@@ -528,14 +543,17 @@
     if not RecordPath:
         iter = 0
         hs = []
         hf = []
         hr = []
         X, lb, ub = initial(pop, dim, ub, lb)
         fitness,res = CalculateFitnessMP(X, fun,n_obj,n_jobs, args)
+        # X t-1
+        Xp = copy.copy(X)
+        fitnessP = copy.copy(fitness)
         hr.append(res)
         hs.append(copy.copy(X))
         hf.append(copy.copy(fitness))
         Progress_Bar.update(len(hf))
 
         # initialize the archive set
         archive, arFits,arRes = getNonDominationPops(X, fitness,res)
@@ -543,29 +561,31 @@
         # the first iteration use the sorted X as the flame
         ranks = nonDominationSort(X, fitness)
         distances = crowdingDistanceSort(X, fitness, ranks)
         #Xs, fitnessS = select1(pop, X, fitness, ranks, distances)
         Xs, fitnessS = rank_distance_sort(X, fitness, ranks, distances)
         record = save.MOswarmRecord(pop=pop,dim=dim,lb=lb,ub=ub,hf=hf,hs=hs,hr=hr,
                          X=X,fitness=fitness,iteration=0,
-                         Xs=Xs,fitnessS=fitnessS,n_obj=n_obj)
+                         Xs=Xs,fitnessS=fitnessS,Xp=Xp,fitnessP=fitnessP,archive=archive,arFits=arFits,arRes=arRes,n_obj=n_obj)
         record.save()
 
     else:
         record = save.SwarmRecord.load(RecordPath)
         hs = record.hs
         hf = record.hf
         hr = record.hr
         archive = record.archive
         arFits = record.arFits
         arRes = record.arRes
         X = record.X
         Xs = record.Xs
+        Xp = record.Xp
         fitnessS = record.fitnessS
         fitness = record.fitness
+        fitnessP = record.fitnessP
         iter = record.iteration
         a_lb = record.lb
         a_ub = record.ub
         a_pop = record.pop
         a_dim = record.dim
         same = record_check(pop,dim,lb,ub,a_pop,a_dim,a_lb,a_ub)
         if not same:
@@ -591,24 +611,33 @@
                     X[i, j] = distance_to_flame * np.exp(b * r) * np.cos(r * 2 * math.pi) + Xs[Flame_no-1, j]
 
 
         X = checker.BorderCheck(X, ub, lb, pop, dim)
         fitness, res = CalculateFitnessMP(X, fun,n_obj,n_jobs, args)
         archive, arFits,arRes = updateArchive(X, fitness,res, archive, arFits,arRes)
         archive, arFits,arRes = checkArchive(archive, arFits,arRes, nAr, M)
-        # merge the flame and moth
-        fitnessM = np.concatenate([fitnessS,fitness],axis=0)
-        Xm = np.concatenate([Xs,X],axis=0)
+        if Mode == 0:
+            # Mirjalili's original version
+            fitnessM = np.concatenate([fitnessP, fitness], axis=0)
+            Xm = np.concatenate([Xp, X], axis=0)
+        elif Mode == 1:
+            # My version: Remain the historical local optimums, v1 and v2 will be the same in iteration 0 and 1
+            fitnessM = np.concatenate([fitnessS,fitness],axis=0)
+            Xm = np.concatenate([Xs,X],axis=0)
+        else:
+            raise NotImplementedError("The mode should be 0 or 1.")
         ranks = nonDominationSort(Xm, fitnessM)
         distances = crowdingDistanceSort(Xm, fitnessM, ranks)
         Xm, fitnessM = rank_distance_sort(Xm, fitnessM, ranks, distances)
         # update the Xs (flame population)
         Xs = Xm[0:Flame_no,:]
         fitnessS = fitnessM[0:Flame_no]
 
+        Xp = copy.copy(X)
+        fitnessP = copy.copy(fitness)
         X2file = copy.copy(X)
         fitness2file = copy.copy(fitness)
         res2file = copy.copy(res)
         if EliteOppoSwitch:
 
             EliteNumber = int(np.ceil(Xs.shape[0] * OppoFactor))
             if EliteNumber > 0:
@@ -640,15 +669,15 @@
         hs.append(X2file)
         hf.append(fitness2file)
 
         Progress_Bar.update(len(hf))
 
         record = save.MOswarmRecord(pop=pop,dim=dim,lb=lb,ub=ub,hf=hf,hs=hs,hr=hr,
                          X=X,fitness=fitness,iteration=t+1,
-                         Xs=Xs,fitnessS=fitnessS,archive=archive,arFits=arFits,arRes=arRes,n_obj=n_obj)
+                         Xs=Xs,fitnessS=fitnessS,Xp=Xp,fitnessP=fitnessP,archive=archive,arFits=arFits,arRes=arRes,n_obj=n_obj)
         record.save()
 
     paretoPops, paretoFits, paretoRes = getNonDominationPops(archive, arFits, arRes)
     print("")  # for progress bar
 
     if Reslib.UseResObject:
         hr = Reslib.ResultDataPackage(l_result=hr,method_info="Algorithm")
```

### Comparing `pycup-0.1.7.1/pycup/MOPSO.py` & `pycup-0.1.7.2/pycup/MOPSO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/NSGA2.py` & `pycup-0.1.7.2/pycup/NSGA2.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/PESTclasses.py` & `pycup-0.1.7.2/pycup/PESTclasses.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/PSO.py` & `pycup-0.1.7.2/pycup/PSO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/Reslib.py` & `pycup-0.1.7.2/pycup/Reslib.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/SCA.py` & `pycup-0.1.7.2/pycup/SCA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/SOA.py` & `pycup-0.1.7.2/pycup/SOA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/SSA.py` & `pycup-0.1.7.2/pycup/SSA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/TOPSIS.py` & `pycup-0.1.7.2/pycup/TOPSIS.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/TSA.py` & `pycup-0.1.7.2/pycup/TSA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/WOA.py` & `pycup-0.1.7.2/pycup/WOA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/__init__.py` & `pycup-0.1.7.2/pycup/__init__.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/calc_utils.py` & `pycup-0.1.7.2/pycup/calc_utils.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/document/Documentation.pdf` & `pycup-0.1.7.2/pycup/document/Documentation.pdf`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/evaluation_metrics.py` & `pycup-0.1.7.2/pycup/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/integrate.py` & `pycup-0.1.7.2/pycup/integrate.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/multi_jobs.py` & `pycup-0.1.7.2/pycup/multi_jobs.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/plot.py` & `pycup-0.1.7.2/pycup/plot.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/sampling.py` & `pycup-0.1.7.2/pycup/sampling.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/save.py` & `pycup-0.1.7.2/pycup/save.py`

 * *Files 2% similar despite different names*

```diff
@@ -420,15 +420,15 @@
 class SwarmRecord(RecordSaver):
 
     def __init__(self, pop, dim, lb, ub, hf, hs, hr, X, fitness, iteration, GbestPosition, GbestScore, Curve,
                  Pbest=None, fitnessPbest=None, V=None,
                  Alpha_pos=None, Alpha_score=None, Beta_pos=None, Beta_score=None, Delta_pos=None, Delta_score=None,
                  Xs=None, fitnessS=None, resS=None,
                  MS=None, CS=None, DS=None,X_new=None,
-                 Pos=None
+                 Pos=None,Xp=None,fitnessP=None
                  ):
         self.pop = pop
         self.dim = dim
         self.lb = lb
         self.ub = ub
         self.hf = hf
         self.hs = hs
@@ -456,14 +456,16 @@
         self.resS = resS
 
         self.MS = MS
         self.CS = CS
         self.DS = DS
         self.X_new = X_new
         self.Pos = Pos
+        self.Xp=Xp
+        self.fitnessP=fitnessP
 
 
 class GLUERecord(RecordSaver):
 
     def __init__(self,n,dim,lb,ub,hf,hs,hr,iteration,mode):
         self.n = n
         self.dim = dim
@@ -477,15 +479,15 @@
 
 
 class MOswarmRecord(RecordSaver):
 
     def __init__(self,pop,dim,lb,ub,hf,hs,hr,X,iteration,n_obj,V=None,
                  archive=None,arFits=None,arRes=None,Pbest=None,fitnessPbest=None,
                  fitnessGbest = None,GbestPositon=None,fitness=None,res=None,Xs=None,
-                 fitnessS=None,resS=None):
+                 fitnessS=None,resS=None,Xp=None,fitnessP=None):
         self.pop = pop
         self.dim = dim
         self.lb = lb
         self.ub = ub
         self.hf = hf
         self.hs = hs
         self.hr = hr
@@ -501,7 +503,9 @@
         self.Pbest = Pbest
         self.fitnessPbest = fitnessPbest
         self.GbestPositon = GbestPositon
         self.fitnessGbest = fitnessGbest
         self.Xs=Xs
         self.fitnessS=fitnessS
         self.resS=resS
+        self.Xp = Xp
+        self.fitnessP = fitnessP
```

### Comparing `pycup-0.1.7.1/pycup/template.py` & `pycup-0.1.7.2/pycup/template.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/test_functions.py` & `pycup-0.1.7.2/pycup/test_functions.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/uncertainty_analysis_fun.py` & `pycup-0.1.7.2/pycup/uncertainty_analysis_fun.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup/utilize.py` & `pycup-0.1.7.2/pycup/utilize.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/pycup.egg-info/PKG-INFO` & `pycup-0.1.7.2/pycup.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycup
-Version: 0.1.7.1
+Version: 0.1.7.2
 Summary: An auto-calibration tool for environmental models based on heuristic algorithms and uncertainty estimation theory.
 Home-page: https://github.com/QianyangWang/PyCUP
 Author: Qianyang Wang
 Author-email: wqy07010944@hotmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/QianyangWang/PyCUP/DOCUMENT
 Project-URL: Source, https://github.com/QianyangWang/PyCUP/pycup
@@ -12,15 +12,16 @@
         
         <img src="https://img.shields.io/badge/Version-0.1.7-brightgreen" /><img src="https://img.shields.io/badge/Language-Python-blue" />	
         
         This is an open-source package designed for (environmental) model calibration and uncertainty analysis. The current version is the very first version, we welcome all comments, suggestions, and improvements.
         
         ## v 0.1.7 Update
         
-        A new superior algorithm MOMFO (multi-objective moth-flame optimizer)  based on archive and crowding distance non-domination sort, and its elite-opposition improved version (EO-MOMFO) have been designed and provided in the new version. The elite opposition mechanism was modified based on the concept of non-domination and was embedded for updating the flame population of MOMFO. The implemented MOMFO has a similar principle as the current literature, although with some differences in details, while the elite-opposition version is original in this package.
+        1.  A new superior algorithm MOMFO (multi-objective moth-flame optimizer)  based on archive and crowding distance non-domination sort, and its elite-opposition improved version (EO-MOMFO) have been designed and provided in the new version. The elite opposition mechanism was modified based on the concept of non-domination and was embedded for updating the flame population of MOMFO. The implemented MOMFO has a similar principle as the current literature, although with some differences in details, while the elite-opposition version is original in this package.
+        1.  A "Mode" variable for MFO and MOMFO for switching the flame updating mechanism has been provided. A "Mode" value of 0 is for Mirjalili's original version, while a "Mode" value of 1 (default) is my modification. Details about the differences will be given in the upcoming algorithm introduction documentations.
         
         ## What does it have
         
         ### (1) For model calibration/optimization
         
         1. Single-objective heuristic algorithms including PSO, GWO, MFO, SOA, SCA, SSA, TSA, and WOA.
         2. Multi-objective heuristic algorithms including MOPSO, MODE, and NSGA-II.
```

### Comparing `pycup-0.1.7.1/pycup.egg-info/SOURCES.txt` & `pycup-0.1.7.2/pycup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycup-0.1.7.1/setup.py` & `pycup-0.1.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open(r"README.md",encoding="utf-8") as f:
   long_description = f.read()
 
 
 setup(
     name='pycup',
-  version='0.1.7.1',
+  version='0.1.7.2',
   description='An auto-calibration tool for environmental models based on heuristic algorithms and uncertainty estimation theory.',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='Qianyang Wang',
   author_email='wqy07010944@hotmail.com',
   url='https://github.com/QianyangWang/PyCUP',
   license='MIT License',
```

