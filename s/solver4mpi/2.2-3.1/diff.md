# Comparing `tmp/solver4mpi-2.2.tar.gz` & `tmp/solver4mpi-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver4mpi-2.2.tar", last modified: Thu May 25 01:21:31 2023, max compression
+gzip compressed data, was "solver4mpi-3.1.tar", last modified: Thu Jun  8 10:45:13 2023, max compression
```

## Comparing `solver4mpi-2.2.tar` & `solver4mpi-3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-05-25 01:21:31.314658 solver4mpi-2.2/
--rw-r--r--   0 mregnier   (501) staff       (20)      226 2023-05-25 01:21:31.314292 solver4mpi-2.2/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-05-25 01:20:51.000000 solver4mpi-2.2/README.md
--rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-05-25 01:21:31.314780 solver4mpi-2.2/setup.cfg
--rw-r--r--   0 mregnier   (501) staff       (20)      718 2023-05-25 01:21:22.000000 solver4mpi-2.2/setup.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-05-25 01:21:31.308509 solver4mpi-2.2/solver4mpi/
--rw-r--r--   0 mregnier   (501) staff       (20)       55 2023-05-25 01:20:51.000000 solver4mpi-2.2/solver4mpi/__init__.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2488 2023-05-25 01:20:51.000000 solver4mpi-2.2/solver4mpi/minimizer_multiprocess.py
--rw-r--r--   0 mregnier   (501) staff       (20)     1877 2023-05-25 01:20:51.000000 solver4mpi-2.2/solver4mpi/test.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-05-25 01:21:31.313785 solver4mpi-2.2/solver4mpi.egg-info/
--rw-r--r--   0 mregnier   (501) staff       (20)      226 2023-05-25 01:21:31.000000 solver4mpi-2.2/solver4mpi.egg-info/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)      266 2023-05-25 01:21:31.000000 solver4mpi-2.2/solver4mpi.egg-info/SOURCES.txt
--rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-05-25 01:21:31.000000 solver4mpi-2.2/solver4mpi.egg-info/dependency_links.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       13 2023-05-25 01:21:31.000000 solver4mpi-2.2/solver4mpi.egg-info/requires.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-05-25 01:21:31.000000 solver4mpi-2.2/solver4mpi.egg-info/top_level.txt
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 10:45:13.186433 solver4mpi-3.1/
+-rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-08 10:45:13.186303 solver4mpi-3.1/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.1/README.md
+-rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-08 10:45:13.186477 solver4mpi-3.1/setup.cfg
+-rw-r--r--   0 mregnier   (501) staff       (20)      738 2023-06-08 10:43:28.000000 solver4mpi-3.1/setup.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 10:45:13.183708 solver4mpi-3.1/solver4mpi/
+-rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.1/solver4mpi/__init__.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     3405 2023-06-08 10:41:31.000000 solver4mpi-3.1/solver4mpi/minimizer_multiprocess.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2120 2023-06-08 10:41:41.000000 solver4mpi-3.1/solver4mpi/test.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 10:45:13.186136 solver4mpi-3.1/solver4mpi.egg-info/
+-rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-08 10:45:13.000000 solver4mpi-3.1/solver4mpi.egg-info/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)      266 2023-06-08 10:45:13.000000 solver4mpi-3.1/solver4mpi.egg-info/SOURCES.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-08 10:45:13.000000 solver4mpi-3.1/solver4mpi.egg-info/dependency_links.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-08 10:45:13.000000 solver4mpi-3.1/solver4mpi.egg-info/requires.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-08 10:45:13.000000 solver4mpi-3.1/solver4mpi.egg-info/top_level.txt
```

### Comparing `solver4mpi-2.2/setup.py` & `solver4mpi-3.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     name='solver4mpi',
     url='https://github.com/mathias77515/optimized_minimizer',
     author='Mathias Regnier',
     author_email='mathias.p.regnier@gmail.com',
     # Needed to actually package something
     packages=find_packages(),
     # Needed for dependencies
