# Comparing `tmp/sphecerix-0.2.1-py3-none-any.whl.zip` & `tmp/sphecerix-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6275 bytes, number of entries: 9
--rw-r--r--  2.0 unx      219 b- defN 23-Jun-03 12:02 sphecerix/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-03 12:02 sphecerix/_version.py
--rw-r--r--  2.0 unx     3394 b- defN 23-Jun-03 12:02 sphecerix/atomic_wave_functions.py
--rw-r--r--  2.0 unx     1220 b- defN 23-Jun-03 12:02 sphecerix/tesseral.py
--rw-r--r--  2.0 unx     5712 b- defN 23-Jun-03 12:02 sphecerix/wignerd.py
--rw-r--r--  2.0 unx     2873 b- defN 23-Jun-03 12:02 sphecerix-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 12:02 sphecerix-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-03 12:02 sphecerix-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      705 b- defN 23-Jun-03 12:02 sphecerix-0.2.1.dist-info/RECORD
-9 files, 14246 bytes uncompressed, 5063 bytes compressed:  64.5%
+Zip file size: 6717 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      245 b- defN 23-Jun-08 19:14 sphecerix/__init__.py
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-08 19:14 sphecerix/_version.py
+-rw-r--r--  2.0 unx     3394 b- defN 23-Jun-08 19:14 sphecerix/atomic_wave_functions.py
+-rw-r--r--  2.0 unx     1220 b- defN 23-Jun-08 19:14 sphecerix/tesseral.py
+-rw-r--r--  2.0 unx     7925 b- defN 23-Jun-08 19:14 sphecerix/wignerd.py
+-rw-r--r--  2.0 unx     2873 b- defN 23-Jun-08 19:14 sphecerix-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 19:14 sphecerix-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-08 19:14 sphecerix-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      705 b- defN 23-Jun-08 19:14 sphecerix-0.3.0.dist-info/RECORD
+9 files, 16485 bytes uncompressed, 5505 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: sphecerix/tesseral.py
 Comment: 
 
 Filename: sphecerix/wignerd.py
 Comment: 
 
-Filename: sphecerix-0.2.1.dist-info/METADATA
+Filename: sphecerix-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: sphecerix-0.2.1.dist-info/WHEEL
+Filename: sphecerix-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: sphecerix-0.2.1.dist-info/top_level.txt
+Filename: sphecerix-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sphecerix-0.2.1.dist-info/RECORD
+Filename: sphecerix-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sphecerix/__init__.py

```diff
@@ -1,5 +1,5 @@
-from .wignerd import tesseral_wigner_D, wigner_D
+from .wignerd import tesseral_wigner_D, wigner_D, tesseral_wigner_D_mirror
 from .tesseral import tesseral_transformation, permutation_sh_car
 from .atomic_wave_functions import wfcart, wf, wffield, wffield_l
 
 from ._version import __version__
```

## sphecerix/_version.py

```diff
@@ -1 +1 @@
-__version__ = "0.2.1"
+__version__ = "0.3.0"
```

## sphecerix/wignerd.py

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 from scipy.special import factorial
 from scipy.spatial.transform import Rotation as R
 from .tesseral import tesseral_transformation
+import warnings
 
 def tesseral_wigner_D(l, Robj):
     """
     Produce the Wigner D-matrix for tesseral spherical harmonics
 
     Parameters
     ----------
@@ -25,25 +26,25 @@
     ------
     TypeError
         If the Robj object is not of type scipy.spatial.transform.R.
 
     Examples
     --------
     >>> from sphecerix import tesseral_wigner_D
-    >>> from scipy.spatial.transform import Rotation as R
-    >>> import numpy as np
-    >>> 
-    >>> # build rotation axis and set angle
-    >>> axis = np.ones(3) / np.sqrt(3)
-    >>> angle = np.pi
-    >>> Robj = R.from_rotvec(axis * angle)
-    >>> 
-    >>> # construct tesseral Wigner D matrix
-    >>> D = tesseral_wigner_D(2, Robj)
-    >>> print(D)
+    ... from scipy.spatial.transform import Rotation as R
+    ... import numpy as np
+    ...
+    ... # build rotation axis and set angle
+    ... axis = np.ones(3) / np.sqrt(3)
+    ... angle = np.pi
+    ... Robj = R.from_rotvec(axis * angle)
+    ...
+    ... # construct tesseral Wigner D matrix
+    ... D = tesseral_wigner_D(2, Robj)
+    ... print(D)
     [[ 5.55555556e-01  2.22222222e-01  7.69800359e-01  2.22222222e-01
        1.89744731e-16]
      [ 2.22222222e-01  5.55555556e-01 -3.84900179e-01  2.22222222e-01
        6.66666667e-01]
      [ 7.69800359e-01 -3.84900179e-01 -3.33333333e-01 -3.84900179e-01
        5.42310034e-16]
      [ 2.22222222e-01  2.22222222e-01 -3.84900179e-01  5.55555556e-01
@@ -56,19 +57,76 @@
 
     """
     # verify that Robj is a rotation object
     if not isinstance(Robj, R):
         raise TypeError('Second argument Robj should be of type scipy.spatial.transform.R')
     
     T = tesseral_transformation(l)
