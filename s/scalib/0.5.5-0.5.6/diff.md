# Comparing `tmp/scalib-0.5.5.tar.gz` & `tmp/scalib-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalib-0.5.5.tar", last modified: Tue May 30 11:22:27 2023, max compression
+gzip compressed data, was "scalib-0.5.6.tar", last modified: Thu Jun  8 10:35:09 2023, max compression
```

## Comparing `scalib-0.5.5.tar` & `scalib-0.5.6.tar`

### file list

```diff
@@ -1,575 +1,585 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.046273 scalib-0.5.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.982273 scalib-0.5.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.990273 scalib-0.5.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-30 11:22:17.000000 scalib-0.5.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-30 11:22:17.000000 scalib-0.5.5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.990273 scalib-0.5.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-05-30 11:22:17.000000 scalib-0.5.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-30 11:22:17.000000 scalib-0.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-30 11:22:17.000000 scalib-0.5.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-30 11:22:17.000000 scalib-0.5.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-30 11:22:17.000000 scalib-0.5.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-30 11:22:17.000000 scalib-0.5.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-30 11:22:17.000000 scalib-0.5.5/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-30 11:22:17.000000 scalib-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-30 11:22:17.000000 scalib-0.5.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-30 11:22:27.046273 scalib-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-30 11:22:17.000000 scalib-0.5.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.990273 scalib-0.5.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.982273 scalib-0.5.5/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.990273 scalib-0.5.5/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.990273 scalib-0.5.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 11:22:17.000000 scalib-0.5.5/docs/source/copyright.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-30 11:22:17.000000 scalib-0.5.5/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-30 11:22:17.000000 scalib-0.5.5/examples/aes_attack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-30 11:22:17.000000 scalib-0.5.5/examples/aes_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-30 11:22:17.000000 scalib-0.5.5/examples/aes_tvla.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-30 11:22:17.000000 scalib-0.5.5/examples/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-30 11:22:17.000000 scalib-0.5.5/examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/paper/
--rwxr-xr-x   0 runner    (1001) docker     (123)      111 2023-05-30 11:22:17.000000 scalib-0.5.5/paper/build_paper.sh
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-05-30 11:22:17.000000 scalib-0.5.5/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-05-30 11:22:17.000000 scalib-0.5.5/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-30 11:22:17.000000 scalib-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-30 11:22:27.046273 scalib-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-30 11:22:17.000000 scalib-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.986273 scalib-0.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/src/scalib/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/src/scalib/attacks/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/attacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/attacks/factor_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    24799 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/attacks/sascagraph.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib/build_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/src/scalib/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/config/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/src/scalib/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/metrics/snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/metrics/ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/src/scalib/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/modeling/ldaclassifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/src/scalib/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/postprocessing/rankestimation.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.994273 scalib-0.5.5/src/scalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27051 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 11:22:26.000000 scalib-0.5.5/src/scalib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.998273 scalib-0.5.5/src/scalib_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    45960 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.998273 scalib-0.5.5/src/scalib_ext/geigen/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.998273 scalib-0.5.5/src/scalib_ext/geigen/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.998273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Cholesky
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/CholmodSupport
--rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Core
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Dense
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Eigen
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Eigenvalues
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Geometry
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Householder
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Jacobi
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/LU
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/MetisSupport
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/OrderingMethods
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/PaStiXSupport
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/PardisoSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/QR
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SPQRSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SVD
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Sparse
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseCholesky
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseCore
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseLU
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseQR
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/StdDeque
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/StdList
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/StdVector
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SuperLUSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/UmfPackSupport
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.986273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.002273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Cholesky/
--rw-r--r--   0 runner    (1001) docker     (123)    24480 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.002273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    12479 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner    (1001) docker     (123)    62197 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    31424 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner    (1001) docker     (123)    27551 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    24212 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h
--rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    41000 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    23276 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner    (1001) docker     (123)    20694 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    45354 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h
--rw-r--r--   0 runner    (1001) docker     (123)    51070 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h
--rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h
--rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner    (1001) docker     (123)    37304 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner    (1001) docker     (123)    29441 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:26.986273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    27841 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    50865 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    37671 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    23547 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    35476 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (123)    17706 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    28726 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    35843 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    32283 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.010273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    18263 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    27946 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.014273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/
--rw-r--r--   0 runner    (1001) docker     (123)    81646 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (123)    18887 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    26808 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.014273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/
--rwxr-xr-x   0 runner    (1001) docker     (123)    19307 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4360 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4026 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner    (1001) docker     (123)    38322 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner    (1001) docker     (123)    40579 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    21356 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner    (1001) docker     (123)    34903 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.018273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    22944 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    33705 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    22444 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.018273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 runner    (1001) docker     (123)    32704 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 runner    (1001) docker     (123)    60555 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.018273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.018273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Householder/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h
--rw-r--r--   0 runner    (1001) docker     (123)    20603 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Jacobi/
--rw-r--r--   0 runner    (1001) docker     (123)    15902 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h
--rw-r--r--   0 runner    (1001) docker     (123)    32803 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    21538 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/arch/
--rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/
--rw-r--r--   0 runner    (1001) docker     (123)    16396 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 runner    (1001) docker     (123)    62266 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    22248 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    20060 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    20805 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (123)    25478 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/
--rw-r--r--   0 runner    (1001) docker     (123)    49870 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 runner    (1001) docker     (123)    32949 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.022273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/
--rw-r--r--   0 runner    (1001) docker     (123)    24017 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.026273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 runner    (1001) docker     (123)    25592 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    12487 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 runner    (1001) docker     (123)    52401 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 runner    (1001) docker     (123)    25721 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.030273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/
--rw-r--r--   0 runner    (1001) docker     (123)    27844 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.030273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseQR/
--rw-r--r--   0 runner    (1001) docker     (123)    28373 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.030273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.030273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    34345 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.030273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.030273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 runner    (1001) docker     (123)    30560 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h
--rwxr-xr-x   0 runner    (1001) docker     (123)  1058368 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.034273 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    16929 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    37403 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.034273 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.034273 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h
--rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h
--rw-r--r--   0 runner    (1001) docker     (123)    14768 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    28001 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/Version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/include/geigen.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/geigen/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/src/geigen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/src/geigen.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/geigen/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/ranklib/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/ranklib/fuzz/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/fuzz/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/fuzz/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.038273 scalib-0.5.5/src/scalib_ext/ranklib/fuzz/fuzz_targets/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.042273 scalib-0.5.5/src/scalib_ext/ranklib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/aes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/aes.h
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/bignumpoly.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/bignumpoly.h
--rw-r--r--   0 runner    (1001) docker     (123)    22744 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_enum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_enum.h
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_execute.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_execute.h
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_histo.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_histo.h
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_if.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_if.h
--rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_init.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_init.h
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_struct.h
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_util.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/hel_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/histogram.rs
--rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16237 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/main_example.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/rank.rs
--rw-r--r--   0 runner    (1001) docker     (123)   274225 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/score_example_data.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/scores_example.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/scores_example.h
--rw-r--r--   0 runner    (1001) docker     (123)   224884 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/scores_example_data.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/ranklib/src/top.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.042273 scalib-0.5.5/src/scalib_ext/scalib/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.042273 scalib-0.5.5/src/scalib_ext/scalib/benches/
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/benches/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/benches/get_snr.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/benches/mttest.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/benches/snr_update.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/benches/ttest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.046273 scalib-0.5.5/src/scalib_ext/scalib/src/
--rw-r--r--   0 runner    (1001) docker     (123)    24746 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/lda.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/matrixmul.rs
--rw-r--r--   0 runner    (1001) docker     (123)    25704 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/mttest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.046273 scalib-0.5.5/src/scalib_ext/scalib/src/sasca/
--rw-r--r--   0 runner    (1001) docker     (123)    26307 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/sasca/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/sasca/bp_compute.rs
--rw-r--r--   0 runner    (1001) docker     (123)    13668 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/sasca/factor_graph.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/sasca/fg_build.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/sasca/fg_parser.rs
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/sasca/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    18507 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/snr.rs
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/ttest.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/src/utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.046273 scalib-0.5.5/src/scalib_ext/scalib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/tests/lda.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/tests/multivarcs.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib/tests/ttest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.042273 scalib-0.5.5/src/scalib_ext/scalib-py/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.042273 scalib-0.5.5/src/scalib_ext/scalib-py/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/factor_graph.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/lda.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/ranking.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/snr.rs
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/thread_pool.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-30 11:22:17.000000 scalib-0.5.5/src/scalib_ext/scalib-py/src/ttest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.046273 scalib-0.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/mttest_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/test_factorgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/test_lda.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/test_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/test_sascagraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/test_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-30 11:22:17.000000 scalib-0.5.5/tests/test_ttest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-30 11:22:17.000000 scalib-0.5.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.715186 scalib-0.5.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.615186 scalib-0.5.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.627186 scalib-0.5.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-08 10:34:53.000000 scalib-0.5.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-08 10:34:53.000000 scalib-0.5.6/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.627186 scalib-0.5.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-06-08 10:34:53.000000 scalib-0.5.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-08 10:34:53.000000 scalib-0.5.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-08 10:34:53.000000 scalib-0.5.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-08 10:34:53.000000 scalib-0.5.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-08 10:34:53.000000 scalib-0.5.6/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-08 10:34:53.000000 scalib-0.5.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-08 10:34:53.000000 scalib-0.5.6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-08 10:34:53.000000 scalib-0.5.6/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-08 10:34:53.000000 scalib-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-08 10:34:53.000000 scalib-0.5.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-08 10:35:09.715186 scalib-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-08 10:34:53.000000 scalib-0.5.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.627186 scalib-0.5.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-08 10:34:53.000000 scalib-0.5.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.615186 scalib-0.5.6/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.627186 scalib-0.5.6/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-08 10:34:53.000000 scalib-0.5.6/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-08 10:34:53.000000 scalib-0.5.6/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-08 10:34:53.000000 scalib-0.5.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-08 10:34:53.000000 scalib-0.5.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-08 10:34:53.000000 scalib-0.5.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-08 10:34:53.000000 scalib-0.5.6/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-08 10:34:53.000000 scalib-0.5.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.627186 scalib-0.5.6/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-08 10:34:53.000000 scalib-0.5.6/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-08 10:34:53.000000 scalib-0.5.6/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 10:34:53.000000 scalib-0.5.6/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-08 10:34:53.000000 scalib-0.5.6/docs/source/copyright.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-08 10:34:53.000000 scalib-0.5.6/docs/source/papers.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.631186 scalib-0.5.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-08 10:34:53.000000 scalib-0.5.6/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-08 10:34:53.000000 scalib-0.5.6/examples/aes_attack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-08 10:34:53.000000 scalib-0.5.6/examples/aes_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-08 10:34:53.000000 scalib-0.5.6/examples/aes_tvla.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-08 10:34:53.000000 scalib-0.5.6/examples/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-08 10:34:53.000000 scalib-0.5.6/examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.631186 scalib-0.5.6/paper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      111 2023-06-08 10:34:53.000000 scalib-0.5.6/paper/build_paper.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-06-08 10:34:53.000000 scalib-0.5.6/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-06-08 10:34:53.000000 scalib-0.5.6/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-08 10:34:53.000000 scalib-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-08 10:35:09.715186 scalib-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-08 10:34:53.000000 scalib-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.615186 scalib-0.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.631186 scalib-0.5.6/src/scalib/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.631186 scalib-0.5.6/src/scalib/attacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/attacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/attacks/factor_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24799 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/attacks/sascagraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 10:35:09.000000 scalib-0.5.6/src/scalib/build_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.631186 scalib-0.5.6/src/scalib/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/config/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.635186 scalib-0.5.6/src/scalib/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/metrics/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/metrics/snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/metrics/ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.635186 scalib-0.5.6/src/scalib/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/modeling/ldaclassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/modeling/rldaclassifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.635186 scalib-0.5.6/src/scalib/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/postprocessing/rankestimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 10:35:09.000000 scalib-0.5.6/src/scalib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.631186 scalib-0.5.6/src/scalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-08 10:35:09.000000 scalib-0.5.6/src/scalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27348 2023-06-08 10:35:09.000000 scalib-0.5.6/src/scalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:35:09.000000 scalib-0.5.6/src/scalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:35:09.000000 scalib-0.5.6/src/scalib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 10:35:09.000000 scalib-0.5.6/src/scalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 10:35:09.000000 scalib-0.5.6/src/scalib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.635186 scalib-0.5.6/src/scalib_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    45613 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.635186 scalib-0.5.6/src/scalib_ext/geigen/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.635186 scalib-0.5.6/src/scalib_ext/geigen/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.639186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Cholesky
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/CholmodSupport
+-rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Core
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Dense
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Eigen
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Eigenvalues
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Geometry
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Householder
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Jacobi
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/LU
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/MetisSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/OrderingMethods
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/PaStiXSupport
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/PardisoSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/QR
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/SPQRSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/SVD
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Sparse
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/SparseCholesky
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/SparseCore
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/SparseLU
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/SparseQR
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/StdDeque
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/StdList
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/StdVector
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/SuperLUSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/UmfPackSupport
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.623185 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.639186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Cholesky/
+-rw-r--r--   0 runner    (1001) docker     (123)    24480 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.639186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.655186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12479 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    62197 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31424 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27551 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24212 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41000 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23276 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20694 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45354 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51070 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37304 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29441 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.619186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.655186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27841 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.655186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    50865 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.655186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37671 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.655186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23547 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35476 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.655186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.659186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (123)    17706 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28726 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.659186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35843 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.659186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32283 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.659186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/functors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18263 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27946 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.663186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/
+-rw-r--r--   0 runner    (1001) docker     (123)    81646 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18887 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26808 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.667186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19307 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4360 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4026 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38322 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40579 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21356 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34903 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.667186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22944 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33705 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22444 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.671186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32704 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 runner    (1001) docker     (123)    60555 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.671186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.671186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Householder/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20603 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.675186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.675186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Jacobi/
+-rw-r--r--   0 runner    (1001) docker     (123)    15902 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.675186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/LU/
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32803 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21538 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.675186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/LU/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.675186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.675186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/
+-rw-r--r--   0 runner    (1001) docker     (123)    16396 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    62266 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.675186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    22248 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.675186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    20060 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.679186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/QR/
+-rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20805 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25478 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.679186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.679186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SVD/
+-rw-r--r--   0 runner    (1001) docker     (123)    49870 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32949 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.679186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/
+-rw-r--r--   0 runner    (1001) docker     (123)    24017 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.683186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25592 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12487 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52401 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25721 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.687186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/
+-rw-r--r--   0 runner    (1001) docker     (123)    27844 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.687186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseQR/
+-rw-r--r--   0 runner    (1001) docker     (123)    28373 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.687186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/StlSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.687186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    34345 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.687186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.691186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30560 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1058368 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.691186 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16929 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37403 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.695186 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.695186 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14768 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28001 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.699186 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.699186 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.699186 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/Util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/Util/Version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.699186 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/include/geigen.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.699186 scalib-0.5.6/src/scalib_ext/geigen/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/src/geigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/src/geigen.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/geigen/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.703186 scalib-0.5.6/src/scalib_ext/ranklib/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.703186 scalib-0.5.6/src/scalib_ext/ranklib/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/fuzz/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/fuzz/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.703186 scalib-0.5.6/src/scalib_ext/ranklib/fuzz/fuzz_targets/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.707186 scalib-0.5.6/src/scalib_ext/ranklib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/aes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/aes.h
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/bignumpoly.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/bignumpoly.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22744 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/hel_enum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/hel_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/hel_execute.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/hel_execute.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/hel_histo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/hel_histo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/hel_if.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/hel_if.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/hel_init.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/hel_init.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/hel_struct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/hel_util.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/hel_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/histogram.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16237 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/main_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/rank.rs
+-rw-r--r--   0 runner    (1001) docker     (123)   274225 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/score_example_data.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/scores_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/scores_example.h
+-rw-r--r--   0 runner    (1001) docker     (123)   224884 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/scores_example_data.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/ranklib/src/top.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.707186 scalib-0.5.6/src/scalib_ext/scalib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.711186 scalib-0.5.6/src/scalib_ext/scalib/benches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/benches/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/benches/get_snr.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/benches/mttest.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/benches/snr_update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/benches/ttest.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.711186 scalib-0.5.6/src/scalib_ext/scalib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    24746 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/information.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/lda.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/matrixmul.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    25704 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/mttest.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    30637 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/rlda.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.711186 scalib-0.5.6/src/scalib_ext/scalib/src/sasca/
+-rw-r--r--   0 runner    (1001) docker     (123)    26307 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/sasca/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/sasca/bp_compute.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    13668 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/sasca/factor_graph.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/sasca/fg_build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/sasca/fg_parser.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/sasca/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    18507 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/snr.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/ttest.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/src/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.711186 scalib-0.5.6/src/scalib_ext/scalib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/tests/lda.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/tests/multivarcs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib/tests/ttest.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.707186 scalib-0.5.6/src/scalib_ext/scalib-py/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib-py/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.707186 scalib-0.5.6/src/scalib_ext/scalib-py/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib-py/src/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib-py/src/factor_graph.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib-py/src/information.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib-py/src/lda.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib-py/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib-py/src/ranking.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib-py/src/rlda.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib-py/src/snr.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib-py/src/thread_pool.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-08 10:34:53.000000 scalib-0.5.6/src/scalib_ext/scalib-py/src/ttest.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:35:09.715186 scalib-0.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-08 10:34:53.000000 scalib-0.5.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-08 10:34:53.000000 scalib-0.5.6/tests/mttest_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 10:34:53.000000 scalib-0.5.6/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-06-08 10:34:53.000000 scalib-0.5.6/tests/test_factorgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-06-08 10:34:53.000000 scalib-0.5.6/tests/test_lda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-08 10:34:53.000000 scalib-0.5.6/tests/test_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-08 10:34:53.000000 scalib-0.5.6/tests/test_rlda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-06-08 10:34:53.000000 scalib-0.5.6/tests/test_sascagraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-08 10:34:53.000000 scalib-0.5.6/tests/test_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-08 10:34:53.000000 scalib-0.5.6/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-08 10:34:53.000000 scalib-0.5.6/tests/test_ttest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-08 10:34:53.000000 scalib-0.5.6/tox.ini
```

### Comparing `scalib-0.5.5/.github/ISSUE_TEMPLATE/bug_report.md` & `scalib-0.5.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/.github/ISSUE_TEMPLATE/feature_request.md` & `scalib-0.5.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/.github/workflows/ci.yml` & `scalib-0.5.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/CHANGELOG.rst` & `scalib-0.5.6/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 =========
 Changelog
 =========
 
 Not released
 ------------
 
