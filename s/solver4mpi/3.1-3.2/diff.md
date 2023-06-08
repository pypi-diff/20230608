# Comparing `tmp/solver4mpi-3.1.tar.gz` & `tmp/solver4mpi-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver4mpi-3.1.tar", last modified: Thu Jun  8 10:45:13 2023, max compression
+gzip compressed data, was "solver4mpi-3.2.tar", last modified: Thu Jun  8 13:20:14 2023, max compression
```

## Comparing `solver4mpi-3.1.tar` & `solver4mpi-3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 10:45:13.186433 solver4mpi-3.1/
--rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-08 10:45:13.186303 solver4mpi-3.1/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.1/README.md
--rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-08 10:45:13.186477 solver4mpi-3.1/setup.cfg
--rw-r--r--   0 mregnier   (501) staff       (20)      738 2023-06-08 10:43:28.000000 solver4mpi-3.1/setup.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 10:45:13.183708 solver4mpi-3.1/solver4mpi/
--rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.1/solver4mpi/__init__.py
--rw-r--r--   0 mregnier   (501) staff       (20)     3405 2023-06-08 10:41:31.000000 solver4mpi-3.1/solver4mpi/minimizer_multiprocess.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2120 2023-06-08 10:41:41.000000 solver4mpi-3.1/solver4mpi/test.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 10:45:13.186136 solver4mpi-3.1/solver4mpi.egg-info/
--rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-08 10:45:13.000000 solver4mpi-3.1/solver4mpi.egg-info/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)      266 2023-06-08 10:45:13.000000 solver4mpi-3.1/solver4mpi.egg-info/SOURCES.txt
--rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-08 10:45:13.000000 solver4mpi-3.1/solver4mpi.egg-info/dependency_links.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-08 10:45:13.000000 solver4mpi-3.1/solver4mpi.egg-info/requires.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-08 10:45:13.000000 solver4mpi-3.1/solver4mpi.egg-info/top_level.txt
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 13:20:14.532200 solver4mpi-3.2/
+-rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-08 13:20:14.532044 solver4mpi-3.2/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.2/README.md
+-rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-08 13:20:14.532248 solver4mpi-3.2/setup.cfg
+-rw-r--r--   0 mregnier   (501) staff       (20)      738 2023-06-08 13:19:39.000000 solver4mpi-3.2/setup.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 13:20:14.529478 solver4mpi-3.2/solver4mpi/
+-rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.2/solver4mpi/__init__.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     4313 2023-06-08 13:16:59.000000 solver4mpi-3.2/solver4mpi/minimizer_multiprocess.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2133 2023-06-08 13:14:23.000000 solver4mpi-3.2/solver4mpi/test.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 13:20:14.531847 solver4mpi-3.2/solver4mpi.egg-info/
+-rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-08 13:20:14.000000 solver4mpi-3.2/solver4mpi.egg-info/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)      266 2023-06-08 13:20:14.000000 solver4mpi-3.2/solver4mpi.egg-info/SOURCES.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-08 13:20:14.000000 solver4mpi-3.2/solver4mpi.egg-info/dependency_links.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-08 13:20:14.000000 solver4mpi-3.2/solver4mpi.egg-info/requires.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-08 13:20:14.000000 solver4mpi-3.2/solver4mpi.egg-info/top_level.txt
```

### Comparing `solver4mpi-3.1/setup.py` & `solver4mpi-3.2/setup.py`

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
-    version='3.1',
+    version='3.2',
     # The license can be anything you like
     license='',
     description='Optimized minimizer for MPI in python.',
     # We will also need a readme eventually (there will be a warning)
     # long_description=open('README.txt').read(),
 )
```

### Comparing `solver4mpi-3.1/solver4mpi/minimizer_multiprocess.py` & `solver4mpi-3.2/solver4mpi/minimizer_multiprocess.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 from pyoperators import *
 from scipy.optimize import minimize
 import os
 import multiprocess as mp