-    alpha, beta, gamma = Robj.as_euler('zyz', degrees=False)
+    with warnings.catch_warnings():
+        warnings.filterwarnings('ignore', r'Gimbal lock detected. Setting third angle to zero since it is not possible to uniquely determine all angles.')
+        alpha, beta, gamma = Robj.as_euler('zyz', degrees=False)
+        
     D = wigner_D(l, Robj)
     
     return np.real(T @ D @ T.conjugate().transpose())
 
+def tesseral_wigner_D_mirror(l, normal):
+    """
+    Produce the Wigner D-matrix for tesseral spherical harmonics for a mirror operation
+
+    Parameters
+    ----------
+    l : int
+        Order of the spherical harmonics
+    normal : np.array
+        Normal vector
+
+    Returns
+    -------
+    D : numpy.ndarray
+        Real-valued Wigner-D matrix with dimensions :math:`(2l+1) \\times (2l+1)`
+
+    Examples
+    --------
+    >>> from sphecerix import tesseral_wigner_D_mirror
+    ... import numpy as np
+    ... 
+    ... # construct mirror normal vector
+    ... normal = np.array([-1,1,0]) / np.sqrt(2)
+    ... 
+    ... # construct wigner D matrix
+    ... D = tesseral_wigner_D_mirror(1, normal)
+    ... 
+    ... print(D)
+    [[-2.83276945e-16 -0.00000000e+00  1.00000000e+00]
+     [ 1.22464680e-16  1.00000000e+00  3.46914204e-32]
+     [ 1.00000000e+00 -1.22464680e-16  2.83276945e-16]]
+
+    Construct the Wigner-D matrix for the tesseral p-orbitals for a mirror
+    operation with the mirror plane corresponding to the xz plane rotated
+    around the z-axis by 45 degrees.
+
+    """    
+    # construct mirror matrix
+    normal /= np.linalg.norm(normal) # ensure normalization
+    M = np.identity(3) - 2 * np.outer(normal, normal)
+    
+    # decompose mirror operation into a rotation and an inversion
+    Robj = R.from_matrix(-M)
+    inv = (-1)**l
+    
+    T = tesseral_transformation(l)
+    with warnings.catch_warnings():
+        warnings.filterwarnings('ignore', r'Gimbal lock detected. Setting third angle to zero since it is not possible to uniquely determine all angles.')
+        alpha, beta, gamma = Robj.as_euler('zyz', degrees=False)
+        
+    D = wigner_D(l, Robj)
+    
+    return inv * np.real(T @ D @ T.conjugate().transpose())
+
 def wigner_D(l, Robj):
     """
     Produce Wigner D-matrix for canonical spherical harmonics
 
     Parameters
     ----------
     l : int
@@ -85,25 +143,25 @@
     ------
     TypeError
         If the Robj object is not of type scipy.spatial.transform.R. 
 
     Examples
     --------
     >>> from sphecerix import wigner_D
-    >>> from scipy.spatial.transform import Rotation as R
-    >>> import numpy as np
-    >>> 
-    >>> # build rotation axis and set angle
-    >>> axis = np.ones(3) / np.sqrt(3)
-    >>> angle = np.pi
-    >>> Robj = R.from_rotvec(axis * angle)
-    >>> 
-    >>> # construct tesseral Wigner D matrix
-    >>> D = wigner_D(2, Robj)
-    >>> print(D)
+    ... from scipy.spatial.transform import Rotation as R
+    ... import numpy as np
+    ...
+    ... # build rotation axis and set angle
+    ... axis = np.ones(3) / np.sqrt(3)
+    ... angle = np.pi
+    ... Robj = R.from_rotvec(axis * angle)
+    ...
+    ... # construct tesseral Wigner D matrix
+    ... D = wigner_D(2, Robj)
+    ... print(D)
     [[ 1.11111111e-01-1.45486986e-16j -2.22222222e-01+2.22222222e-01j
       -3.29266657e-16-5.44331054e-01j  4.44444444e-01+4.44444444e-01j
       -4.44444444e-01-4.42577444e-17j]
      [-2.22222222e-01-2.22222222e-01j  5.55555556e-01-3.33066907e-16j
       -2.72165527e-01+2.72165527e-01j -5.55111512e-17+2.22222222e-01j
       -4.44444444e-01-4.44444444e-01j]
      [ 3.83471103e-16+5.44331054e-01j -2.72165527e-01-2.72165527e-01j
@@ -120,22 +178,24 @@
     the :math:`\\frac{1}{\\sqrt{3}}(1,1,1)` axis by an angle :math:`\\pi`.
 
     """
     # verify that Robj is a rotation object
     if not isinstance(Robj, R):
         raise TypeError('Second argument Robj should be of type scipy.spatial.transform.R')
 