+v0.5.6 (2023/06/08)
+-------------------
+
+* Add ``scalib.modeling.RLDAClassifier`` and ``scalib.metrics.RLDAInformationEstimator``.
+* Fix build dependences and run build in an isolated environment.
+
 v0.5.5 (2023/05/30)
 -------------------
 
 * Fix ``Distribution`` size bug in belief propagation computation (#102).
 * Do not include debug symbols in release builds (makes wheel much smaller).
 * ``Ttest``: do not crash on non-contiguous/fortran-order arrays
 * Improve examples and README
@@ -148,12 +154,12 @@
 
 * Fix "invalid instruction" bug for CI wheel on windows.
 
 v0.1.0 (2021/04/16)
 -------------------
 
 * Initial release, with the following features:
-  * LDA and Gaussian templates modelling
+  * LDA and Gaussian templates modeling
   * SNR
   * T-test any order (for TLVA)
   * Soft Analytical Side-Channel Attack (SASCA)
   * Rank Estimation
```

### Comparing `scalib-0.5.5/CONTRIBUTING.rst` & `scalib-0.5.6/CONTRIBUTING.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ------------
 
 The minimum dependencies for building SCALib are
 
 - A C/C++ compiler.
 - The latest stable release of the `rust toolchain <https://rustup.rs/>`_.
 - Python (see ``setup.cfg`` for supported versions).
-- :code:`pip`
+- The PyPI :code:`build` package.
 
 Moreover, for development, we use
 
 - `tox <https://pypi.org/project/tox>`_
 - :code:`make` (optional)
 
 Development commands
@@ -32,14 +32,16 @@
     make help
 
 Build wheels
 ------------
 
 If you need to get wheels (e.g. to install elsewhere), you can simply
 use ``make wheel_local``, ``make wheel_avx2`` or ``make wheel_portable``.
+(See the content of ``Makefile`` if you cannot use ``make``.)
+The wheels are stored in ``dist/``.
 
 
 Development flow
 ----------------
 
 Multiple builds with misc. trade-offs can be used, depending on what you are working on:
```

### Comparing `scalib-0.5.5/COPYING` & `scalib-0.5.6/COPYING`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/COPYRIGHT` & `scalib-0.5.6/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/MANIFEST.in` & `scalib-0.5.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/Makefile` & `scalib-0.5.6/Makefile`

 * *Files 19% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 codestyle:
 	tox run -e fmt -- --check
 
 fmt:
 	tox run -e fmt
 
 wheel_avx2:
-	SCALIB_AVX2=1 CARGO_TARGET_DIR=.cargo_build_avx2 pip wheel . --no-deps
+	SCALIB_AVX2=1 CARGO_TARGET_DIR=.cargo_build_avx2 python3 -m build -w -o dist/avx2
 
 wheel_local:
-	CARGO_TARGET_DIR=.cargo_build pip wheel . --no-deps
+	CARGO_TARGET_DIR=.cargo_build python3 -m build -w -o dist/local
 
 wheel_portable:
-	SCALIB_PORTABLE=1 CARGO_TARGET_DIR=.cargo_build_portable pip wheel . --no-deps
-
+	SCALIB_PORTABLE=1 CARGO_TARGET_DIR=.cargo_build_portable  python3 -m build -w -o dist/portable
```

### Comparing `scalib-0.5.5/PKG-INFO` & `scalib-0.5.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalib
-Version: 0.5.5
+Version: 0.5.6
 Summary: Side-Channel Analysis Library
 Home-page: https://github.com/simple-crypto/scalib
 Author: Olivier Bronchain, Gaëtan Cassiers
 Author-email: olivier.bronchain@uclouvain.be, gaetan.cassiers@uclouvain.be
 License: GNU AGPL v3+
 Project-URL: Bug Tracker, https://github.com/simple-crypto/scalib/issues
 Requires-Python: >=3.8
@@ -20,14 +20,17 @@
     :alt: PyPI
 .. image:: https://readthedocs.org/projects/scalib/badge/?version=stable
     :target: https://scalib.readthedocs.io/en/stable/
     :alt: Documentation Status
 .. image:: https://img.shields.io/matrix/scalib:matrix.org
     :target: https://matrix.to/#/#scalib:matrix.org
     :alt: Matrix room
+.. image:: https://joss.theoj.org/papers/10.21105/joss.05196/status.svg
+   :target: https://doi.org/10.21105/joss.05196
+   :alt: JOSS paper
 
 The Side-Channel Analysis Library (SCALib) is a Python library that
 contains state-of-the-art tools for side-channel security evaluation.
 
 - **Documentation**: https://scalib.readthedocs.io/
 - **Examples**: `examples/ <examples/>`_
 - **Chat**: `https://matrix.to/#/#scalib:matrix.org`
@@ -124,14 +127,41 @@
 You can also come discuss on `matrix <https://matrix.to/#/#scalib:matrix.org>`_
 (announcements, questions, community support, open discussion, etc.).
 
 All code contributions are subject to the Contributor License Agreement (`CLA
 <https://www.simple-crypto.dev/organization>`_) of SIMPLE-Crypto, which ensures
 a thriving future for open-source hardware security.
 
+
+Citation
+========
+
+If you use SCALib in your research, please cite our `software paper <https://doi.org/10.21105/joss.05196>`_:
+
+.. code-block::
+
+    Cassiers et al., (2023). SCALib: A Side-Channel Analysis Library. Journal of Open Source Software, 8(86), 5196, https://doi.org/10.21105/joss.05196
+
+Bibtex:
+
+.. code-block::
+
+   @article{scalib,
+       doi = {10.21105/joss.05196},
+       url = {https://doi.org/10.21105/joss.05196},
+       year = {2023},
+       publisher = {The Open Journal},
+       volume = {8},
+       number = {86},
+       pages = {5196},
+       author = {Gaëtan Cassiers and Olivier Bronchain},
+       title = {SCALib: A Side-Channel Analysis Library}, journal = {Journal of Open Source Software}
+   }
+
+
 License
 =======
 This project is licensed under GNU AFFERO GENERAL PUBLIC LICENSE, Version 3.
 See `COPYRIGHT <COPYRIGHT>`_ and `COPYING <COPYING>`_ for more information.
 
 For licensing-related matters, please contact info@simple-crypto.dev.
```

### Comparing `scalib-0.5.5/README.rst` & `scalib-0.5.6/src/scalib.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,36 @@
+Metadata-Version: 2.1
+Name: scalib
+Version: 0.5.6
+Summary: Side-Channel Analysis Library
+Home-page: https://github.com/simple-crypto/scalib
+Author: Olivier Bronchain, Gaëtan Cassiers
+Author-email: olivier.bronchain@uclouvain.be, gaetan.cassiers@uclouvain.be
+License: GNU AGPL v3+
+Project-URL: Bug Tracker, https://github.com/simple-crypto/scalib/issues
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: COPYING
+
 ======
 SCALib
 ======
 
 .. image:: https://badge.fury.io/py/scalib.svg
     :target: https://pypi.org/project/scalib/
     :alt: PyPI
 .. image:: https://readthedocs.org/projects/scalib/badge/?version=stable
     :target: https://scalib.readthedocs.io/en/stable/
     :alt: Documentation Status
 .. image:: https://img.shields.io/matrix/scalib:matrix.org
     :target: https://matrix.to/#/#scalib:matrix.org
     :alt: Matrix room
+.. image:: https://joss.theoj.org/papers/10.21105/joss.05196/status.svg
+   :target: https://doi.org/10.21105/joss.05196
+   :alt: JOSS paper
 
 The Side-Channel Analysis Library (SCALib) is a Python library that
 contains state-of-the-art tools for side-channel security evaluation.
 
 - **Documentation**: https://scalib.readthedocs.io/
 - **Examples**: `examples/ <examples/>`_
 - **Chat**: `https://matrix.to/#/#scalib:matrix.org`
@@ -111,14 +127,41 @@
 You can also come discuss on `matrix <https://matrix.to/#/#scalib:matrix.org>`_
 (announcements, questions, community support, open discussion, etc.).
 
 All code contributions are subject to the Contributor License Agreement (`CLA
 <https://www.simple-crypto.dev/organization>`_) of SIMPLE-Crypto, which ensures
 a thriving future for open-source hardware security.
 
+
+Citation
+========
+
+If you use SCALib in your research, please cite our `software paper <https://doi.org/10.21105/joss.05196>`_:
+
+.. code-block::
+
+    Cassiers et al., (2023). SCALib: A Side-Channel Analysis Library. Journal of Open Source Software, 8(86), 5196, https://doi.org/10.21105/joss.05196
+
+Bibtex:
+
+.. code-block::
+
+   @article{scalib,
+       doi = {10.21105/joss.05196},
+       url = {https://doi.org/10.21105/joss.05196},
+       year = {2023},
+       publisher = {The Open Journal},
+       volume = {8},
+       number = {86},
+       pages = {5196},
+       author = {Gaëtan Cassiers and Olivier Bronchain},
+       title = {SCALib: A Side-Channel Analysis Library}, journal = {Journal of Open Source Software}
+   }
+
+
 License
 =======
 This project is licensed under GNU AFFERO GENERAL PUBLIC LICENSE, Version 3.
 See `COPYRIGHT <COPYRIGHT>`_ and `COPYING <COPYING>`_ for more information.
 
 For licensing-related matters, please contact info@simple-crypto.dev.
```

### Comparing `scalib-0.5.5/docs/Makefile` & `scalib-0.5.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/docs/_templates/autosummary/class.rst` & `scalib-0.5.6/docs/_templates/autosummary/class.rst`

 * *Files 27% similar despite different names*

```diff
@@ -27,7 +27,16 @@
    .. autosummary::
    {% for item in attributes %}
       ~{{ name }}.{{ item }}
    {%- endfor %}
    {% endif %}
    {% endblock %}
 
+   {% block classes %}
+
+   .. autosummary::
+   {% for item in elements %}
+       {% if item[0].isupper() %}
+          ~{{ name }}.{{ item }}
+       {%- endif %}
+   {%- endfor %}
+   {% endblock %}
```

### Comparing `scalib-0.5.5/docs/_templates/autosummary/module.rst` & `scalib-0.5.6/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/docs/conf.py` & `scalib-0.5.6/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,23 +13,25 @@
     'sphinx.ext.autodoc',
     'sphinx.ext.napoleon',
     'sphinx.ext.intersphinx',
     'sphinx.ext.coverage',
     'sphinx.ext.autosummary',
     'sphinx.ext.mathjax',
     'sphinx.ext.viewcode',
+    'sphinxcontrib.bibtex',
 ]
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
+bibtex_bibfiles = ['refs.bib']
 
 # -- Options for HTML output -------------------------------------------------
 html_theme = 'furo'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
```

### Comparing `scalib-0.5.5/docs/make.bat` & `scalib-0.5.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/examples/README.rst` & `scalib-0.5.6/examples/README.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/examples/aes_attack.py` & `scalib-0.5.6/examples/aes_attack.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/examples/aes_info.py` & `scalib-0.5.6/examples/aes_info.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/examples/aes_tvla.py` & `scalib-0.5.6/examples/aes_tvla.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/examples/utils.py` & `scalib-0.5.6/examples/utils.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/paper/paper.bib` & `scalib-0.5.6/paper/paper.bib`

 * *Files 8% similar despite different names*

```diff
@@ -40,65 +40,67 @@
 @inproceedings{DBLP:conf/asiacrypt/Veyrat-CharvillonGS14,
   author    = {Nicolas Veyrat{-}Charvillon and
                Beno{\^{\i}}t G{\'{e}}rard and
                Fran{\c{c}}ois{-}Xavier Standaert},
   editor    = {Palash Sarkar and
                Tetsu Iwata},
   title     = {Soft Analytical Side-Channel Attacks},
-  booktitle = {Advances in Cryptology - {ASIACRYPT} 2014 - 20th International Conference
-               on the Theory and Application of Cryptology and Information Security,
-               Kaoshiung, Taiwan, R.O.C., December 7-11, 2014. Proceedings, Part
-               {I}},
+  booktitle = {{Advances in Cryptology - Proceedings of 20th International Conference
+               on the Theory and Application of Cryptology and Information Security (ASIACRYPT} 2014), Part I}},
   series    = {Lecture Notes in Computer Science},
   volume    = {8873},
   pages     = {282--296},
   publisher = {Springer},
   year      = {2014},
+  month = dec,
+  location = {Kaoshiung, Taiwan, R.O.C.},
   url       = {https://doi.org/10.1007/978-3-662-45611-8_15},
   doi       = {10.1007/978-3-662-45611-8_15},
   timestamp = {Thu, 14 Oct 2021 10:07:58 +0200},
   biburl    = {https://dblp.org/rec/conf/asiacrypt/Veyrat-CharvillonGS14.bib},
   bibsource = {dblp computer science bibliography, https://dblp.org}
 }
 
 @inproceedings{DBLP:conf/ches/StandaertA08,
   author    = {Fran{\c{c}}ois{-}Xavier Standaert and
                C{\'{e}}dric Archambeau},
   editor    = {Elisabeth Oswald and
                Pankaj Rohatgi},
   title     = {Using Subspace-Based Template Attacks to Compare and Combine Power
                and Electromagnetic Information Leakages},
-  booktitle = {Cryptographic Hardware and Embedded Systems - {CHES} 2008, 10th International
-               Workshop, Washington, D.C., USA, August 10-13, 2008. Proceedings},
+  booktitle = {{Proceedings of 10th International Workshop on Cryptographic Hardware and Embedded Systems (CHES 2008)}},
   series    = {Lecture Notes in Computer Science},
   volume    = {5154},
   pages     = {411--425},
   publisher = {Springer},
   year      = {2008},
+  month = aug,
+  location = {Washington, D.C., USA},
   url       = {https://doi.org/10.1007/978-3-540-85053-3_26},
   doi       = {10.1007/978-3-540-85053-3_26},
   timestamp = {Thu, 14 Oct 2021 10:28:51 +0200},
   biburl    = {https://dblp.org/rec/conf/ches/StandaertA08.bib},
   bibsource = {dblp computer science bibliography, https://dblp.org}
 }
 
 @inproceedings{DBLP:conf/ches/SchneiderM15,
   author    = {Tobias Schneider and
                Amir Moradi},
   editor    = {Tim G{\"{u}}neysu and
                Helena Handschuh},
   title     = {Leakage Assessment Methodology - {A} Clear Roadmap for Side-Channel
                Evaluations},
-  booktitle = {Cryptographic Hardware and Embedded Systems - {CHES} 2015 - 17th International
-               Workshop, Saint-Malo, France, September 13-16, 2015, Proceedings},
+  booktitle = {{Proceedings of 17th International Workshop on Cryptographic Hardware and Embedded Systems (CHES 2015)}},
   series    = {Lecture Notes in Computer Science},
   volume    = {9293},
   pages     = {495--513},
   publisher = {Springer},
   year      = {2015},
+  month = sep,
+  location = {Saint-Malo, France},
   url       = {https://doi.org/10.1007/978-3-662-48324-4_25},
   doi       = {10.1007/978-3-662-48324-4_25},
   timestamp = {Thu, 31 Oct 2019 17:50:49 +0100},
   biburl    = {https://dblp.org/rec/conf/ches/SchneiderM15.bib},
   bibsource = {dblp computer science bibliography, https://dblp.org}
 }
 
@@ -106,20 +108,21 @@
   author    = {Romain Poussier and
                Fran{\c{c}}ois{-}Xavier Standaert and
                Vincent Grosso},
   editor    = {Benedikt Gierlichs and
                Axel Y. Poschmann},
   title     = {Simple Key Enumeration (and Rank Estimation) Using Histograms: An
                Integrated Approach},
-  booktitle = {Cryptographic Hardware and Embedded Systems - {CHES} 2016 - 18th International
-               Conference, Santa Barbara, CA, USA, August 17-19, 2016, Proceedings},
+  booktitle = {{Proceedings of 18th International Conference on Cryptographic Hardware and Embedded Systems - (CHES 2016)}},
   series    = {Lecture Notes in Computer Science},
   volume    = {9813},
   pages     = {61--81},
   publisher = {Springer},
+  month = aug,
+  location = {Santa Barbara, CA, USA},
   year      = {2016},
   url       = {https://doi.org/10.1007/978-3-662-53140-2_4},
   doi       = {10.1007/978-3-662-53140-2_4},
   timestamp = {Thu, 14 Oct 2021 10:28:51 +0200},
   biburl    = {https://dblp.org/rec/conf/ches/PoussierSG16.bib},
   bibsource = {dblp computer science bibliography, https://dblp.org}
 }
@@ -128,20 +131,21 @@
   author    = {Suresh Chari and
                Josyula R. Rao and
                Pankaj Rohatgi},
   editor    = {Burton S. Kaliski Jr. and
                {\c{C}}etin Kaya Ko{\c{c}} and
                Christof Paar},
   title     = {Template Attacks},
-  booktitle = {Cryptographic Hardware and Embedded Systems - {CHES} 2002, 4th International
-               Workshop, Redwood Shores, CA, USA, August 13-15, 2002, Revised Papers},
+  booktitle = {{4th International Workshop on Cryptographic Hardware and Embedded Systems (CHES 2002), Revised Papers}},
   series    = {Lecture Notes in Computer Science},
   volume    = {2523},
   pages     = {13--28},
   publisher = {Springer},
+  month = aug,
+  location = {Redwood Shores, CA, USA},
   year      = {2002},
   url       = {https://doi.org/10.1007/3-540-36400-5_3},
   doi       = {10.1007/3-540-36400-5_3},
   timestamp = {Tue, 14 May 2019 10:00:47 +0200},
   biburl    = {https://dblp.org/rec/conf/ches/ChariRR02.bib},
   bibsource = {dblp computer science bibliography, https://dblp.org}
 }
@@ -149,22 +153,22 @@
 @inproceedings{DBLP:conf/eurocrypt/StandaertMY09,
   author    = {Fran{\c{c}}ois{-}Xavier Standaert and
                Tal Malkin and
                Moti Yung},
   editor    = {Antoine Joux},
   title     = {A Unified Framework for the Analysis of Side-Channel Key Recovery
                Attacks},
-  booktitle = {Advances in Cryptology - {EUROCRYPT} 2009, 28th Annual International
-               Conference on the Theory and Applications of Cryptographic Techniques,
-               Cologne, Germany, April 26-30, 2009. Proceedings},
+  booktitle = {{Advances in Cryptology - Proceedings of 28th Annual International Conference on the Theory and Applications of Cryptographic Techniques (EUROCRYPT 200:9)}},
   series    = {Lecture Notes in Computer Science},
   volume    = {5479},
   pages     = {443--461},
   publisher = {Springer},
   year      = {2009},
+  month = apr,
+  location = {Cologne, Germany},
   url       = {https://doi.org/10.1007/978-3-642-01001-9_26},
   doi       = {10.1007/978-3-642-01001-9_26},
   timestamp = {Tue, 14 May 2019 10:00:53 +0200},
   biburl    = {https://dblp.org/rec/conf/eurocrypt/StandaertMY09.bib},
   bibsource = {dblp computer science bibliography, https://dblp.org}
 }
```

### Comparing `scalib-0.5.5/paper/paper.md` & `scalib-0.5.6/paper/paper.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 title: 'SCALib: A Side-Channel Analysis Library'
 tags:
   - Side-channel evaluation
   - Security
   - Python
   - Rust
 authors:
-  - name: Olivier Bronchain
-    orcid: 0000-0001-7595-718X
-    equal-contrib: true
-    affiliation: 1
   - name: Gaëtan Cassiers
     orcid: 0000-0001-5426-9345
     equal-contrib: true
     corresponding: true
-    affiliation: "1, 2"
+    affiliation: "2, 1"
+  - name: Olivier Bronchain
+    orcid: 0000-0001-7595-718X
+    equal-contrib: true
+    affiliation: 1
 affiliations:
  - name: UCLouvain, Belgium
    index: 1
- - name: Graz University of Technology, Austria
+ - name: TU Graz, Austria
    index: 2
-date: 16 February 2023
+date: 30 May 2023
 bibliography: paper.bib
 
 ---
 
 # Summary
 
 Side-channel attacks exploit unintended leakage from an electronic device in
 order to retrieve secret data.
 In particular, attacks exploiting physical side-channels such as power
 consumption or electromagnetic radiations to recover cryptographic keys are an
 important threat to embedded devices.
 Countermeasures against these attacks have been extensively researched for more
 than two decades and are often deployed in security-critical devices.
 
-A side-channel attack is made of three steps: first, the leakage is measured.
+A side-channel attack is made of three steps. First, the leakage is measured.
 Then, a statistical processing is applied to this leakage in order to infer the
 internal behavior of the device (typically, an intermediate state of the
 cryptographic algorithm). Finally, the cryptographic key is recovered from the
 known behavior [@DBLP:conf/eurocrypt/StandaertMY09].
 
 For the statistical processing, we distinguish between two classes of attacks,
 based on the use of a profiling dataset.
@@ -62,15 +62,15 @@
 analyzing the effectiveness of a newly proposed countermeasure or analyzing a
 widely deployed device.
 In `SCALib`, we implement algorithms for commonly used metrics and methods in
 side-channel security evaluations, attack-based and evaluation-based.
 We focus on the requirements of evaluations and do not implement
 complete attacks when they are not needed to evaluate the security of a device.
 
-`SCALib` is distributed as a Python package and uses 16-bit integer `numpy` [@numpy] arrays
+`SCALib` is distributed as a Python package and uses 16-bit integer NumPy [@numpy] arrays
 for leakage traces.
 For the sake of efficiency, most algorithms are implemented in Rust,
 allowing fine control of the memory accesses and enabling efficient
 parallelization.
 
 
 # Statement of need
@@ -90,15 +90,15 @@
 Moreover, while the leakage samples are acquired at a fairly low-resolution
 (8-bit to 16-bit integers), detection of very small effect sizes is
 needed, as they can potentially be exploited to mount an attack.
 Besides this requirement, leakage traces contain many points (typically
 thousands), and many metrics have to be computed for each of these points,
 providing parallelization opportunities.
 As a result of these characteristics, dedicated implementations can achieve
-much better accuracy and performance than generic or naive (e.g., pure `numpy`)
+much better accuracy and performance than generic or naive (e.g., pure NumPy)
 ones.
 
 On the other hand, security-specific algorithms are also used, such as key rank
 estimation (which allows us to know the computational cost of the last part of a
 side-channel attack without actually running it) [@DBLP:conf/ches/PoussierSG16].
 
 While multiple open-source side-channel attack and evaluation
@@ -127,14 +127,14 @@
 designs [@DBLP:journals/tches/NagpalGPM22], to publish new attacks on public
 implementations [@DBLP:journals/iacr/BronchainCS21], and also as a basis
 to develop new attack and evaluation methodologies [@DBLP:journals/tches/BronchainS21].
 
 
 # Acknowledgments
 
-This work has been funded in part by the Belgian Fund for Scientific Research
+This work has been funded in part by SGS, by the Belgian Fund for Scientific Research
 (F.R.S.-FNRS) through the Equipment Project SCALAB, by the European Union (EU)
 and the Walloon Region through the FEDER project USERMedia (convention number
-501907-379156), by the European Union (EU) through the ERC project 724725
-(acronym SWORD), and by SGS.
+501907-379156) and by the European Union (EU) through the ERC project 724725
+(acronym SWORD).
 
 # References
```

### Comparing `scalib-0.5.5/pyproject.toml` & `scalib-0.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [
-    "setuptools>=42",
+    "setuptools>=62.4",
      "setuptools-scm[toml]>=3.4",
      "setuptools-scm-git-archive",
     "wheel",
-    "setuptools-rust",
+    "setuptools-rust>=1.6",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "src/scalib/version.py"
 
 [tool.pytest.ini_options]
```

### Comparing `scalib-0.5.5/setup.cfg` & `scalib-0.5.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/setup.py` & `scalib-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib/__init__.py` & `scalib-0.5.6/src/scalib/__init__.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib/attacks/factor_graph.py` & `scalib-0.5.6/src/scalib/attacks/factor_graph.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib/attacks/sascagraph.py` & `scalib-0.5.6/src/scalib/attacks/sascagraph.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib/config/__init__.py` & `scalib-0.5.6/src/scalib/config/__init__.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib/config/threading.py` & `scalib-0.5.6/src/scalib/config/threading.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib/metrics/snr.py` & `scalib-0.5.6/src/scalib/metrics/snr.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib/metrics/ttest.py` & `scalib-0.5.6/src/scalib/metrics/ttest.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 .. math::
     t = \frac{\mu_0 - \mu_1}{\sqrt{\frac{v_0}{n_0} + \frac{v_1}{n_1}}}
 
 where :math:`\mu_0` (resp. :math:`\mu_1`) is the estimated moment of the first
 (resp.second) population and :math:`\frac{v_0}{n_0}` the variance of its
 estimate from :math:`n_0` samples. In the context of side-channel analysis, many of
 these statistical tests are performed independently for each point of the traces. 
-See [1]_ for additional details.
+See :footcite:p:`TVLA` for additional details.
 
 In this module, the definition of :math:`\mu` and :math:`v` are adapted to perform
 higher-order univariate and multivariate :math:`t`-test to compare higher-order moments of
 two distributions:
 
 - *Higher-order t-tests* pre-process the populations by elevating the traces at
   the :math:`d`-th power, after subtracting the mean (for :math:`d>1`) and
@@ -30,51 +30,46 @@
     :toctree:
     :nosignatures:
     :recursive:
 
     Ttest
     MTtest
 
-**Warning**: Ttest should not be used alone as a standalone evaluation tool
-because of its qualitative nature. See [2]_ and [3]_ for cautionary notes.
+Warning
+^^^^^^^
+
+Ttest should not be used alone as a standalone evaluation tool because of its
+qualitative nature. See :footcite:p:`how_not_ttest,critical_analysis_iso17825`
+for cautionary notes.
 
 
 Implementations Details
 ^^^^^^^^^^^^^^^^^^^^^^^
 
 In order to enable both efficient one-core and parallelized performance of the
 :math:`t`-test implementation, SCALib uses the one-pass formula for estimation
-arbitrary order statistical moment from [4]_ and its application to
-side-channel context in [1]_.
+arbitrary order statistical moment from :footcite:p:`onepass_moments` and its
+application to side-channel context in :footcite:p:`TVLA`.
 
 Concretely, the implementations first compute an estimation of the required
 statistical moments using a two-passes algorithms (first pass to compute the
 mean and the variances, and a second pass to compute the centered products).
 This new estimation is then used to update the current estimation using the
-merging rule from [4]_. To enable multi-threading, SCALib internally divides 
-the fresh traces into smaller independent chunks and then merges the output of
-each threads using [4]_. 
+merging rule from :footcite:p:`onepass_moments`. To enable multi-threading,
+SCALib internally divides the fresh traces into smaller independent chunks and
+then merges the output of each threads using :footcite:p:`onepass_moments`. 
 
 As a conclusion, the performance of the SCALib improves if the two-passes
 algorithm can be used on large chunks. Hence, it is recommended to feed a large
 enough amount of data for every call to `fit_u()`. 
 
 References
 ^^^^^^^^^^
 
-.. [1] "Leakage assessment methodology", Tobias Schneider, Amir Moradi, CHES
-   2015
-.. [2] "How (not) to Use Welch’s T-test in Side-Channel Security
-   Evaluations", François-Xavier Standaert, CARDIS 2018
-.. [3] "A Critical Analysis of ISO 17825 ('Testing Methods for the
-   Mitigation of Non-invasive Attack Classes Against Cryptographic
-   Modules')", Carolyn Whitnall, Elisabeth Oswald, ASIACRYPT 2019
-.. [4] "Formulas for Robust, One-Pass Parallel Computation of Covariances and
-    Arbitrary-Order Statistical Moments", Philippe Pébay, 2008
-
+.. footbibliography::
 """
 import numpy as np
 
 from scalib import _scalib_ext
 from scalib.config import get_config
 import scalib.utils
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scalib-0.5.5/src/scalib/modeling/__init__.py` & `scalib-0.5.6/src/scalib/modeling/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,12 +13,14 @@
 .. autosummary::
    :toctree:
    :recursive:
    :nosignatures:
 
    LDAClassifier
    MultiLDA
+   RLDAClassifier
 """
 
-__all__ = ["LDAClassifier", "MultiLDA"]
+__all__ = ["LDAClassifier", "MultiLDA", "RLDAClassifier"]
 
 from .ldaclassifier import LDAClassifier, MultiLDA
+from .rldaclassifier import RLDAClassifier
```

### Comparing `scalib-0.5.5/src/scalib/modeling/ldaclassifier.py` & `scalib-0.5.6/src/scalib/modeling/ldaclassifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     dimensionality reduction.
 
     Based on the training data, linear discriminant analysis build a linear
     dimentionality reduction to :math:`p` dimensions that maximizes class
     separation.
     Then, a multivariate gaussian template is fitted for each class (using the
     same covariance matrix for all the classes) in the reduced dimensionality
-    space to predict leakage likelihood [1]_.
+    space to predict leakage likelihood :footcite:p:`LDA`.
 
     Let :math:`\mathbf{W}` be the dimensionality reduction matrix of size
     (:math:`p`, :math:`n_s`). The likelihood is
 
     .. math::
             \mathsf{\hat{f}}(\mathbf{l} | x) =
                 \frac{1}{\sqrt{(2\pi)^{p} \cdot |\mathbf{\Sigma} |}} \cdot
@@ -59,17 +59,18 @@
     Notes
     -----
     This should have similar behavior as scikit-learn's `LDA
     <https://scikit-learn.org/stable/modules/lda_qda.html#lda-qda>`_, but it
     has better performance and numerical properties (at the cost of
     flexibility).
 
-    .. [1] François-Xavier Standaert and Cédric Archambeau, "Using
-       Subspace-Based Template Attacks to Compare and Combine Power and
-       Electromagnetic Information Leakages", CHES 2008: 411-425
+    References
+    ----------
+
+    .. footbibliography::
 
     Parameters
     ----------
     nc : int
         Number of possible classes (e.g., 256 for 8-bit target). `nc` must
         be smaller than `2**16`.
     p : int
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scalib-0.5.5/src/scalib/postprocessing/rankestimation.py` & `scalib-0.5.6/src/scalib/postprocessing/rankestimation.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,23 +37,23 @@
     :recursive:
 
     rank_accuracy
     rank_nbin
 
 Notes
 -----
-The rank estimation algorithm is based on [1]_, with the following
+The rank estimation algorithm is based on :footcite:p:`rankest_histograms`,
+with the following
 optimization: computation of histogram bins with higher score than the expected
 key is skipped, since it has no impact on the final rank.
 
 References
 ----------
 
-.. [1] "Simple Key Enumeration (and Rank Estimation) Using Histograms: An
-   Integrated Approach", R. Poussier, F.-X. Standaert, V. Grosso in CHES2016.
+.. footbibliography::
 """
 
 import math
 
 from scalib import _scalib_ext
 from scalib.config import get_config
 import scalib.utils
```

### Comparing `scalib-0.5.5/src/scalib/tools.py` & `scalib-0.5.6/src/scalib/tools.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib/utils.py` & `scalib-0.5.6/src/scalib/utils.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib.egg-info/PKG-INFO` & `scalib-0.5.6/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,23 @@
-Metadata-Version: 2.1
-Name: scalib
-Version: 0.5.5
-Summary: Side-Channel Analysis Library
-Home-page: https://github.com/simple-crypto/scalib
-Author: Olivier Bronchain, Gaëtan Cassiers
-Author-email: olivier.bronchain@uclouvain.be, gaetan.cassiers@uclouvain.be
-License: GNU AGPL v3+
-Project-URL: Bug Tracker, https://github.com/simple-crypto/scalib/issues
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: COPYING
-
 ======
 SCALib
 ======
 
 .. image:: https://badge.fury.io/py/scalib.svg
     :target: https://pypi.org/project/scalib/
     :alt: PyPI
 .. image:: https://readthedocs.org/projects/scalib/badge/?version=stable
     :target: https://scalib.readthedocs.io/en/stable/
     :alt: Documentation Status
 .. image:: https://img.shields.io/matrix/scalib:matrix.org
     :target: https://matrix.to/#/#scalib:matrix.org
     :alt: Matrix room
+.. image:: https://joss.theoj.org/papers/10.21105/joss.05196/status.svg
+   :target: https://doi.org/10.21105/joss.05196
+   :alt: JOSS paper
 
 The Side-Channel Analysis Library (SCALib) is a Python library that
 contains state-of-the-art tools for side-channel security evaluation.
 
 - **Documentation**: https://scalib.readthedocs.io/
 - **Examples**: `examples/ <examples/>`_
 - **Chat**: `https://matrix.to/#/#scalib:matrix.org`
@@ -124,14 +114,41 @@
 You can also come discuss on `matrix <https://matrix.to/#/#scalib:matrix.org>`_
 (announcements, questions, community support, open discussion, etc.).
 
 All code contributions are subject to the Contributor License Agreement (`CLA
 <https://www.simple-crypto.dev/organization>`_) of SIMPLE-Crypto, which ensures
 a thriving future for open-source hardware security.
 
+
+Citation
+========
+
+If you use SCALib in your research, please cite our `software paper <https://doi.org/10.21105/joss.05196>`_:
+
+.. code-block::
+
+    Cassiers et al., (2023). SCALib: A Side-Channel Analysis Library. Journal of Open Source Software, 8(86), 5196, https://doi.org/10.21105/joss.05196
+
+Bibtex:
+
+.. code-block::
+
+   @article{scalib,
+       doi = {10.21105/joss.05196},
+       url = {https://doi.org/10.21105/joss.05196},
+       year = {2023},
+       publisher = {The Open Journal},
+       volume = {8},
+       number = {86},
+       pages = {5196},
+       author = {Gaëtan Cassiers and Olivier Bronchain},
+       title = {SCALib: A Side-Channel Analysis Library}, journal = {Journal of Open Source Software}
+   }
+
+
 License
 =======
 This project is licensed under GNU AFFERO GENERAL PUBLIC LICENSE, Version 3.
 See `COPYRIGHT <COPYRIGHT>`_ and `COPYING <COPYING>`_ for more information.
 
 For licensing-related matters, please contact info@simple-crypto.dev.
```

### Comparing `scalib-0.5.5/src/scalib.egg-info/SOURCES.txt` & `scalib-0.5.6/src/scalib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitignore
 .readthedocs.yml
 CHANGELOG.rst
+CITATION.cff
 CONTRIBUTING.rst
 COPYING
 COPYRIGHT
 MANIFEST.in
 Makefile
 README.rst
 pyproject.toml
@@ -14,21 +15,23 @@
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/ci.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
+docs/refs.bib
 docs/requirements.txt
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/module.rst
 docs/source/api_ref.rst
 docs/source/changelog.rst
 docs/source/contributing.rst
 docs/source/copyright.rst
+docs/source/papers.rst
 examples/README.rst
 examples/aes_attack.py
 examples/aes_info.py
 examples/aes_tvla.py
 examples/test_examples.py
 examples/utils.py
 paper/build_paper.sh
@@ -47,18 +50,20 @@
 src/scalib.egg-info/top_level.txt
 src/scalib/attacks/__init__.py
 src/scalib/attacks/factor_graph.py
 src/scalib/attacks/sascagraph.py
 src/scalib/config/__init__.py
 src/scalib/config/threading.py
 src/scalib/metrics/__init__.py
+src/scalib/metrics/information.py
 src/scalib/metrics/snr.py
 src/scalib/metrics/ttest.py
 src/scalib/modeling/__init__.py
 src/scalib/modeling/ldaclassifier.py
+src/scalib/modeling/rldaclassifier.py
 src/scalib/postprocessing/__init__.py
 src/scalib/postprocessing/rankestimation.py
 src/scalib_ext/.gitignore
 src/scalib_ext/Cargo.lock
 src/scalib_ext/Cargo.toml
 src/scalib_ext/geigen/Cargo.toml
 src/scalib_ext/geigen/build.rs
@@ -449,30 +454,34 @@
 src/scalib_ext/ranklib/src/scores_example.h
 src/scalib_ext/ranklib/src/scores_example_data.cpp
 src/scalib_ext/ranklib/src/top.cpp
 src/scalib_ext/scalib/Cargo.toml
 src/scalib_ext/scalib-py/Cargo.toml
 src/scalib_ext/scalib-py/src/belief_propagation.rs
 src/scalib_ext/scalib-py/src/factor_graph.rs
+src/scalib_ext/scalib-py/src/information.rs
 src/scalib_ext/scalib-py/src/lda.rs
 src/scalib_ext/scalib-py/src/lib.rs
 src/scalib_ext/scalib-py/src/ranking.rs
+src/scalib_ext/scalib-py/src/rlda.rs
 src/scalib_ext/scalib-py/src/snr.rs
 src/scalib_ext/scalib-py/src/thread_pool.rs
 src/scalib_ext/scalib-py/src/ttest.rs
 src/scalib_ext/scalib/benches/belief_propagation.rs
 src/scalib_ext/scalib/benches/get_snr.rs
 src/scalib_ext/scalib/benches/mttest.rs
 src/scalib_ext/scalib/benches/snr_update.rs
 src/scalib_ext/scalib/benches/ttest.rs
 src/scalib_ext/scalib/src/belief_propagation.rs
+src/scalib_ext/scalib/src/information.rs
 src/scalib_ext/scalib/src/lda.rs
 src/scalib_ext/scalib/src/lib.rs
 src/scalib_ext/scalib/src/matrixmul.rs
 src/scalib_ext/scalib/src/mttest.rs
+src/scalib_ext/scalib/src/rlda.rs
 src/scalib_ext/scalib/src/snr.rs
 src/scalib_ext/scalib/src/ttest.rs
 src/scalib_ext/scalib/src/utils.rs
 src/scalib_ext/scalib/src/sasca/belief_propagation.rs
 src/scalib_ext/scalib/src/sasca/bp_compute.rs
 src/scalib_ext/scalib/src/sasca/factor_graph.rs
 src/scalib_ext/scalib/src/sasca/fg_build.rs
@@ -483,11 +492,12 @@
 src/scalib_ext/scalib/tests/ttest.rs
 tests/conftest.py
 tests/mttest_test.py
 tests/requirements.txt
 tests/test_factorgraph.py
 tests/test_lda.py
 tests/test_postprocessing.py
+tests/test_rlda.py
 tests/test_sascagraph.py
 tests/test_snr.py
 tests/test_tools.py
 tests/test_ttest.py
```

### Comparing `scalib-0.5.5/src/scalib_ext/.gitignore` & `scalib-0.5.6/src/scalib_ext/.gitignore`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/Cargo.lock` & `scalib-0.5.6/src/scalib_ext/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -660,14 +660,25 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "kdtree"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b63d659081717fe428fbaf9549559083956450194e57e8d28498a0dfa31b3b04"
+dependencies = [
+ "num-traits",
+ "serde",
+ "serde_derive",
+]
+
+[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "lazycell"
@@ -768,42 +779,27 @@
 name = "nalgebra"
 version = "0.30.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb2d0de08694bed883320212c18ee3008576bfe8c306f4c3c4a58b4876998be"
 dependencies = [
  "approx 0.5.1",
  "matrixmultiply",
- "num-complex",
- "num-rational",
- "num-traits",
- "simba 0.7.3",
- "typenum",
-]
-
-[[package]]
-name = "nalgebra"
-version = "0.32.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f6515c882ebfddccaa73ead7320ca28036c4bc84c9bcca3cc0cbba8efe89223a"
-dependencies = [
- "approx 0.5.1",
- "matrixmultiply",
  "nalgebra-macros",
  "num-complex",
  "num-rational",
  "num-traits",
- "simba 0.8.0",
+ "simba",
  "typenum",
 ]
 
 [[package]]
 name = "nalgebra-macros"
-version = "0.2.0"
+version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d232c68884c0c99810a5a4d333ef7e47689cfd0edc85efc9e54e1e6bf5212766"
+checksum = "01fcc0b8149b4632adc89ac3b7b31a12fb6099a0317a4eb2ebff574ef7de7218"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -880,15 +876,15 @@
 [[package]]
 name = "nshare"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4447657cd40e3107416ec4f2ac3e61a18781b00061789e3b8f4bbcbccb26c4c6"
 dependencies = [
  "image",
- "nalgebra 0.30.1",
+ "nalgebra",
  "ndarray",
 ]
 
 [[package]]
 name = "num-complex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1350,16 +1346,17 @@
  "crossbeam-utils",
  "geigen",
  "hytra",
  "index_vec",
  "indexmap",
  "indicatif",
  "itertools",
+ "kdtree",
  "matrixmultiply",
- "nalgebra 0.32.1",
+ "nalgebra",
  "ndarray",
  "ndarray-rand",
  "ndarray-stats",
  "nshare",
  "num-integer",
  "num-traits",
  "petgraph",
@@ -1379,14 +1376,15 @@
  "ndarray",
  "num_cpus",
  "numpy",
  "pyo3",
  "ranklib",
  "rayon",
  "scalib",
+ "serde",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
@@ -1442,27 +1440,14 @@
 dependencies = [
  "approx 0.5.1",
  "num-complex",
  "num-traits",
  "paste",
  "wide",
 ]
-
-[[package]]
-name = "simba"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50582927ed6f77e4ac020c057f37a268fc6aebc29225050365aacbb9deeeddc4"
-dependencies = [
- "approx 0.5.1",
- "num-complex",
- "num-traits",
- "paste",
- "wide",
-]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
```

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/build.rs` & `scalib-0.5.6/src/scalib_ext/geigen/build.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Cholesky` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/CholmodSupport` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Core` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Core`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Eigenvalues` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Geometry` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Householder` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Jacobi` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/LU` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/LU`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/MetisSupport` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/OrderingMethods` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/PaStiXSupport` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/PardisoSupport` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/QR` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/QR`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SPQRSupport` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SVD` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/Sparse` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseCholesky` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseCore` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseLU` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SparseQR` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/StdDeque` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/StdList` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/StdVector` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/SuperLUSupport` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/UmfPackSupport` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/Util/Version.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/Util/Version.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/include/geigen.h` & `scalib-0.5.6/src/scalib_ext/geigen/include/geigen.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/src/geigen.cpp` & `scalib-0.5.6/src/scalib_ext/geigen/src/geigen.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/src/geigen.rs` & `scalib-0.5.6/src/scalib_ext/geigen/src/geigen.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/geigen/src/lib.rs` & `scalib-0.5.6/src/scalib_ext/geigen/src/lib.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/build.rs` & `scalib-0.5.6/src/scalib_ext/ranklib/build.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/fuzz/Cargo.toml` & `scalib-0.5.6/src/scalib_ext/ranklib/fuzz/Cargo.toml`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs` & `scalib-0.5.6/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/aes.cpp` & `scalib-0.5.6/src/scalib_ext/ranklib/src/aes.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/bignumpoly.cpp` & `scalib-0.5.6/src/scalib_ext/ranklib/src/bignumpoly.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/bignumpoly.h` & `scalib-0.5.6/src/scalib_ext/ranklib/src/bignumpoly.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_enum.cpp` & `scalib-0.5.6/src/scalib_ext/ranklib/src/hel_enum.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_enum.h` & `scalib-0.5.6/src/scalib_ext/ranklib/src/hel_enum.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_execute.cpp` & `scalib-0.5.6/src/scalib_ext/ranklib/src/hel_execute.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_histo.cpp` & `scalib-0.5.6/src/scalib_ext/ranklib/src/hel_histo.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_histo.h` & `scalib-0.5.6/src/scalib_ext/ranklib/src/hel_histo.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_if.cpp` & `scalib-0.5.6/src/scalib_ext/ranklib/src/hel_if.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_if.h` & `scalib-0.5.6/src/scalib_ext/ranklib/src/hel_if.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_init.cpp` & `scalib-0.5.6/src/scalib_ext/ranklib/src/hel_init.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_init.h` & `scalib-0.5.6/src/scalib_ext/ranklib/src/hel_init.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_struct.h` & `scalib-0.5.6/src/scalib_ext/ranklib/src/hel_struct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_util.cpp` & `scalib-0.5.6/src/scalib_ext/ranklib/src/hel_util.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/hel_util.h` & `scalib-0.5.6/src/scalib_ext/ranklib/src/hel_util.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/histogram.rs` & `scalib-0.5.6/src/scalib_ext/ranklib/src/histogram.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/lib.rs` & `scalib-0.5.6/src/scalib_ext/ranklib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/main_example.cpp` & `scalib-0.5.6/src/scalib_ext/ranklib/src/main_example.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/rank.rs` & `scalib-0.5.6/src/scalib_ext/ranklib/src/rank.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/score_example_data.rs` & `scalib-0.5.6/src/scalib_ext/ranklib/src/score_example_data.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/scores_example.cpp` & `scalib-0.5.6/src/scalib_ext/ranklib/src/scores_example.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/scores_example.h` & `scalib-0.5.6/src/scalib_ext/ranklib/src/scores_example.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/scores_example_data.cpp` & `scalib-0.5.6/src/scalib_ext/ranklib/src/scores_example_data.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/ranklib/src/top.cpp` & `scalib-0.5.6/src/scalib_ext/ranklib/src/top.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/Cargo.toml` & `scalib-0.5.6/src/scalib_ext/scalib/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 geigen = { path = "../geigen" }
 
 # Numerical libs
 ndarray = { version = "0.15", features = ["rayon", "approx", "serde"] }
 blis-src = { version = "0.2.1", default-features=false, features=["static", "pthreads"], optional = true }
 blis-sys2 = { version = "0.2.1", optional = true }
 matrixmultiply = "0.3"
-nalgebra = "0.32"
+kdtree = { version = "0.5.1", features = ["serialize"] }
+nalgebra = "0.30.1"
 nshare = { version="0.9", features=["nalgebra", "ndarray"] }
 
 realfft = "2.0"
 num-traits = "0.2"
 
 [lib]
 bench = false
```

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/benches/belief_propagation.rs` & `scalib-0.5.6/src/scalib_ext/scalib/benches/belief_propagation.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/benches/get_snr.rs` & `scalib-0.5.6/src/scalib_ext/scalib/benches/get_snr.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/benches/mttest.rs` & `scalib-0.5.6/src/scalib_ext/scalib/benches/mttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/benches/snr_update.rs` & `scalib-0.5.6/src/scalib_ext/scalib/benches/snr_update.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/benches/ttest.rs` & `scalib-0.5.6/src/scalib_ext/scalib/benches/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/src/belief_propagation.rs` & `scalib-0.5.6/src/scalib_ext/scalib/src/belief_propagation.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/src/lda.rs` & `scalib-0.5.6/src/scalib_ext/scalib/src/lda.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/src/lib.rs` & `scalib-0.5.6/src/scalib_ext/scalib/src/lib.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 pub mod belief_propagation;
+pub mod information;
 pub mod lda;
 pub(crate) mod matrixmul;
 pub mod mttest;
+pub mod rlda;
 pub mod sasca;
 pub mod snr;
 pub mod ttest;
 pub(crate) mod utils;
 
 use thiserror::Error;
 
@@ -23,14 +25,20 @@
     )]
     SnrClassOverflow {
         leak_upper_bound: i64,
         max_n_traces: i64,
     },
     #[error("A SNR class value of a variable is larger than the given number of classes.")]
     SnrClassOutOfBound,
+    #[error("Clustering failed due to maximum number of centroids reached.")]
+    MaxCentroidNumber,
+    #[error("Empty KdTree, cannot get nearest centroid")]
+    EmptyKdTree,
+    #[error("No associated classes stored")]
+    NoAssociatedClassesStored,
 }
 
 #[derive(Clone)]
 pub struct Config {
     /// Show progress bars
     pub show_progress: bool,
     /// Computation time after which a progress bar is displayed.
```

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/src/matrixmul.rs` & `scalib-0.5.6/src/scalib_ext/scalib/src/matrixmul.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/src/mttest.rs` & `scalib-0.5.6/src/scalib_ext/scalib/src/mttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/src/sasca/belief_propagation.rs` & `scalib-0.5.6/src/scalib_ext/scalib/src/sasca/belief_propagation.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/src/sasca/bp_compute.rs` & `scalib-0.5.6/src/scalib_ext/scalib/src/sasca/bp_compute.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/src/sasca/factor_graph.rs` & `scalib-0.5.6/src/scalib_ext/scalib/src/sasca/factor_graph.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/src/sasca/fg_build.rs` & `scalib-0.5.6/src/scalib_ext/scalib/src/sasca/fg_build.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/src/sasca/fg_parser.rs` & `scalib-0.5.6/src/scalib_ext/scalib/src/sasca/fg_parser.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/src/sasca/mod.rs` & `scalib-0.5.6/src/scalib_ext/scalib/src/sasca/mod.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/src/snr.rs` & `scalib-0.5.6/src/scalib_ext/scalib/src/snr.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/src/ttest.rs` & `scalib-0.5.6/src/scalib_ext/scalib/src/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/src/utils.rs` & `scalib-0.5.6/src/scalib_ext/scalib/src/utils.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/tests/lda.rs` & `scalib-0.5.6/src/scalib_ext/scalib/tests/lda.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/tests/multivarcs.rs` & `scalib-0.5.6/src/scalib_ext/scalib/tests/multivarcs.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib/tests/ttest.rs` & `scalib-0.5.6/src/scalib_ext/scalib/tests/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib-py/Cargo.toml` & `scalib-0.5.6/src/scalib_ext/scalib-py/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 [features]
 ntl = ["ranklib/ntl"]
 hellib = ["ranklib/hellib"]
 blis = ["scalib/blis"]
 
 [dependencies]
 rayon = "1.7"
-ndarray = { version = "0.15", features = ["rayon"] }
+ndarray = { version = "0.15", features = ["rayon", "serde"] }
 numpy = "0.18"
 indicatif = "0.17"
 num_cpus = "1.15"
-bincode = "1.3" # Serialization for pickle support
+serde = { version = "1.0" }
+bincode = "1.3.3" # Serialization for pickle support
 
 [dependencies.pyo3]
 version = "0.18"
 features = ["extension-module", "abi3-py38"]
 
 [dependencies.ranklib]
 path = "../ranklib"
```

### Comparing `scalib-0.5.5/src/scalib_ext/scalib-py/src/belief_propagation.rs` & `scalib-0.5.6/src/scalib_ext/scalib-py/src/belief_propagation.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib-py/src/factor_graph.rs` & `scalib-0.5.6/src/scalib_ext/scalib-py/src/factor_graph.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib-py/src/lda.rs` & `scalib-0.5.6/src/scalib_ext/scalib-py/src/lda.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib-py/src/lib.rs` & `scalib-0.5.6/src/scalib_ext/scalib-py/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 use pyo3::create_exception;
 use pyo3::exceptions::PyException;
 use pyo3::prelude::*;
 use std::error::Error;
 
 mod belief_propagation;
 mod factor_graph;
+mod information;
 mod lda;
 mod ranking;
+mod rlda;
 mod snr;
 mod thread_pool;
 mod ttest;
 
 create_exception!(_scalib_ext, ScalibError, PyException);
 
 impl ScalibError {
@@ -114,14 +116,17 @@
     m.add("ScalibError", py.get_type::<ScalibError>())?;
     m.add_class::<Config>()?;
     m.add_class::<snr::SNR>()?;
     m.add_class::<ttest::Ttest>()?;
     m.add_class::<ttest::MTtest>()?;
     m.add_class::<lda::LDA>()?;
     m.add_class::<lda::LdaAcc>()?;
+    m.add_class::<rlda::RLDA>()?;
+    m.add_class::<rlda::RLDAClusteredModel>()?;
+    m.add_class::<information::ItEstimator>()?;
     m.add_class::<factor_graph::FactorGraph>()?;
     m.add_class::<factor_graph::BPState>()?;
     m.add_class::<thread_pool::ThreadPool>()?;
     m.add_function(wrap_pyfunction!(ranking::rank_accuracy, m)?)?;
     m.add_function(wrap_pyfunction!(ranking::rank_nbin, m)?)?;
     m.add_function(wrap_pyfunction!(belief_propagation::run_bp, m)?)?;
     m.add_function(wrap_pyfunction!(partial_cp, m)?)?;
```

### Comparing `scalib-0.5.5/src/scalib_ext/scalib-py/src/ranking.rs` & `scalib-0.5.6/src/scalib_ext/scalib-py/src/ranking.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib-py/src/snr.rs` & `scalib-0.5.6/src/scalib_ext/scalib-py/src/snr.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib-py/src/thread_pool.rs` & `scalib-0.5.6/src/scalib_ext/scalib-py/src/thread_pool.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/src/scalib_ext/scalib-py/src/ttest.rs` & `scalib-0.5.6/src/scalib_ext/scalib-py/src/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/tests/mttest_test.py` & `scalib-0.5.6/tests/mttest_test.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/tests/test_factorgraph.py` & `scalib-0.5.6/tests/test_factorgraph.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/tests/test_lda.py` & `scalib-0.5.6/tests/test_lda.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/tests/test_sascagraph.py` & `scalib-0.5.6/tests/test_sascagraph.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/tests/test_snr.py` & `scalib-0.5.6/tests/test_snr.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/tests/test_tools.py` & `scalib-0.5.6/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/tests/test_ttest.py` & `scalib-0.5.6/tests/test_ttest.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.5/tox.ini` & `scalib-0.5.6/tox.ini`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 description = Build the docs
 skip_install = True
 deps =
     -r{toxinidir}/docs/requirements.txt
 changedir = docs
 commands =
     pip freeze
-    sphinx-build  -W -b linkcheck . _build/html
     sphinx-build  -W -b html . _build/html
+    sphinx-build  -W -b linkcheck . _build/html
 
 [testenv:fmt]
 description = Check code style. Pass '--check' to instead check formatting.
 skip_install = True
 changedir = .
 deps =
     black ~= 23.0
```

