# Comparing `tmp/solver4mpi-3.2.3.tar.gz` & `tmp/solver4mpi-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver4mpi-3.2.3.tar", last modified: Thu Jun  8 15:59:28 2023, max compression
+gzip compressed data, was "solver4mpi-3.2.4.tar", last modified: Thu Jun  8 16:19:09 2023, max compression
```

## Comparing `solver4mpi-3.2.3.tar` & `solver4mpi-3.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 15:59:28.328354 solver4mpi-3.2.3/
--rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-08 15:59:28.328049 solver4mpi-3.2.3/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.2.3/README.md
--rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-08 15:59:28.328448 solver4mpi-3.2.3/setup.cfg
--rw-r--r--   0 mregnier   (501) staff       (20)      740 2023-06-08 15:58:56.000000 solver4mpi-3.2.3/setup.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 15:59:28.322960 solver4mpi-3.2.3/solver4mpi/
--rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.2.3/solver4mpi/__init__.py
--rw-r--r--   0 mregnier   (501) staff       (20)     4630 2023-06-08 15:58:01.000000 solver4mpi-3.2.3/solver4mpi/minimizer_multiprocess.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.2.3/solver4mpi/test.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 15:59:28.327654 solver4mpi-3.2.3/solver4mpi.egg-info/
--rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-08 15:59:28.000000 solver4mpi-3.2.3/solver4mpi.egg-info/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)      266 2023-06-08 15:59:28.000000 solver4mpi-3.2.3/solver4mpi.egg-info/SOURCES.txt
--rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-08 15:59:28.000000 solver4mpi-3.2.3/solver4mpi.egg-info/dependency_links.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-08 15:59:28.000000 solver4mpi-3.2.3/solver4mpi.egg-info/requires.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-08 15:59:28.000000 solver4mpi-3.2.3/solver4mpi.egg-info/top_level.txt
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 16:19:09.272207 solver4mpi-3.2.4/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-08 16:19:09.271906 solver4mpi-3.2.4/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.2.4/README.md
+-rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-08 16:19:09.272306 solver4mpi-3.2.4/setup.cfg
+-rw-r--r--   0 mregnier   (501) staff       (20)      740 2023-06-08 16:18:42.000000 solver4mpi-3.2.4/setup.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 16:19:09.266778 solver4mpi-3.2.4/solver4mpi/
+-rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.2.4/solver4mpi/__init__.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     4631 2023-06-08 16:18:13.000000 solver4mpi-3.2.4/solver4mpi/minimizer_multiprocess.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.2.4/solver4mpi/test.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 16:19:09.271512 solver4mpi-3.2.4/solver4mpi.egg-info/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-08 16:19:09.000000 solver4mpi-3.2.4/solver4mpi.egg-info/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)      266 2023-06-08 16:19:09.000000 solver4mpi-3.2.4/solver4mpi.egg-info/SOURCES.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-08 16:19:09.000000 solver4mpi-3.2.4/solver4mpi.egg-info/dependency_links.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-08 16:19:09.000000 solver4mpi-3.2.4/solver4mpi.egg-info/requires.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-08 16:19:09.000000 solver4mpi-3.2.4/solver4mpi.egg-info/top_level.txt
```

### Comparing `solver4mpi-3.2.3/setup.py` & `solver4mpi-3.2.4/setup.py`

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
-    version='3.2.3',
+    version='3.2.4',
     # The license can be anything you like
     license='',
     description='Optimized minimizer for MPI in python.',
     # We will also need a readme eventually (there will be a warning)
     # long_description=open('README.txt').read(),
 )
```

### Comparing `solver4mpi-3.2.3/solver4mpi/minimizer_multiprocess.py` & `solver4mpi-3.2.4/solver4mpi/minimizer_multiprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
             wrap = WrapperCPU(chi2, x0, nproc=ncpu, method=method, tol=tol, options=options, verbose=False)
 
             results[ncpu*i:ncpu*(i+1)] = wrap.perform(x[ncpu*i:ncpu*(i+1)])
 
 
         if rest != 0:
-            wrap = WrapperCPU(chi2, x0, nproc=rest, method=method, tol=tol, options=options, verbose=False)
+            #wrap = WrapperCPU(chi2, x0, nproc=rest, method=method, tol=tol, options=options, verbose=False)
             results[-rest:] = wrap.perform(x[-rest:])
 
         end = time.time()
 
         if verbose:
             print(f'Estimation done on {x.shape[0]} parameters in {end - start} s')
```

### Comparing `solver4mpi-3.2.3/solver4mpi/test.py` & `solver4mpi-3.2.4/solver4mpi/test.py`

 * *Files identical despite different names*

