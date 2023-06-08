# Comparing `tmp/veros-1.4.5.tar.gz` & `tmp/veros-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veros-1.4.5.tar", last modified: Mon Aug 15 07:45:08 2022, max compression
+gzip compressed data, was "veros-1.4.6.tar", last modified: Thu Jun  8 12:20:07 2023, max compression
```

## Comparing `veros-1.4.5.tar` & `veros-1.4.6.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.743001 veros-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-08-15 07:44:54.000000 veros-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-08-15 07:44:54.000000 veros-1.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7497 2022-08-15 07:45:08.743001 veros-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6356 2022-08-15 07:44:54.000000 veros-1.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     4089 2022-08-15 07:44:54.000000 veros-1.4.5/cuda_ext.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-08-15 07:44:54.000000 veros-1.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-08-15 07:44:54.000000 veros-1.4.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-15 07:44:54.000000 veros-1.4.5/requirements_jax.txt
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-08-15 07:45:08.743001 veros-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5018 2022-08-15 07:44:54.000000 veros-1.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.743001 veros-1.4.5/veros/
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2022-08-15 07:44:54.000000 veros-1.4.5/veros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-08-15 07:45:08.747001 veros-1.4.5/veros/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-08-15 07:44:54.000000 veros-1.4.5/veros/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.735001 veros-1.4.5/veros/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-08-15 07:44:54.000000 veros-1.4.5/veros/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-15 07:44:54.000000 veros-1.4.5/veros/cli/veros.py
--rw-r--r--   0 runner    (1001) docker     (121)     3663 2022-08-15 07:44:54.000000 veros-1.4.5/veros/cli/veros_copy_setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-08-15 07:44:54.000000 veros-1.4.5/veros/cli/veros_create_mask.py
--rw-r--r--   0 runner    (1001) docker     (121)     3266 2022-08-15 07:44:54.000000 veros-1.4.5/veros/cli/veros_resubmit.py
--rw-r--r--   0 runner    (1001) docker     (121)     4260 2022-08-15 07:44:54.000000 veros-1.4.5/veros/cli/veros_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.735001 veros-1.4.5/veros/core/
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10303 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/advection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.735001 veros-1.4.5/veros/core/density/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7165 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/density/get_rho.py
--rw-r--r--   0 runner    (1001) docker     (121)    22275 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/density/gsw.py
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/density/linear_eq.py
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/density/nonlinear_eq1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/density/nonlinear_eq2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/density/nonlinear_eq3.py
--rw-r--r--   0 runner    (1001) docker     (121)    10218 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/diffusion.py
--rw-r--r--   0 runner    (1001) docker     (121)     8856 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/eke.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.739001 veros-1.4.5/veros/core/external/
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3843 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/external/island.py
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/external/line_integrals.py
--rw-r--r--   0 runner    (1001) docker     (121)     5215 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/external/poisson_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     5406 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/external/solve_pressure.py
--rw-r--r--   0 runner    (1001) docker     (121)     7556 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/external/solve_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.739001 veros-1.4.5/veros/core/external/solvers/
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/external/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/external/solvers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7067 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/external/solvers/petsc_.py
--rw-r--r--   0 runner    (1001) docker     (121)     5396 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/external/solvers/scipy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4952 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/external/solvers/scipy_jax.py
--rw-r--r--   0 runner    (1001) docker     (121)     5957 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/external/streamfunction_init.py
--rw-r--r--   0 runner    (1001) docker     (121)    37206 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/friction.py
--rw-r--r--   0 runner    (1001) docker     (121)    10359 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/idemix.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.739001 veros-1.4.5/veros/core/isoneutral/
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/isoneutral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10639 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/isoneutral/diffusion.py
--rw-r--r--   0 runner    (1001) docker     (121)     5830 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/isoneutral/friction.py
--rw-r--r--   0 runner    (1001) docker     (121)    11269 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/isoneutral/isoneutral.py
--rw-r--r--   0 runner    (1001) docker     (121)    10504 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/momentum.py
--rw-r--r--   0 runner    (1001) docker     (121)    10532 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/numerics.py
--rw-r--r--   0 runner    (1001) docker     (121)     4603 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.739001 veros-1.4.5/veros/core/special/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3133 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/special/cuda_tdma_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/special/cuda_tdma_kernels.h
--rw-r--r--   0 runner    (1001) docker     (121)     5347 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/special/tdma_.py
--rw-r--r--   0 runner    (1001) docker     (121)   139774 2022-08-15 07:45:08.000000 veros-1.4.5/veros/core/special/tdma_cuda_.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/special/tdma_cuda_.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     3608 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/special/tdma_cython_.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    16470 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/thermodynamics.py
--rw-r--r--   0 runner    (1001) docker     (121)    11654 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/tke.py
--rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-08-15 07:44:54.000000 veros-1.4.5/veros/core/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.739001 veros-1.4.5/veros/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-15 07:44:54.000000 veros-1.4.5/veros/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-08-15 07:44:54.000000 veros-1.4.5/veros/diagnostics/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2757 2022-08-15 07:44:54.000000 veros-1.4.5/veros/diagnostics/averages.py
--rw-r--r--   0 runner    (1001) docker     (121)     3661 2022-08-15 07:44:54.000000 veros-1.4.5/veros/diagnostics/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3020 2022-08-15 07:44:54.000000 veros-1.4.5/veros/diagnostics/cfl_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    14434 2022-08-15 07:44:54.000000 veros-1.4.5/veros/diagnostics/energy.py
--rw-r--r--   0 runner    (1001) docker     (121)     9629 2022-08-15 07:44:54.000000 veros-1.4.5/veros/diagnostics/overturning.py
--rw-r--r--   0 runner    (1001) docker     (121)     2277 2022-08-15 07:44:54.000000 veros-1.4.5/veros/diagnostics/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2022-08-15 07:44:54.000000 veros-1.4.5/veros/diagnostics/tracer_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    18440 2022-08-15 07:44:54.000000 veros-1.4.5/veros/distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.739001 veros-1.4.5/veros/io_tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 07:44:54.000000 veros-1.4.5/veros/io_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-08-15 07:44:54.000000 veros-1.4.5/veros/io_tools/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)     6115 2022-08-15 07:44:54.000000 veros-1.4.5/veros/io_tools/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-08-15 07:44:54.000000 veros-1.4.5/veros/logs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2199 2022-08-15 07:44:54.000000 veros-1.4.5/veros/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     6189 2022-08-15 07:44:54.000000 veros-1.4.5/veros/progress.py
--rw-r--r--   0 runner    (1001) docker     (121)    15954 2022-08-15 07:44:54.000000 veros-1.4.5/veros/pyom_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     6419 2022-08-15 07:44:54.000000 veros-1.4.5/veros/restart.py
--rw-r--r--   0 runner    (1001) docker     (121)    11925 2022-08-15 07:44:54.000000 veros-1.4.5/veros/routines.py
--rw-r--r--   0 runner    (1001) docker     (121)     5579 2022-08-15 07:44:54.000000 veros-1.4.5/veros/runtime.py
--rw-r--r--   0 runner    (1001) docker     (121)     9013 2022-08-15 07:44:54.000000 veros-1.4.5/veros/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.739001 veros-1.4.5/veros/setups/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.743001 veros-1.4.5/veros/setups/acc/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/acc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6625 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/acc/acc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.743001 veros-1.4.5/veros/setups/acc_basic/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/acc_basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6063 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/acc_basic/acc_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.743001 veros-1.4.5/veros/setups/global_1deg/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/global_1deg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/global_1deg/assets.json
--rw-r--r--   0 runner    (1001) docker     (121)    13514 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/global_1deg/global_1deg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.743001 veros-1.4.5/veros/setups/global_4deg/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/global_4deg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/global_4deg/assets.json
--rw-r--r--   0 runner    (1001) docker     (121)    10458 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/global_4deg/global_4deg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.743001 veros-1.4.5/veros/setups/global_flexible/
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/global_flexible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/global_flexible/assets.json
--rw-r--r--   0 runner    (1001) docker     (121)    16921 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/global_flexible/global_flexible.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.743001 veros-1.4.5/veros/setups/north_atlantic/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/north_atlantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/north_atlantic/assets.json
--rw-r--r--   0 runner    (1001) docker     (121)    13781 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/north_atlantic/north_atlantic.py
--rw-r--r--   0 runner    (1001) docker     (121)    62024 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/north_atlantic/tidal_energy.npy
--rw-r--r--   0 runner    (1001) docker     (121)    93891 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/north_atlantic/topo_mask.png
--rw-r--r--   0 runner    (1001) docker     (121)    62024 2022-08-15 07:44:54.000000 veros-1.4.5/veros/setups/north_atlantic/wind_energy.npy
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-08-15 07:44:54.000000 veros-1.4.5/veros/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)    17531 2022-08-15 07:44:54.000000 veros-1.4.5/veros/state.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-08-15 07:44:54.000000 veros-1.4.5/veros/time.py
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-08-15 07:44:54.000000 veros-1.4.5/veros/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.743001 veros-1.4.5/veros/tools/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-08-15 07:44:54.000000 veros-1.4.5/veros/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4584 2022-08-15 07:44:54.000000 veros-1.4.5/veros/tools/assets.py
--rw-r--r--   0 runner    (1001) docker     (121)    12678 2022-08-15 07:44:54.000000 veros-1.4.5/veros/tools/filelock.py
--rw-r--r--   0 runner    (1001) docker     (121)    18010 2022-08-15 07:44:54.000000 veros-1.4.5/veros/tools/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    30439 2022-08-15 07:44:54.000000 veros-1.4.5/veros/variables.py
--rw-r--r--   0 runner    (1001) docker     (121)    15946 2022-08-15 07:44:54.000000 veros-1.4.5/veros/veros.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 07:45:08.735001 veros-1.4.5/veros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7497 2022-08-15 07:45:08.000000 veros-1.4.5/veros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3323 2022-08-15 07:45:08.000000 veros-1.4.5/veros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 07:45:08.000000 veros-1.4.5/veros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-08-15 07:45:08.000000 veros-1.4.5/veros.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 07:45:08.000000 veros-1.4.5/veros.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-08-15 07:45:08.000000 veros-1.4.5/veros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-08-15 07:45:08.000000 veros-1.4.5/veros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    81295 2022-08-15 07:44:54.000000 veros-1.4.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.203230 veros-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-08 12:19:45.000000 veros-1.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-08 12:19:45.000000 veros-1.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-06-08 12:20:07.203230 veros-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-06-08 12:19:45.000000 veros-1.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-08 12:19:45.000000 veros-1.4.6/cuda_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-08 12:19:45.000000 veros-1.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-08 12:19:45.000000 veros-1.4.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 12:19:45.000000 veros-1.4.6/requirements_jax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-08 12:20:07.203230 veros-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-06-08 12:19:45.000000 veros-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.207229 veros-1.4.6/veros/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-08 12:19:45.000000 veros-1.4.6/veros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-08 12:20:07.207229 veros-1.4.6/veros/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-08 12:19:45.000000 veros-1.4.6/veros/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.191229 veros-1.4.6/veros/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-08 12:19:45.000000 veros-1.4.6/veros/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-08 12:19:45.000000 veros-1.4.6/veros/cli/veros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-08 12:19:45.000000 veros-1.4.6/veros/cli/veros_copy_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-08 12:19:45.000000 veros-1.4.6/veros/cli/veros_create_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-08 12:19:45.000000 veros-1.4.6/veros/cli/veros_resubmit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-08 12:19:45.000000 veros-1.4.6/veros/cli/veros_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.195229 veros-1.4.6/veros/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/advection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.195229 veros-1.4.6/veros/core/density/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/density/get_rho.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22275 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/density/gsw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/density/linear_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/density/nonlinear_eq1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/density/nonlinear_eq2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/density/nonlinear_eq3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/eke.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.195229 veros-1.4.6/veros/core/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/external/island.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/external/line_integrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/external/poisson_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/external/solve_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/external/solve_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.195229 veros-1.4.6/veros/core/external/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/external/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/external/solvers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/external/solvers/petsc_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/external/solvers/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/external/solvers/scipy_jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/external/streamfunction_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37206 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/friction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/idemix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.199230 veros-1.4.6/veros/core/isoneutral/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/isoneutral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/isoneutral/diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/isoneutral/friction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/isoneutral/isoneutral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/numerics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.199230 veros-1.4.6/veros/core/special/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/special/cuda_tdma_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/special/cuda_tdma_kernels.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/special/tdma_.py
+-rw-r--r--   0 runner    (1001) docker     (123)   140016 2023-06-08 12:20:06.000000 veros-1.4.6/veros/core/special/tdma_cuda_.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/special/tdma_cuda_.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/special/tdma_cython_.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/thermodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/tke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-08 12:19:45.000000 veros-1.4.6/veros/core/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.199230 veros-1.4.6/veros/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 12:19:45.000000 veros-1.4.6/veros/diagnostics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-08 12:19:45.000000 veros-1.4.6/veros/diagnostics/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-08 12:19:45.000000 veros-1.4.6/veros/diagnostics/averages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-08 12:19:45.000000 veros-1.4.6/veros/diagnostics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-08 12:19:45.000000 veros-1.4.6/veros/diagnostics/cfl_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14434 2023-06-08 12:19:45.000000 veros-1.4.6/veros/diagnostics/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-06-08 12:19:45.000000 veros-1.4.6/veros/diagnostics/overturning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-08 12:19:45.000000 veros-1.4.6/veros/diagnostics/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-08 12:19:45.000000 veros-1.4.6/veros/diagnostics/tracer_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18440 2023-06-08 12:19:45.000000 veros-1.4.6/veros/distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.199230 veros-1.4.6/veros/io_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:19:45.000000 veros-1.4.6/veros/io_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-08 12:19:45.000000 veros-1.4.6/veros/io_tools/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-08 12:19:45.000000 veros-1.4.6/veros/io_tools/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-08 12:19:45.000000 veros-1.4.6/veros/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-08 12:19:45.000000 veros-1.4.6/veros/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-06-08 12:19:45.000000 veros-1.4.6/veros/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-06-08 12:19:45.000000 veros-1.4.6/veros/pyom_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-08 12:19:45.000000 veros-1.4.6/veros/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11925 2023-06-08 12:19:45.000000 veros-1.4.6/veros/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-06-08 12:19:45.000000 veros-1.4.6/veros/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-06-08 12:19:45.000000 veros-1.4.6/veros/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.199230 veros-1.4.6/veros/setups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.199230 veros-1.4.6/veros/setups/acc/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/acc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/acc/acc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.203230 veros-1.4.6/veros/setups/acc_basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/acc_basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/acc_basic/acc_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.203230 veros-1.4.6/veros/setups/global_1deg/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/global_1deg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/global_1deg/assets.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/global_1deg/global_1deg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.203230 veros-1.4.6/veros/setups/global_4deg/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/global_4deg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/global_4deg/assets.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10458 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/global_4deg/global_4deg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.203230 veros-1.4.6/veros/setups/global_flexible/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/global_flexible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/global_flexible/assets.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/global_flexible/global_flexible.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.203230 veros-1.4.6/veros/setups/north_atlantic/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/north_atlantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/north_atlantic/assets.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/north_atlantic/north_atlantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62024 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/north_atlantic/tidal_energy.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    93891 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/north_atlantic/topo_mask.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62024 2023-06-08 12:19:45.000000 veros-1.4.6/veros/setups/north_atlantic/wind_energy.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-08 12:19:45.000000 veros-1.4.6/veros/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17531 2023-06-08 12:19:45.000000 veros-1.4.6/veros/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-08 12:19:45.000000 veros-1.4.6/veros/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-08 12:19:45.000000 veros-1.4.6/veros/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.203230 veros-1.4.6/veros/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-08 12:19:45.000000 veros-1.4.6/veros/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-08 12:19:45.000000 veros-1.4.6/veros/tools/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-06-08 12:19:45.000000 veros-1.4.6/veros/tools/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-06-08 12:19:45.000000 veros-1.4.6/veros/tools/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30439 2023-06-08 12:19:45.000000 veros-1.4.6/veros/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15946 2023-06-08 12:19:45.000000 veros-1.4.6/veros/veros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:20:07.191229 veros-1.4.6/veros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-06-08 12:20:07.000000 veros-1.4.6/veros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-08 12:20:07.000000 veros-1.4.6/veros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:20:07.000000 veros-1.4.6/veros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-08 12:20:07.000000 veros-1.4.6/veros.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:20:07.000000 veros-1.4.6/veros.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-08 12:20:07.000000 veros-1.4.6/veros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 12:20:07.000000 veros-1.4.6/veros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-08 12:19:45.000000 veros-1.4.6/versioneer.py
```

### Comparing `veros-1.4.5/LICENSE` & `veros-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/PKG-INFO` & `veros-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veros
-Version: 1.4.5
+Version: 1.4.6
 Summary: The versatile ocean simulator, in pure Python, powered by JAX.
 Home-page: https://veros.readthedocs.io
 Author: Dion Häfner (NBI Copenhagen)
 Author-email: dion.haefner@nbi.ku.dk
 License: MIT
 Keywords: oceanography python parallel numpy multi-core geophysics ocean-model mpi4py jax
 Classifier: Development Status :: 4 - Beta
