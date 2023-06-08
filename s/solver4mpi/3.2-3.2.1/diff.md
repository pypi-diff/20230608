# Comparing `tmp/solver4mpi-3.2.tar.gz` & `tmp/solver4mpi-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver4mpi-3.2.tar", last modified: Thu Jun  8 13:20:14 2023, max compression
+gzip compressed data, was "solver4mpi-3.2.1.tar", last modified: Thu Jun  8 15:18:09 2023, max compression
```

## Comparing `solver4mpi-3.2.tar` & `solver4mpi-3.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 13:20:14.532200 solver4mpi-3.2/
--rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-08 13:20:14.532044 solver4mpi-3.2/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.2/README.md
--rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-08 13:20:14.532248 solver4mpi-3.2/setup.cfg
--rw-r--r--   0 mregnier   (501) staff       (20)      738 2023-06-08 13:19:39.000000 solver4mpi-3.2/setup.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 13:20:14.529478 solver4mpi-3.2/solver4mpi/
--rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.2/solver4mpi/__init__.py
--rw-r--r--   0 mregnier   (501) staff       (20)     4313 2023-06-08 13:16:59.000000 solver4mpi-3.2/solver4mpi/minimizer_multiprocess.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2133 2023-06-08 13:14:23.000000 solver4mpi-3.2/solver4mpi/test.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 13:20:14.531847 solver4mpi-3.2/solver4mpi.egg-info/
--rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-08 13:20:14.000000 solver4mpi-3.2/solver4mpi.egg-info/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)      266 2023-06-08 13:20:14.000000 solver4mpi-3.2/solver4mpi.egg-info/SOURCES.txt
--rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-08 13:20:14.000000 solver4mpi-3.2/solver4mpi.egg-info/dependency_links.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-08 13:20:14.000000 solver4mpi-3.2/solver4mpi.egg-info/requires.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-08 13:20:14.000000 solver4mpi-3.2/solver4mpi.egg-info/top_level.txt
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 15:18:09.336498 solver4mpi-3.2.1/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-08 15:18:09.336370 solver4mpi-3.2.1/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.2.1/README.md
+-rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-08 15:18:09.336545 solver4mpi-3.2.1/setup.cfg
+-rw-r--r--   0 mregnier   (501) staff       (20)      740 2023-06-08 15:17:27.000000 solver4mpi-3.2.1/setup.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 15:18:09.333624 solver4mpi-3.2.1/solver4mpi/
+-rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.2.1/solver4mpi/__init__.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     4403 2023-06-08 15:14:32.000000 solver4mpi-3.2.1/solver4mpi/minimizer_multiprocess.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2133 2023-06-08 13:14:23.000000 solver4mpi-3.2.1/solver4mpi/test.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 15:18:09.336197 solver4mpi-3.2.1/solver4mpi.egg-info/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-08 15:18:09.000000 solver4mpi-3.2.1/solver4mpi.egg-info/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)      266 2023-06-08 15:18:09.000000 solver4mpi-3.2.1/solver4mpi.egg-info/SOURCES.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-08 15:18:09.000000 solver4mpi-3.2.1/solver4mpi.egg-info/dependency_links.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-08 15:18:09.000000 solver4mpi-3.2.1/solver4mpi.egg-info/requires.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-08 15:18:09.000000 solver4mpi-3.2.1/solver4mpi.egg-info/top_level.txt
```

### Comparing `solver4mpi-3.2/setup.py` & `solver4mpi-3.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     author='Mathias Regnier',
     author_email='mathias.p.regnier@gmail.com',
     # Needed to actually package something
     packages=find_packages(),
     # Needed for dependencies
     install_requires=['scipy', 'pyoperators', 'numpy'],
     # *strongly* suggested for sharing
-    version='3.2',
+    version='3.2.1',
     # The license can be anything you like
     license='',
     description='Optimized minimizer for MPI in python.',
     # We will also need a readme eventually (there will be a warning)
     # long_description=open('README.txt').read(),
 )
```

### Comparing `solver4mpi-3.2/solver4mpi/minimizer_multiprocess.py` & `solver4mpi-3.2.1/solver4mpi/minimizer_multiprocess.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,25 +45,27 @@
         '''
 
         r = minimize(self.chi2, x0=self.x0, args=args, method=self.method, tol=self.tol, options=self.options)
         return r.x
     
     def perform(self, x):
         results = np.zeros(x.shape)
-        loop = len(x) // self.ncpu
-        rest = len(x) % self.ncpu
+        if x.shape[0] < self.ncpu:
+            self.ncpu = x.shape[0]
+            
+        loop = x.shape[0] // self.ncpu
+        rest = x.shape[0] % self.ncpu
         start = time.time()
 
         if self.verbose:
             
             print(f"You're askip to do {loop} loop with {self.ncpu} CPUs each")
             print(f"There is {rest} estimation remain")
 
         for i in range(loop):
-
             pool = mp.Pool(processes=self.ncpu)
             results[self.ncpu*i:self.ncpu*(i+1)] = pool.starmap(self._apply_minimize, [[param_values] for param_values in x[self.ncpu*i:self.ncpu*(i+1)]])
             pool.close()
             pool.join()
         
         pool = mp.Pool(processes=rest)
         results[-rest:] = pool.starmap(self._apply_minimize, [[param_values] for param_values in x[-rest:]])
```

### Comparing `solver4mpi-3.2/solver4mpi/test.py` & `solver4mpi-3.2.1/solver4mpi/test.py`

 * *Files identical despite different names*