-    install_requires=['multiprocess'],
+    install_requires=['scipy', 'pyoperators', 'numpy'],
     # *strongly* suggested for sharing
-    version='2.2',
+    version='3.1',
     # The license can be anything you like
     license='',
-    description='Optimized minimizer for MPI python.',
+    description='Optimized minimizer for MPI in python.',
     # We will also need a readme eventually (there will be a warning)
     # long_description=open('README.txt').read(),
 )
```

### Comparing `solver4mpi-2.2/solver4mpi/test.py` & `solver4mpi-3.1/solver4mpi/test.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 import matplotlib.pyplot as plt
 from minimizer_multiprocess import *
 import sys
 import time
 import pickle
 from functools import partial
 import os
+
 sys.path.append('/Users/mregnier/Desktop/Libs/qubic/qubic/scripts/MapMaking')
 
 import component_model as c
 import mixing_matrix as mm
 
 comm = MPI.COMM_WORLD
+size = comm.Get_size()
+rank = comm.Get_rank()
 
 def _scale_components_1pix(beta, ipix, mref, allnus):
 
     components = c.Dust(nu0=nu0, temp=20)
     A_ev = mm.MixingMatrix(components).evaluator(allnus)
     Aev = A_ev(beta)
     nf, nc = Aev.shape
@@ -33,37 +36,46 @@
 nu0 = 150
 mref = np.array(sky.get_emission(nu0 * u.GHz, None).T * utils.bandpass_unit_conversion(nu0*u.GHz, None, u.uK_CMB))
 
 
 allnus = np.array([140, 150, 160])
 m_nu = np.zeros((len(allnus), 12*nside**2, 3))
 
+beta = np.random.normal(1.54, 0.1, 12*nside**2)
 for j in range(12*nside**2):
-    m_nu[:, j, :] = _scale_components_1pix(np.array([1.54]), j, mref, allnus)
-
+    m_nu[:, j, :] = _scale_components_1pix(beta[j], j, mref, allnus)
 
 def chi2(x, ipix, mref, m_nu, allnus):
 
     #map_beta[ipix] = x
     m_nu_fake = _scale_components_1pix(x, ipix, mref, allnus)
     
     return np.sum((m_nu_fake - m_nu[:, ipix, :])**2)
 
-#val = chi2(np.array([1.54]), 0, A, mref, m_nu)
-nb_cpu = 2#os.cpu_count()
-index_beta = np.arange(0, 100, 1)
-
+index_beta = np.arange(0, 150, 1)
 
-#print(index_beta)
-#print(nb_cpu)
 chi2_partial = partial(chi2, mref=mref, m_nu=m_nu, allnus=allnus)
-#val = chi2_partial(np.array([1.54]), 0)
-#print(val)
-#beta_fit = FitMultiProcessCPU(comm, chi2_partial, nb_cpu, x0=np.ones(1), method='L-BFGS-B', tol=1e-3).perform(list(index_beta))
-#print(beta_fit)
+
+os.environ['OMP_NUM_THREADS'] = '8'
+
+if rank == 0:
+    start = time.time()
+    beta_i = WrapperCPU(chi2_partial, x0=np.ones(1), nproc=8, verbose=True, tol=1e-20, method='TNC').perform(list(index_beta))
+    end = time.time()
+    print(f'Execution time : {end - start} s')
+    print(f'Residuals :', beta_i[:5] - beta[:5])
+    print(f'estimated :', beta_i[:5])
+    print(f'true :', beta[:5])
+    print(f'Execution time : {end - start} s')
+
+
+
+
+#if comm.Get_rank() == 0:
+#    print(f'Execution time : {end - start} s')
+#    print(f'Residuals :', beta_est - beta[:5])
+#    print(f'estimated :', beta_est)
+#    print(f'true :', beta[:5])
 
 
-beta_est = WrapperMPI(comm, chi2_partial, nb_cpu, x0=np.ones(1), verbose=True).perform(index_beta)
-comm.Allreduce(MPI.IN_PLACE, beta_est, op=MPI.SUM)
-print(beta_est)
```