@@ -39,15 +39,15 @@
   <a href="http://veros.readthedocs.io/?badge=latest">
     <img src="https://readthedocs.org/projects/veros/badge/?version=latest" alt="Documentation status">
   </a>
   <a href="https://github.com/team-ocean/veros/actions/workflows/test-all.yml">
     <img src="https://github.com/team-ocean/veros/actions/workflows/test-all.yml/badge.svg" alt="Test status">
   </a>
   <a href="https://codecov.io/gh/team-ocean/veros">
-    <img src="https://codecov.io/gh/team-ocean/veros/branch/master/graph/badge.svg" alt="Code Coverage">
+    <img src="https://codecov.io/gh/team-ocean/veros/branch/main/graph/badge.svg" alt="Code Coverage">
   </a>
   <a href="https://zenodo.org/badge/latestdoi/87419383">
     <img src="https://zenodo.org/badge/87419383.svg" alt="DOI">
   </a>
 </p>
 
 Veros, *the versatile ocean simulator*, aims to be the swiss army knife of ocean modeling. It is a full-fledged primitive equation ocean model that supports anything between idealized toy models and [realistic, high-resolution, global ocean simulations](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2021MS002717). And because Veros is written in pure Python, the days of struggling with complicated model setup workflows, ancient programming environments, and obscure legacy code are finally over.