-    alpha, beta, gamma = Robj.as_euler('zyz', degrees=False)
+    with warnings.catch_warnings():
+        warnings.filterwarnings('ignore', r'Gimbal lock detected. Setting third angle to zero since it is not possible to uniquely determine all angles.')
+        alpha, beta, gamma = Robj.as_euler('zyz', degrees=False)
     d = wigner_d(l, beta)
     m = np.arange(-l, l+1)
     diag_alpha = np.diag(np.exp(1j * m * alpha))
     diag_gamma = np.diag(np.exp(1j * m * gamma))
     
     return diag_gamma @ d @ diag_alpha
-    
+
 def wigner_d(l, beta):
     """
     Produce Wigner (small) d-matrix for order l of spherical harmonics and
     euler angles
     """
     d = np.zeros((2*l+1,2*l+1))
     for i,m1 in enumerate(range(-l,l+1)):
```

## Comparing `sphecerix-0.2.1.dist-info/METADATA` & `sphecerix-0.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphecerix
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python package for constructing Wigner-D matrices
 Home-page: https://github.com/ifilot/sphecerix
 Author: Ivo Filot
 Author-email: ivo@ivofilot.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

## Comparing `sphecerix-0.2.1.dist-info/RECORD` & `sphecerix-0.3.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-sphecerix/__init__.py,sha256=Qq3BOzEm_wsbEA4Shsh5qz7nDqIl82OxlUtcVCMU078,219
-sphecerix/_version.py,sha256=tC9CwL4Nm8brVXJnZNGk_eoZaJj6eOtLKtOrdJMrpoI,21
+sphecerix/__init__.py,sha256=lipL0Aw7iVa-ngZmDHwCi08E1bUYwa4mhvheRrQAK7o,245
+sphecerix/_version.py,sha256=5mDtfU2t04ATmg92S5B-scUcdjCy1ZBq620y3GmpdtQ,21
 sphecerix/atomic_wave_functions.py,sha256=VO9_8spYmPvTbRncdG9aPMzjkA3qFTj6jUTJIsOyER0,3394
 sphecerix/tesseral.py,sha256=7ak1E_tsT5IMavEVyNqaNtY64jUdfuecl8IZr2M9Rfc,1220
-sphecerix/wignerd.py,sha256=MXUOTd1cLyc17I522eaLO75plalRGauIzkRFCI-FmNk,5712
-sphecerix-0.2.1.dist-info/METADATA,sha256=IM2bIOfyc913ibBmQGfho022xodFIkGBn4Iu-XKIL-k,2873
-sphecerix-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sphecerix-0.2.1.dist-info/top_level.txt,sha256=wx-xiducfOhrGJk9tdcB7P1x6P0oMB-LilN7vRs4-rs,10
-sphecerix-0.2.1.dist-info/RECORD,,
+sphecerix/wignerd.py,sha256=s4_KBs4KK6z71OKQt667cutcO07wPjVMe13tkrXyHU8,7925
+sphecerix-0.3.0.dist-info/METADATA,sha256=q-kccg3I1DLfrJhzQLe6bk6sFUgN-_q__KtnU185tvQ,2873
+sphecerix-0.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sphecerix-0.3.0.dist-info/top_level.txt,sha256=wx-xiducfOhrGJk9tdcB7P1x6P0oMB-LilN7vRs4-rs,10
+sphecerix-0.3.0.dist-info/RECORD,,
```