+import time
 
 class WrapperCPU:
 
     def __init__(self, chi2, x0, nproc=None, method='TNC', tol=1e-3, options={}, verbose=False):
 
         ### Do some prints
         self.verbose = verbose
@@ -21,36 +22,61 @@
             self.ncpu = os.cpu_count()
         else:
             self.ncpu = nproc
 
         if self.verbose:
             print(f'Requested for {self.ncpu} CPUs')
 
+    def _split_params(self, index_theta):
+
+        '''
+        
+        Distribute the parameters across all available processes
+
+        '''
+        return np.where(index_theta % self.size == self.rank)[0]
+
     def _apply_minimize(self, args):
 
         '''
         
         Apply the scipy.optimize.minimize method on the fun cost function.
 
             
         '''
 
         r = minimize(self.chi2, x0=self.x0, args=args, method=self.method, tol=self.tol, options=self.options)
         return r.x
     
     def perform(self, x):
+        results = np.zeros(x.shape)
+        loop = len(x) // self.ncpu
+        rest = len(x) % self.ncpu
+        start = time.time()
 
-        pool = mp.Pool(processes=self.ncpu)
+        if self.verbose:
+            
+            print(f"You're askip to do {loop} loop with {self.ncpu} CPUs each")
+            print(f"There is {rest} estimation remain")
+
+        for i in range(loop):
 
-        results = pool.starmap(self._apply_minimize, [[param_values] for param_values in x])
+            pool = mp.Pool(processes=self.ncpu)
+            results[self.ncpu*i:self.ncpu*(i+1)] = pool.starmap(self._apply_minimize, [[param_values] for param_values in x[self.ncpu*i:self.ncpu*(i+1)]])
+            pool.close()
+            pool.join()
+        
+        pool = mp.Pool(processes=rest)
+        results[-rest:] = pool.starmap(self._apply_minimize, [[param_values] for param_values in x[-rest:]])
+        end = time.time()
+        if self.verbose:
+            print(f'Estimation done on {x.shape[0]} parameters in {end - start} s')
         
-        pool.close()
-        pool.join()
 
-        return np.concatenate(results)
+        return results
 
 
 
 
 class WrapperMPI:
 
     def __init__(self, comm, chi2, x0, method='TNC', tol=1e-3, options={}, verbose=False):
```

### Comparing `solver4mpi-3.1/solver4mpi/test.py` & `solver4mpi-3.2/solver4mpi/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 def chi2(x, ipix, mref, m_nu, allnus):
 
     #map_beta[ipix] = x
     m_nu_fake = _scale_components_1pix(x, ipix, mref, allnus)
     
     return np.sum((m_nu_fake - m_nu[:, ipix, :])**2)
 
-index_beta = np.arange(0, 150, 1)
+index_beta = np.arange(0, 15, 1)
 
 chi2_partial = partial(chi2, mref=mref, m_nu=m_nu, allnus=allnus)
 
 os.environ['OMP_NUM_THREADS'] = '8'
 
 if rank == 0:
     start = time.time()
-    beta_i = WrapperCPU(chi2_partial, x0=np.ones(1), nproc=8, verbose=True, tol=1e-20, method='TNC').perform(list(index_beta))
+    beta_i = WrapperCPU(chi2_partial, x0=np.ones(1), nproc=2, verbose=True, tol=1e-20, method='TNC').perform(index_beta)
     end = time.time()
     print(f'Execution time : {end - start} s')
-    print(f'Residuals :', beta_i[:5] - beta[:5])
-    print(f'estimated :', beta_i[:5])
-    print(f'true :', beta[:5])
+    print(f'Residuals :', beta_i - beta[:len(index_beta)])
+    print(f'estimated :', beta_i)
+    print(f'true :', beta[:len(index_beta)])
     print(f'Execution time : {end - start} s')
 
 
 
 
 #if comm.Get_rank() == 0:
 #    print(f'Execution time : {end - start} s')
```