@@ -110,15 +110,15 @@
 ## Basic usage
 
 To run Veros, you need to set up a model --- i.e., specify which settings
 and model domain you want to use. This is done by subclassing the
 `VerosSetup` base class in a *setup script* that is written in Python. You
 should use the `veros copy-setup` command to copy one into your current
 folder. A good place to start is the
-[ACC model](https://github.com/team-ocean/veros/blob/master/veros/setups/acc/acc.py):
+[ACC model](https://github.com/team-ocean/veros/blob/main/veros/setups/acc/acc.py):
 
 ```bash
 $ veros copy-setup acc
 ```
 
 After setting up your model, all you need to do is call the `setup` and
 `run` methods on your setup class. The pre-implemented setups can all be
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: veros Version: 1.4.5 Summary: The versatile ocean
+Metadata-Version: 2.1 Name: veros Version: 1.4.6 Summary: The versatile ocean
 simulator, in pure Python, powered by JAX. Home-page: https://
 veros.readthedocs.io Author: Dion HÃ¤fner (NBI Copenhagen) Author-email:
 dion.haefner@nbi.ku.dk License: MIT Keywords: oceanography python parallel
 numpy multi-core geophysics ocean-model mpi4py jax Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
@@ -49,19 +49,19 @@
 copy-setup acc --to /tmp/acc $ veros run /tmp/acc/acc.py ``` For more detailed
 installation instructions, have a look at [our documentation](https://
 veros.readthedocs.io). ## Basic usage To run Veros, you need to set up a model
 --- i.e., specify which settings and model domain you want to use. This is done
 by subclassing the `VerosSetup` base class in a *setup script* that is written
 in Python. You should use the `veros copy-setup` command to copy one into your
 current folder. A good place to start is the [ACC model](https://github.com/
-team-ocean/veros/blob/master/veros/setups/acc/acc.py): ```bash $ veros copy-
-setup acc ``` After setting up your model, all you need to do is call the
-`setup` and `run` methods on your setup class. The pre-implemented setups can
-all be executed via `veros run`: ```bash $ veros run acc.py ``` For more
-information on using Veros, have a look at [our documentation](http://
+team-ocean/veros/blob/main/veros/setups/acc/acc.py): ```bash $ veros copy-setup
+acc ``` After setting up your model, all you need to do is call the `setup` and
+`run` methods on your setup class. The pre-implemented setups can all be
+executed via `veros run`: ```bash $ veros run acc.py ``` For more information
+on using Veros, have a look at [our documentation](http://
 veros.readthedocs.io). ## Contributing Contributions to Veros are always
 welcome, no matter if you spotted an inaccuracy in [the documentation](https://
 veros.readthedocs.io), wrote a new setup, fixed a bug, or even extended Veros\'
 core mechanics. There are 2 ways to contribute: 1. If you want to report a bug
 or request a missing feature, please [open an issue](https://github.com/team-
 ocean/veros/issues). If you are reporting a bug, make sure to include all
 relevant information for reproducing it (ideally through a *minimal* code
```

### Comparing `veros-1.4.5/README.md` & `veros-1.4.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   <a href="http://veros.readthedocs.io/?badge=latest">
     <img src="https://readthedocs.org/projects/veros/badge/?version=latest" alt="Documentation status">
   </a>
   <a href="https://github.com/team-ocean/veros/actions/workflows/test-all.yml">
     <img src="https://github.com/team-ocean/veros/actions/workflows/test-all.yml/badge.svg" alt="Test status">
   </a>
   <a href="https://codecov.io/gh/team-ocean/veros">
-    <img src="https://codecov.io/gh/team-ocean/veros/branch/master/graph/badge.svg" alt="Code Coverage">
+    <img src="https://codecov.io/gh/team-ocean/veros/branch/main/graph/badge.svg" alt="Code Coverage">
   </a>
   <a href="https://zenodo.org/badge/latestdoi/87419383">
     <img src="https://zenodo.org/badge/87419383.svg" alt="DOI">
   </a>
 </p>
 
 Veros, *the versatile ocean simulator*, aims to be the swiss army knife of ocean modeling. It is a full-fledged primitive equation ocean model that supports anything between idealized toy models and [realistic, high-resolution, global ocean simulations](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2021MS002717). And because Veros is written in pure Python, the days of struggling with complicated model setup workflows, ancient programming environments, and obscure legacy code are finally over.
@@ -81,15 +81,15 @@
 ## Basic usage
 
 To run Veros, you need to set up a model --- i.e., specify which settings
 and model domain you want to use. This is done by subclassing the
 `VerosSetup` base class in a *setup script* that is written in Python. You
 should use the `veros copy-setup` command to copy one into your current
 folder. A good place to start is the
-[ACC model](https://github.com/team-ocean/veros/blob/master/veros/setups/acc/acc.py):
+[ACC model](https://github.com/team-ocean/veros/blob/main/veros/setups/acc/acc.py):
 
 ```bash
 $ veros copy-setup acc
 ```
 
 After setting up your model, all you need to do is call the `setup` and
 `run` methods on your setup class. The pre-implemented setups can all be
```

#### html2text {}

```diff
@@ -33,19 +33,19 @@
 copy-setup acc --to /tmp/acc $ veros run /tmp/acc/acc.py ``` For more detailed
 installation instructions, have a look at [our documentation](https://
 veros.readthedocs.io). ## Basic usage To run Veros, you need to set up a model
 --- i.e., specify which settings and model domain you want to use. This is done
 by subclassing the `VerosSetup` base class in a *setup script* that is written
 in Python. You should use the `veros copy-setup` command to copy one into your
 current folder. A good place to start is the [ACC model](https://github.com/
-team-ocean/veros/blob/master/veros/setups/acc/acc.py): ```bash $ veros copy-
-setup acc ``` After setting up your model, all you need to do is call the
-`setup` and `run` methods on your setup class. The pre-implemented setups can
-all be executed via `veros run`: ```bash $ veros run acc.py ``` For more
-information on using Veros, have a look at [our documentation](http://
+team-ocean/veros/blob/main/veros/setups/acc/acc.py): ```bash $ veros copy-setup
+acc ``` After setting up your model, all you need to do is call the `setup` and
+`run` methods on your setup class. The pre-implemented setups can all be
+executed via `veros run`: ```bash $ veros run acc.py ``` For more information
+on using Veros, have a look at [our documentation](http://
 veros.readthedocs.io). ## Contributing Contributions to Veros are always
 welcome, no matter if you spotted an inaccuracy in [the documentation](https://
 veros.readthedocs.io), wrote a new setup, fixed a bug, or even extended Veros\'
 core mechanics. There are 2 ways to contribute: 1. If you want to report a bug
 or request a missing feature, please [open an issue](https://github.com/team-
 ocean/veros/issues). If you are reporting a bug, make sure to include all
 relevant information for reproducing it (ideally through a *minimal* code
```

### Comparing `veros-1.4.5/cuda_ext.py` & `veros-1.4.6/cuda_ext.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/setup.py` & `veros-1.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 jax_req = parse_requirements("requirements_jax.txt")
 for line in jax_req:  # inject jaxlib requirement
     if line.startswith("jax"):
         jax_req.append(line.replace("jax", "jaxlib"))
         break
 
 EXTRAS_REQUIRE = {
-    "test": ["pytest", "pytest-cov", "pytest-forked", "codecov", "xarray"],
+    "test": ["pytest", "pytest-cov", "pytest-forked", "xarray"],
     "jax": jax_req,
 }
 
 
 def get_extensions(require_cython_ext, require_cuda_ext):
     cuda_info = cuda_ext.cuda_info
```

### Comparing `veros-1.4.5/veros/__init__.py` & `veros-1.4.6/veros/__init__.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/backend.py` & `veros-1.4.6/veros/backend.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/cli/__init__.py` & `veros-1.4.6/veros/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/cli/veros_copy_setup.py` & `veros-1.4.6/veros/cli/veros_copy_setup.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/cli/veros_create_mask.py` & `veros-1.4.6/veros/cli/veros_create_mask.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/cli/veros_resubmit.py` & `veros-1.4.6/veros/cli/veros_resubmit.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/cli/veros_run.py` & `veros-1.4.6/veros/cli/veros_run.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/__init__.py` & `veros-1.4.6/veros/core/__init__.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/advection.py` & `veros-1.4.6/veros/core/advection.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/density/get_rho.py` & `veros-1.4.6/veros/core/density/get_rho.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/density/gsw.py` & `veros-1.4.6/veros/core/density/gsw.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/density/linear_eq.py` & `veros-1.4.6/veros/core/density/linear_eq.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/density/nonlinear_eq1.py` & `veros-1.4.6/veros/core/density/nonlinear_eq1.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/density/nonlinear_eq2.py` & `veros-1.4.6/veros/core/density/nonlinear_eq2.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/density/nonlinear_eq3.py` & `veros-1.4.6/veros/core/density/nonlinear_eq3.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/diffusion.py` & `veros-1.4.6/veros/core/diffusion.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/eke.py` & `veros-1.4.6/veros/core/eke.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/external/island.py` & `veros-1.4.6/veros/core/external/island.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/external/line_integrals.py` & `veros-1.4.6/veros/core/external/line_integrals.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/external/poisson_matrix.py` & `veros-1.4.6/veros/core/external/poisson_matrix.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/external/solve_pressure.py` & `veros-1.4.6/veros/core/external/solve_pressure.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/external/solve_stream.py` & `veros-1.4.6/veros/core/external/solve_stream.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/external/solvers/__init__.py` & `veros-1.4.6/veros/core/external/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/external/solvers/petsc_.py` & `veros-1.4.6/veros/core/external/solvers/petsc_.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
             logger.warning(f"Streamfunction solver did not converge after {iterations} iterations (error code: {info})")
 
         if rs.monitor_streamfunction_residual:
             # re-use rhs vector to store residual
             rhs_norm = self._rhs_petsc.norm(PETSc.NormType.NORM_2)
             self._matrix.multAdd(self._sol_petsc, -self._rhs_petsc, self._rhs_petsc)
             residual_norm = self._rhs_petsc.norm(PETSc.NormType.NORM_2)
-            rel_residual = residual_norm / rhs_norm
+            rel_residual = residual_norm / max(rhs_norm, 1e-22)
 
             if rel_residual > 1e-8:
                 logger.warning(
                     f"Streamfunction solver did not achieve required precision (rel. residual: {rel_residual:.2e})"
                 )
 
         return npx.asarray(self._da.getVecArray(self._sol_petsc)[...])
```

### Comparing `veros-1.4.5/veros/core/external/solvers/scipy.py` & `veros-1.4.6/veros/core/external/solvers/scipy.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/external/solvers/scipy_jax.py` & `veros-1.4.6/veros/core/external/solvers/scipy_jax.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/external/streamfunction_init.py` & `veros-1.4.6/veros/core/external/streamfunction_init.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/friction.py` & `veros-1.4.6/veros/core/friction.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/idemix.py` & `veros-1.4.6/veros/core/idemix.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/isoneutral/diffusion.py` & `veros-1.4.6/veros/core/isoneutral/diffusion.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/isoneutral/friction.py` & `veros-1.4.6/veros/core/isoneutral/friction.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/isoneutral/isoneutral.py` & `veros-1.4.6/veros/core/isoneutral/isoneutral.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/momentum.py` & `veros-1.4.6/veros/core/momentum.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/numerics.py` & `veros-1.4.6/veros/core/numerics.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/operators.py` & `veros-1.4.6/veros/core/operators.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/special/cuda_tdma_kernels.cu` & `veros-1.4.6/veros/core/special/cuda_tdma_kernels.cu`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/special/tdma_.py` & `veros-1.4.6/veros/core/special/tdma_.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/special/tdma_cuda_.cpp` & `veros-1.4.6/veros/core/special/tdma_cuda_.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "veros/core/special/cuda_tdma_kernels.h"
         ],
@@ -32,16 +32,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -101,24 +101,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -226,15 +230,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -265,15 +269,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -589,35 +593,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1161,26 +1165,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1604,15 +1608,15 @@
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -1840,15 +1844,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_veros__core__special__tdma_cuda_) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -2436,15 +2440,15 @@
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 }
 #endif
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -2745,15 +2749,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -3017,15 +3021,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `veros-1.4.5/veros/core/special/tdma_cuda_.pyx` & `veros-1.4.6/veros/core/special/tdma_cuda_.pyx`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/special/tdma_cython_.pyx` & `veros-1.4.6/veros/core/special/tdma_cython_.pyx`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/thermodynamics.py` & `veros-1.4.6/veros/core/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/tke.py` & `veros-1.4.6/veros/core/tke.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/core/utilities.py` & `veros-1.4.6/veros/core/utilities.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/diagnostics/api.py` & `veros-1.4.6/veros/diagnostics/api.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/diagnostics/averages.py` & `veros-1.4.6/veros/diagnostics/averages.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/diagnostics/base.py` & `veros-1.4.6/veros/diagnostics/base.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/diagnostics/cfl_monitor.py` & `veros-1.4.6/veros/diagnostics/cfl_monitor.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/diagnostics/energy.py` & `veros-1.4.6/veros/diagnostics/energy.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/diagnostics/overturning.py` & `veros-1.4.6/veros/diagnostics/overturning.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/diagnostics/snapshot.py` & `veros-1.4.6/veros/diagnostics/snapshot.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/diagnostics/tracer_monitor.py` & `veros-1.4.6/veros/diagnostics/tracer_monitor.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/distributed.py` & `veros-1.4.6/veros/distributed.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/io_tools/hdf5.py` & `veros-1.4.6/veros/io_tools/hdf5.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/io_tools/netcdf.py` & `veros-1.4.6/veros/io_tools/netcdf.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/logs.py` & `veros-1.4.6/veros/logs.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/plugins.py` & `veros-1.4.6/veros/plugins.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/progress.py` & `veros-1.4.6/veros/progress.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/pyom_compat.py` & `veros-1.4.6/veros/pyom_compat.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/restart.py` & `veros-1.4.6/veros/restart.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/routines.py` & `veros-1.4.6/veros/routines.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/runtime.py` & `veros-1.4.6/veros/runtime.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/settings.py` & `veros-1.4.6/veros/settings.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/setups/acc/acc.py` & `veros-1.4.6/veros/setups/acc/acc.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/setups/acc_basic/acc_basic.py` & `veros-1.4.6/veros/setups/acc_basic/acc_basic.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/setups/global_1deg/global_1deg.py` & `veros-1.4.6/veros/setups/global_1deg/global_1deg.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/setups/global_4deg/global_4deg.py` & `veros-1.4.6/veros/setups/global_4deg/global_4deg.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/setups/global_flexible/global_flexible.py` & `veros-1.4.6/veros/setups/global_flexible/global_flexible.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/setups/north_atlantic/north_atlantic.py` & `veros-1.4.6/veros/setups/north_atlantic/north_atlantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,29 +119,36 @@
         settings = state.settings
         vs.coriolis_t = update(
             vs.coriolis_t, at[...], 2 * settings.omega * npx.sin(vs.yt[npx.newaxis, :] / 180.0 * settings.pi)
         )
 
     @veros_routine(dist_safe=False, local_variables=["kbot", "xt", "yt", "zt"])
     def set_topography(self, state):
+        import numpy as onp
+
         vs = state.variables
         settings = state.settings
 
         with h5netcdf.File(DATA_FILES["topography"], "r") as topo_file:
             topo_x, topo_y, topo_bottom_depth = (self._get_data(topo_file, k) for k in ("x", "y", "z"))
 
         topo_mask = npx.flipud(npx.asarray(Image.open(TOPO_MASK_FILE))).T
         topo_bottom_depth = npx.where(topo_mask, 0, topo_bottom_depth)
         topo_bottom_depth = scipy.ndimage.gaussian_filter(
             topo_bottom_depth, sigma=(len(topo_x) / settings.nx, len(topo_y) / settings.ny)
         )
         interp_coords = npx.meshgrid(vs.xt[2:-2], vs.yt[2:-2], indexing="ij")
         interp_coords = npx.rollaxis(npx.asarray(interp_coords), 0, 3)
         z_interp = scipy.interpolate.interpn(
-            (topo_x, topo_y), topo_bottom_depth, interp_coords, method="nearest", bounds_error=False, fill_value=0
+            (onp.array(topo_x), onp.array(topo_y)),
+            topo_bottom_depth,
+            onp.array(interp_coords),
+            method="nearest",
+            bounds_error=False,
+            fill_value=0,
         )
         vs.kbot = update(
             vs.kbot,
             at[2:-2, 2:-2],
             npx.where(
                 z_interp < 0.0,
                 1 + npx.argmin(npx.abs(z_interp[:, :, npx.newaxis] - vs.zt[npx.newaxis, npx.newaxis, :]), axis=2),
```

### Comparing `veros-1.4.5/veros/setups/north_atlantic/tidal_energy.npy` & `veros-1.4.6/veros/setups/north_atlantic/tidal_energy.npy`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/setups/north_atlantic/topo_mask.png` & `veros-1.4.6/veros/setups/north_atlantic/topo_mask.png`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/setups/north_atlantic/wind_energy.npy` & `veros-1.4.6/veros/setups/north_atlantic/wind_energy.npy`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/signals.py` & `veros-1.4.6/veros/signals.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/state.py` & `veros-1.4.6/veros/state.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/time.py` & `veros-1.4.6/veros/time.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/tools/assets.py` & `veros-1.4.6/veros/tools/assets.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/tools/filelock.py` & `veros-1.4.6/veros/tools/filelock.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/tools/setup.py` & `veros-1.4.6/veros/tools/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,20 @@
         var = npx.where(invalid_mask, npx.nan, var)
 
     if var.ndim > 1 and coords[0].ndim == 1:
         interp_grid = npx.rollaxis(npx.array(npx.meshgrid(*interp_coords, indexing="ij")), 0, len(interp_coords) + 1)
     else:
         interp_grid = interp_coords
 
-    coords = [onp.array(c) for c in coords]
+    def as_floatarray(x):
+        return onp.array(x, dtype="float64")
+
+    coords = tuple(as_floatarray(c) for c in coords)
     var = scipy.interpolate.interpn(
-        coords, onp.array(var), interp_grid, bounds_error=False, fill_value=npx.nan, method=kind
+        coords, as_floatarray(var), as_floatarray(interp_grid), bounds_error=False, fill_value=onp.nan, method=kind
     )
     var = npx.asarray(var)
 
     if fill:
         var = fill_holes(var)
 
     return var
```

### Comparing `veros-1.4.5/veros/variables.py` & `veros-1.4.6/veros/variables.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros/veros.py` & `veros-1.4.6/veros/veros.py`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/veros.egg-info/PKG-INFO` & `veros-1.4.6/veros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veros
-Version: 1.4.5
+Version: 1.4.6
 Summary: The versatile ocean simulator, in pure Python, powered by JAX.
 Home-page: https://veros.readthedocs.io
 Author: Dion Häfner (NBI Copenhagen)
 Author-email: dion.haefner@nbi.ku.dk
 License: MIT
 Keywords: oceanography python parallel numpy multi-core geophysics ocean-model mpi4py jax
 Classifier: Development Status :: 4 - Beta
@@ -39,15 +39,15 @@
   <a href="http://veros.readthedocs.io/?badge=latest">
     <img src="https://readthedocs.org/projects/veros/badge/?version=latest" alt="Documentation status">
   </a>
   <a href="https://github.com/team-ocean/veros/actions/workflows/test-all.yml">
     <img src="https://github.com/team-ocean/veros/actions/workflows/test-all.yml/badge.svg" alt="Test status">
   </a>
   <a href="https://codecov.io/gh/team-ocean/veros">
-    <img src="https://codecov.io/gh/team-ocean/veros/branch/master/graph/badge.svg" alt="Code Coverage">
+    <img src="https://codecov.io/gh/team-ocean/veros/branch/main/graph/badge.svg" alt="Code Coverage">
   </a>
   <a href="https://zenodo.org/badge/latestdoi/87419383">
     <img src="https://zenodo.org/badge/87419383.svg" alt="DOI">
   </a>
 </p>
 
 Veros, *the versatile ocean simulator*, aims to be the swiss army knife of ocean modeling. It is a full-fledged primitive equation ocean model that supports anything between idealized toy models and [realistic, high-resolution, global ocean simulations](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2021MS002717). And because Veros is written in pure Python, the days of struggling with complicated model setup workflows, ancient programming environments, and obscure legacy code are finally over.
@@ -110,15 +110,15 @@
 ## Basic usage
 
 To run Veros, you need to set up a model --- i.e., specify which settings
 and model domain you want to use. This is done by subclassing the
 `VerosSetup` base class in a *setup script* that is written in Python. You
 should use the `veros copy-setup` command to copy one into your current
 folder. A good place to start is the
-[ACC model](https://github.com/team-ocean/veros/blob/master/veros/setups/acc/acc.py):
+[ACC model](https://github.com/team-ocean/veros/blob/main/veros/setups/acc/acc.py):
 
 ```bash
 $ veros copy-setup acc
 ```
 
 After setting up your model, all you need to do is call the `setup` and
 `run` methods on your setup class. The pre-implemented setups can all be
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: veros Version: 1.4.5 Summary: The versatile ocean
+Metadata-Version: 2.1 Name: veros Version: 1.4.6 Summary: The versatile ocean
 simulator, in pure Python, powered by JAX. Home-page: https://
 veros.readthedocs.io Author: Dion HÃ¤fner (NBI Copenhagen) Author-email:
 dion.haefner@nbi.ku.dk License: MIT Keywords: oceanography python parallel
 numpy multi-core geophysics ocean-model mpi4py jax Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
@@ -49,19 +49,19 @@
 copy-setup acc --to /tmp/acc $ veros run /tmp/acc/acc.py ``` For more detailed
 installation instructions, have a look at [our documentation](https://
 veros.readthedocs.io). ## Basic usage To run Veros, you need to set up a model
 --- i.e., specify which settings and model domain you want to use. This is done
 by subclassing the `VerosSetup` base class in a *setup script* that is written
 in Python. You should use the `veros copy-setup` command to copy one into your
 current folder. A good place to start is the [ACC model](https://github.com/
-team-ocean/veros/blob/master/veros/setups/acc/acc.py): ```bash $ veros copy-
-setup acc ``` After setting up your model, all you need to do is call the
-`setup` and `run` methods on your setup class. The pre-implemented setups can
-all be executed via `veros run`: ```bash $ veros run acc.py ``` For more
-information on using Veros, have a look at [our documentation](http://
+team-ocean/veros/blob/main/veros/setups/acc/acc.py): ```bash $ veros copy-setup
+acc ``` After setting up your model, all you need to do is call the `setup` and
+`run` methods on your setup class. The pre-implemented setups can all be
+executed via `veros run`: ```bash $ veros run acc.py ``` For more information
+on using Veros, have a look at [our documentation](http://
 veros.readthedocs.io). ## Contributing Contributions to Veros are always
 welcome, no matter if you spotted an inaccuracy in [the documentation](https://
 veros.readthedocs.io), wrote a new setup, fixed a bug, or even extended Veros\'
 core mechanics. There are 2 ways to contribute: 1. If you want to report a bug
 or request a missing feature, please [open an issue](https://github.com/team-
 ocean/veros/issues). If you are reporting a bug, make sure to include all
 relevant information for reproducing it (ideally through a *minimal* code
```

### Comparing `veros-1.4.5/veros.egg-info/SOURCES.txt` & `veros-1.4.6/veros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `veros-1.4.5/versioneer.py` & `veros-1.4.6/versioneer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,64 @@
 
-# Version: 0.23
+# Version: 0.28
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
 * https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain (CC0-1.0)
+* License: Public Domain (Unlicense)
 * Compatible with: Python 3.7, 3.8, 3.9, 3.10 and pypy3
 * [![Latest Version][pypi-image]][pypi-url]
 * [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils/setuptools-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
 * `pip install versioneer` to somewhere in your $PATH
-* add a `[versioneer]` section to your setup.cfg (see [Install](INSTALL.md))
-* run `versioneer install` in your source tree, commit the results
-* Verify version information with `python setup.py version`
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -227,17 +255,18 @@
 
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -259,17 +288,16 @@
 * [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
   plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
 
 [pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
 [pypi-url]: https://pypi.python.org/pypi/versioneer/
 [travis-image]:
 https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
 [travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
@@ -283,17 +311,27 @@
 import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
+from pathlib import Path
 from typing import Callable, Dict
 import functools
 
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
+
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
 
 def get_root():
     """Get the project root directory.
@@ -322,39 +360,49 @@
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         my_path = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
             print("Warning: build in %s is using versioneer.py from %s"
                   % (os.path.dirname(my_path), versioneer_py))
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.ConfigParser()
-    with open(setup_cfg, "r") as cfg_file:
-        parser.read_file(cfg_file)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
+    root = Path(root)
+    pyproject_toml = root / "pyproject.toml"
+    setup_cfg = root / "setup.cfg"
+    section = None
+    if pyproject_toml.exists() and have_tomllib:
+        try:
+            with open(pyproject_toml, 'rb') as fobj:
+                pp = tomllib.load(fobj)
+            section = pp['tool']['versioneer']
+        except (tomllib.TOMLDecodeError, KeyError):
+            pass
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
 
-    # Dict-like interface for non-mandatory entries
-    section = parser["versioneer"]
+        section = parser["versioneer"]
 
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
+    cfg.VCS = section['VCS']
     cfg.style = section.get("style", "")
     cfg.versionfile_source = section.get("versionfile_source")
     cfg.versionfile_build = section.get("versionfile_build")
     cfg.tag_prefix = section.get("tag_prefix")
     if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
     cfg.parentdir_prefix = section.get("parentdir_prefix")
@@ -426,16 +474,17 @@
 LONG_VERSION_PY['git'] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.23 (https://github.com/python-versioneer/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.28
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
@@ -669,26 +718,26 @@
     # It may be intended to be passed to the Versioneer-versioned project,
     # but that should not change where we get our version from.
     env = os.environ.copy()
     env.pop("GIT_DIR", None)
     runner = functools.partial(runner, env=env)
 
     _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=True)
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
     describe_out, rc = runner(GITS, [
         "describe", "--tags", "--dirty", "--always", "--long",
         "--match", f"{tag_prefix}[[:digit:]]*"
-        ], cwd=root)
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -1191,26 +1240,26 @@
     # It may be intended to be passed to the Versioneer-versioned project,
     # but that should not change where we get our version from.
     env = os.environ.copy()
     env.pop("GIT_DIR", None)
     runner = functools.partial(runner, env=env)
 
     _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=True)
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
     describe_out, rc = runner(GITS, [
         "describe", "--tags", "--dirty", "--always", "--long",
         "--match", f"{tag_prefix}[[:digit:]]*"
-        ], cwd=root)
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -1316,22 +1365,23 @@
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
     files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        my_path = __file__
-        if my_path.endswith(".pyc") or my_path.endswith(".pyo"):
-            my_path = os.path.splitext(my_path)[0] + ".py"
-        versioneer_file = os.path.relpath(my_path)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
         with open(".gitattributes", "r") as fobj:
             for line in fobj:
                 if line.strip().startswith(versionfile_source):
                     if "export-subst" in line.strip().split()[1:]:
                         present = True
@@ -1366,15 +1416,15 @@
     if verbose:
         print("Tried directories %s but none started with prefix %s" %
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.23) from
+# This file was generated by 'versioneer.py' (0.28) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1855,14 +1905,16 @@
                 # build_ext --inplace will only build extensions in
                 # build/lib<..> dir with no _version.py to write to.
                 # As in place builds will already have a _version.py
                 # in the module dir, we do not need to write one.
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
+            if not cfg.versionfile_build:
+                return
             target_versionfile = os.path.join(self.build_lib,
                                               cfg.versionfile_build)
             if not os.path.exists(target_versionfile):
                 print(f"Warning: {target_versionfile} does not exist, skipping "
                       "version update. This can happen if you are running build_ext "
                       "without first running build_py.")
                 return
@@ -1899,15 +1951,18 @@
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if 'py2exe' in sys.modules:  # py2exe enabled?
-        from py2exe.distutils_buildexe import py2exe as _py2exe
+        try:
+            from py2exe.setuptools_buildexe import py2exe as _py2exe
+        except ImportError:
+            from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
             def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
@@ -1925,15 +1980,15 @@
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["py2exe"] = cmd_py2exe
 
     # sdist farms its file list building out to egg_info
     if 'egg_info' in cmds:
-        _sdist = cmds['egg_info']
+        _egg_info = cmds['egg_info']
     else:
         from setuptools.command.egg_info import egg_info as _egg_info
 
     class cmd_egg_info(_egg_info):
         def find_sources(self):
             # egg_info.find_sources builds the manifest list and writes it
             # in one shot
@@ -2133,14 +2188,18 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
+def setup_command():
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+        setup_command()
```

